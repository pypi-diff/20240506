# Comparing `tmp/opseestools-0.2.tar.gz` & `tmp/opseestools-0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opseestools-0.2.tar", last modified: Mon Apr  8 15:44:01 2024, max compression
+gzip compressed data, was "opseestools-0.25.tar", last modified: Mon May  6 17:20:14 2024, max compression
```

## Comparing `opseestools-0.2.tar` & `opseestools-0.25.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 15:44:01.458608 opseestools-0.2/
--rw-rw-rw-   0        0        0     4903 2024-04-08 15:44:01.457607 opseestools-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4416 2024-04-08 15:30:07.000000 opseestools-0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-08 15:44:01.444071 opseestools-0.2/opseestools/
--rw-rw-rw-   0        0        0     7214 2024-04-08 15:37:47.000000 opseestools-0.2/opseestools/Lib_frag.py
--rw-rw-rw-   0        0        0       91 2024-03-16 16:37:45.000000 opseestools-0.2/opseestools/__init__.py
--rw-rw-rw-   0        0        0   105586 2024-03-20 20:17:26.000000 opseestools-0.2/opseestools/analisis.py
--rw-rw-rw-   0        0        0    91076 2024-03-20 20:44:02.000000 opseestools-0.2/opseestools/analisis3D.py
--rw-rw-rw-   0        0        0    19939 2024-03-06 21:36:46.000000 opseestools-0.2/opseestools/utilidades.py
-drwxrwxrwx   0        0        0        0 2024-04-08 15:44:01.457607 opseestools-0.2/opseestools.egg-info/
--rw-rw-rw-   0        0        0     4903 2024-04-08 15:44:01.000000 opseestools-0.2/opseestools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      316 2024-04-08 15:44:01.000000 opseestools-0.2/opseestools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 15:44:01.000000 opseestools-0.2/opseestools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-04-08 15:44:01.000000 opseestools-0.2/opseestools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-08 15:44:01.000000 opseestools-0.2/opseestools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-08 15:44:01.458608 opseestools-0.2/setup.cfg
--rw-rw-rw-   0        0        0      926 2024-04-08 15:43:14.000000 opseestools-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 17:20:14.299498 opseestools-0.25/
+-rw-rw-rw-   0        0        0     4904 2024-05-06 17:20:14.298499 opseestools-0.25/PKG-INFO
+-rw-rw-rw-   0        0        0     4416 2024-04-08 15:30:07.000000 opseestools-0.25/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 17:20:14.284481 opseestools-0.25/opseestools/
+-rw-rw-rw-   0        0        0     7214 2024-04-08 15:37:47.000000 opseestools-0.25/opseestools/Lib_frag.py
+-rw-rw-rw-   0        0        0       91 2024-03-16 16:37:45.000000 opseestools-0.25/opseestools/__init__.py
+-rw-rw-rw-   0        0        0   105586 2024-03-20 20:17:26.000000 opseestools-0.25/opseestools/analisis.py
+-rw-rw-rw-   0        0        0    91076 2024-03-20 20:44:02.000000 opseestools-0.25/opseestools/analisis3D.py
+-rw-rw-rw-   0        0        0    22717 2024-05-06 17:16:19.000000 opseestools-0.25/opseestools/utilidades.py
+drwxrwxrwx   0        0        0        0 2024-05-06 17:20:14.298499 opseestools-0.25/opseestools.egg-info/
+-rw-rw-rw-   0        0        0     4904 2024-05-06 17:20:14.000000 opseestools-0.25/opseestools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      316 2024-05-06 17:20:14.000000 opseestools-0.25/opseestools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 17:20:14.000000 opseestools-0.25/opseestools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-05-06 17:20:14.000000 opseestools-0.25/opseestools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-06 17:20:14.000000 opseestools-0.25/opseestools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 17:20:14.299498 opseestools-0.25/setup.cfg
+-rw-rw-rw-   0        0        0      927 2024-05-06 16:11:17.000000 opseestools-0.25/setup.py
```

### Comparing `opseestools-0.2/PKG-INFO` & `opseestools-0.25/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opseestools
-Version: 0.2
+Version: 0.25
 Summary: A collection of OpenSeesPy routines for performing several types of analyses and other tools
 Home-page: https://github.com/odarroyo/opseestools
 Author: Orlando Arroyo
 Author-email: odarroyo@uc.cl
 License: LICENSE
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `opseestools-0.2/README.md` & `opseestools-0.25/README.md`

 * *Files identical despite different names*

### Comparing `opseestools-0.2/opseestools/Lib_frag.py` & `opseestools-0.25/opseestools/Lib_frag.py`

 * *Files identical despite different names*

