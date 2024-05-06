# Comparing `tmp/libzac-0.1.2-py3-none-any.whl.zip` & `tmp/libzac-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 18332 bytes, number of entries: 14
+Zip file size: 23966 bytes, number of entries: 14
 -rw-rw-rw-  2.0 fat      155 b- defN 24-Mar-08 08:44 libzac/__init__.py
 -rw-rw-rw-  2.0 fat     8270 b- defN 24-Mar-08 08:38 libzac/bitfield.py
--rw-rw-rw-  2.0 fat     2997 b- defN 23-Jul-19 08:26 libzac/dsp.py
+-rw-rw-rw-  2.0 fat     7256 b- defN 24-Apr-30 08:22 libzac/dsp.py
 -rw-rw-rw-  2.0 fat     6732 b- defN 24-Jan-23 03:02 libzac/e.py
 -rw-rw-rw-  2.0 fat     4999 b- defN 24-Mar-08 08:37 libzac/io.py
 -rw-rw-rw-  2.0 fat     1777 b- defN 24-Mar-08 09:27 libzac/logic.py
 -rw-rw-rw-  2.0 fat     4357 b- defN 24-Mar-08 08:47 libzac/math.py
--rw-rw-rw-  2.0 fat     3074 b- defN 24-Jan-23 03:54 libzac/plt.py
--rw-rw-rw-  2.0 fat     7592 b- defN 24-Feb-26 07:24 libzac/reg.py
--rw-rw-rw-  2.0 fat     1087 b- defN 24-Mar-08 09:37 libzac-0.1.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2918 b- defN 24-Mar-08 09:37 libzac-0.1.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Mar-08 09:37 libzac-0.1.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 24-Mar-08 09:37 libzac-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1019 b- defN 24-Mar-08 09:37 libzac-0.1.2.dist-info/RECORD
-14 files, 45076 bytes uncompressed, 16684 bytes compressed:  63.0%
+-rw-rw-rw-  2.0 fat    23082 b- defN 24-Mar-21 09:03 libzac/plt.py
+-rw-rw-rw-  2.0 fat     7743 b- defN 24-Mar-21 08:53 libzac/reg.py
+-rw-rw-rw-  2.0 fat     1087 b- defN 24-May-06 02:29 libzac-0.1.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2918 b- defN 24-May-06 02:29 libzac-0.1.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-06 02:29 libzac-0.1.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 24-May-06 02:29 libzac-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1020 b- defN 24-May-06 02:29 libzac-0.1.3.dist-info/RECORD
+14 files, 69495 bytes uncompressed, 22318 bytes compressed:  67.9%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: libzac/plt.py
 Comment: 
 
 Filename: libzac/reg.py
 Comment: 
 
-Filename: libzac-0.1.2.dist-info/LICENSE
+Filename: libzac-0.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: libzac-0.1.2.dist-info/METADATA
+Filename: libzac-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: libzac-0.1.2.dist-info/WHEEL
+Filename: libzac-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: libzac-0.1.2.dist-info/top_level.txt
+Filename: libzac-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: libzac-0.1.2.dist-info/RECORD
+Filename: libzac-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## libzac/dsp.py

```diff
@@ -1,8 +1,9 @@
 import numpy as np
+import scipy
 from packaging import version
 
 def rolling_window(array:np.ndarray, window:int, step:int=1):
     """
     return rolling window matrix of input 1d `array` with `step`,
     drop tails that not enough for one window. 
         
@@ -70,10 +71,138 @@
     n_step = abs(step)
     n_window = (array.size - window)//n_step + 1
     if window+(n_window-1)*n_step < array.size:
         pad_size = window + n_window*n_step - array.size
         array = np.pad(array, (0, pad_size) if step>0 else (pad_size,0), **pad_kwarg)
     return rolling_window(array, window, step)
 
+
+def enbw(windowCol,fs):
+    bw_t = np.mean(windowCol**2)/((np.mean(windowCol))**2)
+    bw = bw_t * fs / len(windowCol)
+    return bw
+
+def bandpower(Sfund,Ffund):
+    width = np.concatenate([[(Ffund[-1]-Ffund[0])/(len(Ffund)-1)], np.diff(Ffund)])
+    power = np.dot(Sfund, width)
+    return power
+
+def idx2psddb(Pxx, F, idx):
+    psd = 10*np.log10(Pxx[idx])
+    freq = F[idx]
+    return psd, freq
+
+def getToneFromPSD(Pxx, F, rbw=None, toneFreq=None):
+    """
+    Retrieve the power and frequency of a windowed sinusoid
+    This function is for internal use only and may be removed in a future
+    release of MATLAB
+    """
+
+    idxTone = idxLeft = idxRight = None
+
+    # force column vector
+    colPxx = np.reshape(Pxx, -1)
+    colF = np.reshape(F, -1)
+
+    if toneFreq is None:
+        idxTone = np.argmax(colPxx)
+    elif colF[0] <= toneFreq and toneFreq <= colF[-1]:
+        # find closest bin to specified freq
+        idxTone = np.argmin(np.abs(colF-toneFreq))
+        # look for local peak in vicinity of tone
+        iLeftBin = max(0, idxTone-1)
+        iRightBin = min(idxTone+1, len(colPxx)-1)
+        idxMax = np.argmax(colPxx[iLeftBin:iRightBin+1])
+        idxTone = iLeftBin + idxMax
+    else:
+        power = np.nan
+        freq = np.nan
+        idxTone = idxLeft = idxRight = None
+        return power, freq, idxTone, idxLeft, idxRight
+
+    idxToneScalar = idxTone
+
+    # sidelobes treated as noise
+    idxLeft = idxToneScalar - 1
+    idxRight = idxToneScalar + 1
+
+    # roll down slope to left
+    while idxLeft > -1 and colPxx[idxLeft] <= colPxx[idxLeft+1]:
+        idxLeft -= 1
+
+    # roll down slope to right
+    while idxRight <= len(colPxx)-1 and colPxx[idxRight-1] >= colPxx[idxRight]:
+        idxRight += 1
+
+    # provide indices to the tone border (inclusive)
+    idxLeft = idxLeft+1
+    idxRight = idxRight
+
+    idxLeftScalar = idxLeft
+    idxRightScalar = idxRight
+
+    # compute the central moment in the neighborhood of the peak
+    Ffund = colF[idxLeftScalar:idxRightScalar]
+    Sfund = colPxx[idxLeftScalar:idxRightScalar]
+    freq = np.dot(Ffund, Sfund) / np.sum(Sfund)
+
+    # report back the integrated power in this band
+    if idxLeftScalar<idxRightScalar:
+        # more than one bin
+        power = bandpower(Sfund, Ffund)
+    elif 1 < idxRightScalar and idxRightScalar < len(colPxx):
+        # otherwise just use the current bin
+        power = colPxx[idxRightScalar] * (colF[idxRightScalar+1] - colF[idxRightScalar-1])/2
+    else:
+        # otherwise just use the average bin width
+        power = colPxx[idxRightScalar] * np.mean(np.diff(colF))
+
+    # protect against nearby tone invading the window kernel
+    if rbw is not None and power < rbw*colPxx[idxToneScalar]:
+        power = rbw*colPxx[idxToneScalar]
+        freq = colF[idxToneScalar]
+
+    return power, freq, idxTone, idxLeft, idxRight
+
+def snr(x,fs=1,nHarmScalar=6):
+    colX = x.reshape(-1)
+    colX = colX - np.mean(colX)
+    n = len(colX)
+    w = scipy.signal.windows.kaiser(n, 38)
+    rbw = enbw(w,fs)
+    F,Pxx = scipy.signal.periodogram(colX,fs,w,n)
+
+    origPxx = Pxx.copy()
+
+    Pxx[0] = 2*Pxx[0]
+    _, _, _, iLeft, iRight = getToneFromPSD(Pxx, F, rbw, 0)
+    if iLeft is not None and iRight is not None:
+        Pxx[iLeft:iRight] = 0
+
+    psdHarmPow = np.zeros(nHarmScalar)
+    psdHarmFreq = np.zeros(nHarmScalar)
+
+    Pfund, Ffund, iFund, iLeft, iRight = getToneFromPSD(Pxx, F, rbw)
+    psdHarmPow[0], psdHarmFreq[0] = idx2psddb(Pxx, F, iFund)
+    if iLeft is not None and iRight is not None:
+        Pxx[iLeft:iRight] = 0
+
+    for i in range(2,nHarmScalar+1):
+        toneFreq = i*Ffund
+        harmPow, _, iHarm, iLeft, iRight = getToneFromPSD(Pxx, F, rbw, toneFreq)
+        psdHarmPow[i-1], psdHarmFreq[i-1] = idx2psddb(Pxx, F, iHarm)
+        if not np.isnan(harmPow) and iLeft is not None and iRight is not None:
+            Pxx[iLeft:iRight] = 0
+
+    estimatedNoiseDensity = np.median(Pxx[Pxx>0])
+    Pxx[Pxx==0] = estimatedNoiseDensity
+    Pxx = np.min([Pxx,origPxx],0)
+    totalNoise = bandpower(Pxx, F)
+    r = 10*np.log10(Pfund / totalNoise)
+    noisePow = 10*np.log10(totalNoise)
+    return r
+
+
 if __name__ == '__main__':
     import doctest
     doctest.testmod()
```