### Comparing `opseestools-0.2/opseestools/analisis.py` & `opseestools-0.25/opseestools/analisis.py`

 * *Files identical despite different names*

### Comparing `opseestools-0.2/opseestools/analisis3D.py` & `opseestools-0.25/opseestools/analisis3D.py`

 * *Files identical despite different names*

### Comparing `opseestools-0.2/opseestools/utilidades.py` & `opseestools-0.25/opseestools/utilidades.py`

 * *Files 10% similar despite different names*

```diff
@@ -304,22 +304,23 @@
         Vel[i+1] = gamma/(betha*delta_t)*(Desplz[i+1]-Desplz[i])+(1-(gamma/betha))*Vel[i]+delta_t*(1-(gamma/(2*betha)))*Acel[i]
         Acel[i+1] = (Desplz[i+1]-Desplz[i])/(betha*(delta_t**2))-Vel[i]/(betha*delta_t)-(1/(2*betha)-1)*Acel[i]
         
     return Tiempo,Desplz,Vel,Acel
 
 
 def newmarkLA(T,xi,GM,delta_t,flag = 'all',betha = 1/6, gamma = 1/2 ,u0 = 0,v0 = 0,P0 = 0):
+    '''
     #T: periodo de la estrutura
     #xi: porcentaje de amortiguamiento crítico
     #GM: registro en unidades consistentes
     #delta_t: delta de tiempo del registro
     #flag: recibe 'max' cuando solo se deseen los valores máximos de tiempo, desplazamiento, velocidad y aceleracion absolutas.
     #betha, gamma: parámetros del Newmark. Por defecto utiliza método lineal de interpolación
     #u0,v0,a0: condiciones iniciales de desplazamiento velocidad y aceleración
-    
+    '''
     
     w = 2*np.pi/T
     m = 1.0
     k = m*w**2
     c = 2*xi*m*w
     # Calculos iniciales
     a0 = (P0-c*v0-k*u0)/m                     # Aceleración inicial
@@ -373,19 +374,19 @@
         V[i] = Vel
         Sa[i] = Desplz*w**2
     return T,Sa
 
 
 def spectrum4(GM,dt,xi=0.05,rango=[0.02,3.0],N=100):
     ''' está basado en la rutina de OpenSees
-        GM: el registro en .txt. Por ejemplo 'GM01.txt'
-        dt: dt del registro
-        xi: porcentaje del amortiguamiento crítico
-        rango: rango de periodos en un vector
-        N: número de puntos
+        \n GM: el registro en .txt. Por ejemplo 'GM01.txt'
+        \n dt: dt del registro
+        \n xi: porcentaje del amortiguamiento crítico
+        \n rango: rango de periodos en un vector
+        \n N: número de puntos
            
     '''
     m = 1
     T = np.linspace(rango[0],rango[1],N)
     w = 2*np.pi/T
     k = m*w**2
     c = 2*xi*m*w
@@ -408,14 +409,57 @@
 #     Sa = (T < T0)*2.5*Aa*Fa*I*(0.4+0.6*T/T0) + ((T0 < T) & (T < Tc))*2.5*Aa*Fa*I + ((Tc < T) & (T < Tl))*1.2*Av*Fv*I/T + (Tl < T)*1.2*Av*Fv*I*Tl/T**2
 #     return T,Sa
 
 # T,Sa = espectroNSR(0.15, 0.2, 2.1, 3.2, 1.0)
 
 # plt.plot(T,Sa)
 
+def creategrid(xloc,yloc):
+    ''' funcion para crear grilla de puntos en OpenSeesPy
+        \n xloc: coordenadas de x
+        \n yloc: coordenadas de y
+        La función devuelve los nodos comenzando en 1000,1001... para la primera columna, luego 2000,2001...
+    '''
+    ny = len(yloc)
+    nx = len(xloc)
+    # ----------------------Crear nodos de la estructura----------------------|
+    for i in range(nx):
+        for j in range(ny):
+            nnode = 1000*(i+1)+j
+            node(nnode,xloc[i],yloc[j])
+
+def BuildISection(secID,matID,d,tw,bf,tf,nfdw,nftw,nfbf,nftf):
+    ''' función para crear una sección en forma de I. 
+        \n Recibe:
+        \n secID: ID para la sección a crear
+        \n matID: material de la sección
+        \n d: altura total de la sección
+        \n tw: espesor del alma
+        \n bf: ancho de la aleta
+        \n tf: espesor de la aleta
+        \n nfdw, nftw, nfbf, nftf: fibras a lo largo de la longitud del alma, ancho del alma, ancho y espesor de la aleta
+    '''
+    
+    
+    dw = d-2*tf
+    y1 = -d/2
+    y2 = -dw/2 
+    y3 = dw/2
+    y4 = d/2 
+    
+    z1 =-bf/2
+    z2 =-tw/2 
+    z3 = tw/2 
+    z4 = bf/2 
+    GJ = 1e6
+    section('Fiber',secID,'-GJ',GJ)
+    patch('quad',matID,nfbf,nftf,y1,z4,y1,z1,y2,z1,y2,z4)
+    patch('quad',matID,nftw,nfdw,y2,z3,y2,z2,y3,z2,y3,z3)
+    patch('quad',matID,nfbf,nftf,y3,z4,y3,z1,y4,z1,y4,z4)
+
 def plot_Wall_T_BE(matConf, matInco, bW, bF, BEU, BED, BEL, BER, Lww, LwF, nMax, nMin):
     
     cover = 0.025
     SteelTag = 4
     
     fib_sec_1 = [['section', 'Fiber', 2, '-GJ', 1e16],
          ['patch','rect',matInco, nMax, nMin, -Lww/2, -bW/2, Lww/2, bW/2], 
@@ -460,14 +504,53 @@
     #Fy = esfuerzo de fluencia del acero [MPa]
     #Fu = esfuerzo último del acero [MPa]
     #ey, eh, eu = deformaciones unitarias del acero
     #L = Espaciamiento entre estribos (Longitud libre para pandearse) [mm]
     #D = Diámetro de la barra [mm]
     fy = Fyy
     fu = Fuu
+    fh = fy+0.01
+    ey = eyy
+    eu = euu
+    eh = ehh
+    L = Lb
+    D = Db
+    alfa = 0.75
+    efracture = 0.05
+    espalling = 0.004
+    sigma_u = 0.2*fy
+    p1 = [eh,eu]
+    p2 = [fh,fu]
+    Es = fy/ey
+    m = -0.02*Es
+    eas = np.max([(55-2.3*np.sqrt(fy/100)*L/D)*ey,7*ey])
+    sigma_l = np.interp(eas,p1,p2)
+    sigma_as = np.max([alfa*(1.1-0.016*np.sqrt(fy/100)*L/D)*sigma_l,0.2*fy])
+    eu_d = (sigma_u-sigma_as)/m + eas
+    sigma_f = np.interp(efracture,p1,p2)
+    sigma_s = np.interp(espalling,p1,p2)
+    # strain = [-eu_d,-espalling,-ey,0.0,ey,efracture,eu]
+    # stress = [-sigma_u,-sigma_s,-fy,0.0, fy,sigma_f, sigma_u]
+    strain = [-eu_d,-eas,-espalling,-ey,0.0,ey,eh,efracture,eu]
+    stress = [-sigma_u,-sigma_as,-sigma_s,-fy,0.0, fy,fh,sigma_f, sigma_u]
+
+    s = [fy*1000,fh*1000,sigma_f*1000, sigma_u*1000,-fy*1000,-sigma_s*1000,-sigma_as*1000,-sigma_u*1000]
+    e = [ey,eh,efracture,eu,-ey,-espalling,-eas,-eu_d]
+ 
+    
+    return s, e
+
+def dhakal(Fyy, Fuu, eyy, ehh, euu, Lb, Db):
+    #Fy = esfuerzo de fluencia del acero [MPa]
+    #Fu = esfuerzo último del acero [MPa]
+    #ey, eh, eu = deformaciones unitarias del acero
+    #L = Espaciamiento entre estribos (Longitud libre para pandearse) [mm]
+    #D = Diámetro de la barra [mm]
+    fy = Fyy
+    fu = Fuu
     fh = fy+0.01
     ey = eyy
     eu = euu
     eh = ehh
     L = Lb
     D = Db
     alfa = 0.75
```

### Comparing `opseestools-0.2/opseestools.egg-info/PKG-INFO` & `opseestools-0.25/opseestools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opseestools
-Version: 0.2
+Version: 0.25
 Summary: A collection of OpenSeesPy routines for performing several types of analyses and other tools
 Home-page: https://github.com/odarroyo/opseestools
 Author: Orlando Arroyo
 Author-email: odarroyo@uc.cl
 License: LICENSE
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `opseestools-0.2/setup.py` & `opseestools-0.25/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 @author: HOME
 """
 
 from setuptools import setup, find_packages
 
 setup(
     name='opseestools',
-    version='0.2',
+    version='0.25',
     author='Orlando Arroyo',
     author_email='odarroyo@uc.cl',
     packages=find_packages(),
     description='A collection of OpenSeesPy routines for performing several types of analyses and other tools',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     install_requires=[
```