## libzac/plt.py

```diff
@@ -1,12 +1,18 @@
+from __future__ import print_function
 import numpy as np
 import matplotlib.pyplot as plt
+from matplotlib.widgets import AxesWidget
+from matplotlib.text import Text
+import mplcursors
 
-def shift_factory(fig, shift=0.05):
+def shift_factory(fig=None, shift=0.05):
     """shift <shift>% of current x axis with wheel, up-right down-left"""
+    if fig is None:
+        fig = plt.gcf()
     def shift_fun(event):
         # get axes where scroll event happened
         ax = event.inaxes
         if ax is None: # if outside axe 
             return
         x_range = ax.get_xlim()[1] - ax.get_xlim()[0]
         for line in ax.get_lines():
@@ -20,16 +26,18 @@
             # set new x data
             line.set_xdata(x)
         plt.draw() # force re-draw
     # attach the call back
     fig.canvas.mpl_connect('scroll_event',shift_fun)
     return shift_fun
 
-def zoom_factory(fig, base_scale = 1.1):
+def zoom_factory(fig=None, base_scale = 1.1):
     """zoom <base_scale> of current axes with wheel, up-zoom in down-zoom out"""
+    if fig is None:
+        fig = plt.gcf()
     def zoom_fun(event):
         """zoom when scrolling"""
         ax = event.inaxes
         scale_factor = np.power(base_scale, -event.step)
         xdata = event.xdata
         ydata = event.ydata
         x_left = xdata - ax.get_xlim()[0]
@@ -74,8 +82,578 @@
 
     ax.bar3d(xpos, ypos, zpos, dx, dy, dz, color=rgba, zsort='average')
     plt.title(title)
     plt.xlabel(ylabel) # this is not typo, x/y axis is swaped
     plt.ylabel(xlabel)
     plt.show()
 
-    return fig
+    return fig
+
+class Ruler(AxesWidget):
+    """
+    A ruler to measure distances and angles on an axes instance. 
+    
+    For the ruler to remain responsive you must keep a reference to it.
+
+    Parameters
+    ----------
+    ax  : the  :class:`matplotlib.axes.Axes` instance 
+       
+    active : bool, default is True
+        Whether the ruler is active or not. 
+    
+    length_unit  : string, A length unit identifier to use in displayed text  
+        i.e. ('ft', or 'm')
+                        
+    angle_unit  : string, The type of angle unit ('degrees' or 'radians')
+        
+    print_text  : bool, default is False
+        Whether the length measure string is printed to the console
+
+    useblit : bool, default is False
+        If True, use the backend-dependent blitting features for faster
+        canvas updates. 
+
+    lineprops : dict, default is None
+      Dictionary of :class:`matplotlib.lines.Line2D` properties
+                   
+    markerprops : dict, default is None
+      Dictionary of :class:`matplotlib.markers.MarkerStyle` properties
+      
+    textprops: dict, default is None
+        Dictionary of :class:`matplotlib.text.Text` properties. To reposition the 
+        textbox you can overide the defaults which position the box in the top left
+        corner of the axes. 
+          
+    Usage:
+    ----------
+
+    1. Hold left click drag and release to draw the ruler in the axes.
+      - Hold shift while dragging to lock the ruler to the horizontal axis.
+      - Hold control while drawing to lock the ruler to the vertical axis. 
+
+    2. Right click one of the markers to move the ruler. 
+
+    The keyboard can be used to activate and deactivate the ruler and toggle 
+    visibility of the line and text:
+
+    'm' : Toggles the ruler on and off. 
+
+    'ctl+m' : Toggles the visibility of the ruler and text. 
+    
+    Example
+    ----------
+    
+    >>> xCoord = np.arange(0, 5, 1)
+    >>> yCoord = [0, 1, -3, 5, -3]
+    >>> fig = plt.figure()
+    >>> ax = fig.add_subplot(111)
+    
+    >>> markerprops = dict(marker='o', markersize=5, markeredgecolor='red')
+    >>> lineprops = dict(color='red', linewidth=2)
+    
+    >>> ax.grid(True)
+    >>> ax.plot(xCoord, yCoord)
+    
+    >>> ruler = Ruler(ax=ax,
+                  useblit=True,
+                  markerprops=markerprops,
+                  lineprops=lineprops)
+    
+    >>> plt.show()
+    
+    """
+
+    def __init__(self,
+                 ax,
+                 active=True,
+                 length_unit=None,
+                 angle_unit='degree',
+                 print_text=False,
+                 useblit=False,
+                 lineprops=None,
+                 textprops=None,
+                 markerprops=None):
+        """
+        Add a ruler to *ax*. If ``ruler_active=True``, the ruler will be 
+        activated when the plot is first created. If ``ruler_unit`` is set the 
+        string will be appended to the length text annotations. 
+
+        """
+        AxesWidget.__init__(self, ax)
+
+        self.connect_events()
+
+        self.ax = ax
+        self.fig = ax.figure
+
+        self._print_text = print_text
+        self._visible = True
+        self.active = active
+        self.length_unit = length_unit
+        self.angle_unit = angle_unit
+        self.useblit = useblit and self.canvas.supports_blit
+
+        self._mouse1_pressed = False
+        self._mouse3_pressed = False
+        self._shift_pressed = False
+        self._control_pressed = False
+        self._y0 = None
+        self._x1 = None
+        self._y1 = None
+        self._line_start_coords = None
+        self._line_end_coords = None
+        self._ruler_marker = None
+        self._background = None
+        self._ruler_moving = False
+        self._end_a_lock = False
+        self._end_b_lock = False
+        self._end_c_lock = False
+        self._old_marker_a_coords = None
+        self._old_marker_c_coords = None
+        self._old_mid_coords = None
+
+        if lineprops is None:
+            lineprops = {}
+
+        bbox = dict(facecolor='white',
+                    alpha=0.5,
+                    boxstyle='round',
+                    edgecolor='0.75')
+
+        used_textprops = dict(xy=(0, 1),
+                              xytext=(10, -10),
+                              xycoords='axes fraction',
+                              textcoords='offset points',
+                              ha='left',
+                              va='center',
+                              bbox=bbox)
+
+        x0 = np.nan
+        y0 = np.nan
+
+        self._ruler, = self.ax.plot([x0, x0], [y0, y0], **lineprops)
+
+        used_markerprops = dict(marker='s',
+                                markersize=3,
+                                markerfacecolor='white',
+                                markeredgecolor='black',
+                                markeredgewidth=0.5,
+                                picker=5,
+                                visible=False)
+
+        # If marker or text  props are given as an argument combine with the
+        # default marker props. Don't really want to override the entire props
+        # if a user only gives one value.
+
+        if markerprops is not None:
+            used_markerprops.update(markerprops)
+
+        if textprops is not None:
+            used_textprops.update(used_textprops)
+
+        self._axes_text = self.ax.annotate('', **used_textprops)
+        self.ax.add_artist(self._axes_text)
+
+        self._marker_a, = self.ax.plot((x0, y0), **used_markerprops)
+        self._marker_b, = self.ax.plot((x0, y0), **used_markerprops)
+        self._marker_c, = self.ax.plot((x0, y0), **used_markerprops)
+
+        self._artists = [self._axes_text,
+                         self._ruler,
+                         self._marker_a,
+                         self._marker_b,
+                         self._marker_c]
+
+    def connect_events(self):
+        """
+        Connect all events to the various callbacks
+        """
+        self.connect_event('button_press_event', self._on_press)
+        self.connect_event('button_release_event', self._on_release)
+        self.connect_event('motion_notify_event', self._on_move)
+        self.connect_event('key_press_event', self._on_key_press)
+        self.connect_event('key_release_event', self._on_key_release)
+
+    def ignore(self, event):
+        """
+        Ignore events if the cursor is out of the axes or the widget is locked
+        """
+        if not self.canvas.widgetlock.available(self):
+            return True
+        if event.inaxes != self.ax.axes:
+            return True
+        if not self.active:
+            return True
+
+    def _on_key_press(self, event):
+        """
+        Handle key press events. 
+        
+        If shift is pressed the ruler will be constrained to horizontal axis
+        If control is pressed the ruler will be constrained to vertical axis
+        If m is pressed the ruler will be toggled on and off
+        If ctrl+m is pressed the visibility of the ruler will be toggled
+        """
+
+        if event.key == 'shift':
+            self._shift_pressed = True
+
+        if event.key == 'control':
+            self._control_pressed = True
+
+        if event.key == 'm':
+            self.toggle_ruler()
+
+        if event.key == 'ctrl+m':
+            self.toggle_ruler_visibility()
+
+    def _on_key_release(self, event):
+        """
+        Handle key release event, flip the flags to false.
+        """
+        if event.key == 'shift':
+            self._shift_pressed = False
+
+        if event.key == 'control':
+            self._control_pressed = False
+
+    def toggle_ruler(self):
+        """
+        Called when the 'm' key is pressed. If ruler is on turn it off, and 
+        vise versa
+        """
+
+        self.active = not self.active
+
+    def toggle_ruler_visibility(self):
+        """
+        Called when the 'ctl+m' key is pressed. If ruler is visible turn it off
+        , and vise versa
+        """
+        if self._visible is True:
+            for artist in self._artists:
+                artist.set_visible(False)
+            self.active = False
+            self._visible = False
+
+        elif self._visible is False:
+            for artist in self._artists:
+                artist.set_visible(True)
+            self._visible = True
+
+        self.canvas.draw_idle()
+
+    def _on_press(self, event):
+        """
+        On mouse button press check which button has been pressed and handle 
+        """
+        if self.ignore(event):
+            return
+        if event.button == 1 and self._mouse3_pressed is False:
+            self._handle_button1_press(event)
+        elif event.button == 3:
+            self._handle_button3_press(event)
+
+    def _handle_button1_press(self, event):
+        """
+        On button 1 press start drawing the ruler line from the initial 
+        press position
+        """
+
+        self._mouse1_pressed = True
+        self._x0 = event.xdata
+        self._y0 = event.ydata
+        self._marker_a.set_data((event.xdata, event.ydata))
+        self._marker_a.set_visible(True)
+
+        if self.useblit:
+            self._marker_a.set_data(self._x0, self._y0)
+            for artist in self._artists:
+                artist.set_animated(True)
+            self.canvas.draw()
+            self._background = self.canvas.copy_from_bbox(self.fig.bbox)
+
+    def _handle_button3_press(self, event):
+        """
+        If button 3 is pressed (right click) check if cursor is at one of the 
+        ruler markers and the move the ruler accordingly. 
+        """
+        contains_a, _ = self._marker_a.contains(event)
+        contains_b, _ = self._marker_b.contains(event)
+        contains_c, _ = self._marker_c.contains(event)
+
+        if not (contains_a or contains_b or contains_c):
+            return
+
+        self._end_a_lock = contains_a
+        self._end_b_lock = contains_b
+        self._end_c_lock = contains_c
+
+        line_coords = self._ruler.get_path().vertices
+        self._x0 = line_coords[0][0]
+        self._y0 = line_coords[0][1]
+        self._x1 = line_coords[1][0]
+        self._y1 = line_coords[1][1]
+
+        self._old_marker_a_coords = self._marker_a.get_path().vertices
+        self._old_marker_c_coords = self._marker_c.get_path().vertices
+        self._old_mid_coords = self.midline_coords
+
+    def _on_move(self, event):
+        """
+        On motion draw the ruler if button 1 is pressed. If one of the markers
+        is locked indicating move the ruler according to the locked marker
+        """
+
+        if event.inaxes != self.ax.axes:
+            return
+
+        if self._end_a_lock or self._end_b_lock or self._end_c_lock is True:
+            self._move_ruler(event)
+
+        if self._mouse1_pressed is True:
+            self._draw_ruler(event)
+
+    def _move_ruler(self, event):
+        """
+        If one of the markers is locked move the ruler according the selected
+        marker. 
+        """
+
+        # This flag is used to prevent the ruler from clipping when a marker is
+        # first selected
+        if self._ruler_moving is False:
+            if self.useblit:
+                for artist in self._artists:
+                    artist.set_animated(True)
+                self.canvas.draw()
+                self._background = self.canvas.copy_from_bbox(self.fig.bbox)
+                self._ruler_moving = True
+
+        if self._end_a_lock is True:
+            # If marker a is locked only move end a.
+            pos_a = event.xdata, self._x1
+            pos_b = event.ydata, self._y1
+            self._marker_a.set_data(event.xdata, event.ydata)
+            self._ruler.set_data(pos_a, pos_b)
+            self._set_midline_marker()
+
+        if self._end_c_lock is True:
+            # If marker a is locked only move end c.
+            pos_a = self._x0, event.xdata
+            pos_b = self._y0, event.ydata
+            self._marker_c.set_data(event.xdata, event.ydata)
+            self._ruler.set_data(pos_a, pos_b)
+            self._set_midline_marker()
+
+        if self._end_b_lock is True:
+            # If marker b is locked shift the whole ruler.
+            b_dx = event.xdata - self._old_mid_coords[0]
+            b_dy = event.ydata - self._old_mid_coords[1]
+            pos_a = self._x0 + b_dx, self._x1 + b_dx
+            pos_b = self._y0 + b_dy, self._y1 + b_dy
+
+            marker_a_coords = self._old_marker_a_coords[0][0] + b_dx, \
+                              self._old_marker_a_coords[0][1] + b_dy
+            marker_c_coords = self._old_marker_c_coords[0][0] + b_dx, \
+                              self._old_marker_c_coords[0][1] + b_dy
+
+            self._ruler.set_data(pos_a, pos_b)
+            self._marker_a.set_data(marker_a_coords)
+            self._marker_b.set_data(event.xdata, event.ydata)
+            self._marker_c.set_data(marker_c_coords)
+
+        self._update_text()
+        self._update_artists()
+
+    def _set_midline_marker(self):
+        self._marker_b.set_visible(True)
+        self._marker_b.set_data(self.midline_coords)
+
+    @property
+    def midline_coords(self):
+        pos0, pos1 = self._ruler.get_path().vertices
+        mid_line_coords = (pos0[0] + pos1[0]) / 2, (pos0[1] + pos1[1]) / 2
+        return mid_line_coords
+
+    def _draw_ruler(self, event):
+        """
+        If the left mouse button is pressed and held draw the ruler as the 
+        mouse is dragged
+        """
+
+        self._x1 = event.xdata
+        self._y1 = event.ydata
+
+        # If shift is pressed ruler is constrained to horizontal axis
+        if self._shift_pressed is True:
+            pos_a = self._x0, self._x1
+            pos_b = self._y0, self._y0
+        # If control is pressed ruler is constrained to vertical axis
+        elif self._control_pressed is True:
+            pos_a = self._x0, self._x0
+            pos_b = self._y0, self._y1
+        # Else the ruler follow the mouse cursor
+        else:
+            pos_a = self._x0, self._x1
+            pos_b = self._y0, self._y1
+
+        self._ruler.set_data([pos_a], [pos_b])
+        x1 = self._ruler.get_path().vertices[1][0]
+        y1 = self._ruler.get_path().vertices[1][1]
+        self._marker_c.set_visible(True)
+        self._marker_c.set_data(x1, y1)
+        self._set_midline_marker()
+        self._update_text()
+        self._update_artists()
+
+    def _update_artists(self):
+        if self.useblit:
+            if self._background is not None:
+                self.canvas.restore_region(self._background)
+            else:
+                self._background = self.canvas.copy_from_bbox(self.fig.bbox)
+
+            for artist in self._artists:
+                self.ax.draw_artist(artist)
+
+            self.canvas.blit(self.fig.bbox)
+        else:
+            self.canvas.draw_idle()
+
+    def _update_text(self):
+        if self.length_unit is not None:
+            detail_string = 'L: {:0.3f} {}; dx: {:0.3f} {}; dy: {:0.3f} {}; ' \
+                            'angle: {:0.3f} deg'.format(self.ruler_length,
+                                                        self.length_unit,
+                                                        self.ruler_dx,
+                                                        self.length_unit,
+                                                        self.ruler_dy,
+                                                        self.length_unit,
+                                                        self.ruler_angle)
+        else:
+            detail_string = 'L: {:0.3f}; dx: {:0.3f}; dy: {:0.3f}; ' \
+                            'ang: {:0.3f} deg'.format(self.ruler_length,
+                                                        self.ruler_dx,
+                                                        self.ruler_dy,
+                                                        self.ruler_angle)
+
+        self._axes_text.set_text(detail_string)
+        if self._print_text is True:
+            print(detail_string)
+
+    def _on_release(self, event):
+        self._mouse1_pressed = False
+        self._mouse3_pressed = False
+        self._ruler_moving = False
+        self._end_a_lock = False
+        self._end_b_lock = False
+        self._end_c_lock = False
+
+    @property
+    def ruler_length(self):
+        pos0, pos1 = self._ruler.get_path().vertices
+        return np.hypot((pos1[0] - pos0[0]), (pos0[1] - pos1[1]))
+
+    @property
+    def ruler_dx(self):
+        pos0, pos1 = self._ruler.get_path().vertices
+        return pos1[0] - pos0[0]
+
+    @property
+    def ruler_dy(self):
+        pos0, pos1 = self._ruler.get_path().vertices
+        return pos1[1] - pos0[1]
+
+    @property
+    def ruler_angle(self):
+        pos0, pos1 = self._ruler.get_path().vertices
+        angle = np.arctan2(pos1[0] - pos0[0], pos1[1] - pos0[1])
+
+        if self.angle_unit == 'degree':
+            return angle * 180 / np.pi
+        else:
+            return angle
+
+class TextMover(object):
+    """
+    A simple little tool to move text annotation in an axes by clicking and dragging them. 
+
+    """
+
+    def __init__(self, ax, active=True):
+        self.ax = ax
+        self.active = active
+        self.selectedText = None
+        self.mousePressed = False
+        self.background = None
+        self.connect_events()
+
+    def connect_events(self):
+        self.ax.figure.canvas.mpl_connect("pick_event", self.on_pick_event)
+        self.ax.figure.canvas.mpl_connect('motion_notify_event', self.on_motion)
+        self.ax.figure.canvas.mpl_connect('button_release_event', self.on_release)
+
+    def on_pick_event(self, event):
+
+        if self.active is False:
+            return
+
+        if event.mouseevent.button != 1:
+            return
+
+        if isinstance(event.artist, Text):
+            self.mousePressed = True
+            self.selectedText = event.artist
+
+            canvas = self.selectedText.figure.canvas
+            axes = self.selectedText.axes
+            self.selectedText.set_animated(True)
+            canvas.draw()
+            self.background = canvas.copy_from_bbox(self.selectedText.axes.bbox)
+
+            axes.draw_artist(self.selectedText)
+            canvas.blit(axes.bbox)
+
+    def on_motion(self, event):
+        if event.inaxes != self.ax.axes:
+            return
+
+        if self.mousePressed is True and self.selectedText:
+            self.x1 = event.xdata
+            self.y1 = event.ydata
+
+            coords = (self.x1, self.y1)
+
+            self.selectedText.set_position(coords)
+            canvas = self.selectedText.figure.canvas
+            axes = self.selectedText.axes
+            canvas.restore_region(self.background)
+            axes.draw_artist(self.selectedText)
+            canvas.blit(axes.bbox)
+
+    def on_release(self, event):
+
+        if self.selectedText is None:
+            return
+
+        self.mousePressed = False
+        self.selectedText.set_animated(False)
+
+        self.background = None
+        self.selectedText.figure.canvas.draw()
+        self.selectedText = None
+
+def use_ruler(ax=None):
+    if ax is None:
+        ax = plt.gca()
+    markerprops = dict(marker='o', markersize=5, markeredgecolor='red')
+    lineprops = dict(color='red', linewidth=2)
+    ruler = Ruler(ax=ax, useblit=False, markerprops=markerprops, lineprops=lineprops)
+    return ruler
+
+def use_cursor(ax=None):
+    if ax is None:
+        ax = plt.gca()
+    lines = list(ax.get_lines())
+    mplcursors.cursor(lines,multiple=True)
```

## libzac/reg.py

```diff
@@ -1,8 +1,9 @@
 import re
+import sys
 import numpy as np
 import pandas as pd
 import xlrd
 import openpyxl
 from .e import e2int
 from typing import Union
 
@@ -165,7 +166,10 @@
             if start >= 0 and not pd.isna(table.loc[i,addr_name]):            
                 addr = re.search(r"[\da-f]{4,}",table.loc[i,addr_name])
                 if addr is not None:     
                     table.loc[i,new_column] = parse_reg(int(addr.group(),16), mem_map, start, stop)
         except Exception as e:
             print(f"Unable to parse table line {i}: \n{table.loc[i]}\n")
             raise e
+
+def load_reg_1121M(MODULE_PATH = "E:\\Work\\Yichip\\1121M\\Soft_Doc\\xlsxtoStructTool\\reg_1121M"):    
+    sys.path.append(MODULE_PATH)
```

## Comparing `libzac-0.1.2.dist-info/LICENSE` & `libzac-0.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `libzac-0.1.2.dist-info/METADATA` & `libzac-0.1.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libzac
-Version: 0.1.2
+Version: 0.1.3
 Summary: A private use library
 Author-email: ZinGer_KyoN <zinger.kyon@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 YiChip Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

## Comparing `libzac-0.1.2.dist-info/RECORD` & `libzac-0.1.3.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 libzac/__init__.py,sha256=q2j0YQCdjF2QZ0dPQfY6Vpm4jlRVrcwTWIoJ3JhfZF8,155
 libzac/bitfield.py,sha256=gL2_pKgYdpc5fdia-6Cd5L1CpV9FEmUHXp2zVEmT6yM,8270
-libzac/dsp.py,sha256=hhdkZWR-vHf9UuCWus80sBRzhxeI63lQxKIKEyueplM,2997
+libzac/dsp.py,sha256=VyHQi44eIiWf0KVWnXYMxwrErwJSAI3tGq1bfqlKG_I,7256
 libzac/e.py,sha256=eEMbFM-FfR9kQNgn7QwqYFN2Hqs8YhkvHaSO9Cp0diA,6732
 libzac/io.py,sha256=amqV6oYfXa7qMM_N7krOK1tMbRn-Jv7JxcrsYRdVKd4,4999
 libzac/logic.py,sha256=ZkPLtxrEf5PNHg7YH_HGJdIvcTa_bnWP2W-KOnKNCRI,1777
 libzac/math.py,sha256=2tvM7t48qipyC2uHUFegHIHYQSv-bw3v5iiS5yBZLfE,4357
-libzac/plt.py,sha256=hM9rXy5scVtrXJMjclhvQEds88raY97C6efYz7o8d1w,3074
-libzac/reg.py,sha256=HAQdMjybPSEPR8XoovOCIsyJEbVIJ8N-MkGBlApnsnU,7592
-libzac-0.1.2.dist-info/LICENSE,sha256=e0NpGwn8zCo3MShVy2LEvMsZBJlB9lwWbz8g94O4ge4,1087
-libzac-0.1.2.dist-info/METADATA,sha256=m-lNn4XopIuEm_Q3O2f47CG6eDpPVZEh86Tw0gJI0p0,2918
-libzac-0.1.2.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-libzac-0.1.2.dist-info/top_level.txt,sha256=4aG8bWAEZg_5zIiME4cwpZVGHvRZzdameIcLGWTf950,7
-libzac-0.1.2.dist-info/RECORD,,
+libzac/plt.py,sha256=SrmZLVFC212vXCga4gAW4rQn-jR6_o80oF-4kqFDLSw,23082
+libzac/reg.py,sha256=eljchPaLEBgjXvsoCGaetLaLQR0a1-q4gKV-o4Fuay8,7743
+libzac-0.1.3.dist-info/LICENSE,sha256=e0NpGwn8zCo3MShVy2LEvMsZBJlB9lwWbz8g94O4ge4,1087
+libzac-0.1.3.dist-info/METADATA,sha256=Fia-Q6rDBHA1tEVU_cYMOfYqJmYLA5xqbfv4yoCCrvg,2918
+libzac-0.1.3.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+libzac-0.1.3.dist-info/top_level.txt,sha256=4aG8bWAEZg_5zIiME4cwpZVGHvRZzdameIcLGWTf950,7
+libzac-0.1.3.dist-info/RECORD,,
```

