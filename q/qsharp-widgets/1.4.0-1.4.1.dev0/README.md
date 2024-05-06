# Comparing `tmp/qsharp_widgets-1.4.0-py2.py3-none-any.whl.zip` & `tmp/qsharp_widgets-1.4.1.dev0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 150156 bytes, number of entries: 6
+Zip file size: 150269 bytes, number of entries: 6
 -rw-r--r--  2.0 unx     7449 b- defN 20-Feb-02 00:00 qsharp_widgets/__init__.py
--rw-r--r--  2.0 unx    12066 b- defN 20-Feb-02 00:00 qsharp_widgets/static/index.css
--rw-r--r--  2.0 unx   485694 b- defN 20-Feb-02 00:00 qsharp_widgets/static/index.js
-?rw-r--r--  2.0 unx      187 b- defN 20-Feb-02 00:00 qsharp_widgets-1.4.0.dist-info/METADATA
-?rw-r--r--  2.0 unx      105 b- defN 20-Feb-02 00:00 qsharp_widgets-1.4.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx      488 b- defN 20-Feb-02 00:00 qsharp_widgets-1.4.0.dist-info/RECORD
-6 files, 505989 bytes uncompressed, 149280 bytes compressed:  70.5%
+-rw-r--r--  2.0 unx    12078 b- defN 20-Feb-02 00:00 qsharp_widgets/static/index.css
+-rw-r--r--  2.0 unx   485817 b- defN 20-Feb-02 00:00 qsharp_widgets/static/index.js
+?rw-r--r--  2.0 unx      192 b- defN 20-Feb-02 00:00 qsharp_widgets-1.4.1.dev0.dist-info/METADATA
+?rw-r--r--  2.0 unx      105 b- defN 20-Feb-02 00:00 qsharp_widgets-1.4.1.dev0.dist-info/WHEEL
+?rw-r--r--  2.0 unx      503 b- defN 20-Feb-02 00:00 qsharp_widgets-1.4.1.dev0.dist-info/RECORD
+6 files, 506144 bytes uncompressed, 149363 bytes compressed:  70.5%
```

## zipnote {}

```diff
@@ -3,17 +3,17 @@
 
 Filename: qsharp_widgets/static/index.css
 Comment: 
 
 Filename: qsharp_widgets/static/index.js
 Comment: 
 
-Filename: qsharp_widgets-1.4.0.dist-info/METADATA
+Filename: qsharp_widgets-1.4.1.dev0.dist-info/METADATA
 Comment: 
 
-Filename: qsharp_widgets-1.4.0.dist-info/WHEEL
+Filename: qsharp_widgets-1.4.1.dev0.dist-info/WHEEL
 Comment: 
 
-Filename: qsharp_widgets-1.4.0.dist-info/RECORD
+Filename: qsharp_widgets-1.4.1.dev0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qsharp_widgets/static/index.css

```diff
@@ -1 +1 @@
-:root{--heading-background: #262679;--main-background: var( --vscode-editor-background, var(--jp-layout-color0, #ececf0) );--main-color: var( --vscode-editor-foreground, var(--jp-widgets-color, #202020) );--qs-tr-nth-color: var( --vscode-list-hoverBackground, var(--jp-layout-color1, var(--colab-secondary-surface-color, #f2f2f2)) );--nav-background: #bed1f4;--nav-hover-background: #b3bede;--nav-current-background: #b5c5f2;--border-color: #768f9c;--menu-box-fill: var(--main-background);--error-background-color: #ffe3e3;--bar-selected-outline: #587ddd}*,*:before,*:after{box-sizing:inherit;margin:0;padding:0}html{box-sizing:border-box;font-size:16px}.qs-play-body{position:relative;min-height:100vh;font-family:system-ui,Segoe UI,SegoeUI,Roboto,Helvetica,Arial,sans-serif;color:var(--main-color);background-color:var(--main-background);display:grid;grid-template-areas:"header header header" "nav editor results";grid-template-rows:auto 1fr;grid-template-columns:minmax(180px,auto) 8fr 8fr;column-gap:16px}.page-header{grid-area:header;background:var(--heading-background);color:var(--main-background);font-size:2rem;font-weight:600;text-align:center;padding-top:4px;padding-bottom:8px}#popup{position:absolute;display:none;background-color:#fff;border:1px solid black;border-radius:2px;padding:8px 16px;font-size:16px}.nav-column{grid-area:nav;background-color:var(--nav-background)}.nav-1{font-size:1.2rem;font-weight:200;color:var(--main-color);border-top:1px solid var(--border-color);padding-top:4px;padding-bottom:4px;padding-left:8px}.nav-2{font-size:1rem;font-weight:200;padding:4px 4px 4px 16px}.nav-selectable:hover{background-color:var(--nav-hover-background);cursor:pointer}.nav-current{font-weight:700;background-color:var(--nav-current-background)}.editor-column{grid-area:editor;margin:32px 16px 16px}.file-name{border:1px solid var(--border-color);border-bottom:0px;width:100px;text-align:center;height:32px;line-height:32px;background-color:#fff}.icon-row>*{margin-left:4px;font-size:1.4rem;cursor:pointer}.code-editor{height:40vh;min-height:400px;border:1px solid var(--border-color)}.button-row{display:flex;justify-content:flex-end;align-items:center;margin-top:8px}.button-row>*{margin-left:10px;font-size:1rem}.main-button{background-color:var(--nav-background);font-size:1rem;color:var(--main-color);width:72px;height:24px;border-radius:8px;border:1px solid var(--border-color);cursor:pointer}.main-button:disabled{background-color:gray;cursor:default}.error-list{margin-top:24px;margin-bottom:24px;min-height:48px}.error-row{border:1px solid var(--border-color);background-color:var(--error-background-color);padding:4px;border-bottom:.5px solid gray;font-size:.9rem;margin-bottom:-1px}.error-row>span{font-weight:200}.error-help{font-weight:200;font-style:italic}.kata-override{background-color:var(--main-background)}.results-column{grid-area:results;margin-left:0;margin-top:32px;margin-right:120px}.active-tab{font-size:1.1rem;font-weight:600;text-decoration:underline}.results-labels{display:flex;height:32px}.results-labels>div{margin-right:40px;text-align:left;vertical-align:middle;cursor:pointer}.ast-output,.hir-output{height:40vh;min-height:400px;width:100%;resize:none;white-space:pre}.output-header{font-size:1.1rem;font-weight:400;margin-top:16px;margin-bottom:16px;display:flex;justify-content:space-between}.prev-next{font-weight:200;cursor:pointer}.result-label{margin-bottom:24px;font-style:italic;font-weight:300}.message-output{font-weight:300;font-size:1.1rem;margin-bottom:16px}.state-table{border-collapse:collapse;font-size:.9rem;width:100%;min-width:400px;margin-bottom:16px}.state-table thead tr{background:var(--nav-background)}.state-table tbody tr{border-top:1px solid gray}.state-table td,.state-table th{text-align:center;padding:6px;white-space:nowrap}.state-table progress{margin-right:2px}.histogram{max-height:calc(100vh - 40px);max-width:600px;border:1px solid var(--border-color);background-color:var(--vscode-sideBar-background, white)}.bar{fill:var(--vscode-button-background, var(--nav-background))}.bar:hover{fill:var(--vscode-button-hoverBackground, var(--nav-hover-background))}.bar-selected{stroke:var(--bar-selected-outline);fill:var(--nav-current-background)}.bar-label{font-size:3pt;fill:var(--vscode-button-foreground, var(--main-color));text-anchor:end;pointer-events:none}.histo-label{font-size:3.5pt;fill:var(--vscode-foreground, #3b3b3b)}.hover-text{font-size:3.5pt;fill:gray;text-anchor:middle}.menu-icon *{stroke:#000;fill:var(--vscode-sideBar-background, white);stroke:var(--vscode-icon-foreground, #3b3b3b)}.menu-box{fill:var(--menu-box-fill);stroke:#000;stroke-width:.1}.menu-item{width:32px;height:10px;fill:var(--vscode-list-inactiveSelectionBackground, var(--nav-background));stroke:gray;stroke-width:.2}.menu-item:hover{stroke-width:.6;fill:var(--vscode-list-hoverBackground, var(--nav-hover-background))}.menu-selected{fill:var( --vscode-list-activeSelectionBackground, var(--nav-current-background) )}.menu-text{font-size:4.5px;pointer-events:none;fill:var(--main-color)}.menu-separator{stroke:gray;stroke-width:.25}.help-info{fill:var(--menu-box-fill);stroke:gray;stroke-width:.5}.help-info-text{font-size:4.5px;pointer-events:none;fill:var(--main-color)}.estimate-details{padding:1em}.estimate-details>summary{font-size:1.1em}.estimate-table{margin-top:1em;font-size:.9em}.estimate-table tr:nth-child(2n){background-color:var(--qs-tr-nth-color)}.estimate-cell{vertical-align:top;padding-right:8px}.title-cell{font-weight:700;white-space:nowrap}.value-cell{text-align:center;width:100px;white-space:nowrap}.estimate-explanation{margin-top:1em;margin-bottom:1em;max-width:500px}.estimate-assumption{margin:1em}.cell-output-ipywidget-background{background-color:transparent!important}#pieChart{fill:var(--main-color)}.spaceReport{display:flex;flex-direction:column}.spaceReportHeader{font-size:13px;background-color:var(--qs-tr-nth-color);border-top:.5px gray solid;border-bottom:.5px gray solid;padding:10px}.spaceReportRow{display:flex;font-size:12px;padding:10px 24px}.spaceDetailText{width:200px}.qs-help{font-size:14px;line-height:1.5;word-wrap:break-word}.qs-help h1{margin-top:16px;margin-bottom:8px;line-height:1.25;font-weight:600;padding-bottom:.3em;font-size:2em;border-bottom:1px solid var(--vscode-editorWidget-border)}.qs-help h2{margin-top:16px;margin-bottom:8px;font-weight:600;line-height:1.25;padding-bottom:.3em;font-size:1.4em;border-bottom:1px solid var(--vscode-editorWidget-border)}.qs-resultsTable-sortedTable{border-collapse:collapse;margin:12px 0;outline:none}.qs-resultsTable-sortedTable th,.qs-resultsTable-sortedTable td{padding:4px 8px;text-align:left}.qs-resultsTable-dragEnter{background-color:#8888;border-left:1.5px solid blue;border-right:1.5px solid blue}.qs-resultsTable-sortedTable tr:nth-child(2n){background:var(--qs-tr-nth-color)}.qs-resultsTable-sortedTable tbody tr:hover{background:var(--vscode-list-hoverBackground, var(--js-layout-color2))}.qs-resultsTable-sortedTableSelectedRow td{background:var(--vscode-button-background, var(--jp-layout-color3));color:var(--vscode-button-foreground);font-weight:600}.qs-resultsTable-columnMenu{display:none;width:160px}.qs-resultsTable-showColumnMenu{display:block;position:absolute;background-color:var(--vscode-menu-background, var(--main-background));border:1px solid #8888;padding:4px;z-index:100;text-align:left}.qs-resultsTable-menuItem{cursor:pointer;background-color:var(--vscode-list-hoverBackground, var(--jp-layout-color1));padding:4px;margin:2px;font-size:14px;font-weight:400}.qs-resultsTable-menuItem:hover{background-color:var(--vscode-menu-border, var(--jp-layout-color2))}.qs-resultsTable-columnSelected{cursor:pointer;padding:4px;font-weight:400;font-size:14px;background-color:var(--vscode-button-background, var(--jp-brand-color1));color:var(--vscode-button-foreground, var(--jp-ui-inverse-font-color0));margin:2px;border-radius:3px}.qs-resultsTable-headerCell{padding-right:20px}.qs-resultsTable-sortHeaderCell{padding-right:4px}@keyframes codicon-spin{to{transform:rotate(360deg);transform-origin:center}}.codicon-modifier-spin{fill:var(--vscode-icon-foreground, gray);animation:codicon-spin 1.5s steps(45) infinite}.qs-scatterChart-x-axisTitle,.qs-scatterChart-y-axisTitle{text-anchor:middle;font-size:16px;fill:var(--main-color)}.qs-scatterChart-y-axisTitle{writing-mode:vertical-lr;transform:rotate(180deg)}.qs-scatterChart-point{r:2px;stroke-width:4px}.qs-scatterChart-hover:hover{r:4px;stroke-width:4px;fill:#fff}.qs-scatterChart-point-selected{r:8px;stroke-width:4px;fill:#fff}.qs-scatterChart-watermark{font-size:16px;fill:var(--main-color)}.qs-scatterChart-tooltip,.qs-scatterChart-selectedInfo{position:absolute;visibility:hidden;background:var(--main-background);color:var(--main-color);border:var(--border-color) 1px solid;padding:4px}.qs-scatterChart-tooltip:after,.qs-scatterChart-selectedInfo:after{content:"";position:absolute;bottom:100%;left:50%;margin-left:-5px;border-width:5px;border-style:solid;border-color:transparent transparent var(--border-color) transparent}.qs-scatterChart-axis,.qs-scatterChart-tick-line{stroke:var(--border-color)}.qs-scatterChart-x-tick-text{text-anchor:middle;fill:var(--main-color)}.qs-scatterChart-y-tick-text{text-anchor:end;fill:var(--main-color)}.qs-estimatesOverview-error{color:red}.qs-circuit-panel p,.qs-circuit-error,.qs-circuit-error p{padding:10px 0}.qs-circuit{background:var(--main-background)}.qs-circuit line,.qs-circuit circle,.qs-circuit rect{stroke:var(--main-color);stroke-width:1}.qs-circuit text{fill:var(--main-color);dominant-baseline:middle;text-anchor:middle;font-family:Arial}.qs-circuit .gate-unitary{fill:var(--vscode-button-secondaryBackground, #d9f1fa)}.qs-circuit .gate text{fill:var(--vscode-button-secondaryForeground, #000000)}.qs-circuit .gate>line,.qs-circuit .control-dot{fill:var(--main-color)}.qs-circuit .gate>.oplus>line,.qs-circuit .gate>.oplus>circle{fill:var(--main-background);stroke:var(--main-color);stroke-width:2}.qs-circuit .gate-measure{fill:var(--vscode-button-background, #ffde86)}.qs-circuit .gate>g>line,.qs-circuit .arc-measure{stroke:var(--vscode-button-foreground, #000000);fill:none;stroke-width:1}.qs-circuit rect.gate-swap{fill:transparent;stroke:transparent}.qs-circuit .register-classical{stroke-width:.5}.qs-circuit .hidden{display:none}.qs-circuit .classically-controlled-unknown{opacity:.25}.qs-circuit .classically-controlled-one .classical-container,.qs-circuit .classically-controlled-one .classical-line{stroke:#4059bd;stroke-width:1.3;fill:#4059bd;fill-opacity:.1}.qs-circuit .classically-controlled-zero .classical-container,.qs-circuit .classically-controlled-zero .classical-line{stroke:#c40000;stroke-width:1.3;fill:#c40000;fill-opacity:.1}.qs-circuit .classically-controlled-btn{cursor:pointer}.qs-circuit .classically-controlled-unknown .classically-controlled-btn{fill:#e5e5e5}.qs-circuit .classically-controlled-one .classically-controlled-btn{fill:#4059bd}.qs-circuit .classically-controlled-zero .classically-controlled-btn{fill:#c40000}.qs-circuit .classically-controlled-btn text{dominant-baseline:middle;text-anchor:middle;stroke:none;font-family:Arial}.qs-circuit .classically-controlled-unknown .classically-controlled-btn text{fill:#000}.qs-circuit .classically-controlled-one .classically-controlled-btn text{fill:#fff}.qs-circuit .classically-controlled-zero .classically-controlled-btn text{fill:#fff}.qs-circuit .qviz .gate-collapse,.qs-circuit .qviz .gate-expand{opacity:0;transition:opacity 1s}.qs-circuit .qviz:hover .gate-collapse,.qs-circuit .qviz:hover .gate-expand{visibility:visible;opacity:.2;transition:visibility 1s;transition:opacity 1s}.qs-circuit .gate-expand,.gate-collapse{cursor:pointer}.qs-circuit .gate-collapse circle,.qs-circuit .gate-expand circle{fill:#fff;stroke-width:2px;stroke:#000}.qs-circuit .gate-collapse path,.qs-circuit .gate-expand path{stroke-width:4px;stroke:#000}.qs-circuit .gate:hover>.gate-collapse,.qs-circuit .gate:hover>.gate-expand{visibility:visible;opacity:1;transition:opacity 1s}
+:root{--heading-background: #262679;--main-background: var( --vscode-editor-background, var(--jp-layout-color0, #ececf0) );--main-color: var( --vscode-editor-foreground, var(--jp-widgets-color, #202020) );--qs-tr-nth-color: var( --vscode-list-hoverBackground, var(--jp-layout-color1, var(--colab-secondary-surface-color, #f2f2f2)) );--nav-background: #bed1f4;--nav-hover-background: #b3bede;--nav-current-background: #b5c5f2;--border-color: #768f9c;--menu-box-fill: var(--main-background);--error-background-color: #ffe3e3;--bar-selected-outline: #587ddd}*,*:before,*:after{box-sizing:inherit;margin:0;padding:0}html{box-sizing:border-box;font-size:16px}.qs-play-body{position:relative;min-height:100vh;font-family:system-ui,Segoe UI,SegoeUI,Roboto,Helvetica,Arial,sans-serif;color:var(--main-color);background-color:var(--main-background);display:grid;grid-template-areas:"header header header" "nav editor results";grid-template-rows:auto 1fr;grid-template-columns:minmax(180px,auto) 8fr 8fr;column-gap:16px}.page-header{grid-area:header;background:var(--heading-background);color:var(--main-background);font-size:2rem;font-weight:600;text-align:center;padding-top:4px;padding-bottom:8px}#popup{position:absolute;display:none;background-color:#fff;border:1px solid black;border-radius:2px;padding:8px 16px;font-size:16px}.nav-column{grid-area:nav;background-color:var(--nav-background)}.nav-1{font-size:1.2rem;font-weight:200;color:var(--main-color);border-top:1px solid var(--border-color);padding-top:4px;padding-bottom:4px;padding-left:8px}.nav-2{font-size:1rem;font-weight:200;padding:4px 4px 4px 16px}.nav-selectable:hover{background-color:var(--nav-hover-background);cursor:pointer}.nav-current{font-weight:700;background-color:var(--nav-current-background)}.editor-column{grid-area:editor;margin:32px 16px 16px}.file-name{border:1px solid var(--border-color);border-bottom:0px;width:100px;text-align:center;height:32px;line-height:32px;background-color:#fff}.icon-row>*{margin-left:4px;font-size:1.4rem;cursor:pointer}.code-editor{height:40vh;min-height:400px;border:1px solid var(--border-color)}.button-row{display:flex;justify-content:flex-end;align-items:center;margin-top:8px}.button-row>*{margin-left:10px;font-size:1rem}.main-button{background-color:var(--nav-background);font-size:1rem;color:var(--main-color);width:72px;height:24px;border-radius:8px;border:1px solid var(--border-color);cursor:pointer}.main-button:disabled{background-color:gray;cursor:default}.error-list{margin-top:24px;margin-bottom:24px;min-height:48px}.error-row{border:1px solid var(--border-color);background-color:var(--error-background-color);padding:4px;border-bottom:.5px solid gray;font-size:.9rem;margin-bottom:-1px}.error-row>span{font-weight:200}.error-help{font-weight:200;font-style:italic}.kata-override{background-color:var(--main-background)}.results-column{grid-area:results;margin-left:0;margin-top:32px;margin-right:120px}.active-tab{font-size:1.1rem;font-weight:600;text-decoration:underline}.results-labels{display:flex;height:32px}.results-labels>div{margin-right:40px;text-align:left;vertical-align:middle;cursor:pointer}.ast-output,.hir-output,.qir-output{height:40vh;min-height:400px;width:100%;resize:none;white-space:pre}.output-header{font-size:1.1rem;font-weight:400;margin-top:16px;margin-bottom:16px;display:flex;justify-content:space-between}.prev-next{font-weight:200;cursor:pointer}.result-label{margin-bottom:24px;font-style:italic;font-weight:300}.message-output{font-weight:300;font-size:1.1rem;margin-bottom:16px}.state-table{border-collapse:collapse;font-size:.9rem;width:100%;min-width:400px;margin-bottom:16px}.state-table thead tr{background:var(--nav-background)}.state-table tbody tr{border-top:1px solid gray}.state-table td,.state-table th{text-align:center;padding:6px;white-space:nowrap}.state-table progress{margin-right:2px}.histogram{max-height:calc(100vh - 40px);max-width:600px;border:1px solid var(--border-color);background-color:var(--vscode-sideBar-background, white)}.bar{fill:var(--vscode-button-background, var(--nav-background))}.bar:hover{fill:var(--vscode-button-hoverBackground, var(--nav-hover-background))}.bar-selected{stroke:var(--bar-selected-outline);fill:var(--nav-current-background)}.bar-label{font-size:3pt;fill:var(--vscode-button-foreground, var(--main-color));text-anchor:end;pointer-events:none}.histo-label{font-size:3.5pt;fill:var(--vscode-foreground, #3b3b3b)}.hover-text{font-size:3.5pt;fill:gray;text-anchor:middle}.menu-icon *{stroke:#000;fill:var(--vscode-sideBar-background, white);stroke:var(--vscode-icon-foreground, #3b3b3b)}.menu-box{fill:var(--menu-box-fill);stroke:#000;stroke-width:.1}.menu-item{width:32px;height:10px;fill:var(--vscode-list-inactiveSelectionBackground, var(--nav-background));stroke:gray;stroke-width:.2}.menu-item:hover{stroke-width:.6;fill:var(--vscode-list-hoverBackground, var(--nav-hover-background))}.menu-selected{fill:var( --vscode-list-activeSelectionBackground, var(--nav-current-background) )}.menu-text{font-size:4.5px;pointer-events:none;fill:var(--main-color)}.menu-separator{stroke:gray;stroke-width:.25}.help-info{fill:var(--menu-box-fill);stroke:gray;stroke-width:.5}.help-info-text{font-size:4.5px;pointer-events:none;fill:var(--main-color)}.estimate-details{padding:1em}.estimate-details>summary{font-size:1.1em}.estimate-table{margin-top:1em;font-size:.9em}.estimate-table tr:nth-child(2n){background-color:var(--qs-tr-nth-color)}.estimate-cell{vertical-align:top;padding-right:8px}.title-cell{font-weight:700;white-space:nowrap}.value-cell{text-align:center;width:100px;white-space:nowrap}.estimate-explanation{margin-top:1em;margin-bottom:1em;max-width:500px}.estimate-assumption{margin:1em}.cell-output-ipywidget-background{background-color:transparent!important}#pieChart{fill:var(--main-color)}.spaceReport{display:flex;flex-direction:column}.spaceReportHeader{font-size:13px;background-color:var(--qs-tr-nth-color);border-top:.5px gray solid;border-bottom:.5px gray solid;padding:10px}.spaceReportRow{display:flex;font-size:12px;padding:10px 24px}.spaceDetailText{width:200px}.qs-help{font-size:14px;line-height:1.5;word-wrap:break-word}.qs-help h1{margin-top:16px;margin-bottom:8px;line-height:1.25;font-weight:600;padding-bottom:.3em;font-size:2em;border-bottom:1px solid var(--vscode-editorWidget-border)}.qs-help h2{margin-top:16px;margin-bottom:8px;font-weight:600;line-height:1.25;padding-bottom:.3em;font-size:1.4em;border-bottom:1px solid var(--vscode-editorWidget-border)}.qs-resultsTable-sortedTable{border-collapse:collapse;margin:12px 0;outline:none}.qs-resultsTable-sortedTable th,.qs-resultsTable-sortedTable td{padding:4px 8px;text-align:left}.qs-resultsTable-dragEnter{background-color:#8888;border-left:1.5px solid blue;border-right:1.5px solid blue}.qs-resultsTable-sortedTable tr:nth-child(2n){background:var(--qs-tr-nth-color)}.qs-resultsTable-sortedTable tbody tr:hover{background:var(--vscode-list-hoverBackground, var(--js-layout-color2))}.qs-resultsTable-sortedTableSelectedRow td{background:var(--vscode-button-background, var(--jp-layout-color3));color:var(--vscode-button-foreground);font-weight:600}.qs-resultsTable-columnMenu{display:none;width:160px}.qs-resultsTable-showColumnMenu{display:block;position:absolute;background-color:var(--vscode-menu-background, var(--main-background));border:1px solid #8888;padding:4px;z-index:100;text-align:left}.qs-resultsTable-menuItem{cursor:pointer;background-color:var(--vscode-list-hoverBackground, var(--jp-layout-color1));padding:4px;margin:2px;font-size:14px;font-weight:400}.qs-resultsTable-menuItem:hover{background-color:var(--vscode-menu-border, var(--jp-layout-color2))}.qs-resultsTable-columnSelected{cursor:pointer;padding:4px;font-weight:400;font-size:14px;background-color:var(--vscode-button-background, var(--jp-brand-color1));color:var(--vscode-button-foreground, var(--jp-ui-inverse-font-color0));margin:2px;border-radius:3px}.qs-resultsTable-headerCell{padding-right:20px}.qs-resultsTable-sortHeaderCell{padding-right:4px}@keyframes codicon-spin{to{transform:rotate(360deg);transform-origin:center}}.codicon-modifier-spin{fill:var(--vscode-icon-foreground, gray);animation:codicon-spin 1.5s steps(45) infinite}.qs-scatterChart-x-axisTitle,.qs-scatterChart-y-axisTitle{text-anchor:middle;font-size:16px;fill:var(--main-color)}.qs-scatterChart-y-axisTitle{writing-mode:vertical-lr;transform:rotate(180deg)}.qs-scatterChart-point{r:2px;stroke-width:4px}.qs-scatterChart-hover:hover{r:4px;stroke-width:4px;fill:#fff}.qs-scatterChart-point-selected{r:8px;stroke-width:4px;fill:#fff}.qs-scatterChart-watermark{font-size:16px;fill:var(--main-color)}.qs-scatterChart-tooltip,.qs-scatterChart-selectedInfo{position:absolute;visibility:hidden;background:var(--main-background);color:var(--main-color);border:var(--border-color) 1px solid;padding:4px}.qs-scatterChart-tooltip:after,.qs-scatterChart-selectedInfo:after{content:"";position:absolute;bottom:100%;left:50%;margin-left:-5px;border-width:5px;border-style:solid;border-color:transparent transparent var(--border-color) transparent}.qs-scatterChart-axis,.qs-scatterChart-tick-line{stroke:var(--border-color)}.qs-scatterChart-x-tick-text{text-anchor:middle;fill:var(--main-color)}.qs-scatterChart-y-tick-text{text-anchor:end;fill:var(--main-color)}.qs-estimatesOverview-error{color:red}.qs-circuit-panel p,.qs-circuit-error,.qs-circuit-error p{padding:10px 0}.qs-circuit{background:var(--main-background)}.qs-circuit line,.qs-circuit circle,.qs-circuit rect{stroke:var(--main-color);stroke-width:1}.qs-circuit text{fill:var(--main-color);dominant-baseline:middle;text-anchor:middle;font-family:Arial}.qs-circuit .gate-unitary{fill:var(--vscode-button-secondaryBackground, #d9f1fa)}.qs-circuit .gate text{fill:var(--vscode-button-secondaryForeground, #000000)}.qs-circuit .gate>line,.qs-circuit .control-dot{fill:var(--main-color)}.qs-circuit .gate>.oplus>line,.qs-circuit .gate>.oplus>circle{fill:var(--main-background);stroke:var(--main-color);stroke-width:2}.qs-circuit .gate-measure{fill:var(--vscode-button-background, #ffde86)}.qs-circuit .gate>g>line,.qs-circuit .arc-measure{stroke:var(--vscode-button-foreground, #000000);fill:none;stroke-width:1}.qs-circuit rect.gate-swap{fill:transparent;stroke:transparent}.qs-circuit .register-classical{stroke-width:.5}.qs-circuit .hidden{display:none}.qs-circuit .classically-controlled-unknown{opacity:.25}.qs-circuit .classically-controlled-one .classical-container,.qs-circuit .classically-controlled-one .classical-line{stroke:#4059bd;stroke-width:1.3;fill:#4059bd;fill-opacity:.1}.qs-circuit .classically-controlled-zero .classical-container,.qs-circuit .classically-controlled-zero .classical-line{stroke:#c40000;stroke-width:1.3;fill:#c40000;fill-opacity:.1}.qs-circuit .classically-controlled-btn{cursor:pointer}.qs-circuit .classically-controlled-unknown .classically-controlled-btn{fill:#e5e5e5}.qs-circuit .classically-controlled-one .classically-controlled-btn{fill:#4059bd}.qs-circuit .classically-controlled-zero .classically-controlled-btn{fill:#c40000}.qs-circuit .classically-controlled-btn text{dominant-baseline:middle;text-anchor:middle;stroke:none;font-family:Arial}.qs-circuit .classically-controlled-unknown .classically-controlled-btn text{fill:#000}.qs-circuit .classically-controlled-one .classically-controlled-btn text{fill:#fff}.qs-circuit .classically-controlled-zero .classically-controlled-btn text{fill:#fff}.qs-circuit .qviz .gate-collapse,.qs-circuit .qviz .gate-expand{opacity:0;transition:opacity 1s}.qs-circuit .qviz:hover .gate-collapse,.qs-circuit .qviz:hover .gate-expand{visibility:visible;opacity:.2;transition:visibility 1s;transition:opacity 1s}.qs-circuit .gate-expand,.gate-collapse{cursor:pointer}.qs-circuit .gate-collapse circle,.qs-circuit .gate-expand circle{fill:#fff;stroke-width:2px;stroke:#000}.qs-circuit .gate-collapse path,.qs-circuit .gate-expand path{stroke-width:4px;stroke:#000}.qs-circuit .gate:hover>.gate-collapse,.qs-circuit .gate:hover>.gate-expand{visibility:visible;opacity:1;transition:opacity 1s}
```

## qsharp_widgets/static/index.js

### js-beautify {}

```diff
@@ -1,38 +1,38 @@
-var rh = Object.create;
-var na = Object.defineProperty;
-var nh = Object.getOwnPropertyDescriptor;
-var ih = Object.getOwnPropertyNames;
-var oh = Object.getPrototypeOf,
-    ah = Object.prototype.hasOwnProperty;
+var ih = Object.create;
+var oa = Object.defineProperty;
+var oh = Object.getOwnPropertyDescriptor;
+var ah = Object.getOwnPropertyNames;
+var sh = Object.getPrototypeOf,
+    lh = Object.prototype.hasOwnProperty;
 var W = (r, e) => () => (e || r((e = {
     exports: {}
 }).exports, e), e.exports);
-var sh = (r, e, i, a) => {
+var ch = (r, e, i, a) => {
     if (e && typeof e == "object" || typeof e == "function")
-        for (let l of ih(e)) !ah.call(r, l) && l !== i && na(r, l, {
+        for (let l of ah(e)) !lh.call(r, l) && l !== i && oa(r, l, {
             get: () => e[l],
-            enumerable: !(a = nh(e, l)) || a.enumerable
+            enumerable: !(a = oh(e, l)) || a.enumerable
         });
     return r
 };
-var Mn = (r, e, i) => (i = r != null ? rh(oh(r)) : {}, sh(e || !r || !r.__esModule ? na(i, "default", {
+var En = (r, e, i) => (i = r != null ? ih(sh(r)) : {}, ch(e || !r || !r.__esModule ? oa(i, "default", {
     value: r,
     enumerable: !0
 }) : i, r));
-var $n = W(Dr => {
+var Vn = W(Dr => {
     "use strict";
     Object.defineProperty(Dr, "__esModule", {
         value: !0
     });
     Dr.RegisterType = void 0;
-    var Bh;
+    var Lh;
     (function(r) {
         r[r.Qubit = 0] = "Qubit", r[r.Classical = 1] = "Classical"
-    })(Bh = Dr.RegisterType || (Dr.RegisterType = {}))
+    })(Lh = Dr.RegisterType || (Dr.RegisterType = {}))
 });
 var Wt = W(me => {
     "use strict";
     Object.defineProperty(me, "__esModule", {
         value: !0
     });
     me.regLineStart = me.argsFontSize = me.labelFontSize = me.controlBtnRadius = me.controlBtnOffset = me.nestedGroupPadding = me.groupBoxPadding = me.classicalRegHeight = me.registerHeight = me.labelPadding = me.gatePadding = me.gateHeight = me.minGateWidth = me.startY = me.startX = me.leftPadding = me.svgNS = void 0;
@@ -50,223 +50,223 @@
     me.nestedGroupPadding = 2;
     me.controlBtnOffset = 40;
     me.controlBtnRadius = 15;
     me.labelFontSize = 14;
     me.argsFontSize = 12;
     me.regLineStart = 40
 });
-var y0 = W(_e => {
+var x0 = W(_e => {
     "use strict";
     Object.defineProperty(_e, "__esModule", {
         value: !0
     });
     _e.dashedBox = _e.dashedLine = _e.arc = _e.text = _e.box = _e.controlDot = _e.circle = _e.line = _e.group = _e.createSvgElement = void 0;
-    var Ia = Wt(),
-        Nh = function(r, e) {
+    var Ha = Wt(),
+        Ph = function(r, e) {
             e === void 0 && (e = {});
-            var i = document.createElementNS(Ia.svgNS, r);
+            var i = document.createElementNS(Ha.svgNS, r);
             return Object.entries(e).forEach(function(a) {
                 var l = a[0],
                     c = a[1];
                 return i.setAttribute(l, c)
             }), i
         };
-    _e.createSvgElement = Nh;
-    var Lh = function(r, e) {
+    _e.createSvgElement = Ph;
+    var Ih = function(r, e) {
         e === void 0 && (e = {});
         var i = (0, _e.createSvgElement)("g", e);
         return r.forEach(function(a) {
             return i.appendChild(a)
         }), i
     };
-    _e.group = Lh;
-    var Ph = function(r, e, i, a, l) {
+    _e.group = Ih;
+    var Oh = function(r, e, i, a, l) {
         var c = {
             x1: r.toString(),
             x2: i.toString(),
             y1: e.toString(),
             y2: a.toString()
         };
         return l != null && (c.class = l), (0, _e.createSvgElement)("line", c)
     };
-    _e.line = Ph;
-    var Ih = function(r, e, i, a) {
+    _e.line = Oh;
+    var Hh = function(r, e, i, a) {
         var l = {
             cx: r.toString(),
             cy: e.toString(),
             r: i.toString()
         };
         return a != null && (l.class = a), (0, _e.createSvgElement)("circle", l)
     };
-    _e.circle = Ih;
-    var Oh = function(r, e, i) {
+    _e.circle = Hh;
+    var $h = function(r, e, i) {
         return i === void 0 && (i = 5), (0, _e.circle)(r, e, i, "control-dot")
     };
-    _e.controlDot = Oh;
-    var Hh = function(r, e, i, a, l) {
+    _e.controlDot = $h;
+    var Gh = function(r, e, i, a, l) {
         return l === void 0 && (l = "gate-unitary"), (0, _e.createSvgElement)("rect", {
             class: l,
             x: r.toString(),
             y: e.toString(),
             width: i.toString(),
             height: a.toString()
         })
     };
-    _e.box = Hh;
-    var $h = function(r, e, i, a) {
-        a === void 0 && (a = Ia.labelFontSize);
+    _e.box = Gh;
+    var Vh = function(r, e, i, a) {
+        a === void 0 && (a = Ha.labelFontSize);
         var l = (0, _e.createSvgElement)("text", {
             "font-size": a.toString(),
             x: e.toString(),
             y: i.toString()
         });
         return l.textContent = r, l
     };
-    _e.text = $h;
-    var Gh = function(r, e, i, a) {
+    _e.text = Vh;
+    var jh = function(r, e, i, a) {
         return (0, _e.createSvgElement)("path", {
             class: "arc-measure",
             d: "M ".concat(r + 2 * i, " ").concat(e, " A ").concat(i, " ").concat(a, " 0 0 0 ").concat(r, " ").concat(e)
         })
     };
-    _e.arc = Gh;
-    var Vh = function(r, e, i, a, l) {
+    _e.arc = jh;
+    var Uh = function(r, e, i, a, l) {
         var c = (0, _e.line)(r, e, i, a, l);
         return c.setAttribute("stroke-dasharray", "8, 8"), c
     };
-    _e.dashedLine = Vh;
-    var jh = function(r, e, i, a, l) {
+    _e.dashedLine = Uh;
+    var Wh = function(r, e, i, a, l) {
         var c = (0, _e.box)(r, e, i, a, l);
         return c.setAttribute("fill-opacity", "0"), c.setAttribute("stroke-dasharray", "8, 8"), c
     };
-    _e.dashedBox = jh
+    _e.dashedBox = Wh
 });
-var Ga = W(ur => {
+var ja = W(ur => {
     "use strict";
     Object.defineProperty(ur, "__esModule", {
         value: !0
     });
     ur._qubitInput = ur.formatInputs = void 0;
-    var Oa = $n(),
+    var $a = Vn(),
         zr = Wt(),
-        Ha = y0(),
-        Uh = function(r) {
+        Ga = x0(),
+        Yh = function(r) {
             var e = [],
                 i = {},
                 a = zr.startY;
             return r.forEach(function(l) {
                 var c = l.id,
                     d = l.numChildren;
-                if (e.push($a(a)), i[c] = {
-                        type: Oa.RegisterType.Qubit,
+                if (e.push(Va(a)), i[c] = {
+                        type: $a.RegisterType.Qubit,
                         y: a
                     }, d == null || d === 0) {
                     a += zr.registerHeight;
                     return
                 }
                 a += zr.classicalRegHeight, i[c].children = Array.from(Array(d), function() {
                     var f = {
-                        type: Oa.RegisterType.Classical,
+                        type: $a.RegisterType.Classical,
                         y: a
                     };
                     return a += zr.classicalRegHeight, f
                 })
             }), {
-                qubitWires: (0, Ha.group)(e),
+                qubitWires: (0, Ga.group)(e),
                 registers: i,
                 svgHeight: a
             }
         };
-    ur.formatInputs = Uh;
-    var $a = function(r) {
-        var e = (0, Ha.text)("|0\u27E9", zr.leftPadding, r, 16);
+    ur.formatInputs = Yh;
+    var Va = function(r) {
+        var e = (0, Ga.text)("|0\u27E9", zr.leftPadding, r, 16);
         return e.setAttribute("text-anchor", "start"), e.setAttribute("dominant-baseline", "middle"), e
     };
-    ur._qubitInput = $a
+    ur._qubitInput = Va
 });
 var hr = W(Rr => {
     "use strict";
     Object.defineProperty(Rr, "__esModule", {
         value: !0
     });
     Rr.GateType = void 0;
-    var Wh;
+    var Zh;
     (function(r) {
         r[r.Measure = 0] = "Measure", r[r.Cnot = 1] = "Cnot", r[r.Swap = 2] = "Swap", r[r.X = 3] = "X", r[r.Unitary = 4] = "Unitary", r[r.ControlledUnitary = 5] = "ControlledUnitary", r[r.ClassicalControlled = 6] = "ClassicalControlled", r[r.Group = 7] = "Group", r[r.Invalid = 8] = "Invalid"
-    })(Wh = Rr.GateType || (Rr.GateType = {}))
+    })(Zh = Rr.GateType || (Rr.GateType = {}))
 });
-var Ja = W(Le => {
+var es = W(Le => {
     "use strict";
     var Nt = Le && Le.__spreadArray || function(r, e, i) {
         if (i || arguments.length === 2)
             for (var a = 0, l = e.length, c; a < l; a++)(c || !(a in e)) && (c || (c = Array.prototype.slice.call(e, 0, a)), c[a] = e[a]);
         return r.concat(c || Array.prototype.slice.call(e))
     };
     Object.defineProperty(Le, "__esModule", {
         value: !0
     });
     Le._classicalControlled = Le._groupedOperations = Le._controlledGate = Le._swap = Le._unitary = Le._measure = Le._zoomButton = Le._createGate = Le._formatGate = Le.formatGates = void 0;
     var gt = hr(),
         Re = Wt(),
-        be = y0(),
-        x0 = function(r, e) {
+        be = x0(),
+        v0 = function(r, e) {
             e === void 0 && (e = 0);
             var i = r.map(function(a) {
-                return Va(a, e)
+                return Ua(a, e)
             });
             return (0, be.group)(i)
         };
-    Le.formatGates = x0;
-    var Va = function(r, e) {
+    Le.formatGates = v0;
+    var Ua = function(r, e) {
         e === void 0 && (e = 0);
         var i = r.type,
             a = r.x,
             l = r.controlsY,
             c = r.targetsY,
             d = r.label,
             f = r.displayArgs,
             g = r.width;
         switch (i) {
             case gt.GateType.Measure:
-                return nr([Ua(a, l[0])], r, e);
+                return nr([Ya(a, l[0])], r, e);
             case gt.GateType.Unitary:
-                return nr([jn(d, a, c, g, f)], r, e);
+                return nr([Wn(d, a, c, g, f)], r, e);
             case gt.GateType.X:
-                return nr([Zh(r, e)], r, e);
+                return nr([Xh(r, e)], r, e);
             case gt.GateType.Swap:
-                return l.length > 0 ? Gn(r, e) : nr([Wa(r, e)], r, e);
+                return l.length > 0 ? jn(r, e) : nr([Za(r, e)], r, e);
             case gt.GateType.Cnot:
             case gt.GateType.ControlledUnitary:
-                return Gn(r, e);
+                return jn(r, e);
             case gt.GateType.Group:
-                return Qa(r, e);
+                return Ja(r, e);
             case gt.GateType.ClassicalControlled:
-                return Xa(r);
+                return Ka(r);
             default:
                 throw new Error("ERROR: unknown gate (".concat(d, ") of type ").concat(i, "."))
         }
     };
-    Le._formatGate = Va;
+    Le._formatGate = Ua;
     var nr = function(r, e, i) {
         var a = (e || {}).dataAttributes,
             l = {
                 class: "gate"
             };
         Object.entries(a || {}).forEach(function(d) {
             var f = d[0],
                 g = d[1];
             return l["data-".concat(f)] = g
         });
-        var c = ja(e, i);
+        var c = Wa(e, i);
         return c != null && (r = r.concat([c])), (0, be.group)(r, l)
     };
     Le._createGate = nr;
-    var ja = function(r, e) {
+    var Wa = function(r, e) {
         if (r == null) return null;
-        var i = Vn(r, e),
+        var i = Un(r, e),
             a = i[0],
             l = i[1],
             c = r.dataAttributes;
         c = c || {};
         var d = "expanded" in c,
             f = a + 2,
             g = l + 2,
@@ -286,16 +286,16 @@
                 w = [y, T];
             return (0, be.group)(w, {
                 class: "gate-control gate-expand"
             })
         }
         return null
     };
-    Le._zoomButton = ja;
-    var Vn = function(r, e) {
+    Le._zoomButton = Wa;
+    var Un = function(r, e) {
             var i = r.x,
                 a = r.width,
                 l = r.type,
                 c = r.targetsY,
                 d = c?.flatMap(function(L) {
                     return L
                 }) || [],
@@ -307,166 +307,166 @@
                     var A = Re.groupBoxPadding - e * Re.nestedGroupPadding;
                     return y = i - 2 * A, _ = g - Re.gateHeight / 2 - A, w = a + 2 * A, T = f + +Re.gateHeight / 2 + A - (g - Re.gateHeight / 2 - A), [y, _, w, T];
                 default:
                     y = i - a / 2, _ = g - Re.gateHeight / 2, w = i + a, T = f + Re.gateHeight / 2
             }
             return [y, _, w, T]
         },
-        Ua = function(r, e) {
+        Ya = function(r, e) {
             r -= Re.minGateWidth / 2;
             var i = Re.minGateWidth,
                 a = Re.gateHeight,
                 l = (0, be.box)(r, e - a / 2, i, a, "gate-measure"),
                 c = (0, be.arc)(r + 5, e + 2, i / 2 - 5, a / 2 - 8),
                 d = (0, be.line)(r + i / 2, e + 8, r + i - 8, e - a / 2 + 8);
             return (0, be.group)([l, c, d])
         };
-    Le._measure = Ua;
-    var jn = function(r, e, i, a, l, c) {
+    Le._measure = Ya;
+    var Wn = function(r, e, i, a, l, c) {
         if (c === void 0 && (c = !0), i.length === 0) throw new Error("Failed to render unitary gate (".concat(r, "): has no y-values"));
         var d = i.map(function(T) {
             var A = T[T.length - 1],
                 L = T[0],
                 R = A - L + Re.gateHeight;
-            return Yh(r, e, L, a, R, l)
+            return Qh(r, e, L, a, R, l)
         });
         if (c && d.length > 1) {
             var f = i[i.length - 1],
                 g = i[0],
                 y = f[f.length - 1],
                 _ = g[0],
                 w = (0, be.dashedLine)(e, _, e, y);
             return (0, be.group)(Nt([w], d, !0))
         }
         return (0, be.group)(d)
     };
-    Le._unitary = jn;
-    var Yh = function(r, e, i, a, l, c) {
+    Le._unitary = Wn;
+    var Qh = function(r, e, i, a, l, c) {
             l === void 0 && (l = Re.gateHeight), i -= Re.gateHeight / 2;
             var d = (0, be.box)(e - a / 2, i, a, l),
                 f = i + l / 2 - (c == null ? 0 : 7),
                 g = (0, be.text)(r, e, f),
                 y = [d, g];
             if (c != null) {
                 var _ = i + l / 2 + 8,
                     w = (0, be.text)(c, e, _, Re.argsFontSize);
                 y.push(w)
             }
             return (0, be.group)(y)
         },
-        Wa = function(r, e) {
+        Za = function(r, e) {
             var i = r.x,
                 a = r.targetsY,
-                l = Vn(r, e),
+                l = Un(r, e),
                 c = l[0],
                 d = l[1],
                 f = l[2],
                 g = l[3],
                 y = a?.flatMap(function(A) {
                     return A
                 }) || [],
                 _ = (0, be.box)(c, d, f, g, "gate-swap"),
                 w = y.map(function(A) {
-                    return Ya(i, A)
+                    return Qa(i, A)
                 }),
                 T = (0, be.line)(i, y[0], i, y[1]);
             return (0, be.group)(Nt(Nt([_], w, !0), [T], !1))
         };
-    Le._swap = Wa;
-    var Zh = function(r, e) {
+    Le._swap = Za;
+    var Xh = function(r, e) {
             var i = r.x,
                 a = r.targetsY,
                 l = a.flatMap(function(c) {
                     return c
                 });
-            return Za(i, l[0])
+            return Xa(i, l[0])
         },
-        Ya = function(r, e) {
+        Qa = function(r, e) {
             var i = 8,
                 a = (0, be.line)(r - i, e - i, r + i, e + i),
                 l = (0, be.line)(r - i, e + i, r + i, e - i);
             return (0, be.group)([a, l])
         },
-        Gn = function(r, e) {
+        jn = function(r, e) {
             var i = [],
                 a = r.type,
                 l = r.x,
                 c = r.controlsY,
                 d = r.label,
                 f = r.displayArgs,
                 g = r.width,
                 y = r.targetsY;
             switch (a) {
                 case gt.GateType.Cnot:
                     y.forEach(function(O) {
-                        return i.push(Za(l, O))
+                        return i.push(Xa(l, O))
                     });
                     break;
                 case gt.GateType.Swap:
                     y.forEach(function(O) {
-                        return i.push(Ya(l, O))
+                        return i.push(Qa(l, O))
                     });
                     break;
                 case gt.GateType.ControlledUnitary:
                     var _ = y;
-                    i.push(jn(d, l, _, g, f, !1)), y = y.flat();
+                    i.push(Wn(d, l, _, g, f, !1)), y = y.flat();
                     break;
                 default:
                     throw new Error("ERROR: Unrecognized gate: ".concat(d, " of type ").concat(a))
             }
             var w = c.map(function(O) {
                     return (0, be.controlDot)(l, O)
                 }),
                 T = Math.max.apply(Math, Nt(Nt([], c, !1), y, !1)),
                 A = Math.min.apply(Math, Nt(Nt([], c, !1), y, !1)),
                 L = (0, be.line)(l, A, l, T),
                 R = nr(Nt(Nt([L], w, !0), i, !0), r, e);
             return R
         };
-    Le._controlledGate = Gn;
-    var Za = function(r, e, i) {
+    Le._controlledGate = jn;
+    var Xa = function(r, e, i) {
             i === void 0 && (i = 15);
             var a = (0, be.circle)(r, e, i),
                 l = (0, be.line)(r, e - i, r, e + i),
                 c = (0, be.line)(r - i, e, r + i, e);
             return (0, be.group)([a, l, c], {
                 class: "oplus"
             })
         },
-        Qa = function(r, e) {
+        Ja = function(r, e) {
             var i = r.children,
-                a = Vn(r, e),
+                a = Un(r, e),
                 l = a[0],
                 c = a[1],
                 d = a[2],
                 f = a[3],
                 g = (0, be.dashedBox)(l, c, d, f),
                 y = [g];
-            return i != null && y.push(x0(i, e + 1)), nr(y, r, e)
+            return i != null && y.push(v0(i, e + 1)), nr(y, r, e)
         };
-    Le._groupedOperations = Qa;
-    var Xa = function(r, e) {
+    Le._groupedOperations = Ja;
+    var Ka = function(r, e) {
         e === void 0 && (e = Re.groupBoxPadding);
         var i = r.controlsY,
             a = r.dataAttributes,
             l = r.targetsY,
             c = r.children,
             d = r.x,
             f = r.width,
             g = i[0],
             y = [];
         if (c != null) {
             if (c.length !== 2) throw new Error("Invalid number of children found for classically-controlled gate: ".concat(c.length));
-            var _ = x0(c[0]);
+            var _ = v0(c[0]);
             _.setAttribute("class", "gates-zero"), y.push(_);
-            var w = x0(c[1]);
+            var w = v0(c[1]);
             w.setAttribute("class", "gates-one"), y.push(w)
         }
         var T = d + Re.controlBtnRadius,
-            A = Qh(T, g),
+            A = Jh(T, g),
             L = g + Re.controlBtnRadius,
             R = g + Re.classicalRegHeight / 2,
             O = (0, be.dashedLine)(T, L, T, R, "classical-line");
         d += Re.controlBtnOffset;
         var P = (0, be.dashedLine)(T, R, d, R, "classical-line");
         f = f - Re.controlBtnOffset + (e - Re.groupBoxPadding) * 2, d += Re.groupBoxPadding - e;
         var I = l[0] - Re.gateHeight / 2 - e,
@@ -478,194 +478,194 @@
         };
         return a != null && Object.entries(a).forEach(function(j) {
             var ne = j[0],
                 pe = j[1];
             return te["data-".concat(ne)] = pe
         }), (0, be.group)(y, te)
     };
-    Le._classicalControlled = Xa;
-    var Qh = function(r, e, i) {
+    Le._classicalControlled = Ka;
+    var Jh = function(r, e, i) {
         return i === void 0 && (i = Re.controlBtnRadius), (0, be.group)([(0, be.circle)(r, e, i), (0, be.text)("?", r, e, Re.labelFontSize)], {
             class: "classically-controlled-btn"
         })
     }
 });
-var rs = W(Yt => {
+var is = W(Yt => {
     "use strict";
     Object.defineProperty(Yt, "__esModule", {
         value: !0
     });
     Yt._qubitRegister = Yt._classicalRegister = Yt.formatRegisters = void 0;
-    var Ka = Wt(),
-        Xh = hr(),
-        Lt = y0(),
-        Jh = function(r, e, i) {
+    var ts = Wt(),
+        Kh = hr(),
+        Lt = x0(),
+        ed = function(r, e, i) {
             var a = [];
-            for (var l in r) a.push(ts(Number(l), i, r[l].y));
+            for (var l in r) a.push(ns(Number(l), i, r[l].y));
             return e.forEach(function(c) {
                 var d = c.type,
                     f = c.x,
                     g = c.targetsY,
                     y = c.controlsY;
-                if (d === Xh.GateType.Measure) {
+                if (d === Kh.GateType.Measure) {
                     var _ = y[0];
                     g.forEach(function(w) {
-                        a.push(es(f, _, i, w))
+                        a.push(rs(f, _, i, w))
                     })
                 }
             }), (0, Lt.group)(a)
         };
-    Yt.formatRegisters = Jh;
-    var es = function(r, e, i, a) {
+    Yt.formatRegisters = ed;
+    var rs = function(r, e, i, a) {
         var l = 1,
             c = (0, Lt.line)(r + l, e, r + l, a - l, "register-classical"),
             d = (0, Lt.line)(r - l, e, r - l, a + l, "register-classical"),
             f = (0, Lt.line)(r + l, a - l, i, a - l, "register-classical"),
             g = (0, Lt.line)(r - l, a + l, i, a + l, "register-classical");
         return (0, Lt.group)([c, d, f, g])
     };
-    Yt._classicalRegister = es;
-    var ts = function(r, e, i, a) {
+    Yt._classicalRegister = rs;
+    var ns = function(r, e, i, a) {
         a === void 0 && (a = 16);
-        var l = (0, Lt.line)(Ka.regLineStart, i, e, i),
-            c = (0, Lt.text)("q".concat(r), Ka.regLineStart, i - a);
+        var l = (0, Lt.line)(ts.regLineStart, i, e, i),
+            c = (0, Lt.text)("q".concat(r), ts.regLineStart, i - a);
         return c.setAttribute("dominant-baseline", "hanging"), c.setAttribute("text-anchor", "start"), c.setAttribute("font-size", "75%"), (0, Lt.group)([l, c])
     };
-    Yt._qubitRegister = ts
+    Yt._qubitRegister = ns
 });
-var Un = W(Fr => {
+var Yn = W(Fr => {
     "use strict";
     Object.defineProperty(Fr, "__esModule", {
         value: !0
     });
     Fr.ConditionalRender = void 0;
-    var Kh;
+    var td;
     (function(r) {
         r[r.Always = 0] = "Always", r[r.OnZero = 1] = "OnZero", r[r.OnOne = 2] = "OnOne", r[r.AsGroup = 3] = "AsGroup"
-    })(Kh = Fr.ConditionalRender || (Fr.ConditionalRender = {}))
+    })(td = Fr.ConditionalRender || (Fr.ConditionalRender = {}))
 });
-var Zn = W(Zt => {
+var Xn = W(Zt => {
     "use strict";
     Object.defineProperty(Zt, "__esModule", {
         value: !0
     });
     Zt._getStringWidth = Zt.getGateWidth = Zt.createUUID = void 0;
-    var Wn = hr(),
+    var Zn = hr(),
         Br = Wt(),
-        ed = function() {
+        rd = function() {
             return "xxxxxxxx-xxxx-4xxx-yxxx-xxxxxxxxxxxx".replace(/[xy]/g, function(r) {
                 var e = Math.random() * 16 | 0,
                     i = r == "x" ? e : e & 3 | 8;
                 return i.toString(16)
             })
         };
-    Zt.createUUID = ed;
-    var td = function(r) {
+    Zt.createUUID = rd;
+    var nd = function(r) {
         var e = r.type,
             i = r.label,
             a = r.displayArgs,
             l = r.width;
         if (l > 0) return l;
         switch (e) {
-            case Wn.GateType.Measure:
-            case Wn.GateType.Cnot:
-            case Wn.GateType.Swap:
+            case Zn.GateType.Measure:
+            case Zn.GateType.Cnot:
+            case Zn.GateType.Swap:
                 return Br.minGateWidth;
             default:
-                var c = Yn(i),
-                    d = a != null ? Yn(a, Br.argsFontSize) : 0,
+                var c = Qn(i),
+                    d = a != null ? Qn(a, Br.argsFontSize) : 0,
                     f = Math.max(c, d) + Br.labelPadding * 2;
                 return Math.max(Br.minGateWidth, f)
         }
     };
-    Zt.getGateWidth = td;
-    var Yn = function(r, e) {
+    Zt.getGateWidth = nd;
+    var Qn = function(r, e) {
         e === void 0 && (e = Br.labelFontSize);
         var i = document.createElement("canvas"),
             a = i.getContext("2d");
         if (a == null) throw new Error("Null canvas");
         a.font = "".concat(e, "px Arial");
         var l = a.measureText(r);
         return l.width
     };
-    Zt._getStringWidth = Yn
+    Zt._getStringWidth = Qn
 });
-var cs = W(Pe => {
+var hs = W(Pe => {
     "use strict";
-    var w0 = Pe && Pe.__assign || function() {
-            return w0 = Object.assign || function(r) {
+    var k0 = Pe && Pe.__assign || function() {
+            return k0 = Object.assign || function(r) {
                 for (var e, i = 1, a = arguments.length; i < a; i++) {
                     e = arguments[i];
                     for (var l in e) Object.prototype.hasOwnProperty.call(e, l) && (r[l] = e[l])
                 }
                 return r
-            }, w0.apply(this, arguments)
+            }, k0.apply(this, arguments)
         },
         dr = Pe && Pe.__spreadArray || function(r, e, i) {
             if (i || arguments.length === 2)
                 for (var a = 0, l = e.length, c; a < l; a++)(c || !(a in e)) && (c || (c = Array.prototype.slice.call(e, 0, a)), c[a] = e[a]);
             return r.concat(c || Array.prototype.slice.call(e))
         };
     Object.defineProperty(Pe, "__esModule", {
         value: !0
     });
     Pe._offsetChildrenX = Pe._fillMetadataX = Pe._splitTargetsY = Pe._getRegY = Pe._opToMetadata = Pe._getClassicalRegStart = Pe._alignOps = Pe._groupOperations = Pe.processOperations = void 0;
     var ot = Wt(),
-        Qn = Un(),
+        Jn = Yn(),
         rt = hr(),
-        ir = $n(),
-        rd = Zn(),
-        v0 = function(r, e) {
+        ir = Vn(),
+        id = Xn(),
+        w0 = function(r, e) {
             if (r.length === 0) return {
                 metadataList: [],
                 svgWidth: ot.startX
             };
-            var i = ns(r, e),
-                a = is(i),
+            var i = os(r, e),
+                a = as(i),
                 l = Math.max.apply(Math, dr([0], a.map(function(w) {
                     return w.length
                 }), !1)),
                 c = new Array(l).fill(ot.minGateWidth),
-                d = os(r, a),
+                d = ss(r, a),
                 f = {},
                 g = a.map(function(w) {
                     return w.map(function(T, A) {
                         var L = null;
                         T != null && !f.hasOwnProperty(T) && (L = r[T], f[T] = !0);
-                        var R = as(L, e);
+                        var R = ls(L, e);
                         if (L != null && [rt.GateType.Unitary, rt.GateType.ControlledUnitary].includes(R.type)) {
                             var O = d.filter(function(P) {
                                 var I = P[0],
                                     Y = P[1];
                                 return I <= A
                             }).map(function(P) {
                                 var I = P[0],
                                     Y = P[1];
                                 if (Y.cId == null) throw new Error("Could not find cId for classical register.");
                                 var re = e[Y.qId].children;
                                 if (re == null) throw new Error("Failed to find classical registers for qubit ID ".concat(Y.qId, "."));
                                 return re[Y.cId].y
                             });
-                            R.targetsY = ss(L.targets, O, e)
+                            R.targetsY = cs(L.targets, O, e)
                         }
                         return R.width > c[A] && (c[A] = R.width), R
                     })
                 }),
-                y = ls(g, c),
+                y = us(g, c),
                 _ = g.flat().filter(function(w) {
                     var T = w.type;
                     return T != rt.GateType.Invalid
                 });
             return {
                 metadataList: _,
                 svgWidth: y
             }
         };
-    Pe.processOperations = v0;
-    var ns = function(r, e) {
+    Pe.processOperations = w0;
+    var os = function(r, e) {
         var i = Math.max.apply(Math, dr([-1], Object.keys(e).map(Number), !1)) + 1,
             a = Array.from(Array(i), function() {
                 return new Array(0)
             });
         return r.forEach(function(l, c) {
             var d = l.targets,
                 f = l.controls,
@@ -683,16 +683,16 @@
                     return (P || ir.RegisterType.Qubit) === ir.RegisterType.Classical
                 }),
                 T = w.length > 0;
             if (!(!T && y.length === 0))
                 for (var A = T ? 0 : Math.min.apply(Math, _), L = T ? i - 1 : Math.max.apply(Math, _), R = A; R <= L; R++) a[R].push(c)
         }), a
     };
-    Pe._groupOperations = ns;
-    var is = function(r) {
+    Pe._groupOperations = os;
+    var as = function(r) {
         for (var e = Math.max.apply(Math, dr([0], r.map(function(d) {
                 return d.length
             }), !1)), i = 0, a = JSON.parse(JSON.stringify(r)); i < e;) {
             for (var l = function(d) {
                     var f = a[d];
                     if (f.length <= i) return "continue";
                     var g = f[i],
@@ -702,16 +702,16 @@
                         _ = Math.max.apply(Math, dr([-1], y, !1));
                     i < _ && (a[d].splice(i, 0, null), e = Math.max(e, a[d].length))
                 }, c = 0; c < a.length; c++) l(c);
             i++
         }
         return a
     };
-    Pe._alignOps = is;
-    var os = function(r, e) {
+    Pe._alignOps = as;
+    var ss = function(r, e) {
         var i = [];
         return e.forEach(function(a) {
             for (var l = function(d) {
                     var f = a[d];
                     if (f != null && r[f].isMeasurement) {
                         var g = r[f].targets.filter(function(y) {
                             return y.type === ir.RegisterType.Classical
@@ -719,16 +719,16 @@
                         g.forEach(function(y) {
                             return i.push([d, y])
                         })
                     }
                 }, c = 0; c < a.length; c++) l(c)
         }), i
     };
-    Pe._getClassicalRegStart = os;
-    var as = function(r, e) {
+    Pe._getClassicalRegStart = ss;
+    var ls = function(r, e) {
         var i = {
             type: rt.GateType.Invalid,
             x: 0,
             controlsY: [],
             targetsY: [],
             label: "",
             width: -1
@@ -742,48 +742,48 @@
             g = r.isControlled,
             y = r.isAdjoint,
             _ = r.controls,
             w = r.targets,
             T = r.children,
             A = r.conditionalRender;
         if (i.controlsY = _?.map(function(ne) {
-                return k0(ne, e)
+                return _0(ne, e)
             }) || [], i.targetsY = w.map(function(ne) {
-                return k0(ne, e)
+                return _0(ne, e)
             }), f) {
             if (T == null || T.length == 0) throw new Error("No children operations found for classically-controlled operation.");
             var L = T.filter(function(ne) {
-                    return ne.conditionalRender !== Qn.ConditionalRender.OnOne
+                    return ne.conditionalRender !== Jn.ConditionalRender.OnOne
                 }),
-                R = v0(L, e),
+                R = w0(L, e),
                 O = R.metadataList,
                 P = R.svgWidth,
                 I = T.filter(function(ne) {
-                    return ne.conditionalRender !== Qn.ConditionalRender.OnZero
+                    return ne.conditionalRender !== Jn.ConditionalRender.OnZero
                 });
-            R = v0(I, e);
+            R = w0(I, e);
             var Y = R.metadataList,
                 re = R.svgWidth,
                 te = Math.max(P, re) - ot.startX - ot.gatePadding * 2;
             i.type = rt.GateType.ClassicalControlled, i.children = [O, Y], i.width = te + ot.controlBtnOffset + ot.groupBoxPadding * 2;
             var j = Object.values(e).map(function(ne) {
                 var pe = ne.y;
                 return pe
             });
             j.length > 0 && (i.targetsY = [Math.min.apply(Math, j), Math.max.apply(Math, j)])
-        } else if (A == Qn.ConditionalRender.AsGroup && (T?.length || 0) > 0) {
-            var R = v0(T, e);
+        } else if (A == Jn.ConditionalRender.AsGroup && (T?.length || 0) > 0) {
+            var R = w0(T, e);
             i.type = rt.GateType.Group, i.children = R.metadataList, i.dataAttributes = {
                 expanded: "true"
             }, i.width = R.svgWidth - ot.startX + (ot.groupBoxPadding - ot.gatePadding) * 2
         } else d ? i.type = rt.GateType.Measure : a === "SWAP" ? i.type = rt.GateType.Swap : g ? (i.type = a === "X" ? rt.GateType.Cnot : rt.GateType.ControlledUnitary, i.label = a) : a === "X" ? (i.type = rt.GateType.X, i.label = a) : (i.type = rt.GateType.Unitary, i.label = a);
-        return y && i.label.length > 0 && (i.label += "'"), c != null && (i.displayArgs = c), i.width = (0, rd.getGateWidth)(i), l != null && (i.dataAttributes = w0(w0({}, i.dataAttributes), l)), i
+        return y && i.label.length > 0 && (i.label += "'"), c != null && (i.displayArgs = c), i.width = (0, id.getGateWidth)(i), l != null && (i.dataAttributes = k0(k0({}, i.dataAttributes), l)), i
     };
-    Pe._opToMetadata = as;
-    var k0 = function(r, e) {
+    Pe._opToMetadata = ls;
+    var _0 = function(r, e) {
         var i = r.type,
             a = r.qId,
             l = r.cId;
         if (!e.hasOwnProperty(a)) throw new Error("ERROR: Qubit register with ID ".concat(a, " not found."));
         var c = e[a],
             d = c.y,
             f = c.children;
@@ -796,16 +796,16 @@
                 if (l == null) throw new Error("ERROR: No ID defined for classical register associated with qubit ID ".concat(a, "."));
                 if (f.length <= l) throw new Error("ERROR: Classical register ID ".concat(l, " invalid for qubit ID ").concat(a, " with ").concat(f.length, " classical register(s)."));
                 return f[l].y;
             default:
                 throw new Error("ERROR: Unknown register type ".concat(i, "."))
         }
     };
-    Pe._getRegY = k0;
-    var ss = function(r, e, i) {
+    Pe._getRegY = _0;
+    var cs = function(r, e, i) {
         if (r.length === 0) return [];
         var a = Object.keys(i).map(Number);
         a.sort(function(f, g) {
             return i[f].y - i[g].y
         });
         var l = {};
         a.forEach(function(f, g) {
@@ -815,120 +815,120 @@
             return y === 0 && f.cId != null && g.cId != null ? f.cId - g.cId : y
         }), e = e.slice(), e.sort(function(f, g) {
             return f - g
         });
         var c = 0,
             d = 0;
         return r.reduce(function(f, g) {
-            var y = k0(g, i),
+            var y = _0(g, i),
                 _ = l[g.qId];
             for (f.length === 0 || _ > c + 1 || e[0] > d && e[0] < y ? f.push([y]) : f[f.length - 1].push(y), c = _, d = y; e.length > 0 && e[0] <= y;) e.shift();
             return f
         }, [])
     };
-    Pe._splitTargetsY = ss;
-    var ls = function(r, e) {
+    Pe._splitTargetsY = cs;
+    var us = function(r, e) {
         var i = ot.startX,
             a = e.map(function(c) {
                 var d = i;
                 return i += c + ot.gatePadding * 2, d
             }),
             l = i;
         return r.forEach(function(c) {
             return c.forEach(function(d, f) {
                 var g = a[f];
                 switch (d.type) {
                     case rt.GateType.ClassicalControlled:
                     case rt.GateType.Group:
                         var y = g - ot.startX + ot.groupBoxPadding;
-                        d.type === rt.GateType.ClassicalControlled && (y += ot.controlBtnOffset), Xn(d.children, y), d.x = g;
+                        d.type === rt.GateType.ClassicalControlled && (y += ot.controlBtnOffset), Kn(d.children, y), d.x = g;
                         break;
                     default:
                         d.x = g + e[f] / 2;
                         break
                 }
             })
         }), l
     };
-    Pe._fillMetadataX = ls;
-    var Xn = function(r, e) {
+    Pe._fillMetadataX = us;
+    var Kn = function(r, e) {
         r?.flat().forEach(function(i) {
-            i.x += e, Xn(i.children, e)
+            i.x += e, Kn(i.children, e)
         })
     };
-    Pe._offsetChildrenX = Xn
+    Pe._offsetChildrenX = Kn
 });
-var Jn = W(Qt => {
+var ei = W(Qt => {
     "use strict";
-    var _0 = Qt && Qt.__assign || function() {
-        return _0 = Object.assign || function(r) {
+    var S0 = Qt && Qt.__assign || function() {
+        return S0 = Object.assign || function(r) {
             for (var e, i = 1, a = arguments.length; i < a; i++) {
                 e = arguments[i];
                 for (var l in e) Object.prototype.hasOwnProperty.call(e, l) && (r[l] = e[l])
             }
             return r
-        }, _0.apply(this, arguments)
+        }, S0.apply(this, arguments)
     };
     Object.defineProperty(Qt, "__esModule", {
         value: !0
     });
     Qt.style = Qt.STYLES = void 0;
-    var us = {
+    var ds = {
             lineStroke: "#000000",
             lineWidth: 1,
             textColour: "#000000",
             unitary: "#D9F1FA",
             oplus: "#FFFFFF",
             measure: "#FFDE86",
             classicalUnknown: "#E5E5E5",
             classicalZero: "#C40000",
             classicalOne: "#4059BD",
             classicalZeroText: "#FFFFFF",
             classicalOneText: "#FFFFFF"
         },
-        nd = {
+        od = {
             lineStroke: "#000000",
             lineWidth: 1,
             textColour: "#000000",
             unitary: "#FFFFFF",
             oplus: "#FFFFFF",
             measure: "#FFFFFF",
             classicalUnknown: "#FFFFFF",
             classicalZero: "#000000",
             classicalOne: "#000000",
             classicalZeroText: "#FFFFFF",
             classicalOneText: "#FFFFFF"
         },
-        id = {
+        ad = {
             lineStroke: "#FFFFFF",
             lineWidth: 1,
             textColour: "#FFFFFF",
             unitary: "#000000",
             oplus: "#000000",
             measure: "#000000",
             classicalUnknown: "#000000",
             classicalZero: "#FFFFFF",
             classicalOne: "#FFFFFF",
             classicalZeroText: "#000000",
             classicalOneText: "#000000"
         };
     Qt.STYLES = {
-        Default: us,
-        BlackAndWhite: nd,
-        Inverted: id
+        Default: ds,
+        BlackAndWhite: od,
+        Inverted: ad
     };
-    var od = function(r) {
+    var sd = function(r) {
         r === void 0 && (r = {});
-        var e = _0(_0({}, us), r);
-        return "".concat(ad(e), `
-    `).concat(sd(e), `
-    `).concat(ld)
+        var e = S0(S0({}, ds), r);
+        return "".concat(ld(e), `
+    `).concat(cd(e), `
+    `).concat(ud)
     };
-    Qt.style = od;
-    var ad = function(r) {
+    Qt.style = sd;
+    var ld = function(r) {
             return `
     line,
     circle,
     rect {
         stroke: `.concat(r.lineStroke, `;
         stroke-width: `).concat(r.lineWidth, `;
     }
@@ -960,15 +960,15 @@
         fill: none;
         stroke-width: `).concat(r.lineWidth, `;
     }
     .register-classical {
         stroke-width: `).concat((r.lineWidth || 0) / 2, `;
     }`)
         },
-        sd = function(r) {
+        cd = function(r) {
             var e = `
     .classically-controlled-one .classical-container,
     .classically-controlled-one .classical-line {
         stroke: `.concat(r.classicalOne, `;
         stroke-width: `).concat((r.lineWidth || 0) + .3, `;
         fill: `).concat(r.classicalOne, `;
         fill-opacity: 0.1;
@@ -1017,15 +1017,15 @@
         opacity: 0.25;
     }
 
     `.concat(e, `
     `).concat(i, `
     `).concat(a)
         },
-        ld = `
+        ud = `
     .qviz .gate-collapse,
     .qviz .gate-expand {
         opacity: 0;
         transition: opacity 1s;
     }
 
     .qviz:hover .gate-collapse,
@@ -1055,30 +1055,30 @@
     .gate:hover > .gate-collapse,
     .gate:hover > .gate-expand {
         visibility: visible;
         opacity: 1;
         transition: opacity 1s;
     }`
 });
-var hs = W(C0 => {
+var ms = W(T0 => {
     "use strict";
-    Object.defineProperty(C0, "__esModule", {
+    Object.defineProperty(T0, "__esModule", {
         value: !0
     });
-    C0.Sqore = void 0;
-    var cd = Ga(),
-        ud = Ja(),
-        hd = rs(),
-        dd = cs(),
-        S0 = Un(),
-        md = hr(),
-        Kn = Jn(),
-        pd = Zn(),
-        fd = Wt(),
-        gd = function() {
+    T0.Sqore = void 0;
+    var hd = ja(),
+        dd = es(),
+        md = is(),
+        pd = hs(),
+        C0 = Yn(),
+        fd = hr(),
+        ti = ei(),
+        gd = Xn(),
+        bd = Wt(),
+        yd = function() {
             function r(e, i) {
                 i === void 0 && (i = {}), this.style = {}, this.gateRegistry = {}, this.circuit = e, this.style = this.getStyle(i)
             }
             return r.prototype.draw = function(e, i) {
                 var a = this;
                 if (i === void 0 && (i = 0), e == null) throw new Error("Container not provided.");
                 var l = JSON.parse(JSON.stringify(this.circuit));
@@ -1088,16 +1088,16 @@
                     var c = l.operations[0].dataAttributes.id;
                     this.expandOperation(l.operations, c)
                 }
                 this.renderCircuit(e, l)
             }, r.prototype.getStyle = function(e) {
                 if (e === void 0 && (e = {}), typeof e == "string" || e instanceof String) {
                     var i = e;
-                    if (!Kn.STYLES.hasOwnProperty(i)) return console.error("No style ".concat(i, " found in STYLES.")), {};
-                    e = Kn.STYLES[i]
+                    if (!ti.STYLES.hasOwnProperty(i)) return console.error("No style ".concat(i, " found in STYLES.")), {};
+                    e = ti.STYLES[i]
                 }
                 return e
             }, r.prototype.renderCircuit = function(e, i) {
                 var a = this.compose(i),
                     l = this.generateSvg(a);
                 e.innerHTML = "", e.appendChild(l), this.addGateClickHandlers(e, i)
             }, r.prototype.compose = function(e) {
@@ -1111,42 +1111,42 @@
                     },
                     a = function(P) {
                         var I = [];
                         return i(I, P), I
                     },
                     l = e.qubits,
                     c = e.operations,
-                    d = (0, cd.formatInputs)(l),
+                    d = (0, hd.formatInputs)(l),
                     f = d.qubitWires,
                     g = d.registers,
                     y = d.svgHeight,
-                    _ = (0, dd.processOperations)(c, g),
+                    _ = (0, pd.processOperations)(c, g),
                     w = _.metadataList,
                     T = _.svgWidth,
-                    A = (0, ud.formatGates)(w),
+                    A = (0, dd.formatGates)(w),
                     L = a(w).filter(function(P) {
                         var I = P.type;
-                        return I === md.GateType.Measure
+                        return I === fd.GateType.Measure
                     }),
-                    R = (0, hd.formatRegisters)(g, L, T),
+                    R = (0, md.formatRegisters)(g, L, T),
                     O = {
                         width: T,
                         height: y,
                         elements: [f, R, A]
                     };
                 return O
             }, r.prototype.generateSvg = function(e) {
                 var i = e.width,
                     a = e.height,
                     l = e.elements,
-                    c = (0, pd.createUUID)(),
-                    d = document.createElementNS(fd.svgNS, "svg");
+                    c = (0, gd.createUUID)(),
+                    d = document.createElementNS(bd.svgNS, "svg");
                 d.setAttribute("id", c), d.setAttribute("class", "qviz"), d.setAttribute("width", i.toString()), d.setAttribute("height", a.toString()), d.style.setProperty("max-width", "fit-content");
                 var f = document.createElement("style");
-                return f.innerHTML = (0, Kn.style)(this.style), d.appendChild(f), l.forEach(function(g) {
+                return f.innerHTML = (0, ti.style)(this.style), d.appendChild(f), l.forEach(function(g) {
                     return d.appendChild(g)
                 }), d
             }, r.prototype.fillGateRegistry = function(e, i) {
                 var a = this,
                     l;
                 e.dataAttributes == null && (e.dataAttributes = {}), e.dataAttributes.id = i, e.dataAttributes["zoom-out"] = "false", this.gateRegistry[i] = e, (l = e.children) === null || l === void 0 || l.forEach(function(c, d) {
                     a.fillGateRegistry(c, "".concat(i, "-").concat(d)), c.dataAttributes == null && (c.dataAttributes = {}), c.dataAttributes["zoom-out"] = "true"
@@ -1190,52 +1190,52 @@
                         var d, f = (d = l.parentElement) === null || d === void 0 ? void 0 : d.getAttribute("data-id");
                         typeof f == "string" && (l.classList.contains("gate-collapse") ? a.collapseOperation(i.operations, f) : l.classList.contains("gate-expand") && a.expandOperation(i.operations, f), a.renderCircuit(e, i), c.stopPropagation())
                     })
                 })
             }, r.prototype.expandOperation = function(e, i) {
                 var a = this;
                 e.forEach(function(l) {
-                    if (l.conditionalRender === S0.ConditionalRender.AsGroup && a.expandOperation(l.children || [], i), l.dataAttributes == null) return l;
+                    if (l.conditionalRender === C0.ConditionalRender.AsGroup && a.expandOperation(l.children || [], i), l.dataAttributes == null) return l;
                     var c = l.dataAttributes.id;
-                    c === i && l.children != null && (l.conditionalRender = S0.ConditionalRender.AsGroup, l.dataAttributes.expanded = "true")
+                    c === i && l.children != null && (l.conditionalRender = C0.ConditionalRender.AsGroup, l.dataAttributes.expanded = "true")
                 })
             }, r.prototype.collapseOperation = function(e, i) {
                 var a = this;
                 e.forEach(function(l) {
-                    if (l.conditionalRender === S0.ConditionalRender.AsGroup && a.collapseOperation(l.children || [], i), l.dataAttributes == null) return l;
+                    if (l.conditionalRender === C0.ConditionalRender.AsGroup && a.collapseOperation(l.children || [], i), l.dataAttributes == null) return l;
                     var c = l.dataAttributes.id;
-                    c.startsWith(i) && (l.conditionalRender = S0.ConditionalRender.Always, delete l.dataAttributes.expanded)
+                    c.startsWith(i) && (l.conditionalRender = C0.ConditionalRender.Always, delete l.dataAttributes.expanded)
                 })
             }, r
         }();
-    C0.Sqore = gd
+    T0.Sqore = yd
 });
-var ds = W(mr => {
+var ps = W(mr => {
     "use strict";
     Object.defineProperty(mr, "__esModule", {
         value: !0
     });
     mr.STYLES = mr.draw = void 0;
-    var bd = hs(),
-        yd = function(r, e, i, a) {
+    var xd = ms(),
+        vd = function(r, e, i, a) {
             i === void 0 && (i = {}), a === void 0 && (a = 0);
-            var l = new bd.Sqore(r, i);
+            var l = new xd.Sqore(r, i);
             l.draw(e, a)
         };
-    mr.draw = yd;
-    var xd = Jn();
+    mr.draw = vd;
+    var wd = ei();
     Object.defineProperty(mr, "STYLES", {
         enumerable: !0,
         get: function() {
-            return xd.STYLES
+            return wd.STYLES
         }
     })
 });
-var ps = W((P4, _d) => {
-    _d.exports = {
+var gs = W((j4, Cd) => {
+    Cd.exports = {
         Aacute: "\xC1",
         aacute: "\xE1",
         Abreve: "\u0102",
         abreve: "\u0103",
         ac: "\u223E",
         acd: "\u223F",
         acE: "\u223E\u0333",
@@ -3356,36 +3356,36 @@
         Zopf: "\u2124",
         Zscr: "\u{1D4B5}",
         zscr: "\u{1D4CF}",
         zwj: "\u200D",
         zwnj: "\u200C"
     }
 });
-var ni = W((I4, fs) => {
+var oi = W((U4, bs) => {
     "use strict";
-    fs.exports = ps()
+    bs.exports = gs()
 });
-var T0 = W((O4, gs) => {
-    gs.exports = /[!-#%-\*,-\/:;\?@\[-\]_\{\}\xA1\xA7\xAB\xB6\xB7\xBB\xBF\u037E\u0387\u055A-\u055F\u0589\u058A\u05BE\u05C0\u05C3\u05C6\u05F3\u05F4\u0609\u060A\u060C\u060D\u061B\u061E\u061F\u066A-\u066D\u06D4\u0700-\u070D\u07F7-\u07F9\u0830-\u083E\u085E\u0964\u0965\u0970\u09FD\u0A76\u0AF0\u0C84\u0DF4\u0E4F\u0E5A\u0E5B\u0F04-\u0F12\u0F14\u0F3A-\u0F3D\u0F85\u0FD0-\u0FD4\u0FD9\u0FDA\u104A-\u104F\u10FB\u1360-\u1368\u1400\u166D\u166E\u169B\u169C\u16EB-\u16ED\u1735\u1736\u17D4-\u17D6\u17D8-\u17DA\u1800-\u180A\u1944\u1945\u1A1E\u1A1F\u1AA0-\u1AA6\u1AA8-\u1AAD\u1B5A-\u1B60\u1BFC-\u1BFF\u1C3B-\u1C3F\u1C7E\u1C7F\u1CC0-\u1CC7\u1CD3\u2010-\u2027\u2030-\u2043\u2045-\u2051\u2053-\u205E\u207D\u207E\u208D\u208E\u2308-\u230B\u2329\u232A\u2768-\u2775\u27C5\u27C6\u27E6-\u27EF\u2983-\u2998\u29D8-\u29DB\u29FC\u29FD\u2CF9-\u2CFC\u2CFE\u2CFF\u2D70\u2E00-\u2E2E\u2E30-\u2E4E\u3001-\u3003\u3008-\u3011\u3014-\u301F\u3030\u303D\u30A0\u30FB\uA4FE\uA4FF\uA60D-\uA60F\uA673\uA67E\uA6F2-\uA6F7\uA874-\uA877\uA8CE\uA8CF\uA8F8-\uA8FA\uA8FC\uA92E\uA92F\uA95F\uA9C1-\uA9CD\uA9DE\uA9DF\uAA5C-\uAA5F\uAADE\uAADF\uAAF0\uAAF1\uABEB\uFD3E\uFD3F\uFE10-\uFE19\uFE30-\uFE52\uFE54-\uFE61\uFE63\uFE68\uFE6A\uFE6B\uFF01-\uFF03\uFF05-\uFF0A\uFF0C-\uFF0F\uFF1A\uFF1B\uFF1F\uFF20\uFF3B-\uFF3D\uFF3F\uFF5B\uFF5D\uFF5F-\uFF65]|\uD800[\uDD00-\uDD02\uDF9F\uDFD0]|\uD801\uDD6F|\uD802[\uDC57\uDD1F\uDD3F\uDE50-\uDE58\uDE7F\uDEF0-\uDEF6\uDF39-\uDF3F\uDF99-\uDF9C]|\uD803[\uDF55-\uDF59]|\uD804[\uDC47-\uDC4D\uDCBB\uDCBC\uDCBE-\uDCC1\uDD40-\uDD43\uDD74\uDD75\uDDC5-\uDDC8\uDDCD\uDDDB\uDDDD-\uDDDF\uDE38-\uDE3D\uDEA9]|\uD805[\uDC4B-\uDC4F\uDC5B\uDC5D\uDCC6\uDDC1-\uDDD7\uDE41-\uDE43\uDE60-\uDE6C\uDF3C-\uDF3E]|\uD806[\uDC3B\uDE3F-\uDE46\uDE9A-\uDE9C\uDE9E-\uDEA2]|\uD807[\uDC41-\uDC45\uDC70\uDC71\uDEF7\uDEF8]|\uD809[\uDC70-\uDC74]|\uD81A[\uDE6E\uDE6F\uDEF5\uDF37-\uDF3B\uDF44]|\uD81B[\uDE97-\uDE9A]|\uD82F\uDC9F|\uD836[\uDE87-\uDE8B]|\uD83A[\uDD5E\uDD5F]/
+var A0 = W((W4, ys) => {
+    ys.exports = /[!-#%-\*,-\/:;\?@\[-\]_\{\}\xA1\xA7\xAB\xB6\xB7\xBB\xBF\u037E\u0387\u055A-\u055F\u0589\u058A\u05BE\u05C0\u05C3\u05C6\u05F3\u05F4\u0609\u060A\u060C\u060D\u061B\u061E\u061F\u066A-\u066D\u06D4\u0700-\u070D\u07F7-\u07F9\u0830-\u083E\u085E\u0964\u0965\u0970\u09FD\u0A76\u0AF0\u0C84\u0DF4\u0E4F\u0E5A\u0E5B\u0F04-\u0F12\u0F14\u0F3A-\u0F3D\u0F85\u0FD0-\u0FD4\u0FD9\u0FDA\u104A-\u104F\u10FB\u1360-\u1368\u1400\u166D\u166E\u169B\u169C\u16EB-\u16ED\u1735\u1736\u17D4-\u17D6\u17D8-\u17DA\u1800-\u180A\u1944\u1945\u1A1E\u1A1F\u1AA0-\u1AA6\u1AA8-\u1AAD\u1B5A-\u1B60\u1BFC-\u1BFF\u1C3B-\u1C3F\u1C7E\u1C7F\u1CC0-\u1CC7\u1CD3\u2010-\u2027\u2030-\u2043\u2045-\u2051\u2053-\u205E\u207D\u207E\u208D\u208E\u2308-\u230B\u2329\u232A\u2768-\u2775\u27C5\u27C6\u27E6-\u27EF\u2983-\u2998\u29D8-\u29DB\u29FC\u29FD\u2CF9-\u2CFC\u2CFE\u2CFF\u2D70\u2E00-\u2E2E\u2E30-\u2E4E\u3001-\u3003\u3008-\u3011\u3014-\u301F\u3030\u303D\u30A0\u30FB\uA4FE\uA4FF\uA60D-\uA60F\uA673\uA67E\uA6F2-\uA6F7\uA874-\uA877\uA8CE\uA8CF\uA8F8-\uA8FA\uA8FC\uA92E\uA92F\uA95F\uA9C1-\uA9CD\uA9DE\uA9DF\uAA5C-\uAA5F\uAADE\uAADF\uAAF0\uAAF1\uABEB\uFD3E\uFD3F\uFE10-\uFE19\uFE30-\uFE52\uFE54-\uFE61\uFE63\uFE68\uFE6A\uFE6B\uFF01-\uFF03\uFF05-\uFF0A\uFF0C-\uFF0F\uFF1A\uFF1B\uFF1F\uFF20\uFF3B-\uFF3D\uFF3F\uFF5B\uFF5D\uFF5F-\uFF65]|\uD800[\uDD00-\uDD02\uDF9F\uDFD0]|\uD801\uDD6F|\uD802[\uDC57\uDD1F\uDD3F\uDE50-\uDE58\uDE7F\uDEF0-\uDEF6\uDF39-\uDF3F\uDF99-\uDF9C]|\uD803[\uDF55-\uDF59]|\uD804[\uDC47-\uDC4D\uDCBB\uDCBC\uDCBE-\uDCC1\uDD40-\uDD43\uDD74\uDD75\uDDC5-\uDDC8\uDDCD\uDDDB\uDDDD-\uDDDF\uDE38-\uDE3D\uDEA9]|\uD805[\uDC4B-\uDC4F\uDC5B\uDC5D\uDCC6\uDDC1-\uDDD7\uDE41-\uDE43\uDE60-\uDE6C\uDF3C-\uDF3E]|\uD806[\uDC3B\uDE3F-\uDE46\uDE9A-\uDE9C\uDE9E-\uDEA2]|\uD807[\uDC41-\uDC45\uDC70\uDC71\uDEF7\uDEF8]|\uD809[\uDC70-\uDC74]|\uD81A[\uDE6E\uDE6F\uDEF5\uDF37-\uDF3B\uDF44]|\uD81B[\uDE97-\uDE9A]|\uD82F\uDC9F|\uD836[\uDE87-\uDE8B]|\uD83A[\uDD5E\uDD5F]/
 });
-var xs = W((H4, ys) => {
+var ws = W((Y4, vs) => {
     "use strict";
-    var bs = {};
+    var xs = {};
 
-    function Sd(r) {
-        var e, i, a = bs[r];
+    function Td(r) {
+        var e, i, a = xs[r];
         if (a) return a;
-        for (a = bs[r] = [], e = 0; e < 128; e++) i = String.fromCharCode(e), /^[0-9a-z]$/i.test(i) ? a.push(i) : a.push("%" + ("0" + e.toString(16).toUpperCase()).slice(-2));
+        for (a = xs[r] = [], e = 0; e < 128; e++) i = String.fromCharCode(e), /^[0-9a-z]$/i.test(i) ? a.push(i) : a.push("%" + ("0" + e.toString(16).toUpperCase()).slice(-2));
         for (e = 0; e < r.length; e++) a[r.charCodeAt(e)] = r[e];
         return a
     }
 
-    function A0(r, e, i) {
+    function q0(r, e, i) {
         var a, l, c, d, f, g = "";
-        for (typeof e != "string" && (i = e, e = A0.defaultChars), typeof i > "u" && (i = !0), f = Sd(e), a = 0, l = r.length; a < l; a++) {
+        for (typeof e != "string" && (i = e, e = q0.defaultChars), typeof i > "u" && (i = !0), f = Td(e), a = 0, l = r.length; a < l; a++) {
             if (c = r.charCodeAt(a), i && c === 37 && a + 2 < l && /^[0-9a-f]{2}$/i.test(r.slice(a + 1, a + 3))) {
                 g += r.slice(a, a + 3), a += 2;
                 continue
             }
             if (c < 128) {
                 g += f[c];
                 continue
@@ -3398,33 +3398,33 @@
                 g += "%EF%BF%BD";
                 continue
             }
             g += encodeURIComponent(r[a])
         }
         return g
     }
-    A0.defaultChars = ";/?:@&=+$,-_.!~*'()#";
-    A0.componentChars = "-_.!~*'()";
-    ys.exports = A0
+    q0.defaultChars = ";/?:@&=+$,-_.!~*'()#";
+    q0.componentChars = "-_.!~*'()";
+    vs.exports = q0
 });
-var ks = W(($4, ws) => {
+var Ss = W((Z4, _s) => {
     "use strict";
-    var vs = {};
+    var ks = {};
 
-    function Cd(r) {
-        var e, i, a = vs[r];
+    function Ad(r) {
+        var e, i, a = ks[r];
         if (a) return a;
-        for (a = vs[r] = [], e = 0; e < 128; e++) i = String.fromCharCode(e), a.push(i);
+        for (a = ks[r] = [], e = 0; e < 128; e++) i = String.fromCharCode(e), a.push(i);
         for (e = 0; e < r.length; e++) i = r.charCodeAt(e), a[i] = "%" + ("0" + i.toString(16).toUpperCase()).slice(-2);
         return a
     }
 
-    function q0(r, e) {
+    function M0(r, e) {
         var i;
-        return typeof e != "string" && (e = q0.defaultChars), i = Cd(e), r.replace(/(%[a-f0-9]{2})+/gi, function(a) {
+        return typeof e != "string" && (e = M0.defaultChars), i = Ad(e), r.replace(/(%[a-f0-9]{2})+/gi, function(a) {
             var l, c, d, f, g, y, _, w = "";
             for (l = 0, c = a.length; l < c; l += 3) {
                 if (d = parseInt(a.slice(l + 1, l + 3), 16), d < 128) {
                     w += i[d];
                     continue
                 }
                 if ((d & 224) === 192 && l + 3 < c && (f = parseInt(a.slice(l + 4, l + 6), 16), (f & 192) === 128)) {
@@ -3440,234 +3440,234 @@
                     continue
                 }
                 w += "\uFFFD"
             }
             return w
         })
     }
-    q0.defaultChars = ";/?:@&=+$,#";
-    q0.componentChars = "";
-    ws.exports = q0
+    M0.defaultChars = ";/?:@&=+$,#";
+    M0.componentChars = "";
+    _s.exports = M0
 });
-var Ss = W((G4, _s) => {
+var Ts = W((Q4, Cs) => {
     "use strict";
-    _s.exports = function(e) {
+    Cs.exports = function(e) {
         var i = "";
         return i += e.protocol || "", i += e.slashes ? "//" : "", i += e.auth ? e.auth + "@" : "", e.hostname && e.hostname.indexOf(":") !== -1 ? i += "[" + e.hostname + "]" : i += e.hostname || "", i += e.port ? ":" + e.port : "", i += e.pathname || "", i += e.search || "", i += e.hash || "", i
     }
 });
-var Ds = W((V4, Es) => {
+var Rs = W((X4, zs) => {
     "use strict";
 
-    function M0() {
+    function E0() {
         this.protocol = null, this.slashes = null, this.auth = null, this.port = null, this.hostname = null, this.hash = null, this.search = null, this.pathname = null
     }
-    var Td = /^([a-z0-9.+-]+:)/i,
-        Ad = /:[0-9]*$/,
-        qd = /^(\/\/?(?!\/)[^\?\s]*)(\?[^\s]*)?$/,
-        Md = ["<", ">", '"', "`", " ", "\r", `
+    var qd = /^([a-z0-9.+-]+:)/i,
+        Md = /:[0-9]*$/,
+        Ed = /^(\/\/?(?!\/)[^\?\s]*)(\?[^\s]*)?$/,
+        Dd = ["<", ">", '"', "`", " ", "\r", `
 `, "	"],
-        Ed = ["{", "}", "|", "\\", "^", "`"].concat(Md),
-        Dd = ["'"].concat(Ed),
-        Cs = ["%", "/", "?", ";", "#"].concat(Dd),
-        Ts = ["/", "?", "#"],
-        zd = 255,
-        As = /^[+a-z0-9A-Z_-]{0,63}$/,
-        Rd = /^([+a-z0-9A-Z_-]{0,63})(.*)$/,
-        qs = {
+        zd = ["{", "}", "|", "\\", "^", "`"].concat(Dd),
+        Rd = ["'"].concat(zd),
+        As = ["%", "/", "?", ";", "#"].concat(Rd),
+        qs = ["/", "?", "#"],
+        Fd = 255,
+        Ms = /^[+a-z0-9A-Z_-]{0,63}$/,
+        Bd = /^([+a-z0-9A-Z_-]{0,63})(.*)$/,
+        Es = {
             javascript: !0,
             "javascript:": !0
         },
-        Ms = {
+        Ds = {
             http: !0,
             https: !0,
             ftp: !0,
             gopher: !0,
             file: !0,
             "http:": !0,
             "https:": !0,
             "ftp:": !0,
             "gopher:": !0,
             "file:": !0
         };
 
-    function Fd(r, e) {
-        if (r && r instanceof M0) return r;
-        var i = new M0;
+    function Nd(r, e) {
+        if (r && r instanceof E0) return r;
+        var i = new E0;
         return i.parse(r, e), i
     }
-    M0.prototype.parse = function(r, e) {
+    E0.prototype.parse = function(r, e) {
         var i, a, l, c, d, f = r;
         if (f = f.trim(), !e && r.split("#").length === 1) {
-            var g = qd.exec(f);
+            var g = Ed.exec(f);
             if (g) return this.pathname = g[1], g[2] && (this.search = g[2]), this
         }
-        var y = Td.exec(f);
-        if (y && (y = y[0], l = y.toLowerCase(), this.protocol = y, f = f.substr(y.length)), (e || y || f.match(/^\/\/[^@\/]+@[^@\/]+/)) && (d = f.substr(0, 2) === "//", d && !(y && qs[y]) && (f = f.substr(2), this.slashes = !0)), !qs[y] && (d || y && !Ms[y])) {
+        var y = qd.exec(f);
+        if (y && (y = y[0], l = y.toLowerCase(), this.protocol = y, f = f.substr(y.length)), (e || y || f.match(/^\/\/[^@\/]+@[^@\/]+/)) && (d = f.substr(0, 2) === "//", d && !(y && Es[y]) && (f = f.substr(2), this.slashes = !0)), !Es[y] && (d || y && !Ds[y])) {
             var _ = -1;
-            for (i = 0; i < Ts.length; i++) c = f.indexOf(Ts[i]), c !== -1 && (_ === -1 || c < _) && (_ = c);
+            for (i = 0; i < qs.length; i++) c = f.indexOf(qs[i]), c !== -1 && (_ === -1 || c < _) && (_ = c);
             var w, T;
-            for (_ === -1 ? T = f.lastIndexOf("@") : T = f.lastIndexOf("@", _), T !== -1 && (w = f.slice(0, T), f = f.slice(T + 1), this.auth = w), _ = -1, i = 0; i < Cs.length; i++) c = f.indexOf(Cs[i]), c !== -1 && (_ === -1 || c < _) && (_ = c);
+            for (_ === -1 ? T = f.lastIndexOf("@") : T = f.lastIndexOf("@", _), T !== -1 && (w = f.slice(0, T), f = f.slice(T + 1), this.auth = w), _ = -1, i = 0; i < As.length; i++) c = f.indexOf(As[i]), c !== -1 && (_ === -1 || c < _) && (_ = c);
             _ === -1 && (_ = f.length), f[_ - 1] === ":" && _--;
             var A = f.slice(0, _);
             f = f.slice(_), this.parseHost(A), this.hostname = this.hostname || "";
             var L = this.hostname[0] === "[" && this.hostname[this.hostname.length - 1] === "]";
             if (!L) {
                 var R = this.hostname.split(/\./);
                 for (i = 0, a = R.length; i < a; i++) {
                     var O = R[i];
-                    if (O && !O.match(As)) {
+                    if (O && !O.match(Ms)) {
                         for (var P = "", I = 0, Y = O.length; I < Y; I++) O.charCodeAt(I) > 127 ? P += "x" : P += O[I];
-                        if (!P.match(As)) {
+                        if (!P.match(Ms)) {
                             var re = R.slice(0, i),
                                 te = R.slice(i + 1),
-                                j = O.match(Rd);
+                                j = O.match(Bd);
                             j && (re.push(j[1]), te.unshift(j[2])), te.length && (f = te.join(".") + f), this.hostname = re.join(".");
                             break
                         }
                     }
                 }
             }
-            this.hostname.length > zd && (this.hostname = ""), L && (this.hostname = this.hostname.substr(1, this.hostname.length - 2))
+            this.hostname.length > Fd && (this.hostname = ""), L && (this.hostname = this.hostname.substr(1, this.hostname.length - 2))
         }
         var ne = f.indexOf("#");
         ne !== -1 && (this.hash = f.substr(ne), f = f.slice(0, ne));
         var pe = f.indexOf("?");
-        return pe !== -1 && (this.search = f.substr(pe), f = f.slice(0, pe)), f && (this.pathname = f), Ms[l] && this.hostname && !this.pathname && (this.pathname = ""), this
+        return pe !== -1 && (this.search = f.substr(pe), f = f.slice(0, pe)), f && (this.pathname = f), Ds[l] && this.hostname && !this.pathname && (this.pathname = ""), this
     };
-    M0.prototype.parseHost = function(r) {
-        var e = Ad.exec(r);
+    E0.prototype.parseHost = function(r) {
+        var e = Md.exec(r);
         e && (e = e[0], e !== ":" && (this.port = e.substr(1)), r = r.substr(0, r.length - e.length)), r && (this.hostname = r)
     };
-    Es.exports = Fd
+    zs.exports = Nd
 });
-var ii = W((j4, Nr) => {
+var ai = W((J4, Nr) => {
     "use strict";
-    Nr.exports.encode = xs();
-    Nr.exports.decode = ks();
-    Nr.exports.format = Ss();
-    Nr.exports.parse = Ds()
+    Nr.exports.encode = ws();
+    Nr.exports.decode = Ss();
+    Nr.exports.format = Ts();
+    Nr.exports.parse = Rs()
 });
-var oi = W((U4, zs) => {
-    zs.exports = /[\0-\uD7FF\uE000-\uFFFF]|[\uD800-\uDBFF][\uDC00-\uDFFF]|[\uD800-\uDBFF](?![\uDC00-\uDFFF])|(?:[^\uD800-\uDBFF]|^)[\uDC00-\uDFFF]/
+var si = W((K4, Fs) => {
+    Fs.exports = /[\0-\uD7FF\uE000-\uFFFF]|[\uD800-\uDBFF][\uDC00-\uDFFF]|[\uD800-\uDBFF](?![\uDC00-\uDFFF])|(?:[^\uD800-\uDBFF]|^)[\uDC00-\uDFFF]/
 });
-var ai = W((W4, Rs) => {
-    Rs.exports = /[\0-\x1F\x7F-\x9F]/
+var li = W((e2, Bs) => {
+    Bs.exports = /[\0-\x1F\x7F-\x9F]/
 });
-var Bs = W((Y4, Fs) => {
-    Fs.exports = /[\xAD\u0600-\u0605\u061C\u06DD\u070F\u08E2\u180E\u200B-\u200F\u202A-\u202E\u2060-\u2064\u2066-\u206F\uFEFF\uFFF9-\uFFFB]|\uD804[\uDCBD\uDCCD]|\uD82F[\uDCA0-\uDCA3]|\uD834[\uDD73-\uDD7A]|\uDB40[\uDC01\uDC20-\uDC7F]/
+var Ls = W((t2, Ns) => {
+    Ns.exports = /[\xAD\u0600-\u0605\u061C\u06DD\u070F\u08E2\u180E\u200B-\u200F\u202A-\u202E\u2060-\u2064\u2066-\u206F\uFEFF\uFFF9-\uFFFB]|\uD804[\uDCBD\uDCCD]|\uD82F[\uDCA0-\uDCA3]|\uD834[\uDD73-\uDD7A]|\uDB40[\uDC01\uDC20-\uDC7F]/
 });
-var si = W((Z4, Ns) => {
-    Ns.exports = /[ \xA0\u1680\u2000-\u200A\u2028\u2029\u202F\u205F\u3000]/
+var ci = W((r2, Ps) => {
+    Ps.exports = /[ \xA0\u1680\u2000-\u200A\u2028\u2029\u202F\u205F\u3000]/
 });
-var Ls = W(pr => {
+var Is = W(pr => {
     "use strict";
-    pr.Any = oi();
-    pr.Cc = ai();
-    pr.Cf = Bs();
-    pr.P = T0();
-    pr.Z = si()
+    pr.Any = si();
+    pr.Cc = li();
+    pr.Cf = Ls();
+    pr.P = A0();
+    pr.Z = ci()
 });
 var Se = W(Ke => {
     "use strict";
 
-    function Bd(r) {
+    function Ld(r) {
         return Object.prototype.toString.call(r)
     }
 
-    function Nd(r) {
-        return Bd(r) === "[object String]"
+    function Pd(r) {
+        return Ld(r) === "[object String]"
     }
-    var Ld = Object.prototype.hasOwnProperty;
+    var Id = Object.prototype.hasOwnProperty;
 
-    function Is(r, e) {
-        return Ld.call(r, e)
+    function Hs(r, e) {
+        return Id.call(r, e)
     }
 
-    function Pd(r) {
+    function Od(r) {
         var e = Array.prototype.slice.call(arguments, 1);
         return e.forEach(function(i) {
             if (i) {
                 if (typeof i != "object") throw new TypeError(i + "must be object");
                 Object.keys(i).forEach(function(a) {
                     r[a] = i[a]
                 })
             }
         }), r
     }
 
-    function Id(r, e, i) {
+    function Hd(r, e, i) {
         return [].concat(r.slice(0, e), i, r.slice(e + 1))
     }
 
-    function Os(r) {
+    function $s(r) {
         return !(r >= 55296 && r <= 57343 || r >= 64976 && r <= 65007 || (r & 65535) === 65535 || (r & 65535) === 65534 || r >= 0 && r <= 8 || r === 11 || r >= 14 && r <= 31 || r >= 127 && r <= 159 || r > 1114111)
     }
 
-    function Hs(r) {
+    function Gs(r) {
         if (r > 65535) {
             r -= 65536;
             var e = 55296 + (r >> 10),
                 i = 56320 + (r & 1023);
             return String.fromCharCode(e, i)
         }
         return String.fromCharCode(r)
     }
-    var $s = /\\([!"#$%&'()*+,\-.\/:;<=>?@[\\\]^_`{|}~])/g,
-        Od = /&([a-z#][a-z0-9]{1,31});/gi,
-        Hd = new RegExp($s.source + "|" + Od.source, "gi"),
-        $d = /^#((?:x[a-f0-9]{1,8}|[0-9]{1,8}))$/i,
-        Ps = ni();
+    var Vs = /\\([!"#$%&'()*+,\-.\/:;<=>?@[\\\]^_`{|}~])/g,
+        $d = /&([a-z#][a-z0-9]{1,31});/gi,
+        Gd = new RegExp(Vs.source + "|" + $d.source, "gi"),
+        Vd = /^#((?:x[a-f0-9]{1,8}|[0-9]{1,8}))$/i,
+        Os = oi();
 
-    function Gd(r, e) {
+    function jd(r, e) {
         var i;
-        return Is(Ps, e) ? Ps[e] : e.charCodeAt(0) === 35 && $d.test(e) && (i = e[1].toLowerCase() === "x" ? parseInt(e.slice(2), 16) : parseInt(e.slice(1), 10), Os(i)) ? Hs(i) : r
+        return Hs(Os, e) ? Os[e] : e.charCodeAt(0) === 35 && Vd.test(e) && (i = e[1].toLowerCase() === "x" ? parseInt(e.slice(2), 16) : parseInt(e.slice(1), 10), $s(i)) ? Gs(i) : r
     }
 
-    function Vd(r) {
-        return r.indexOf("\\") < 0 ? r : r.replace($s, "$1")
+    function Ud(r) {
+        return r.indexOf("\\") < 0 ? r : r.replace(Vs, "$1")
     }
 
-    function jd(r) {
-        return r.indexOf("\\") < 0 && r.indexOf("&") < 0 ? r : r.replace(Hd, function(e, i, a) {
-            return i || Gd(e, a)
+    function Wd(r) {
+        return r.indexOf("\\") < 0 && r.indexOf("&") < 0 ? r : r.replace(Gd, function(e, i, a) {
+            return i || jd(e, a)
         })
     }
-    var Ud = /[&<>"]/,
-        Wd = /[&<>"]/g,
-        Yd = {
+    var Yd = /[&<>"]/,
+        Zd = /[&<>"]/g,
+        Qd = {
             "&": "&amp;",
             "<": "&lt;",
             ">": "&gt;",
             '"': "&quot;"
         };
 
-    function Zd(r) {
-        return Yd[r]
+    function Xd(r) {
+        return Qd[r]
     }
 
-    function Qd(r) {
-        return Ud.test(r) ? r.replace(Wd, Zd) : r
+    function Jd(r) {
+        return Yd.test(r) ? r.replace(Zd, Xd) : r
     }
-    var Xd = /[.?*+^$[\]\\(){}|-]/g;
+    var Kd = /[.?*+^$[\]\\(){}|-]/g;
 
-    function Jd(r) {
-        return r.replace(Xd, "\\$&")
+    function em(r) {
+        return r.replace(Kd, "\\$&")
     }
 
-    function Kd(r) {
+    function tm(r) {
         switch (r) {
             case 9:
             case 32:
                 return !0
         }
         return !1
     }
 
-    function em(r) {
+    function rm(r) {
         if (r >= 8192 && r <= 8202) return !0;
         switch (r) {
             case 9:
             case 10:
             case 11:
             case 12:
             case 13:
@@ -3677,21 +3677,21 @@
             case 8239:
             case 8287:
             case 12288:
                 return !0
         }
         return !1
     }
-    var tm = T0();
+    var nm = A0();
 
-    function rm(r) {
-        return tm.test(r)
+    function im(r) {
+        return nm.test(r)
     }
 
-    function nm(r) {
+    function om(r) {
         switch (r) {
             case 33:
             case 34:
             case 35:
             case 36:
             case 37:
             case 38:
@@ -3723,39 +3723,39 @@
             case 126:
                 return !0;
             default:
                 return !1
         }
     }
 
-    function im(r) {
+    function am(r) {
         return r = r.trim().replace(/\s+/g, " "), "\u1E9E".toLowerCase() === "\u1E7E" && (r = r.replace(/ẞ/g, "\xDF")), r.toLowerCase().toUpperCase()
     }
     Ke.lib = {};
-    Ke.lib.mdurl = ii();
-    Ke.lib.ucmicro = Ls();
-    Ke.assign = Pd;
-    Ke.isString = Nd;
-    Ke.has = Is;
-    Ke.unescapeMd = Vd;
-    Ke.unescapeAll = jd;
-    Ke.isValidEntityCode = Os;
-    Ke.fromCodePoint = Hs;
-    Ke.escapeHtml = Qd;
-    Ke.arrayReplaceAt = Id;
-    Ke.isSpace = Kd;
-    Ke.isWhiteSpace = em;
-    Ke.isMdAsciiPunct = nm;
-    Ke.isPunctChar = rm;
-    Ke.escapeRE = Jd;
-    Ke.normalizeReference = im
+    Ke.lib.mdurl = ai();
+    Ke.lib.ucmicro = Is();
+    Ke.assign = Od;
+    Ke.isString = Pd;
+    Ke.has = Hs;
+    Ke.unescapeMd = Ud;
+    Ke.unescapeAll = Wd;
+    Ke.isValidEntityCode = $s;
+    Ke.fromCodePoint = Gs;
+    Ke.escapeHtml = Jd;
+    Ke.arrayReplaceAt = Hd;
+    Ke.isSpace = tm;
+    Ke.isWhiteSpace = rm;
+    Ke.isMdAsciiPunct = om;
+    Ke.isPunctChar = im;
+    Ke.escapeRE = em;
+    Ke.normalizeReference = am
 });
-var Vs = W((J4, Gs) => {
+var Us = W((o2, js) => {
     "use strict";
-    Gs.exports = function(e, i, a) {
+    js.exports = function(e, i, a) {
         var l, c, d, f, g = -1,
             y = e.posMax,
             _ = e.pos;
         for (e.pos = i + 1, l = 1; e.pos < y;) {
             if (d = e.src.charCodeAt(e.pos), d === 93 && (l--, l === 0)) {
                 c = !0;
                 break
@@ -3764,29 +3764,29 @@
                 if (f === e.pos - 1) l++;
                 else if (a) return e.pos = _, -1
             }
         }
         return c && (g = e.pos), e.pos = _, g
     }
 });
-var Ws = W((K4, Us) => {
+var Zs = W((a2, Ys) => {
     "use strict";
-    var js = Se().unescapeAll;
-    Us.exports = function(e, i, a) {
+    var Ws = Se().unescapeAll;
+    Ys.exports = function(e, i, a) {
         var l, c, d = i,
             f = {
                 ok: !1,
                 pos: 0,
                 lines: 0,
                 str: ""
             };
         if (e.charCodeAt(d) === 60) {
             for (d++; d < a;) {
                 if (l = e.charCodeAt(d), l === 10 || l === 60) return f;
-                if (l === 62) return f.pos = d + 1, f.str = js(e.slice(i + 1, d)), f.ok = !0, f;
+                if (l === 62) return f.pos = d + 1, f.str = Ws(e.slice(i + 1, d)), f.ok = !0, f;
                 if (l === 92 && d + 1 < a) {
                     d += 2;
                     continue
                 }
                 d++
             }
             return f
@@ -3800,62 +3800,62 @@
             if (l === 40 && (c++, c > 32)) return f;
             if (l === 41) {
                 if (c === 0) break;
                 c--
             }
             d++
         }
-        return i === d || c !== 0 || (f.str = js(e.slice(i, d)), f.pos = d, f.ok = !0), f
+        return i === d || c !== 0 || (f.str = Ws(e.slice(i, d)), f.pos = d, f.ok = !0), f
     }
 });
-var Zs = W((e2, Ys) => {
+var Xs = W((s2, Qs) => {
     "use strict";
-    var om = Se().unescapeAll;
-    Ys.exports = function(e, i, a) {
+    var sm = Se().unescapeAll;
+    Qs.exports = function(e, i, a) {
         var l, c, d = 0,
             f = i,
             g = {
                 ok: !1,
                 pos: 0,
                 lines: 0,
                 str: ""
             };
         if (f >= a || (c = e.charCodeAt(f), c !== 34 && c !== 39 && c !== 40)) return g;
         for (f++, c === 40 && (c = 41); f < a;) {
-            if (l = e.charCodeAt(f), l === c) return g.pos = f + 1, g.lines = d, g.str = om(e.slice(i + 1, f)), g.ok = !0, g;
+            if (l = e.charCodeAt(f), l === c) return g.pos = f + 1, g.lines = d, g.str = sm(e.slice(i + 1, f)), g.ok = !0, g;
             if (l === 40 && c === 41) return g;
             l === 10 ? d++ : l === 92 && f + 1 < a && (f++, e.charCodeAt(f) === 10 && d++), f++
         }
         return g
     }
 });
-var Qs = W(E0 => {
+var Js = W(D0 => {
     "use strict";
-    E0.parseLinkLabel = Vs();
-    E0.parseLinkDestination = Ws();
-    E0.parseLinkTitle = Zs()
+    D0.parseLinkLabel = Us();
+    D0.parseLinkDestination = Zs();
+    D0.parseLinkTitle = Xs()
 });
-var Js = W((r2, Xs) => {
+var el = W((c2, Ks) => {
     "use strict";
-    var am = Se().assign,
-        sm = Se().unescapeAll,
+    var lm = Se().assign,
+        cm = Se().unescapeAll,
         or = Se().escapeHtml,
         Ct = {};
     Ct.code_inline = function(r, e, i, a, l) {
         var c = r[e];
         return "<code" + l.renderAttrs(c) + ">" + or(c.content) + "</code>"
     };
     Ct.code_block = function(r, e, i, a, l) {
         var c = r[e];
         return "<pre" + l.renderAttrs(c) + "><code>" + or(r[e].content) + `</code></pre>
 `
     };
     Ct.fence = function(r, e, i, a, l) {
         var c = r[e],
-            d = c.info ? sm(c.info).trim() : "",
+            d = c.info ? cm(c.info).trim() : "",
             f = "",
             g = "",
             y, _, w, T, A;
         return d && (w = d.split(/(\s+)/g), f = w[0], g = w.slice(2).join("")), i.highlight ? y = i.highlight(c.content, f, g) || or(c.content) : y = or(c.content), y.indexOf("<pre") === 0 ? y + `
 ` : d ? (_ = c.attrIndex("class"), T = c.attrs ? c.attrs.slice() : [], _ < 0 ? T.push(["class", i.langPrefix + f]) : (T[_] = T[_].slice(), T[_][1] += " " + i.langPrefix + f), A = {
             attrs: T
         }, "<pre><code" + l.renderAttrs(A) + ">" + y + `</code></pre>
@@ -3884,15 +3884,15 @@
         return r[e].content
     };
     Ct.html_inline = function(r, e) {
         return r[e].content
     };
 
     function fr() {
-        this.rules = am({}, Ct)
+        this.rules = lm({}, Ct)
     }
     fr.prototype.renderAttrs = function(e) {
         var i, a, l;
         if (!e.attrs) return "";
         for (l = "", i = 0, a = e.attrs.length; i < a; i++) l += " " + or(e.attrs[i][0]) + '="' + or(e.attrs[i][1]) + '"';
         return l
     };
@@ -3915,17 +3915,17 @@
     };
     fr.prototype.render = function(r, e, i) {
         var a, l, c, d = "",
             f = this.rules;
         for (a = 0, l = r.length; a < l; a++) c = r[a].type, c === "inline" ? d += this.renderInline(r[a].children, e, i) : typeof f[c] < "u" ? d += f[c](r, a, e, i, this) : d += this.renderToken(r, a, e, i);
         return d
     };
-    Xs.exports = fr
+    Ks.exports = fr
 });
-var D0 = W((n2, Ks) => {
+var z0 = W((u2, tl) => {
     "use strict";
 
     function xt() {
         this.__rules__ = [], this.__cache__ = null
     }
     xt.prototype.__find__ = function(r) {
         for (var e = 0; e < this.__rules__.length; e++)
@@ -4010,175 +4010,175 @@
             }
             this.__rules__[l].enabled = !1, i.push(a)
         }, this), this.__cache__ = null, i
     };
     xt.prototype.getRules = function(r) {
         return this.__cache__ === null && this.__compile__(), this.__cache__[r] || []
     };
-    Ks.exports = xt
+    tl.exports = xt
 });
-var tl = W((i2, el) => {
+var nl = W((h2, rl) => {
     "use strict";
-    var lm = /\r\n?|\n/g,
-        cm = /\0/g;
-    el.exports = function(e) {
+    var um = /\r\n?|\n/g,
+        hm = /\0/g;
+    rl.exports = function(e) {
         var i;
-        i = e.src.replace(lm, `
-`), i = i.replace(cm, "\uFFFD"), e.src = i
+        i = e.src.replace(um, `
+`), i = i.replace(hm, "\uFFFD"), e.src = i
     }
 });
-var nl = W((o2, rl) => {
+var ol = W((d2, il) => {
     "use strict";
-    rl.exports = function(e) {
+    il.exports = function(e) {
         var i;
         e.inlineMode ? (i = new e.Token("inline", "", 0), i.content = e.src, i.map = [0, 1], i.children = [], e.tokens.push(i)) : e.md.block.parse(e.src, e.md, e.env, e.tokens)
     }
 });
-var ol = W((a2, il) => {
+var sl = W((m2, al) => {
     "use strict";
-    il.exports = function(e) {
+    al.exports = function(e) {
         var i = e.tokens,
             a, l, c;
         for (l = 0, c = i.length; l < c; l++) a = i[l], a.type === "inline" && e.md.inline.parse(a.content, e.md, e.env, a.children)
     }
 });
-var sl = W((s2, al) => {
+var cl = W((p2, ll) => {
     "use strict";
-    var um = Se().arrayReplaceAt;
+    var dm = Se().arrayReplaceAt;
 
-    function hm(r) {
+    function mm(r) {
         return /^<a[>\s]/i.test(r)
     }
 
-    function dm(r) {
+    function pm(r) {
         return /^<\/a\s*>/i.test(r)
     }
-    al.exports = function(e) {
+    ll.exports = function(e) {
         var i, a, l, c, d, f, g, y, _, w, T, A, L, R, O, P, I = e.tokens,
             Y;
         if (e.md.options.linkify) {
             for (a = 0, l = I.length; a < l; a++)
                 if (!(I[a].type !== "inline" || !e.md.linkify.pretest(I[a].content)))
                     for (c = I[a].children, L = 0, i = c.length - 1; i >= 0; i--) {
                         if (f = c[i], f.type === "link_close") {
                             for (i--; c[i].level !== f.level && c[i].type !== "link_open";) i--;
                             continue
                         }
-                        if (f.type === "html_inline" && (hm(f.content) && L > 0 && L--, dm(f.content) && L++), !(L > 0) && f.type === "text" && e.md.linkify.test(f.content)) {
+                        if (f.type === "html_inline" && (mm(f.content) && L > 0 && L--, pm(f.content) && L++), !(L > 0) && f.type === "text" && e.md.linkify.test(f.content)) {
                             for (_ = f.content, Y = e.md.linkify.match(_), g = [], A = f.level, T = 0, Y.length > 0 && Y[0].index === 0 && i > 0 && c[i - 1].type === "text_special" && (Y = Y.slice(1)), y = 0; y < Y.length; y++) R = Y[y].url, O = e.md.normalizeLink(R), e.md.validateLink(O) && (P = Y[y].text, Y[y].schema ? Y[y].schema === "mailto:" && !/^mailto:/i.test(P) ? P = e.md.normalizeLinkText("mailto:" + P).replace(/^mailto:/, "") : P = e.md.normalizeLinkText(P) : P = e.md.normalizeLinkText("http://" + P).replace(/^http:\/\//, ""), w = Y[y].index, w > T && (d = new e.Token("text", "", 0), d.content = _.slice(T, w), d.level = A, g.push(d)), d = new e.Token("link_open", "a", 1), d.attrs = [
                                 ["href", O]
                             ], d.level = A++, d.markup = "linkify", d.info = "auto", g.push(d), d = new e.Token("text", "", 0), d.content = P, d.level = A, g.push(d), d = new e.Token("link_close", "a", -1), d.level = --A, d.markup = "linkify", d.info = "auto", g.push(d), T = Y[y].lastIndex);
-                            T < _.length && (d = new e.Token("text", "", 0), d.content = _.slice(T), d.level = A, g.push(d)), I[a].children = c = um(c, i, g)
+                            T < _.length && (d = new e.Token("text", "", 0), d.content = _.slice(T), d.level = A, g.push(d)), I[a].children = c = dm(c, i, g)
                         }
                     }
         }
     }
 });
-var ul = W((l2, cl) => {
+var dl = W((f2, hl) => {
     "use strict";
-    var ll = /\+-|\.\.|\?\?\?\?|!!!!|,,|--/,
-        mm = /\((c|tm|r)\)/i,
-        pm = /\((c|tm|r)\)/ig,
-        fm = {
+    var ul = /\+-|\.\.|\?\?\?\?|!!!!|,,|--/,
+        fm = /\((c|tm|r)\)/i,
+        gm = /\((c|tm|r)\)/ig,
+        bm = {
             c: "\xA9",
             r: "\xAE",
             tm: "\u2122"
         };
 
-    function gm(r, e) {
-        return fm[e.toLowerCase()]
+    function ym(r, e) {
+        return bm[e.toLowerCase()]
     }
 
-    function bm(r) {
+    function xm(r) {
         var e, i, a = 0;
-        for (e = r.length - 1; e >= 0; e--) i = r[e], i.type === "text" && !a && (i.content = i.content.replace(pm, gm)), i.type === "link_open" && i.info === "auto" && a--, i.type === "link_close" && i.info === "auto" && a++
+        for (e = r.length - 1; e >= 0; e--) i = r[e], i.type === "text" && !a && (i.content = i.content.replace(gm, ym)), i.type === "link_open" && i.info === "auto" && a--, i.type === "link_close" && i.info === "auto" && a++
     }
 
-    function ym(r) {
+    function vm(r) {
         var e, i, a = 0;
-        for (e = r.length - 1; e >= 0; e--) i = r[e], i.type === "text" && !a && ll.test(i.content) && (i.content = i.content.replace(/\+-/g, "\xB1").replace(/\.{2,}/g, "\u2026").replace(/([?!])…/g, "$1..").replace(/([?!]){4,}/g, "$1$1$1").replace(/,{2,}/g, ",").replace(/(^|[^-])---(?=[^-]|$)/mg, "$1\u2014").replace(/(^|\s)--(?=\s|$)/mg, "$1\u2013").replace(/(^|[^-\s])--(?=[^-\s]|$)/mg, "$1\u2013")), i.type === "link_open" && i.info === "auto" && a--, i.type === "link_close" && i.info === "auto" && a++
+        for (e = r.length - 1; e >= 0; e--) i = r[e], i.type === "text" && !a && ul.test(i.content) && (i.content = i.content.replace(/\+-/g, "\xB1").replace(/\.{2,}/g, "\u2026").replace(/([?!])…/g, "$1..").replace(/([?!]){4,}/g, "$1$1$1").replace(/,{2,}/g, ",").replace(/(^|[^-])---(?=[^-]|$)/mg, "$1\u2014").replace(/(^|\s)--(?=\s|$)/mg, "$1\u2013").replace(/(^|[^-\s])--(?=[^-\s]|$)/mg, "$1\u2013")), i.type === "link_open" && i.info === "auto" && a--, i.type === "link_close" && i.info === "auto" && a++
     }
-    cl.exports = function(e) {
+    hl.exports = function(e) {
         var i;
         if (e.md.options.typographer)
-            for (i = e.tokens.length - 1; i >= 0; i--) e.tokens[i].type === "inline" && (mm.test(e.tokens[i].content) && bm(e.tokens[i].children), ll.test(e.tokens[i].content) && ym(e.tokens[i].children))
+            for (i = e.tokens.length - 1; i >= 0; i--) e.tokens[i].type === "inline" && (fm.test(e.tokens[i].content) && xm(e.tokens[i].children), ul.test(e.tokens[i].content) && vm(e.tokens[i].children))
     }
 });
-var bl = W((c2, gl) => {
+var xl = W((g2, yl) => {
     "use strict";
-    var hl = Se().isWhiteSpace,
-        dl = Se().isPunctChar,
-        ml = Se().isMdAsciiPunct,
-        xm = /['"]/,
-        pl = /['"]/g,
-        fl = "\u2019";
+    var ml = Se().isWhiteSpace,
+        pl = Se().isPunctChar,
+        fl = Se().isMdAsciiPunct,
+        wm = /['"]/,
+        gl = /['"]/g,
+        bl = "\u2019";
 
-    function z0(r, e, i) {
+    function R0(r, e, i) {
         return r.slice(0, e) + i + r.slice(e + 1)
     }
 
-    function vm(r, e) {
+    function km(r, e) {
         var i, a, l, c, d, f, g, y, _, w, T, A, L, R, O, P, I, Y, re, te, j;
         for (re = [], i = 0; i < r.length; i++) {
             for (a = r[i], g = r[i].level, I = re.length - 1; I >= 0 && !(re[I].level <= g); I--);
             if (re.length = I + 1, a.type === "text") {
                 l = a.content, d = 0, f = l.length;
-                e: for (; d < f && (pl.lastIndex = d, c = pl.exec(l), !!c);) {
+                e: for (; d < f && (gl.lastIndex = d, c = gl.exec(l), !!c);) {
                     if (O = P = !0, d = c.index + 1, Y = c[0] === "'", _ = 32, c.index - 1 >= 0) _ = l.charCodeAt(c.index - 1);
                     else
                         for (I = i - 1; I >= 0 && !(r[I].type === "softbreak" || r[I].type === "hardbreak"); I--)
                             if (r[I].content) {
                                 _ = r[I].content.charCodeAt(r[I].content.length - 1);
                                 break
                             } if (w = 32, d < f) w = l.charCodeAt(d);
                     else
                         for (I = i + 1; I < r.length && !(r[I].type === "softbreak" || r[I].type === "hardbreak"); I++)
                             if (r[I].content) {
                                 w = r[I].content.charCodeAt(0);
                                 break
-                            } if (T = ml(_) || dl(String.fromCharCode(_)), A = ml(w) || dl(String.fromCharCode(w)), L = hl(_), R = hl(w), R ? O = !1 : A && (L || T || (O = !1)), L ? P = !1 : T && (R || A || (P = !1)), w === 34 && c[0] === '"' && _ >= 48 && _ <= 57 && (P = O = !1), O && P && (O = T, P = A), !O && !P) {
-                        Y && (a.content = z0(a.content, c.index, fl));
+                            } if (T = fl(_) || pl(String.fromCharCode(_)), A = fl(w) || pl(String.fromCharCode(w)), L = ml(_), R = ml(w), R ? O = !1 : A && (L || T || (O = !1)), L ? P = !1 : T && (R || A || (P = !1)), w === 34 && c[0] === '"' && _ >= 48 && _ <= 57 && (P = O = !1), O && P && (O = T, P = A), !O && !P) {
+                        Y && (a.content = R0(a.content, c.index, bl));
                         continue
                     }
                     if (P) {
                         for (I = re.length - 1; I >= 0 && (y = re[I], !(re[I].level < g)); I--)
                             if (y.single === Y && re[I].level === g) {
-                                y = re[I], Y ? (te = e.md.options.quotes[2], j = e.md.options.quotes[3]) : (te = e.md.options.quotes[0], j = e.md.options.quotes[1]), a.content = z0(a.content, c.index, j), r[y.token].content = z0(r[y.token].content, y.pos, te), d += j.length - 1, y.token === i && (d += te.length - 1), l = a.content, f = l.length, re.length = I;
+                                y = re[I], Y ? (te = e.md.options.quotes[2], j = e.md.options.quotes[3]) : (te = e.md.options.quotes[0], j = e.md.options.quotes[1]), a.content = R0(a.content, c.index, j), r[y.token].content = R0(r[y.token].content, y.pos, te), d += j.length - 1, y.token === i && (d += te.length - 1), l = a.content, f = l.length, re.length = I;
                                 continue e
                             }
                     }
                     O ? re.push({
                         token: i,
                         pos: c.index,
                         single: Y,
                         level: g
-                    }) : P && Y && (a.content = z0(a.content, c.index, fl))
+                    }) : P && Y && (a.content = R0(a.content, c.index, bl))
                 }
             }
         }
     }
-    gl.exports = function(e) {
+    yl.exports = function(e) {
         var i;
         if (e.md.options.typographer)
-            for (i = e.tokens.length - 1; i >= 0; i--) e.tokens[i].type !== "inline" || !xm.test(e.tokens[i].content) || vm(e.tokens[i].children, e)
+            for (i = e.tokens.length - 1; i >= 0; i--) e.tokens[i].type !== "inline" || !wm.test(e.tokens[i].content) || km(e.tokens[i].children, e)
     }
 });
-var xl = W((u2, yl) => {
+var wl = W((b2, vl) => {
     "use strict";
-    yl.exports = function(e) {
+    vl.exports = function(e) {
         var i, a, l, c, d, f, g = e.tokens;
         for (i = 0, a = g.length; i < a; i++)
             if (g[i].type === "inline") {
                 for (l = g[i].children, d = l.length, c = 0; c < d; c++) l[c].type === "text_special" && (l[c].type = "text");
                 for (c = f = 0; c < d; c++) l[c].type === "text" && c + 1 < d && l[c + 1].type === "text" ? l[c + 1].content = l[c].content + l[c + 1].content : (c !== f && (l[f] = l[c]), f++);
                 c !== f && (l.length = f)
             }
     }
 });
-var R0 = W((h2, vl) => {
+var F0 = W((y2, kl) => {
     "use strict";
 
     function gr(r, e, i) {
         this.type = r, this.tag = e, this.attrs = null, this.map = null, this.nesting = i, this.level = 0, this.children = null, this.content = "", this.markup = "", this.info = "", this.meta = null, this.block = !1, this.hidden = !1
     }
     gr.prototype.attrIndex = function(e) {
         var i, a, l;
@@ -4200,107 +4200,107 @@
             a = null;
         return i >= 0 && (a = this.attrs[i][1]), a
     };
     gr.prototype.attrJoin = function(e, i) {
         var a = this.attrIndex(e);
         a < 0 ? this.attrPush([e, i]) : this.attrs[a][1] = this.attrs[a][1] + " " + i
     };
-    vl.exports = gr
+    kl.exports = gr
 });
-var _l = W((d2, kl) => {
+var Cl = W((x2, Sl) => {
     "use strict";
-    var wm = R0();
+    var _m = F0();
 
-    function wl(r, e, i) {
+    function _l(r, e, i) {
         this.src = r, this.env = i, this.tokens = [], this.inlineMode = !1, this.md = e
     }
-    wl.prototype.Token = wm;
-    kl.exports = wl
+    _l.prototype.Token = _m;
+    Sl.exports = _l
 });
-var Cl = W((m2, Sl) => {
+var Al = W((v2, Tl) => {
     "use strict";
-    var km = D0(),
-        li = [
-            ["normalize", tl()],
-            ["block", nl()],
-            ["inline", ol()],
-            ["linkify", sl()],
-            ["replacements", ul()],
-            ["smartquotes", bl()],
-            ["text_join", xl()]
+    var Sm = z0(),
+        ui = [
+            ["normalize", nl()],
+            ["block", ol()],
+            ["inline", sl()],
+            ["linkify", cl()],
+            ["replacements", dl()],
+            ["smartquotes", xl()],
+            ["text_join", wl()]
         ];
 
-    function ci() {
-        this.ruler = new km;
-        for (var r = 0; r < li.length; r++) this.ruler.push(li[r][0], li[r][1])
+    function hi() {
+        this.ruler = new Sm;
+        for (var r = 0; r < ui.length; r++) this.ruler.push(ui[r][0], ui[r][1])
     }
-    ci.prototype.process = function(r) {
+    hi.prototype.process = function(r) {
         var e, i, a;
         for (a = this.ruler.getRules(""), e = 0, i = a.length; e < i; e++) a[e](r)
     };
-    ci.prototype.State = _l();
-    Sl.exports = ci
+    hi.prototype.State = Cl();
+    Tl.exports = hi
 });
-var ql = W((p2, Al) => {
+var El = W((w2, Ml) => {
     "use strict";
-    var ui = Se().isSpace;
+    var di = Se().isSpace;
 
-    function hi(r, e) {
+    function mi(r, e) {
         var i = r.bMarks[e] + r.tShift[e],
             a = r.eMarks[e];
         return r.src.slice(i, a)
     }
 
-    function Tl(r) {
+    function ql(r) {
         var e = [],
             i = 0,
             a = r.length,
             l, c = !1,
             d = 0,
             f = "";
         for (l = r.charCodeAt(i); i < a;) l === 124 && (c ? (f += r.substring(d, i - 1), d = i) : (e.push(f + r.substring(d, i)), f = "", d = i + 1)), c = l === 92, i++, l = r.charCodeAt(i);
         return e.push(f + r.substring(d)), e
     }
-    Al.exports = function(e, i, a, l) {
+    Ml.exports = function(e, i, a, l) {
         var c, d, f, g, y, _, w, T, A, L, R, O, P, I, Y, re, te, j;
-        if (i + 2 > a || (_ = i + 1, e.sCount[_] < e.blkIndent) || e.sCount[_] - e.blkIndent >= 4 || (f = e.bMarks[_] + e.tShift[_], f >= e.eMarks[_]) || (te = e.src.charCodeAt(f++), te !== 124 && te !== 45 && te !== 58) || f >= e.eMarks[_] || (j = e.src.charCodeAt(f++), j !== 124 && j !== 45 && j !== 58 && !ui(j)) || te === 45 && ui(j)) return !1;
+        if (i + 2 > a || (_ = i + 1, e.sCount[_] < e.blkIndent) || e.sCount[_] - e.blkIndent >= 4 || (f = e.bMarks[_] + e.tShift[_], f >= e.eMarks[_]) || (te = e.src.charCodeAt(f++), te !== 124 && te !== 45 && te !== 58) || f >= e.eMarks[_] || (j = e.src.charCodeAt(f++), j !== 124 && j !== 45 && j !== 58 && !di(j)) || te === 45 && di(j)) return !1;
         for (; f < e.eMarks[_];) {
-            if (c = e.src.charCodeAt(f), c !== 124 && c !== 45 && c !== 58 && !ui(c)) return !1;
+            if (c = e.src.charCodeAt(f), c !== 124 && c !== 45 && c !== 58 && !di(c)) return !1;
             f++
         }
-        for (d = hi(e, i + 1), w = d.split("|"), L = [], g = 0; g < w.length; g++) {
+        for (d = mi(e, i + 1), w = d.split("|"), L = [], g = 0; g < w.length; g++) {
             if (R = w[g].trim(), !R) {
                 if (g === 0 || g === w.length - 1) continue;
                 return !1
             }
             if (!/^:?-+:?$/.test(R)) return !1;
             R.charCodeAt(R.length - 1) === 58 ? L.push(R.charCodeAt(0) === 58 ? "center" : "right") : R.charCodeAt(0) === 58 ? L.push("left") : L.push("")
         }
-        if (d = hi(e, i).trim(), d.indexOf("|") === -1 || e.sCount[i] - e.blkIndent >= 4 || (w = Tl(d), w.length && w[0] === "" && w.shift(), w.length && w[w.length - 1] === "" && w.pop(), T = w.length, T === 0 || T !== L.length)) return !1;
+        if (d = mi(e, i).trim(), d.indexOf("|") === -1 || e.sCount[i] - e.blkIndent >= 4 || (w = ql(d), w.length && w[0] === "" && w.shift(), w.length && w[w.length - 1] === "" && w.pop(), T = w.length, T === 0 || T !== L.length)) return !1;
         if (l) return !0;
         for (I = e.parentType, e.parentType = "table", re = e.md.block.ruler.getRules("blockquote"), A = e.push("table_open", "table", 1), A.map = O = [i, 0], A = e.push("thead_open", "thead", 1), A.map = [i, i + 1], A = e.push("tr_open", "tr", 1), A.map = [i, i + 1], g = 0; g < w.length; g++) A = e.push("th_open", "th", 1), L[g] && (A.attrs = [
             ["style", "text-align:" + L[g]]
         ]), A = e.push("inline", "", 0), A.content = w[g].trim(), A.children = [], A = e.push("th_close", "th", -1);
         for (A = e.push("tr_close", "tr", -1), A = e.push("thead_close", "thead", -1), _ = i + 2; _ < a && !(e.sCount[_] < e.blkIndent); _++) {
             for (Y = !1, g = 0, y = re.length; g < y; g++)
                 if (re[g](e, _, a, !0)) {
                     Y = !0;
                     break
-                } if (Y || (d = hi(e, _).trim(), !d) || e.sCount[_] - e.blkIndent >= 4) break;
-            for (w = Tl(d), w.length && w[0] === "" && w.shift(), w.length && w[w.length - 1] === "" && w.pop(), _ === i + 2 && (A = e.push("tbody_open", "tbody", 1), A.map = P = [i + 2, 0]), A = e.push("tr_open", "tr", 1), A.map = [_, _ + 1], g = 0; g < T; g++) A = e.push("td_open", "td", 1), L[g] && (A.attrs = [
+                } if (Y || (d = mi(e, _).trim(), !d) || e.sCount[_] - e.blkIndent >= 4) break;
+            for (w = ql(d), w.length && w[0] === "" && w.shift(), w.length && w[w.length - 1] === "" && w.pop(), _ === i + 2 && (A = e.push("tbody_open", "tbody", 1), A.map = P = [i + 2, 0]), A = e.push("tr_open", "tr", 1), A.map = [_, _ + 1], g = 0; g < T; g++) A = e.push("td_open", "td", 1), L[g] && (A.attrs = [
                 ["style", "text-align:" + L[g]]
             ]), A = e.push("inline", "", 0), A.content = w[g] ? w[g].trim() : "", A.children = [], A = e.push("td_close", "td", -1);
             A = e.push("tr_close", "tr", -1)
         }
         return P && (A = e.push("tbody_close", "tbody", -1), P[1] = _), A = e.push("table_close", "table", -1), O[1] = _, e.parentType = I, e.line = _, !0
     }
 });
-var El = W((f2, Ml) => {
+var zl = W((k2, Dl) => {
     "use strict";
-    Ml.exports = function(e, i, a) {
+    Dl.exports = function(e, i, a) {
         var l, c, d;
         if (e.sCount[i] - e.blkIndent < 4) return !1;
         for (c = l = i + 1; l < a;) {
             if (e.isEmpty(l)) {
                 l++;
                 continue
             }
@@ -4310,41 +4310,41 @@
             }
             break
         }
         return e.line = c, d = e.push("code_block", "code", 0), d.content = e.getLines(i, c, 4 + e.blkIndent, !1) + `
 `, d.map = [i, e.line], !0
     }
 });
-var zl = W((g2, Dl) => {
+var Fl = W((_2, Rl) => {
     "use strict";
-    Dl.exports = function(e, i, a, l) {
+    Rl.exports = function(e, i, a, l) {
         var c, d, f, g, y, _, w, T = !1,
             A = e.bMarks[i] + e.tShift[i],
             L = e.eMarks[i];
         if (e.sCount[i] - e.blkIndent >= 4 || A + 3 > L || (c = e.src.charCodeAt(A), c !== 126 && c !== 96) || (y = A, A = e.skipChars(A, c), d = A - y, d < 3) || (w = e.src.slice(y, A), f = e.src.slice(A, L), c === 96 && f.indexOf(String.fromCharCode(c)) >= 0)) return !1;
         if (l) return !0;
         for (g = i; g++, !(g >= a || (A = y = e.bMarks[g] + e.tShift[g], L = e.eMarks[g], A < L && e.sCount[g] < e.blkIndent));)
             if (e.src.charCodeAt(A) === c && !(e.sCount[g] - e.blkIndent >= 4) && (A = e.skipChars(A, c), !(A - y < d) && (A = e.skipSpaces(A), !(A < L)))) {
                 T = !0;
                 break
             } return d = e.sCount[i], e.line = g + (T ? 1 : 0), _ = e.push("fence", "code", 0), _.info = f, _.content = e.getLines(i + 1, g, d, !0), _.markup = w, _.map = [i, e.line], !0
     }
 });
-var Fl = W((b2, Rl) => {
+var Nl = W((S2, Bl) => {
     "use strict";
-    var _m = Se().isSpace;
-    Rl.exports = function(e, i, a, l) {
+    var Cm = Se().isSpace;
+    Bl.exports = function(e, i, a, l) {
         var c, d, f, g, y, _, w, T, A, L, R, O, P, I, Y, re, te, j, ne, pe, ue = e.lineMax,
             ce = e.bMarks[i] + e.tShift[i],
             Ce = e.eMarks[i];
         if (e.sCount[i] - e.blkIndent >= 4 || e.src.charCodeAt(ce) !== 62) return !1;
         if (l) return !0;
         for (L = [], R = [], I = [], Y = [], j = e.md.block.ruler.getRules("blockquote"), P = e.parentType, e.parentType = "blockquote", T = i; T < a && (pe = e.sCount[T] < e.blkIndent, ce = e.bMarks[T] + e.tShift[T], Ce = e.eMarks[T], !(ce >= Ce)); T++) {
             if (e.src.charCodeAt(ce++) === 62 && !pe) {
-                for (g = e.sCount[T] + 1, e.src.charCodeAt(ce) === 32 ? (ce++, g++, c = !1, re = !0) : e.src.charCodeAt(ce) === 9 ? (re = !0, (e.bsCount[T] + g) % 4 === 3 ? (ce++, g++, c = !1) : c = !0) : re = !1, A = g, L.push(e.bMarks[T]), e.bMarks[T] = ce; ce < Ce && (d = e.src.charCodeAt(ce), _m(d));) {
+                for (g = e.sCount[T] + 1, e.src.charCodeAt(ce) === 32 ? (ce++, g++, c = !1, re = !0) : e.src.charCodeAt(ce) === 9 ? (re = !0, (e.bsCount[T] + g) % 4 === 3 ? (ce++, g++, c = !1) : c = !0) : re = !1, A = g, L.push(e.bMarks[T]), e.bMarks[T] = ce; ce < Ce && (d = e.src.charCodeAt(ce), Cm(d));) {
                     d === 9 ? A += 4 - (A + e.bsCount[T] + (c ? 1 : 0)) % 4 : A++;
                     ce++
                 }
                 _ = ce >= Ce, R.push(e.bsCount[T]), e.bsCount[T] = e.sCount[T] + 1 + (re ? 1 : 0), I.push(e.sCount[T]), e.sCount[T] = A - g, Y.push(e.tShift[T]), e.tShift[T] = ce - e.bMarks[T];
                 continue
             }
             if (_) break;
@@ -4358,66 +4358,66 @@
             }
             L.push(e.bMarks[T]), R.push(e.bsCount[T]), Y.push(e.tShift[T]), I.push(e.sCount[T]), e.sCount[T] = -1
         }
         for (O = e.blkIndent, e.blkIndent = 0, ne = e.push("blockquote_open", "blockquote", 1), ne.markup = ">", ne.map = w = [i, 0], e.md.block.tokenize(e, i, T), ne = e.push("blockquote_close", "blockquote", -1), ne.markup = ">", e.lineMax = ue, e.parentType = P, w[1] = e.line, f = 0; f < Y.length; f++) e.bMarks[f + i] = L[f], e.tShift[f + i] = Y[f], e.sCount[f + i] = I[f], e.bsCount[f + i] = R[f];
         return e.blkIndent = O, !0
     }
 });
-var Nl = W((y2, Bl) => {
+var Pl = W((C2, Ll) => {
     "use strict";
-    var Sm = Se().isSpace;
-    Bl.exports = function(e, i, a, l) {
+    var Tm = Se().isSpace;
+    Ll.exports = function(e, i, a, l) {
         var c, d, f, g, y = e.bMarks[i] + e.tShift[i],
             _ = e.eMarks[i];
         if (e.sCount[i] - e.blkIndent >= 4 || (c = e.src.charCodeAt(y++), c !== 42 && c !== 45 && c !== 95)) return !1;
         for (d = 1; y < _;) {
-            if (f = e.src.charCodeAt(y++), f !== c && !Sm(f)) return !1;
+            if (f = e.src.charCodeAt(y++), f !== c && !Tm(f)) return !1;
             f === c && d++
         }
         return d < 3 ? !1 : (l || (e.line = i + 1, g = e.push("hr", "hr", 0), g.map = [i, e.line], g.markup = Array(d + 1).join(String.fromCharCode(c))), !0)
     }
 });
-var Hl = W((x2, Ol) => {
+var Gl = W((T2, $l) => {
     "use strict";
-    var Il = Se().isSpace;
+    var Hl = Se().isSpace;
 
-    function Ll(r, e) {
+    function Il(r, e) {
         var i, a, l, c;
-        return a = r.bMarks[e] + r.tShift[e], l = r.eMarks[e], i = r.src.charCodeAt(a++), i !== 42 && i !== 45 && i !== 43 || a < l && (c = r.src.charCodeAt(a), !Il(c)) ? -1 : a
+        return a = r.bMarks[e] + r.tShift[e], l = r.eMarks[e], i = r.src.charCodeAt(a++), i !== 42 && i !== 45 && i !== 43 || a < l && (c = r.src.charCodeAt(a), !Hl(c)) ? -1 : a
     }
 
-    function Pl(r, e) {
+    function Ol(r, e) {
         var i, a = r.bMarks[e] + r.tShift[e],
             l = a,
             c = r.eMarks[e];
         if (l + 1 >= c || (i = r.src.charCodeAt(l++), i < 48 || i > 57)) return -1;
         for (;;) {
             if (l >= c) return -1;
             if (i = r.src.charCodeAt(l++), i >= 48 && i <= 57) {
                 if (l - a >= 10) return -1;
                 continue
             }
             if (i === 41 || i === 46) break;
             return -1
         }
-        return l < c && (i = r.src.charCodeAt(l), !Il(i)) ? -1 : l
+        return l < c && (i = r.src.charCodeAt(l), !Hl(i)) ? -1 : l
     }
 
-    function Cm(r, e) {
+    function Am(r, e) {
         var i, a, l = r.level + 2;
         for (i = e + 2, a = r.tokens.length - 2; i < a; i++) r.tokens[i].level === l && r.tokens[i].type === "paragraph_open" && (r.tokens[i + 2].hidden = !0, r.tokens[i].hidden = !0, i += 2)
     }
-    Ol.exports = function(e, i, a, l) {
+    $l.exports = function(e, i, a, l) {
         var c, d, f, g, y, _, w, T, A, L, R, O, P, I, Y, re, te, j, ne, pe, ue, ce, Ce, De, U, X, he, oe = i,
             ae = !1,
             ee = !0;
         if (e.sCount[oe] - e.blkIndent >= 4 || e.listIndent >= 0 && e.sCount[oe] - e.listIndent >= 4 && e.sCount[oe] < e.blkIndent) return !1;
-        if (l && e.parentType === "paragraph" && e.sCount[oe] >= e.blkIndent && (ae = !0), (ce = Pl(e, oe)) >= 0) {
+        if (l && e.parentType === "paragraph" && e.sCount[oe] >= e.blkIndent && (ae = !0), (ce = Ol(e, oe)) >= 0) {
             if (w = !0, De = e.bMarks[oe] + e.tShift[oe], P = Number(e.src.slice(De, ce - 1)), ae && P !== 1) return !1
-        } else if ((ce = Ll(e, oe)) >= 0) w = !1;
+        } else if ((ce = Il(e, oe)) >= 0) w = !1;
         else return !1;
         if (ae && e.skipSpaces(ce) >= e.eMarks[oe]) return !1;
         if (l) return !0;
         for (O = e.src.charCodeAt(ce - 1), R = e.tokens.length, w ? (he = e.push("ordered_list_open", "ol", 1), P !== 1 && (he.attrs = [
                 ["start", P]
             ])) : he = e.push("bullet_list_open", "ul", 1), he.map = L = [oe, 0], he.markup = String.fromCharCode(O), Ce = !1, X = e.md.block.ruler.getRules("list"), te = e.parentType, e.parentType = "list"; oe < a;) {
             for (ue = ce, I = e.eMarks[oe], _ = Y = e.sCount[oe] + ce - (e.bMarks[oe] + e.tShift[oe]); ue < I;) {
@@ -4429,27 +4429,27 @@
             if (d = ue, d >= I ? y = 1 : y = Y - _, y > 4 && (y = 1), g = _ + y, he = e.push("list_item_open", "li", 1), he.markup = String.fromCharCode(O), he.map = T = [oe, 0], w && (he.info = e.src.slice(De, ce - 1)), pe = e.tight, ne = e.tShift[oe], j = e.sCount[oe], re = e.listIndent, e.listIndent = e.blkIndent, e.blkIndent = g, e.tight = !0, e.tShift[oe] = d - e.bMarks[oe], e.sCount[oe] = Y, d >= I && e.isEmpty(oe + 1) ? e.line = Math.min(e.line + 2, a) : e.md.block.tokenize(e, oe, a, !0), (!e.tight || Ce) && (ee = !1), Ce = e.line - oe > 1 && e.isEmpty(e.line - 1), e.blkIndent = e.listIndent, e.listIndent = re, e.tShift[oe] = ne, e.sCount[oe] = j, e.tight = pe, he = e.push("list_item_close", "li", -1), he.markup = String.fromCharCode(O), oe = e.line, T[1] = oe, oe >= a || e.sCount[oe] < e.blkIndent || e.sCount[oe] - e.blkIndent >= 4) break;
             for (U = !1, f = 0, A = X.length; f < A; f++)
                 if (X[f](e, oe, a, !0)) {
                     U = !0;
                     break
                 } if (U) break;
             if (w) {
-                if (ce = Pl(e, oe), ce < 0) break;
+                if (ce = Ol(e, oe), ce < 0) break;
                 De = e.bMarks[oe] + e.tShift[oe]
-            } else if (ce = Ll(e, oe), ce < 0) break;
+            } else if (ce = Il(e, oe), ce < 0) break;
             if (O !== e.src.charCodeAt(ce - 1)) break
         }
-        return w ? he = e.push("ordered_list_close", "ol", -1) : he = e.push("bullet_list_close", "ul", -1), he.markup = String.fromCharCode(O), L[1] = oe, e.line = oe, e.parentType = te, ee && Cm(e, R), !0
+        return w ? he = e.push("ordered_list_close", "ol", -1) : he = e.push("bullet_list_close", "ul", -1), he.markup = String.fromCharCode(O), L[1] = oe, e.line = oe, e.parentType = te, ee && Am(e, R), !0
     }
 });
-var Gl = W((v2, $l) => {
+var jl = W((A2, Vl) => {
     "use strict";
-    var Tm = Se().normalizeReference,
-        F0 = Se().isSpace;
-    $l.exports = function(e, i, a, l) {
+    var qm = Se().normalizeReference,
+        B0 = Se().isSpace;
+    Vl.exports = function(e, i, a, l) {
         var c, d, f, g, y, _, w, T, A, L, R, O, P, I, Y, re, te = 0,
             j = e.bMarks[i] + e.tShift[i],
             ne = e.eMarks[i],
             pe = i + 1;
         if (e.sCount[i] - e.blkIndent >= 4 || e.src.charCodeAt(j) !== 91) return !1;
         for (; ++j < ne;)
             if (e.src.charCodeAt(j) === 93 && e.src.charCodeAt(j - 1) !== 92) {
@@ -4468,65 +4468,65 @@
                 A = j;
                 break
             } else c === 10 ? te++ : c === 92 && (j++, j < ne && P.charCodeAt(j) === 10 && te++)
         }
         if (A < 0 || P.charCodeAt(A + 1) !== 58) return !1;
         for (j = A + 2; j < ne; j++)
             if (c = P.charCodeAt(j), c === 10) te++;
-            else if (!F0(c)) break;
+            else if (!B0(c)) break;
         if (R = e.md.helpers.parseLinkDestination(P, j, ne), !R.ok || (y = e.md.normalizeLink(R.str), !e.md.validateLink(y))) return !1;
         for (j = R.pos, te += R.lines, d = j, f = te, O = j; j < ne; j++)
             if (c = P.charCodeAt(j), c === 10) te++;
-            else if (!F0(c)) break;
-        for (R = e.md.helpers.parseLinkTitle(P, j, ne), j < ne && O !== j && R.ok ? (re = R.str, j = R.pos, te += R.lines) : (re = "", j = d, te = f); j < ne && (c = P.charCodeAt(j), !!F0(c));) j++;
+            else if (!B0(c)) break;
+        for (R = e.md.helpers.parseLinkTitle(P, j, ne), j < ne && O !== j && R.ok ? (re = R.str, j = R.pos, te += R.lines) : (re = "", j = d, te = f); j < ne && (c = P.charCodeAt(j), !!B0(c));) j++;
         if (j < ne && P.charCodeAt(j) !== 10 && re)
-            for (re = "", j = d, te = f; j < ne && (c = P.charCodeAt(j), !!F0(c));) j++;
-        return j < ne && P.charCodeAt(j) !== 10 || (T = Tm(P.slice(1, A)), !T) ? !1 : (l || (typeof e.env.references > "u" && (e.env.references = {}), typeof e.env.references[T] > "u" && (e.env.references[T] = {
+            for (re = "", j = d, te = f; j < ne && (c = P.charCodeAt(j), !!B0(c));) j++;
+        return j < ne && P.charCodeAt(j) !== 10 || (T = qm(P.slice(1, A)), !T) ? !1 : (l || (typeof e.env.references > "u" && (e.env.references = {}), typeof e.env.references[T] > "u" && (e.env.references[T] = {
             title: re,
             href: y
         }), e.parentType = L, e.line = i + te + 1), !0)
     }
 });
-var jl = W((w2, Vl) => {
+var Wl = W((q2, Ul) => {
     "use strict";
-    Vl.exports = ["address", "article", "aside", "base", "basefont", "blockquote", "body", "caption", "center", "col", "colgroup", "dd", "details", "dialog", "dir", "div", "dl", "dt", "fieldset", "figcaption", "figure", "footer", "form", "frame", "frameset", "h1", "h2", "h3", "h4", "h5", "h6", "head", "header", "hr", "html", "iframe", "legend", "li", "link", "main", "menu", "menuitem", "nav", "noframes", "ol", "optgroup", "option", "p", "param", "section", "source", "summary", "table", "tbody", "td", "tfoot", "th", "thead", "title", "tr", "track", "ul"]
+    Ul.exports = ["address", "article", "aside", "base", "basefont", "blockquote", "body", "caption", "center", "col", "colgroup", "dd", "details", "dialog", "dir", "div", "dl", "dt", "fieldset", "figcaption", "figure", "footer", "form", "frame", "frameset", "h1", "h2", "h3", "h4", "h5", "h6", "head", "header", "hr", "html", "iframe", "legend", "li", "link", "main", "menu", "menuitem", "nav", "noframes", "ol", "optgroup", "option", "p", "param", "section", "source", "summary", "table", "tbody", "td", "tfoot", "th", "thead", "title", "tr", "track", "ul"]
 });
-var mi = W((k2, di) => {
+var fi = W((M2, pi) => {
     "use strict";
-    var Am = "[a-zA-Z_:][a-zA-Z0-9:._-]*",
-        qm = "[^\"'=<>`\\x00-\\x20]+",
-        Mm = "'[^']*'",
-        Em = '"[^"]*"',
-        Dm = "(?:" + qm + "|" + Mm + "|" + Em + ")",
-        zm = "(?:\\s+" + Am + "(?:\\s*=\\s*" + Dm + ")?)",
-        Ul = "<[A-Za-z][A-Za-z0-9\\-]*" + zm + "*\\s*\\/?>",
-        Wl = "<\\/[A-Za-z][A-Za-z0-9\\-]*\\s*>",
-        Rm = "<!---->|<!--(?:-?[^>-])(?:-?[^-])*-->",
-        Fm = "<[?][\\s\\S]*?[?]>",
-        Bm = "<![A-Z]+\\s+[^>]*>",
-        Nm = "<!\\[CDATA\\[[\\s\\S]*?\\]\\]>",
-        Lm = new RegExp("^(?:" + Ul + "|" + Wl + "|" + Rm + "|" + Fm + "|" + Bm + "|" + Nm + ")"),
-        Pm = new RegExp("^(?:" + Ul + "|" + Wl + ")");
-    di.exports.HTML_TAG_RE = Lm;
-    di.exports.HTML_OPEN_CLOSE_TAG_RE = Pm
+    var Mm = "[a-zA-Z_:][a-zA-Z0-9:._-]*",
+        Em = "[^\"'=<>`\\x00-\\x20]+",
+        Dm = "'[^']*'",
+        zm = '"[^"]*"',
+        Rm = "(?:" + Em + "|" + Dm + "|" + zm + ")",
+        Fm = "(?:\\s+" + Mm + "(?:\\s*=\\s*" + Rm + ")?)",
+        Yl = "<[A-Za-z][A-Za-z0-9\\-]*" + Fm + "*\\s*\\/?>",
+        Zl = "<\\/[A-Za-z][A-Za-z0-9\\-]*\\s*>",
+        Bm = "<!---->|<!--(?:-?[^>-])(?:-?[^-])*-->",
+        Nm = "<[?][\\s\\S]*?[?]>",
+        Lm = "<![A-Z]+\\s+[^>]*>",
+        Pm = "<!\\[CDATA\\[[\\s\\S]*?\\]\\]>",
+        Im = new RegExp("^(?:" + Yl + "|" + Zl + "|" + Bm + "|" + Nm + "|" + Lm + "|" + Pm + ")"),
+        Om = new RegExp("^(?:" + Yl + "|" + Zl + ")");
+    pi.exports.HTML_TAG_RE = Im;
+    pi.exports.HTML_OPEN_CLOSE_TAG_RE = Om
 });
-var Zl = W((_2, Yl) => {
+var Xl = W((E2, Ql) => {
     "use strict";
-    var Im = jl(),
-        Om = mi().HTML_OPEN_CLOSE_TAG_RE,
+    var Hm = Wl(),
+        $m = fi().HTML_OPEN_CLOSE_TAG_RE,
         br = [
             [/^<(script|pre|style|textarea)(?=(\s|>|$))/i, /<\/(script|pre|style|textarea)>/i, !0],
             [/^<!--/, /-->/, !0],
             [/^<\?/, /\?>/, !0],
             [/^<![A-Z]/, />/, !0],
             [/^<!\[CDATA\[/, /\]\]>/, !0],
-            [new RegExp("^</?(" + Im.join("|") + ")(?=(\\s|/?>|$))", "i"), /^$/, !0],
-            [new RegExp(Om.source + "\\s*$"), /^$/, !1]
+            [new RegExp("^</?(" + Hm.join("|") + ")(?=(\\s|/?>|$))", "i"), /^$/, !0],
+            [new RegExp($m.source + "\\s*$"), /^$/, !1]
         ];
-    Yl.exports = function(e, i, a, l) {
+    Ql.exports = function(e, i, a, l) {
         var c, d, f, g, y = e.bMarks[i] + e.tShift[i],
             _ = e.eMarks[i];
         if (e.sCount[i] - e.blkIndent >= 4 || !e.md.options.html || e.src.charCodeAt(y) !== 60) return !1;
         for (g = e.src.slice(y, _), c = 0; c < br.length && !br[c][0].test(g); c++);
         if (c === br.length) return !1;
         if (l) return br[c][2];
         if (d = i + 1, !br[c][1].test(g)) {
@@ -4535,28 +4535,28 @@
                     g.length !== 0 && d++;
                     break
                 }
         }
         return e.line = d, f = e.push("html_block", "", 0), f.map = [i, d], f.content = e.getLines(i, d, e.blkIndent, !0), !0
     }
 });
-var Jl = W((S2, Xl) => {
+var ec = W((D2, Kl) => {
     "use strict";
-    var Ql = Se().isSpace;
-    Xl.exports = function(e, i, a, l) {
+    var Jl = Se().isSpace;
+    Kl.exports = function(e, i, a, l) {
         var c, d, f, g, y = e.bMarks[i] + e.tShift[i],
             _ = e.eMarks[i];
         if (e.sCount[i] - e.blkIndent >= 4 || (c = e.src.charCodeAt(y), c !== 35 || y >= _)) return !1;
         for (d = 1, c = e.src.charCodeAt(++y); c === 35 && y < _ && d <= 6;) d++, c = e.src.charCodeAt(++y);
-        return d > 6 || y < _ && !Ql(c) ? !1 : (l || (_ = e.skipSpacesBack(_, y), f = e.skipCharsBack(_, 35, y), f > y && Ql(e.src.charCodeAt(f - 1)) && (_ = f), e.line = i + 1, g = e.push("heading_open", "h" + String(d), 1), g.markup = "########".slice(0, d), g.map = [i, e.line], g = e.push("inline", "", 0), g.content = e.src.slice(y, _).trim(), g.map = [i, e.line], g.children = [], g = e.push("heading_close", "h" + String(d), -1), g.markup = "########".slice(0, d)), !0)
+        return d > 6 || y < _ && !Jl(c) ? !1 : (l || (_ = e.skipSpacesBack(_, y), f = e.skipCharsBack(_, 35, y), f > y && Jl(e.src.charCodeAt(f - 1)) && (_ = f), e.line = i + 1, g = e.push("heading_open", "h" + String(d), 1), g.markup = "########".slice(0, d), g.map = [i, e.line], g = e.push("inline", "", 0), g.content = e.src.slice(y, _).trim(), g.map = [i, e.line], g.children = [], g = e.push("heading_close", "h" + String(d), -1), g.markup = "########".slice(0, d)), !0)
     }
 });
-var ec = W((C2, Kl) => {
+var rc = W((z2, tc) => {
     "use strict";
-    Kl.exports = function(e, i, a) {
+    tc.exports = function(e, i, a) {
         var l, c, d, f, g, y, _, w, T, A = i + 1,
             L, R = e.md.block.ruler.getRules("paragraph");
         if (e.sCount[i] - e.blkIndent >= 4) return !1;
         for (L = e.parentType, e.parentType = "paragraph"; A < a && !e.isEmpty(A); A++)
             if (!(e.sCount[A] - e.blkIndent > 3)) {
                 if (e.sCount[A] >= e.blkIndent && (y = e.bMarks[A] + e.tShift[A], _ = e.eMarks[A], y < _ && (T = e.src.charCodeAt(y), (T === 45 || T === 61) && (y = e.skipChars(y, T), y = e.skipSpaces(y), y >= _)))) {
                     w = T === 61 ? 1 : 2;
@@ -4568,65 +4568,65 @@
                             c = !0;
                             break
                         } if (c) break
                 }
             } return w ? (l = e.getLines(i, A, e.blkIndent, !1).trim(), e.line = A + 1, g = e.push("heading_open", "h" + String(w), 1), g.markup = String.fromCharCode(T), g.map = [i, e.line], g = e.push("inline", "", 0), g.content = l, g.map = [i, e.line - 1], g.children = [], g = e.push("heading_close", "h" + String(w), -1), g.markup = String.fromCharCode(T), e.parentType = L, !0) : !1
     }
 });
-var rc = W((T2, tc) => {
+var ic = W((R2, nc) => {
     "use strict";
-    tc.exports = function(e, i, a) {
+    nc.exports = function(e, i, a) {
         var l, c, d, f, g, y, _ = i + 1,
             w = e.md.block.ruler.getRules("paragraph");
         for (y = e.parentType, e.parentType = "paragraph"; _ < a && !e.isEmpty(_); _++)
             if (!(e.sCount[_] - e.blkIndent > 3) && !(e.sCount[_] < 0)) {
                 for (c = !1, d = 0, f = w.length; d < f; d++)
                     if (w[d](e, _, a, !0)) {
                         c = !0;
                         break
                     } if (c) break
             } return l = e.getLines(i, _, e.blkIndent, !1).trim(), e.line = _, g = e.push("paragraph_open", "p", 1), g.map = [i, e.line], g = e.push("inline", "", 0), g.content = l, g.map = [i, e.line], g.children = [], g = e.push("paragraph_close", "p", -1), e.parentType = y, !0
     }
 });
-var oc = W((A2, ic) => {
+var sc = W((F2, ac) => {
     "use strict";
-    var nc = R0(),
-        B0 = Se().isSpace;
+    var oc = F0(),
+        N0 = Se().isSpace;
 
     function Tt(r, e, i, a) {
         var l, c, d, f, g, y, _, w;
         for (this.src = r, this.md = e, this.env = i, this.tokens = a, this.bMarks = [], this.eMarks = [], this.tShift = [], this.sCount = [], this.bsCount = [], this.blkIndent = 0, this.line = 0, this.lineMax = 0, this.tight = !1, this.ddIndent = -1, this.listIndent = -1, this.parentType = "root", this.level = 0, this.result = "", c = this.src, w = !1, d = f = y = _ = 0, g = c.length; f < g; f++) {
             if (l = c.charCodeAt(f), !w)
-                if (B0(l)) {
+                if (N0(l)) {
                     y++, l === 9 ? _ += 4 - _ % 4 : _++;
                     continue
                 } else w = !0;
             (l === 10 || f === g - 1) && (l !== 10 && f++, this.bMarks.push(d), this.eMarks.push(f), this.tShift.push(y), this.sCount.push(_), this.bsCount.push(0), w = !1, y = 0, _ = 0, d = f + 1)
         }
         this.bMarks.push(c.length), this.eMarks.push(c.length), this.tShift.push(0), this.sCount.push(0), this.bsCount.push(0), this.lineMax = this.bMarks.length - 1
     }
     Tt.prototype.push = function(r, e, i) {
-        var a = new nc(r, e, i);
+        var a = new oc(r, e, i);
         return a.block = !0, i < 0 && this.level--, a.level = this.level, i > 0 && this.level++, this.tokens.push(a), a
     };
     Tt.prototype.isEmpty = function(e) {
         return this.bMarks[e] + this.tShift[e] >= this.eMarks[e]
     };
     Tt.prototype.skipEmptyLines = function(e) {
         for (var i = this.lineMax; e < i && !(this.bMarks[e] + this.tShift[e] < this.eMarks[e]); e++);
         return e
     };
     Tt.prototype.skipSpaces = function(e) {
-        for (var i, a = this.src.length; e < a && (i = this.src.charCodeAt(e), !!B0(i)); e++);
+        for (var i, a = this.src.length; e < a && (i = this.src.charCodeAt(e), !!N0(i)); e++);
         return e
     };
     Tt.prototype.skipSpacesBack = function(e, i) {
         if (e <= i) return e;
         for (; e > i;)
-            if (!B0(this.src.charCodeAt(--e))) return e + 1;
+            if (!N0(this.src.charCodeAt(--e))) return e + 1;
         return e
     };
     Tt.prototype.skipChars = function(e, i) {
         for (var a = this.src.length; e < a && this.src.charCodeAt(e) === i; e++);
         return e
     };
     Tt.prototype.skipCharsBack = function(e, i, a) {
@@ -4636,74 +4636,74 @@
         return e
     };
     Tt.prototype.getLines = function(e, i, a, l) {
         var c, d, f, g, y, _, w, T = e;
         if (e >= i) return "";
         for (_ = new Array(i - e), c = 0; T < i; T++, c++) {
             for (d = 0, w = g = this.bMarks[T], T + 1 < i || l ? y = this.eMarks[T] + 1 : y = this.eMarks[T]; g < y && d < a;) {
-                if (f = this.src.charCodeAt(g), B0(f)) f === 9 ? d += 4 - (d + this.bsCount[T]) % 4 : d++;
+                if (f = this.src.charCodeAt(g), N0(f)) f === 9 ? d += 4 - (d + this.bsCount[T]) % 4 : d++;
                 else if (g - w < this.tShift[T]) d++;
                 else break;
                 g++
             }
             d > a ? _[c] = new Array(d - a + 1).join(" ") + this.src.slice(g, y) : _[c] = this.src.slice(g, y)
         }
         return _.join("")
     };
-    Tt.prototype.Token = nc;
-    ic.exports = Tt
+    Tt.prototype.Token = oc;
+    ac.exports = Tt
 });
-var sc = W((q2, ac) => {
+var cc = W((B2, lc) => {
     "use strict";
-    var Hm = D0(),
-        N0 = [
-            ["table", ql(), ["paragraph", "reference"]],
-            ["code", El()],
-            ["fence", zl(), ["paragraph", "reference", "blockquote", "list"]],
-            ["blockquote", Fl(), ["paragraph", "reference", "blockquote", "list"]],
-            ["hr", Nl(), ["paragraph", "reference", "blockquote", "list"]],
-            ["list", Hl(), ["paragraph", "reference", "blockquote"]],
-            ["reference", Gl()],
-            ["html_block", Zl(), ["paragraph", "reference", "blockquote"]],
-            ["heading", Jl(), ["paragraph", "reference", "blockquote"]],
-            ["lheading", ec()],
-            ["paragraph", rc()]
+    var Gm = z0(),
+        L0 = [
+            ["table", El(), ["paragraph", "reference"]],
+            ["code", zl()],
+            ["fence", Fl(), ["paragraph", "reference", "blockquote", "list"]],
+            ["blockquote", Nl(), ["paragraph", "reference", "blockquote", "list"]],
+            ["hr", Pl(), ["paragraph", "reference", "blockquote", "list"]],
+            ["list", Gl(), ["paragraph", "reference", "blockquote"]],
+            ["reference", jl()],
+            ["html_block", Xl(), ["paragraph", "reference", "blockquote"]],
+            ["heading", ec(), ["paragraph", "reference", "blockquote"]],
+            ["lheading", rc()],
+            ["paragraph", ic()]
         ];
 
-    function L0() {
-        this.ruler = new Hm;
-        for (var r = 0; r < N0.length; r++) this.ruler.push(N0[r][0], N0[r][1], {
-            alt: (N0[r][2] || []).slice()
+    function P0() {
+        this.ruler = new Gm;
+        for (var r = 0; r < L0.length; r++) this.ruler.push(L0[r][0], L0[r][1], {
+            alt: (L0[r][2] || []).slice()
         })
     }
-    L0.prototype.tokenize = function(r, e, i) {
+    P0.prototype.tokenize = function(r, e, i) {
         for (var a, l, c, d = this.ruler.getRules(""), f = d.length, g = e, y = !1, _ = r.md.options.maxNesting; g < i && (r.line = g = r.skipEmptyLines(g), !(g >= i || r.sCount[g] < r.blkIndent));) {
             if (r.level >= _) {
                 r.line = i;
                 break
             }
             for (c = r.line, l = 0; l < f; l++)
                 if (a = d[l](r, g, i, !1), a) {
                     if (c >= r.line) throw new Error("block rule didn't increment state.line");
                     break
                 } if (!a) throw new Error("none of the block rules matched");
             r.tight = !y, r.isEmpty(r.line - 1) && (y = !0), g = r.line, g < i && r.isEmpty(g) && (y = !0, g++, r.line = g)
         }
     };
-    L0.prototype.parse = function(r, e, i, a) {
+    P0.prototype.parse = function(r, e, i, a) {
         var l;
         r && (l = new this.State(r, e, i, a), this.tokenize(l, l.line, l.lineMax))
     };
-    L0.prototype.State = oc();
-    ac.exports = L0
+    P0.prototype.State = sc();
+    lc.exports = P0
 });
-var cc = W((M2, lc) => {
+var hc = W((N2, uc) => {
     "use strict";
 
-    function $m(r) {
+    function Vm(r) {
         switch (r) {
             case 10:
             case 33:
             case 35:
             case 36:
             case 37:
             case 38:
@@ -4725,263 +4725,263 @@
             case 125:
             case 126:
                 return !0;
             default:
                 return !1
         }
     }
-    lc.exports = function(e, i) {
-        for (var a = e.pos; a < e.posMax && !$m(e.src.charCodeAt(a));) a++;
+    uc.exports = function(e, i) {
+        for (var a = e.pos; a < e.posMax && !Vm(e.src.charCodeAt(a));) a++;
         return a === e.pos ? !1 : (i || (e.pending += e.src.slice(e.pos, a)), e.pos = a, !0)
     }
 });
-var hc = W((E2, uc) => {
+var mc = W((L2, dc) => {
     "use strict";
-    var Gm = /(?:^|[^a-z0-9.+-])([a-z][a-z0-9.+-]*)$/i;
-    uc.exports = function(e, i) {
+    var jm = /(?:^|[^a-z0-9.+-])([a-z][a-z0-9.+-]*)$/i;
+    dc.exports = function(e, i) {
         var a, l, c, d, f, g, y, _;
-        return !e.md.options.linkify || e.linkLevel > 0 || (a = e.pos, l = e.posMax, a + 3 > l) || e.src.charCodeAt(a) !== 58 || e.src.charCodeAt(a + 1) !== 47 || e.src.charCodeAt(a + 2) !== 47 || (c = e.pending.match(Gm), !c) || (d = c[1], f = e.md.linkify.matchAtStart(e.src.slice(a - d.length)), !f) || (g = f.url, g.length <= d.length) || (g = g.replace(/\*+$/, ""), y = e.md.normalizeLink(g), !e.md.validateLink(y)) ? !1 : (i || (e.pending = e.pending.slice(0, -d.length), _ = e.push("link_open", "a", 1), _.attrs = [
+        return !e.md.options.linkify || e.linkLevel > 0 || (a = e.pos, l = e.posMax, a + 3 > l) || e.src.charCodeAt(a) !== 58 || e.src.charCodeAt(a + 1) !== 47 || e.src.charCodeAt(a + 2) !== 47 || (c = e.pending.match(jm), !c) || (d = c[1], f = e.md.linkify.matchAtStart(e.src.slice(a - d.length)), !f) || (g = f.url, g.length <= d.length) || (g = g.replace(/\*+$/, ""), y = e.md.normalizeLink(g), !e.md.validateLink(y)) ? !1 : (i || (e.pending = e.pending.slice(0, -d.length), _ = e.push("link_open", "a", 1), _.attrs = [
             ["href", y]
         ], _.markup = "linkify", _.info = "auto", _ = e.push("text", "", 0), _.content = e.md.normalizeLinkText(g), _ = e.push("link_close", "a", -1), _.markup = "linkify", _.info = "auto"), e.pos += g.length - d.length, !0)
     }
 });
-var mc = W((D2, dc) => {
+var fc = W((P2, pc) => {
     "use strict";
-    var Vm = Se().isSpace;
-    dc.exports = function(e, i) {
+    var Um = Se().isSpace;
+    pc.exports = function(e, i) {
         var a, l, c, d = e.pos;
         if (e.src.charCodeAt(d) !== 10) return !1;
         if (a = e.pending.length - 1, l = e.posMax, !i)
             if (a >= 0 && e.pending.charCodeAt(a) === 32)
                 if (a >= 1 && e.pending.charCodeAt(a - 1) === 32) {
                     for (c = a - 1; c >= 1 && e.pending.charCodeAt(c - 1) === 32;) c--;
                     e.pending = e.pending.slice(0, c), e.push("hardbreak", "br", 0)
                 } else e.pending = e.pending.slice(0, -1), e.push("softbreak", "br", 0);
         else e.push("softbreak", "br", 0);
-        for (d++; d < l && Vm(e.src.charCodeAt(d));) d++;
+        for (d++; d < l && Um(e.src.charCodeAt(d));) d++;
         return e.pos = d, !0
     }
 });
-var fc = W((z2, pc) => {
+var bc = W((I2, gc) => {
     "use strict";
-    var jm = Se().isSpace,
-        fi = [];
-    for (pi = 0; pi < 256; pi++) fi.push(0);
-    var pi;
+    var Wm = Se().isSpace,
+        bi = [];
+    for (gi = 0; gi < 256; gi++) bi.push(0);
+    var gi;
     "\\!\"#$%&'()*+,./:;<=>?@[]^_`{|}~-".split("").forEach(function(r) {
-        fi[r.charCodeAt(0)] = 1
+        bi[r.charCodeAt(0)] = 1
     });
-    pc.exports = function(e, i) {
+    gc.exports = function(e, i) {
         var a, l, c, d, f, g = e.pos,
             y = e.posMax;
         if (e.src.charCodeAt(g) !== 92 || (g++, g >= y)) return !1;
         if (a = e.src.charCodeAt(g), a === 10) {
-            for (i || e.push("hardbreak", "br", 0), g++; g < y && (a = e.src.charCodeAt(g), !!jm(a));) g++;
+            for (i || e.push("hardbreak", "br", 0), g++; g < y && (a = e.src.charCodeAt(g), !!Wm(a));) g++;
             return e.pos = g, !0
         }
-        return d = e.src[g], a >= 55296 && a <= 56319 && g + 1 < y && (l = e.src.charCodeAt(g + 1), l >= 56320 && l <= 57343 && (d += e.src[g + 1], g++)), c = "\\" + d, i || (f = e.push("text_special", "", 0), a < 256 && fi[a] !== 0 ? f.content = d : f.content = c, f.markup = c, f.info = "escape"), e.pos = g + 1, !0
+        return d = e.src[g], a >= 55296 && a <= 56319 && g + 1 < y && (l = e.src.charCodeAt(g + 1), l >= 56320 && l <= 57343 && (d += e.src[g + 1], g++)), c = "\\" + d, i || (f = e.push("text_special", "", 0), a < 256 && bi[a] !== 0 ? f.content = d : f.content = c, f.markup = c, f.info = "escape"), e.pos = g + 1, !0
     }
 });
-var bc = W((R2, gc) => {
+var xc = W((O2, yc) => {
     "use strict";
-    gc.exports = function(e, i) {
+    yc.exports = function(e, i) {
         var a, l, c, d, f, g, y, _, w = e.pos,
             T = e.src.charCodeAt(w);
         if (T !== 96) return !1;
         for (a = w, w++, l = e.posMax; w < l && e.src.charCodeAt(w) === 96;) w++;
         if (c = e.src.slice(a, w), y = c.length, e.backticksScanned && (e.backticks[y] || 0) <= a) return i || (e.pending += c), e.pos += y, !0;
         for (g = w;
             (f = e.src.indexOf("`", g)) !== -1;) {
             for (g = f + 1; g < l && e.src.charCodeAt(g) === 96;) g++;
             if (_ = g - f, _ === y) return i || (d = e.push("code_inline", "code", 0), d.markup = c, d.content = e.src.slice(w, f).replace(/\n/g, " ").replace(/^ (.+) $/, "$1")), e.pos = g, !0;
             e.backticks[_] = f
         }
         return e.backticksScanned = !0, i || (e.pending += c), e.pos += y, !0
     }
 });
-var bi = W((F2, gi) => {
+var xi = W((H2, yi) => {
     "use strict";
-    gi.exports.tokenize = function(e, i) {
+    yi.exports.tokenize = function(e, i) {
         var a, l, c, d, f, g = e.pos,
             y = e.src.charCodeAt(g);
         if (i || y !== 126 || (l = e.scanDelims(e.pos, !0), d = l.length, f = String.fromCharCode(y), d < 2)) return !1;
         for (d % 2 && (c = e.push("text", "", 0), c.content = f, d--), a = 0; a < d; a += 2) c = e.push("text", "", 0), c.content = f + f, e.delimiters.push({
             marker: y,
             length: 0,
             token: e.tokens.length - 1,
             end: -1,
             open: l.can_open,
             close: l.can_close
         });
         return e.pos += l.length, !0
     };
 
-    function yc(r, e) {
+    function vc(r, e) {
         var i, a, l, c, d, f = [],
             g = e.length;
         for (i = 0; i < g; i++) l = e[i], l.marker === 126 && l.end !== -1 && (c = e[l.end], d = r.tokens[l.token], d.type = "s_open", d.tag = "s", d.nesting = 1, d.markup = "~~", d.content = "", d = r.tokens[c.token], d.type = "s_close", d.tag = "s", d.nesting = -1, d.markup = "~~", d.content = "", r.tokens[c.token - 1].type === "text" && r.tokens[c.token - 1].content === "~" && f.push(c.token - 1));
         for (; f.length;) {
             for (i = f.pop(), a = i + 1; a < r.tokens.length && r.tokens[a].type === "s_close";) a++;
             a--, i !== a && (d = r.tokens[a], r.tokens[a] = r.tokens[i], r.tokens[i] = d)
         }
     }
-    gi.exports.postProcess = function(e) {
+    yi.exports.postProcess = function(e) {
         var i, a = e.tokens_meta,
             l = e.tokens_meta.length;
-        for (yc(e, e.delimiters), i = 0; i < l; i++) a[i] && a[i].delimiters && yc(e, a[i].delimiters)
+        for (vc(e, e.delimiters), i = 0; i < l; i++) a[i] && a[i].delimiters && vc(e, a[i].delimiters)
     }
 });
-var xi = W((B2, yi) => {
+var wi = W(($2, vi) => {
     "use strict";
-    yi.exports.tokenize = function(e, i) {
+    vi.exports.tokenize = function(e, i) {
         var a, l, c, d = e.pos,
             f = e.src.charCodeAt(d);
         if (i || f !== 95 && f !== 42) return !1;
         for (l = e.scanDelims(e.pos, f === 42), a = 0; a < l.length; a++) c = e.push("text", "", 0), c.content = String.fromCharCode(f), e.delimiters.push({
             marker: f,
             length: l.length,
             token: e.tokens.length - 1,
             end: -1,
             open: l.can_open,
             close: l.can_close
         });
         return e.pos += l.length, !0
     };
 
-    function xc(r, e) {
+    function wc(r, e) {
         var i, a, l, c, d, f, g = e.length;
         for (i = g - 1; i >= 0; i--) a = e[i], !(a.marker !== 95 && a.marker !== 42) && a.end !== -1 && (l = e[a.end], f = i > 0 && e[i - 1].end === a.end + 1 && e[i - 1].marker === a.marker && e[i - 1].token === a.token - 1 && e[a.end + 1].token === l.token + 1, d = String.fromCharCode(a.marker), c = r.tokens[a.token], c.type = f ? "strong_open" : "em_open", c.tag = f ? "strong" : "em", c.nesting = 1, c.markup = f ? d + d : d, c.content = "", c = r.tokens[l.token], c.type = f ? "strong_close" : "em_close", c.tag = f ? "strong" : "em", c.nesting = -1, c.markup = f ? d + d : d, c.content = "", f && (r.tokens[e[i - 1].token].content = "", r.tokens[e[a.end + 1].token].content = "", i--))
     }
-    yi.exports.postProcess = function(e) {
+    vi.exports.postProcess = function(e) {
         var i, a = e.tokens_meta,
             l = e.tokens_meta.length;
-        for (xc(e, e.delimiters), i = 0; i < l; i++) a[i] && a[i].delimiters && xc(e, a[i].delimiters)
+        for (wc(e, e.delimiters), i = 0; i < l; i++) a[i] && a[i].delimiters && wc(e, a[i].delimiters)
     }
 });
-var wc = W((N2, vc) => {
+var _c = W((G2, kc) => {
     "use strict";
-    var Um = Se().normalizeReference,
-        vi = Se().isSpace;
-    vc.exports = function(e, i) {
+    var Ym = Se().normalizeReference,
+        ki = Se().isSpace;
+    kc.exports = function(e, i) {
         var a, l, c, d, f, g, y, _, w, T = "",
             A = "",
             L = e.pos,
             R = e.posMax,
             O = e.pos,
             P = !0;
         if (e.src.charCodeAt(e.pos) !== 91 || (f = e.pos + 1, d = e.md.helpers.parseLinkLabel(e, e.pos, !0), d < 0)) return !1;
         if (g = d + 1, g < R && e.src.charCodeAt(g) === 40) {
-            for (P = !1, g++; g < R && (l = e.src.charCodeAt(g), !(!vi(l) && l !== 10)); g++);
+            for (P = !1, g++; g < R && (l = e.src.charCodeAt(g), !(!ki(l) && l !== 10)); g++);
             if (g >= R) return !1;
             if (O = g, y = e.md.helpers.parseLinkDestination(e.src, g, e.posMax), y.ok) {
-                for (T = e.md.normalizeLink(y.str), e.md.validateLink(T) ? g = y.pos : T = "", O = g; g < R && (l = e.src.charCodeAt(g), !(!vi(l) && l !== 10)); g++);
+                for (T = e.md.normalizeLink(y.str), e.md.validateLink(T) ? g = y.pos : T = "", O = g; g < R && (l = e.src.charCodeAt(g), !(!ki(l) && l !== 10)); g++);
                 if (y = e.md.helpers.parseLinkTitle(e.src, g, e.posMax), g < R && O !== g && y.ok)
-                    for (A = y.str, g = y.pos; g < R && (l = e.src.charCodeAt(g), !(!vi(l) && l !== 10)); g++);
+                    for (A = y.str, g = y.pos; g < R && (l = e.src.charCodeAt(g), !(!ki(l) && l !== 10)); g++);
             }(g >= R || e.src.charCodeAt(g) !== 41) && (P = !0), g++
         }
         if (P) {
             if (typeof e.env.references > "u") return !1;
-            if (g < R && e.src.charCodeAt(g) === 91 ? (O = g + 1, g = e.md.helpers.parseLinkLabel(e, g), g >= 0 ? c = e.src.slice(O, g++) : g = d + 1) : g = d + 1, c || (c = e.src.slice(f, d)), _ = e.env.references[Um(c)], !_) return e.pos = L, !1;
+            if (g < R && e.src.charCodeAt(g) === 91 ? (O = g + 1, g = e.md.helpers.parseLinkLabel(e, g), g >= 0 ? c = e.src.slice(O, g++) : g = d + 1) : g = d + 1, c || (c = e.src.slice(f, d)), _ = e.env.references[Ym(c)], !_) return e.pos = L, !1;
             T = _.href, A = _.title
         }
         return i || (e.pos = f, e.posMax = d, w = e.push("link_open", "a", 1), w.attrs = a = [
             ["href", T]
         ], A && a.push(["title", A]), e.linkLevel++, e.md.inline.tokenize(e), e.linkLevel--, w = e.push("link_close", "a", -1)), e.pos = g, e.posMax = R, !0
     }
 });
-var _c = W((L2, kc) => {
+var Cc = W((V2, Sc) => {
     "use strict";
-    var Wm = Se().normalizeReference,
-        wi = Se().isSpace;
-    kc.exports = function(e, i) {
+    var Zm = Se().normalizeReference,
+        _i = Se().isSpace;
+    Sc.exports = function(e, i) {
         var a, l, c, d, f, g, y, _, w, T, A, L, R, O = "",
             P = e.pos,
             I = e.posMax;
         if (e.src.charCodeAt(e.pos) !== 33 || e.src.charCodeAt(e.pos + 1) !== 91 || (g = e.pos + 2, f = e.md.helpers.parseLinkLabel(e, e.pos + 1, !1), f < 0)) return !1;
         if (y = f + 1, y < I && e.src.charCodeAt(y) === 40) {
-            for (y++; y < I && (l = e.src.charCodeAt(y), !(!wi(l) && l !== 10)); y++);
+            for (y++; y < I && (l = e.src.charCodeAt(y), !(!_i(l) && l !== 10)); y++);
             if (y >= I) return !1;
-            for (R = y, w = e.md.helpers.parseLinkDestination(e.src, y, e.posMax), w.ok && (O = e.md.normalizeLink(w.str), e.md.validateLink(O) ? y = w.pos : O = ""), R = y; y < I && (l = e.src.charCodeAt(y), !(!wi(l) && l !== 10)); y++);
+            for (R = y, w = e.md.helpers.parseLinkDestination(e.src, y, e.posMax), w.ok && (O = e.md.normalizeLink(w.str), e.md.validateLink(O) ? y = w.pos : O = ""), R = y; y < I && (l = e.src.charCodeAt(y), !(!_i(l) && l !== 10)); y++);
             if (w = e.md.helpers.parseLinkTitle(e.src, y, e.posMax), y < I && R !== y && w.ok)
-                for (T = w.str, y = w.pos; y < I && (l = e.src.charCodeAt(y), !(!wi(l) && l !== 10)); y++);
+                for (T = w.str, y = w.pos; y < I && (l = e.src.charCodeAt(y), !(!_i(l) && l !== 10)); y++);
             else T = "";
             if (y >= I || e.src.charCodeAt(y) !== 41) return e.pos = P, !1;
             y++
         } else {
             if (typeof e.env.references > "u") return !1;
-            if (y < I && e.src.charCodeAt(y) === 91 ? (R = y + 1, y = e.md.helpers.parseLinkLabel(e, y), y >= 0 ? d = e.src.slice(R, y++) : y = f + 1) : y = f + 1, d || (d = e.src.slice(g, f)), _ = e.env.references[Wm(d)], !_) return e.pos = P, !1;
+            if (y < I && e.src.charCodeAt(y) === 91 ? (R = y + 1, y = e.md.helpers.parseLinkLabel(e, y), y >= 0 ? d = e.src.slice(R, y++) : y = f + 1) : y = f + 1, d || (d = e.src.slice(g, f)), _ = e.env.references[Zm(d)], !_) return e.pos = P, !1;
             O = _.href, T = _.title
         }
         return i || (c = e.src.slice(g, f), e.md.inline.parse(c, e.md, e.env, L = []), A = e.push("image", "img", 0), A.attrs = a = [
             ["src", O],
             ["alt", ""]
         ], A.children = L, A.content = c, T && a.push(["title", T])), e.pos = y, e.posMax = I, !0
     }
 });
-var Cc = W((P2, Sc) => {
+var Ac = W((j2, Tc) => {
     "use strict";
-    var Ym = /^([a-zA-Z0-9.!#$%&'*+\/=?^_`{|}~-]+@[a-zA-Z0-9](?:[a-zA-Z0-9-]{0,61}[a-zA-Z0-9])?(?:\.[a-zA-Z0-9](?:[a-zA-Z0-9-]{0,61}[a-zA-Z0-9])?)*)$/,
-        Zm = /^([a-zA-Z][a-zA-Z0-9+.\-]{1,31}):([^<>\x00-\x20]*)$/;
-    Sc.exports = function(e, i) {
+    var Qm = /^([a-zA-Z0-9.!#$%&'*+\/=?^_`{|}~-]+@[a-zA-Z0-9](?:[a-zA-Z0-9-]{0,61}[a-zA-Z0-9])?(?:\.[a-zA-Z0-9](?:[a-zA-Z0-9-]{0,61}[a-zA-Z0-9])?)*)$/,
+        Xm = /^([a-zA-Z][a-zA-Z0-9+.\-]{1,31}):([^<>\x00-\x20]*)$/;
+    Tc.exports = function(e, i) {
         var a, l, c, d, f, g, y = e.pos;
         if (e.src.charCodeAt(y) !== 60) return !1;
         for (f = e.pos, g = e.posMax;;) {
             if (++y >= g || (d = e.src.charCodeAt(y), d === 60)) return !1;
             if (d === 62) break
         }
-        return a = e.src.slice(f + 1, y), Zm.test(a) ? (l = e.md.normalizeLink(a), e.md.validateLink(l) ? (i || (c = e.push("link_open", "a", 1), c.attrs = [
+        return a = e.src.slice(f + 1, y), Xm.test(a) ? (l = e.md.normalizeLink(a), e.md.validateLink(l) ? (i || (c = e.push("link_open", "a", 1), c.attrs = [
             ["href", l]
-        ], c.markup = "autolink", c.info = "auto", c = e.push("text", "", 0), c.content = e.md.normalizeLinkText(a), c = e.push("link_close", "a", -1), c.markup = "autolink", c.info = "auto"), e.pos += a.length + 2, !0) : !1) : Ym.test(a) ? (l = e.md.normalizeLink("mailto:" + a), e.md.validateLink(l) ? (i || (c = e.push("link_open", "a", 1), c.attrs = [
+        ], c.markup = "autolink", c.info = "auto", c = e.push("text", "", 0), c.content = e.md.normalizeLinkText(a), c = e.push("link_close", "a", -1), c.markup = "autolink", c.info = "auto"), e.pos += a.length + 2, !0) : !1) : Qm.test(a) ? (l = e.md.normalizeLink("mailto:" + a), e.md.validateLink(l) ? (i || (c = e.push("link_open", "a", 1), c.attrs = [
             ["href", l]
         ], c.markup = "autolink", c.info = "auto", c = e.push("text", "", 0), c.content = e.md.normalizeLinkText(a), c = e.push("link_close", "a", -1), c.markup = "autolink", c.info = "auto"), e.pos += a.length + 2, !0) : !1) : !1
     }
 });
-var Ac = W((I2, Tc) => {
+var Mc = W((U2, qc) => {
     "use strict";
-    var Qm = mi().HTML_TAG_RE;
+    var Jm = fi().HTML_TAG_RE;
 
-    function Xm(r) {
+    function Km(r) {
         return /^<a[>\s]/i.test(r)
     }
 
-    function Jm(r) {
+    function ep(r) {
         return /^<\/a\s*>/i.test(r)
     }
 
-    function Km(r) {
+    function tp(r) {
         var e = r | 32;
         return e >= 97 && e <= 122
     }
-    Tc.exports = function(e, i) {
+    qc.exports = function(e, i) {
         var a, l, c, d, f = e.pos;
-        return !e.md.options.html || (c = e.posMax, e.src.charCodeAt(f) !== 60 || f + 2 >= c) || (a = e.src.charCodeAt(f + 1), a !== 33 && a !== 63 && a !== 47 && !Km(a)) || (l = e.src.slice(f).match(Qm), !l) ? !1 : (i || (d = e.push("html_inline", "", 0), d.content = l[0], Xm(d.content) && e.linkLevel++, Jm(d.content) && e.linkLevel--), e.pos += l[0].length, !0)
+        return !e.md.options.html || (c = e.posMax, e.src.charCodeAt(f) !== 60 || f + 2 >= c) || (a = e.src.charCodeAt(f + 1), a !== 33 && a !== 63 && a !== 47 && !tp(a)) || (l = e.src.slice(f).match(Jm), !l) ? !1 : (i || (d = e.push("html_inline", "", 0), d.content = l[0], Km(d.content) && e.linkLevel++, ep(d.content) && e.linkLevel--), e.pos += l[0].length, !0)
     }
 });
-var Dc = W((O2, Ec) => {
+var Rc = W((W2, zc) => {
     "use strict";
-    var qc = ni(),
-        ep = Se().has,
-        tp = Se().isValidEntityCode,
-        Mc = Se().fromCodePoint,
-        rp = /^&#((?:x[a-f0-9]{1,6}|[0-9]{1,7}));/i,
-        np = /^&([a-z][a-z0-9]{1,31});/i;
-    Ec.exports = function(e, i) {
+    var Ec = oi(),
+        rp = Se().has,
+        np = Se().isValidEntityCode,
+        Dc = Se().fromCodePoint,
+        ip = /^&#((?:x[a-f0-9]{1,6}|[0-9]{1,7}));/i,
+        op = /^&([a-z][a-z0-9]{1,31});/i;
+    zc.exports = function(e, i) {
         var a, l, c, d, f = e.pos,
             g = e.posMax;
         if (e.src.charCodeAt(f) !== 38 || f + 1 >= g) return !1;
         if (a = e.src.charCodeAt(f + 1), a === 35) {
-            if (c = e.src.slice(f).match(rp), c) return i || (l = c[1][0].toLowerCase() === "x" ? parseInt(c[1].slice(1), 16) : parseInt(c[1], 10), d = e.push("text_special", "", 0), d.content = tp(l) ? Mc(l) : Mc(65533), d.markup = c[0], d.info = "entity"), e.pos += c[0].length, !0
-        } else if (c = e.src.slice(f).match(np), c && ep(qc, c[1])) return i || (d = e.push("text_special", "", 0), d.content = qc[c[1]], d.markup = c[0], d.info = "entity"), e.pos += c[0].length, !0;
+            if (c = e.src.slice(f).match(ip), c) return i || (l = c[1][0].toLowerCase() === "x" ? parseInt(c[1].slice(1), 16) : parseInt(c[1], 10), d = e.push("text_special", "", 0), d.content = np(l) ? Dc(l) : Dc(65533), d.markup = c[0], d.info = "entity"), e.pos += c[0].length, !0
+        } else if (c = e.src.slice(f).match(op), c && rp(Ec, c[1])) return i || (d = e.push("text_special", "", 0), d.content = Ec[c[1]], d.markup = c[0], d.info = "entity"), e.pos += c[0].length, !0;
         return !1
     }
 });
-var Fc = W((H2, Rc) => {
+var Nc = W((Y2, Bc) => {
     "use strict";
 
-    function zc(r) {
+    function Fc(r) {
         var e, i, a, l, c, d, f, g, y = {},
             _ = r.length;
         if (_) {
             var w = 0,
                 T = -2,
                 A = [];
             for (e = 0; e < _; e++)
@@ -4990,96 +4990,96 @@
                         if (l = r[i], l.marker === a.marker && l.open && l.end < 0 && (f = !1, (l.close || a.open) && (l.length + a.length) % 3 === 0 && (l.length % 3 !== 0 || a.length % 3 !== 0) && (f = !0), !f)) {
                             g = i > 0 && !r[i - 1].open ? A[i - 1] + 1 : 0, A[e] = e - i + g, A[i] = g, a.open = !1, l.end = e, l.close = !1, d = -1, T = -2;
                             break
                         } d !== -1 && (y[a.marker][(a.open ? 3 : 0) + (a.length || 0) % 3] = d)
                 }
         }
     }
-    Rc.exports = function(e) {
+    Bc.exports = function(e) {
         var i, a = e.tokens_meta,
             l = e.tokens_meta.length;
-        for (zc(e.delimiters), i = 0; i < l; i++) a[i] && a[i].delimiters && zc(a[i].delimiters)
+        for (Fc(e.delimiters), i = 0; i < l; i++) a[i] && a[i].delimiters && Fc(a[i].delimiters)
     }
 });
-var Nc = W(($2, Bc) => {
+var Pc = W((Z2, Lc) => {
     "use strict";
-    Bc.exports = function(e) {
+    Lc.exports = function(e) {
         var i, a, l = 0,
             c = e.tokens,
             d = e.tokens.length;
         for (i = a = 0; i < d; i++) c[i].nesting < 0 && l--, c[i].level = l, c[i].nesting > 0 && l++, c[i].type === "text" && i + 1 < d && c[i + 1].type === "text" ? c[i + 1].content = c[i].content + c[i + 1].content : (i !== a && (c[a] = c[i]), a++);
         i !== a && (c.length = a)
     }
 });
-var Hc = W((G2, Oc) => {
+var Gc = W((Q2, $c) => {
     "use strict";
-    var ki = R0(),
-        Lc = Se().isWhiteSpace,
-        Pc = Se().isPunctChar,
-        Ic = Se().isMdAsciiPunct;
+    var Si = F0(),
+        Ic = Se().isWhiteSpace,
+        Oc = Se().isPunctChar,
+        Hc = Se().isMdAsciiPunct;
 
     function Lr(r, e, i, a) {
         this.src = r, this.env = i, this.md = e, this.tokens = a, this.tokens_meta = Array(a.length), this.pos = 0, this.posMax = this.src.length, this.level = 0, this.pending = "", this.pendingLevel = 0, this.cache = {}, this.delimiters = [], this._prev_delimiters = [], this.backticks = {}, this.backticksScanned = !1, this.linkLevel = 0
     }
     Lr.prototype.pushPending = function() {
-        var r = new ki("text", "", 0);
+        var r = new Si("text", "", 0);
         return r.content = this.pending, r.level = this.pendingLevel, this.tokens.push(r), this.pending = "", r
     };
     Lr.prototype.push = function(r, e, i) {
         this.pending && this.pushPending();
-        var a = new ki(r, e, i),
+        var a = new Si(r, e, i),
             l = null;
         return i < 0 && (this.level--, this.delimiters = this._prev_delimiters.pop()), a.level = this.level, i > 0 && (this.level++, this._prev_delimiters.push(this.delimiters), this.delimiters = [], l = {
             delimiters: this.delimiters
         }), this.pendingLevel = this.level, this.tokens.push(a), this.tokens_meta.push(l), a
     };
     Lr.prototype.scanDelims = function(r, e) {
         var i = r,
             a, l, c, d, f, g, y, _, w, T = !0,
             A = !0,
             L = this.posMax,
             R = this.src.charCodeAt(r);
         for (a = r > 0 ? this.src.charCodeAt(r - 1) : 32; i < L && this.src.charCodeAt(i) === R;) i++;
-        return c = i - r, l = i < L ? this.src.charCodeAt(i) : 32, y = Ic(a) || Pc(String.fromCharCode(a)), w = Ic(l) || Pc(String.fromCharCode(l)), g = Lc(a), _ = Lc(l), _ ? T = !1 : w && (g || y || (T = !1)), g ? A = !1 : y && (_ || w || (A = !1)), e ? (d = T, f = A) : (d = T && (!A || y), f = A && (!T || w)), {
+        return c = i - r, l = i < L ? this.src.charCodeAt(i) : 32, y = Hc(a) || Oc(String.fromCharCode(a)), w = Hc(l) || Oc(String.fromCharCode(l)), g = Ic(a), _ = Ic(l), _ ? T = !1 : w && (g || y || (T = !1)), g ? A = !1 : y && (_ || w || (A = !1)), e ? (d = T, f = A) : (d = T && (!A || y), f = A && (!T || w)), {
             can_open: d,
             can_close: f,
             length: c
         }
     };
-    Lr.prototype.Token = ki;
-    Oc.exports = Lr
+    Lr.prototype.Token = Si;
+    $c.exports = Lr
 });
-var Vc = W((V2, Gc) => {
+var Uc = W((X2, jc) => {
     "use strict";
-    var $c = D0(),
-        _i = [
-            ["text", cc()],
-            ["linkify", hc()],
-            ["newline", mc()],
-            ["escape", fc()],
-            ["backticks", bc()],
-            ["strikethrough", bi().tokenize],
-            ["emphasis", xi().tokenize],
-            ["link", wc()],
-            ["image", _c()],
-            ["autolink", Cc()],
-            ["html_inline", Ac()],
-            ["entity", Dc()]
+    var Vc = z0(),
+        Ci = [
+            ["text", hc()],
+            ["linkify", mc()],
+            ["newline", fc()],
+            ["escape", bc()],
+            ["backticks", xc()],
+            ["strikethrough", xi().tokenize],
+            ["emphasis", wi().tokenize],
+            ["link", _c()],
+            ["image", Cc()],
+            ["autolink", Ac()],
+            ["html_inline", Mc()],
+            ["entity", Rc()]
         ],
-        Si = [
-            ["balance_pairs", Fc()],
-            ["strikethrough", bi().postProcess],
-            ["emphasis", xi().postProcess],
-            ["fragments_join", Nc()]
+        Ti = [
+            ["balance_pairs", Nc()],
+            ["strikethrough", xi().postProcess],
+            ["emphasis", wi().postProcess],
+            ["fragments_join", Pc()]
         ];
 
     function Pr() {
         var r;
-        for (this.ruler = new $c, r = 0; r < _i.length; r++) this.ruler.push(_i[r][0], _i[r][1]);
-        for (this.ruler2 = new $c, r = 0; r < Si.length; r++) this.ruler2.push(Si[r][0], Si[r][1])
+        for (this.ruler = new Vc, r = 0; r < Ci.length; r++) this.ruler.push(Ci[r][0], Ci[r][1]);
+        for (this.ruler2 = new Vc, r = 0; r < Ti.length; r++) this.ruler2.push(Ti[r][0], Ti[r][1])
     }
     Pr.prototype.skipToken = function(r) {
         var e, i, a = r.pos,
             l = this.ruler.getRules(""),
             c = l.length,
             d = r.md.options.maxNesting,
             f = r.cache;
@@ -5113,73 +5113,73 @@
         }
         r.pending && r.pushPending()
     };
     Pr.prototype.parse = function(r, e, i, a) {
         var l, c, d, f = new this.State(r, e, i, a);
         for (this.tokenize(f), c = this.ruler2.getRules(""), d = c.length, l = 0; l < d; l++) c[l](f)
     };
-    Pr.prototype.State = Hc();
-    Gc.exports = Pr
+    Pr.prototype.State = Gc();
+    jc.exports = Pr
 });
-var Uc = W((j2, jc) => {
+var Yc = W((J2, Wc) => {
     "use strict";
-    jc.exports = function(r) {
+    Wc.exports = function(r) {
         var e = {};
-        r = r || {}, e.src_Any = oi().source, e.src_Cc = ai().source, e.src_Z = si().source, e.src_P = T0().source, e.src_ZPCc = [e.src_Z, e.src_P, e.src_Cc].join("|"), e.src_ZCc = [e.src_Z, e.src_Cc].join("|");
+        r = r || {}, e.src_Any = si().source, e.src_Cc = li().source, e.src_Z = ci().source, e.src_P = A0().source, e.src_ZPCc = [e.src_Z, e.src_P, e.src_Cc].join("|"), e.src_ZCc = [e.src_Z, e.src_Cc].join("|");
         var i = "[><\uFF5C]";
         return e.src_pseudo_letter = "(?:(?!" + i + "|" + e.src_ZPCc + ")" + e.src_Any + ")", e.src_ip4 = "(?:(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\\.){3}(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)", e.src_auth = "(?:(?:(?!" + e.src_ZCc + "|[@/\\[\\]()]).)+@)?", e.src_port = "(?::(?:6(?:[0-4]\\d{3}|5(?:[0-4]\\d{2}|5(?:[0-2]\\d|3[0-5])))|[1-5]?\\d{1,4}))?", e.src_host_terminator = "(?=$|" + i + "|" + e.src_ZPCc + ")(?!" + (r["---"] ? "-(?!--)|" : "-|") + "_|:\\d|\\.-|\\.(?!$|" + e.src_ZPCc + "))", e.src_path = "(?:[/?#](?:(?!" + e.src_ZCc + "|" + i + `|[()[\\]{}.,"'?!\\-;]).|\\[(?:(?!` + e.src_ZCc + "|\\]).)*\\]|\\((?:(?!" + e.src_ZCc + "|[)]).)*\\)|\\{(?:(?!" + e.src_ZCc + '|[}]).)*\\}|\\"(?:(?!' + e.src_ZCc + `|["]).)+\\"|\\'(?:(?!` + e.src_ZCc + "|[']).)+\\'|\\'(?=" + e.src_pseudo_letter + "|[-])|\\.{2,}[a-zA-Z0-9%/&]|\\.(?!" + e.src_ZCc + "|[.]|$)|" + (r["---"] ? "\\-(?!--(?:[^-]|$))(?:-*)|" : "\\-+|") + ",(?!" + e.src_ZCc + "|$)|;(?!" + e.src_ZCc + "|$)|\\!+(?!" + e.src_ZCc + "|[!]|$)|\\?(?!" + e.src_ZCc + "|[?]|$))+|\\/)?", e.src_email_name = '[\\-;:&=\\+\\$,\\.a-zA-Z0-9_][\\-;:&=\\+\\$,\\"\\.a-zA-Z0-9_]*', e.src_xn = "xn--[a-z0-9\\-]{1,59}", e.src_domain_root = "(?:" + e.src_xn + "|" + e.src_pseudo_letter + "{1,63})", e.src_domain = "(?:" + e.src_xn + "|(?:" + e.src_pseudo_letter + ")|(?:" + e.src_pseudo_letter + "(?:-|" + e.src_pseudo_letter + "){0,61}" + e.src_pseudo_letter + "))", e.src_host = "(?:(?:(?:(?:" + e.src_domain + ")\\.)*" + e.src_domain + "))", e.tpl_host_fuzzy = "(?:" + e.src_ip4 + "|(?:(?:(?:" + e.src_domain + ")\\.)+(?:%TLDS%)))", e.tpl_host_no_ip_fuzzy = "(?:(?:(?:" + e.src_domain + ")\\.)+(?:%TLDS%))", e.src_host_strict = e.src_host + e.src_host_terminator, e.tpl_host_fuzzy_strict = e.tpl_host_fuzzy + e.src_host_terminator, e.src_host_port_strict = e.src_host + e.src_port + e.src_host_terminator, e.tpl_host_port_fuzzy_strict = e.tpl_host_fuzzy + e.src_port + e.src_host_terminator, e.tpl_host_port_no_ip_fuzzy_strict = e.tpl_host_no_ip_fuzzy + e.src_port + e.src_host_terminator, e.tpl_host_fuzzy_test = "localhost|www\\.|\\.\\d{1,3}\\.|(?:\\.(?:%TLDS%)(?:" + e.src_ZPCc + "|>|$))", e.tpl_email_fuzzy = "(^|" + i + '|"|\\(|' + e.src_ZCc + ")(" + e.src_email_name + "@" + e.tpl_host_fuzzy_strict + ")", e.tpl_link_fuzzy = "(^|(?![.:/\\-_@])(?:[$+<=>^`|\uFF5C]|" + e.src_ZPCc + "))((?![$+<=>^`|\uFF5C])" + e.tpl_host_port_fuzzy_strict + e.src_path + ")", e.tpl_link_no_ip_fuzzy = "(^|(?![.:/\\-_@])(?:[$+<=>^`|\uFF5C]|" + e.src_ZPCc + "))((?![$+<=>^`|\uFF5C])" + e.tpl_host_port_no_ip_fuzzy_strict + e.src_path + ")", e
     }
 });
-var Xc = W((U2, Qc) => {
+var Kc = W((K2, Jc) => {
     "use strict";
 
-    function Ci(r) {
+    function Ai(r) {
         var e = Array.prototype.slice.call(arguments, 1);
         return e.forEach(function(i) {
             i && Object.keys(i).forEach(function(a) {
                 r[a] = i[a]
             })
         }), r
     }
 
-    function I0(r) {
+    function O0(r) {
         return Object.prototype.toString.call(r)
     }
 
-    function ip(r) {
-        return I0(r) === "[object String]"
+    function ap(r) {
+        return O0(r) === "[object String]"
     }
 
-    function op(r) {
-        return I0(r) === "[object Object]"
+    function sp(r) {
+        return O0(r) === "[object Object]"
     }
 
-    function ap(r) {
-        return I0(r) === "[object RegExp]"
+    function lp(r) {
+        return O0(r) === "[object RegExp]"
     }
 
-    function Wc(r) {
-        return I0(r) === "[object Function]"
+    function Zc(r) {
+        return O0(r) === "[object Function]"
     }
 
-    function sp(r) {
+    function cp(r) {
         return r.replace(/[.?*+^$[\]\\(){}|-]/g, "\\$&")
     }
-    var Zc = {
+    var Xc = {
         fuzzyLink: !0,
         fuzzyEmail: !0,
         fuzzyIP: !1
     };
 
-    function lp(r) {
+    function up(r) {
         return Object.keys(r || {}).reduce(function(e, i) {
-            return e || Zc.hasOwnProperty(i)
+            return e || Xc.hasOwnProperty(i)
         }, !1)
     }
-    var cp = {
+    var hp = {
             "http:": {
                 validate: function(r, e, i) {
                     var a = r.slice(e);
                     return i.re.http || (i.re.http = new RegExp("^\\/\\/" + i.re.src_auth + i.re.src_host_port_strict + i.re.src_path, "i")), i.re.http.test(a) ? a.match(i.re.http)[0].length : 0
                 }
             },
             "https:": "http:",
@@ -5193,38 +5193,38 @@
             "mailto:": {
                 validate: function(r, e, i) {
                     var a = r.slice(e);
                     return i.re.mailto || (i.re.mailto = new RegExp("^" + i.re.src_email_name + "@" + i.re.src_host_strict, "i")), i.re.mailto.test(a) ? a.match(i.re.mailto)[0].length : 0
                 }
             }
         },
-        up = "a[cdefgilmnoqrstuwxz]|b[abdefghijmnorstvwyz]|c[acdfghiklmnoruvwxyz]|d[ejkmoz]|e[cegrstu]|f[ijkmor]|g[abdefghilmnpqrstuwy]|h[kmnrtu]|i[delmnoqrst]|j[emop]|k[eghimnprwyz]|l[abcikrstuvy]|m[acdeghklmnopqrstuvwxyz]|n[acefgilopruz]|om|p[aefghklmnrstwy]|qa|r[eosuw]|s[abcdeghijklmnortuvxyz]|t[cdfghjklmnortvwz]|u[agksyz]|v[aceginu]|w[fs]|y[et]|z[amw]",
-        hp = "biz|com|edu|gov|net|org|pro|web|xxx|aero|asia|coop|info|museum|name|shop|\u0440\u0444".split("|");
+        dp = "a[cdefgilmnoqrstuwxz]|b[abdefghijmnorstvwyz]|c[acdfghiklmnoruvwxyz]|d[ejkmoz]|e[cegrstu]|f[ijkmor]|g[abdefghilmnpqrstuwy]|h[kmnrtu]|i[delmnoqrst]|j[emop]|k[eghimnprwyz]|l[abcikrstuvy]|m[acdeghklmnopqrstuvwxyz]|n[acefgilopruz]|om|p[aefghklmnrstwy]|qa|r[eosuw]|s[abcdeghijklmnortuvxyz]|t[cdfghjklmnortvwz]|u[agksyz]|v[aceginu]|w[fs]|y[et]|z[amw]",
+        mp = "biz|com|edu|gov|net|org|pro|web|xxx|aero|asia|coop|info|museum|name|shop|\u0440\u0444".split("|");
 
-    function dp(r) {
+    function pp(r) {
         r.__index__ = -1, r.__text_cache__ = ""
     }
 
-    function mp(r) {
+    function fp(r) {
         return function(e, i) {
             var a = e.slice(i);
             return r.test(a) ? a.match(r)[0].length : 0
         }
     }
 
-    function Yc() {
+    function Qc() {
         return function(r, e) {
             e.normalize(r)
         }
     }
 
-    function P0(r) {
-        var e = r.re = Uc()(r.__opts__),
+    function I0(r) {
+        var e = r.re = Yc()(r.__opts__),
             i = r.__tlds__.slice();
-        r.onCompile(), r.__tlds_replaced__ || i.push(up), i.push(e.src_xn), e.src_tlds = i.join("|");
+        r.onCompile(), r.__tlds_replaced__ || i.push(dp), i.push(e.src_xn), e.src_tlds = i.join("|");
 
         function a(f) {
             return f.replace("%TLDS%", e.src_tlds)
         }
         e.email_fuzzy = RegExp(a(e.tpl_email_fuzzy), "i"), e.link_fuzzy = RegExp(a(e.tpl_link_fuzzy), "i"), e.link_no_ip_fuzzy = RegExp(a(e.tpl_link_no_ip_fuzzy), "i"), e.host_fuzzy_test = RegExp(a(e.tpl_host_fuzzy_test), "i");
         var l = [];
         r.__compiled__ = {};
@@ -5235,57 +5235,57 @@
         Object.keys(r.__schemas__).forEach(function(f) {
             var g = r.__schemas__[f];
             if (g !== null) {
                 var y = {
                     validate: null,
                     link: null
                 };
-                if (r.__compiled__[f] = y, op(g)) {
-                    ap(g.validate) ? y.validate = mp(g.validate) : Wc(g.validate) ? y.validate = g.validate : c(f, g), Wc(g.normalize) ? y.normalize = g.normalize : g.normalize ? c(f, g) : y.normalize = Yc();
+                if (r.__compiled__[f] = y, sp(g)) {
+                    lp(g.validate) ? y.validate = fp(g.validate) : Zc(g.validate) ? y.validate = g.validate : c(f, g), Zc(g.normalize) ? y.normalize = g.normalize : g.normalize ? c(f, g) : y.normalize = Qc();
                     return
                 }
-                if (ip(g)) {
+                if (ap(g)) {
                     l.push(f);
                     return
                 }
                 c(f, g)
             }
         }), l.forEach(function(f) {
             r.__compiled__[r.__schemas__[f]] && (r.__compiled__[f].validate = r.__compiled__[r.__schemas__[f]].validate, r.__compiled__[f].normalize = r.__compiled__[r.__schemas__[f]].normalize)
         }), r.__compiled__[""] = {
             validate: null,
-            normalize: Yc()
+            normalize: Qc()
         };
         var d = Object.keys(r.__compiled__).filter(function(f) {
             return f.length > 0 && r.__compiled__[f]
-        }).map(sp).join("|");
-        r.re.schema_test = RegExp("(^|(?!_)(?:[><\uFF5C]|" + e.src_ZPCc + "))(" + d + ")", "i"), r.re.schema_search = RegExp("(^|(?!_)(?:[><\uFF5C]|" + e.src_ZPCc + "))(" + d + ")", "ig"), r.re.schema_at_start = RegExp("^" + r.re.schema_search.source, "i"), r.re.pretest = RegExp("(" + r.re.schema_test.source + ")|(" + r.re.host_fuzzy_test.source + ")|@", "i"), dp(r)
+        }).map(cp).join("|");
+        r.re.schema_test = RegExp("(^|(?!_)(?:[><\uFF5C]|" + e.src_ZPCc + "))(" + d + ")", "i"), r.re.schema_search = RegExp("(^|(?!_)(?:[><\uFF5C]|" + e.src_ZPCc + "))(" + d + ")", "ig"), r.re.schema_at_start = RegExp("^" + r.re.schema_search.source, "i"), r.re.pretest = RegExp("(" + r.re.schema_test.source + ")|(" + r.re.host_fuzzy_test.source + ")|@", "i"), pp(r)
     }
 
-    function pp(r, e) {
+    function gp(r, e) {
         var i = r.__index__,
             a = r.__last_index__,
             l = r.__text_cache__.slice(i, a);
         this.schema = r.__schema__.toLowerCase(), this.index = i + e, this.lastIndex = a + e, this.raw = l, this.text = l, this.url = l
     }
 
-    function Ti(r, e) {
-        var i = new pp(r, e);
+    function qi(r, e) {
+        var i = new gp(r, e);
         return r.__compiled__[i.schema].normalize(i, r), i
     }
 
     function lt(r, e) {
         if (!(this instanceof lt)) return new lt(r, e);
-        e || lp(r) && (e = r, r = {}), this.__opts__ = Ci({}, Zc, e), this.__index__ = -1, this.__last_index__ = -1, this.__schema__ = "", this.__text_cache__ = "", this.__schemas__ = Ci({}, cp, r), this.__compiled__ = {}, this.__tlds__ = hp, this.__tlds_replaced__ = !1, this.re = {}, P0(this)
+        e || up(r) && (e = r, r = {}), this.__opts__ = Ai({}, Xc, e), this.__index__ = -1, this.__last_index__ = -1, this.__schema__ = "", this.__text_cache__ = "", this.__schemas__ = Ai({}, hp, r), this.__compiled__ = {}, this.__tlds__ = mp, this.__tlds_replaced__ = !1, this.re = {}, I0(this)
     }
     lt.prototype.add = function(e, i) {
-        return this.__schemas__[e] = i, P0(this), this
+        return this.__schemas__[e] = i, I0(this), this
     };
     lt.prototype.set = function(e) {
-        return this.__opts__ = Ci(this.__opts__, e), this
+        return this.__opts__ = Ai(this.__opts__, e), this
     };
     lt.prototype.test = function(e) {
         if (this.__text_cache__ = e, this.__index__ = -1, !e.length) return !1;
         var i, a, l, c, d, f, g, y, _;
         if (this.re.schema_test.test(e)) {
             for (g = this.re.schema_search, g.lastIndex = 0;
                 (i = g.exec(e)) !== null;)
@@ -5301,177 +5301,177 @@
     };
     lt.prototype.testSchemaAt = function(e, i, a) {
         return this.__compiled__[i.toLowerCase()] ? this.__compiled__[i.toLowerCase()].validate(e, a, this) : 0
     };
     lt.prototype.match = function(e) {
         var i = 0,
             a = [];
-        this.__index__ >= 0 && this.__text_cache__ === e && (a.push(Ti(this, i)), i = this.__last_index__);
-        for (var l = i ? e.slice(i) : e; this.test(l);) a.push(Ti(this, i)), l = l.slice(this.__last_index__), i += this.__last_index__;
+        this.__index__ >= 0 && this.__text_cache__ === e && (a.push(qi(this, i)), i = this.__last_index__);
+        for (var l = i ? e.slice(i) : e; this.test(l);) a.push(qi(this, i)), l = l.slice(this.__last_index__), i += this.__last_index__;
         return a.length ? a : null
     };
     lt.prototype.matchAtStart = function(e) {
         if (this.__text_cache__ = e, this.__index__ = -1, !e.length) return null;
         var i = this.re.schema_at_start.exec(e);
         if (!i) return null;
         var a = this.testSchemaAt(e, i[2], i[0].length);
-        return a ? (this.__schema__ = i[2], this.__index__ = i.index + i[1].length, this.__last_index__ = i.index + i[0].length + a, Ti(this, 0)) : null
+        return a ? (this.__schema__ = i[2], this.__index__ = i.index + i[1].length, this.__last_index__ = i.index + i[0].length + a, qi(this, 0)) : null
     };
     lt.prototype.tlds = function(e, i) {
         return e = Array.isArray(e) ? e : [e], i ? (this.__tlds__ = this.__tlds__.concat(e).sort().filter(function(a, l, c) {
             return a !== c[l - 1]
-        }).reverse(), P0(this), this) : (this.__tlds__ = e.slice(), this.__tlds_replaced__ = !0, P0(this), this)
+        }).reverse(), I0(this), this) : (this.__tlds__ = e.slice(), this.__tlds_replaced__ = !0, I0(this), this)
     };
     lt.prototype.normalize = function(e) {
         e.schema || (e.url = "http://" + e.url), e.schema === "mailto:" && !/^mailto:/i.test(e.url) && (e.url = "mailto:" + e.url)
     };
     lt.prototype.onCompile = function() {};
-    Qc.exports = lt
+    Jc.exports = lt
 });
-var au = W((W2, ou) => {
+var lu = W((e5, su) => {
     "use strict";
-    var Kc = "-",
-        fp = /^xn--/,
-        gp = /[^\0-\x7F]/,
-        bp = /[\x2E\u3002\uFF0E\uFF61]/g,
-        yp = {
+    var tu = "-",
+        bp = /^xn--/,
+        yp = /[^\0-\x7F]/,
+        xp = /[\x2E\u3002\uFF0E\uFF61]/g,
+        vp = {
             overflow: "Overflow: input needs wider integers to process",
             "not-basic": "Illegal input >= 0x80 (not a basic code point)",
             "invalid-input": "Invalid input"
         },
-        Ai = 35,
+        Mi = 35,
         At = Math.floor,
-        qi = String.fromCharCode;
+        Ei = String.fromCharCode;
 
     function Xt(r) {
-        throw new RangeError(yp[r])
+        throw new RangeError(vp[r])
     }
 
-    function xp(r, e) {
+    function wp(r, e) {
         let i = [],
             a = r.length;
         for (; a--;) i[a] = e(r[a]);
         return i
     }
 
-    function eu(r, e) {
+    function ru(r, e) {
         let i = r.split("@"),
             a = "";
-        i.length > 1 && (a = i[0] + "@", r = i[1]), r = r.replace(bp, ".");
+        i.length > 1 && (a = i[0] + "@", r = i[1]), r = r.replace(xp, ".");
         let l = r.split("."),
-            c = xp(l, e).join(".");
+            c = wp(l, e).join(".");
         return a + c
     }
 
-    function tu(r) {
+    function nu(r) {
         let e = [],
             i = 0,
             a = r.length;
         for (; i < a;) {
             let l = r.charCodeAt(i++);
             if (l >= 55296 && l <= 56319 && i < a) {
                 let c = r.charCodeAt(i++);
                 (c & 64512) == 56320 ? e.push(((l & 1023) << 10) + (c & 1023) + 65536) : (e.push(l), i--)
             } else e.push(l)
         }
         return e
     }
-    var vp = r => String.fromCodePoint(...r),
-        wp = function(r) {
+    var kp = r => String.fromCodePoint(...r),
+        _p = function(r) {
             return r >= 48 && r < 58 ? 26 + (r - 48) : r >= 65 && r < 91 ? r - 65 : r >= 97 && r < 123 ? r - 97 : 36
         },
-        Jc = function(r, e) {
+        eu = function(r, e) {
             return r + 22 + 75 * (r < 26) - ((e != 0) << 5)
         },
-        ru = function(r, e, i) {
+        iu = function(r, e, i) {
             let a = 0;
-            for (r = i ? At(r / 700) : r >> 1, r += At(r / e); r > Ai * 26 >> 1; a += 36) r = At(r / Ai);
-            return At(a + (Ai + 1) * r / (r + 38))
+            for (r = i ? At(r / 700) : r >> 1, r += At(r / e); r > Mi * 26 >> 1; a += 36) r = At(r / Mi);
+            return At(a + (Mi + 1) * r / (r + 38))
         },
-        nu = function(r) {
+        ou = function(r) {
             let e = [],
                 i = r.length,
                 a = 0,
                 l = 128,
                 c = 72,
-                d = r.lastIndexOf(Kc);
+                d = r.lastIndexOf(tu);
             d < 0 && (d = 0);
             for (let f = 0; f < d; ++f) r.charCodeAt(f) >= 128 && Xt("not-basic"), e.push(r.charCodeAt(f));
             for (let f = d > 0 ? d + 1 : 0; f < i;) {
                 let g = a;
                 for (let _ = 1, w = 36;; w += 36) {
                     f >= i && Xt("invalid-input");
-                    let T = wp(r.charCodeAt(f++));
+                    let T = _p(r.charCodeAt(f++));
                     T >= 36 && Xt("invalid-input"), T > At((2147483647 - a) / _) && Xt("overflow"), a += T * _;
                     let A = w <= c ? 1 : w >= c + 26 ? 26 : w - c;
                     if (T < A) break;
                     let L = 36 - A;
                     _ > At(2147483647 / L) && Xt("overflow"), _ *= L
                 }
                 let y = e.length + 1;
-                c = ru(a - g, y, g == 0), At(a / y) > 2147483647 - l && Xt("overflow"), l += At(a / y), a %= y, e.splice(a++, 0, l)
+                c = iu(a - g, y, g == 0), At(a / y) > 2147483647 - l && Xt("overflow"), l += At(a / y), a %= y, e.splice(a++, 0, l)
             }
             return String.fromCodePoint(...e)
         },
-        iu = function(r) {
+        au = function(r) {
             let e = [];
-            r = tu(r);
+            r = nu(r);
             let i = r.length,
                 a = 128,
                 l = 0,
                 c = 72;
-            for (let g of r) g < 128 && e.push(qi(g));
+            for (let g of r) g < 128 && e.push(Ei(g));
             let d = e.length,
                 f = d;
-            for (d && e.push(Kc); f < i;) {
+            for (d && e.push(tu); f < i;) {
                 let g = 2147483647;
                 for (let _ of r) _ >= a && _ < g && (g = _);
                 let y = f + 1;
                 g - a > At((2147483647 - l) / y) && Xt("overflow"), l += (g - a) * y, a = g;
                 for (let _ of r)
                     if (_ < a && ++l > 2147483647 && Xt("overflow"), _ === a) {
                         let w = l;
                         for (let T = 36;; T += 36) {
                             let A = T <= c ? 1 : T >= c + 26 ? 26 : T - c;
                             if (w < A) break;
                             let L = w - A,
                                 R = 36 - A;
-                            e.push(qi(Jc(A + L % R, 0))), w = At(L / R)
+                            e.push(Ei(eu(A + L % R, 0))), w = At(L / R)
                         }
-                        e.push(qi(Jc(w, 0))), c = ru(l, y, f === d), l = 0, ++f
+                        e.push(Ei(eu(w, 0))), c = iu(l, y, f === d), l = 0, ++f
                     }++ l, ++a
             }
             return e.join("")
         },
-        kp = function(r) {
-            return eu(r, function(e) {
-                return fp.test(e) ? nu(e.slice(4).toLowerCase()) : e
+        Sp = function(r) {
+            return ru(r, function(e) {
+                return bp.test(e) ? ou(e.slice(4).toLowerCase()) : e
             })
         },
-        _p = function(r) {
-            return eu(r, function(e) {
-                return gp.test(e) ? "xn--" + iu(e) : e
+        Cp = function(r) {
+            return ru(r, function(e) {
+                return yp.test(e) ? "xn--" + au(e) : e
             })
         },
-        Sp = {
+        Tp = {
             version: "2.3.1",
             ucs2: {
-                decode: tu,
-                encode: vp
+                decode: nu,
+                encode: kp
             },
-            decode: nu,
-            encode: iu,
-            toASCII: _p,
-            toUnicode: kp
+            decode: ou,
+            encode: au,
+            toASCII: Cp,
+            toUnicode: Sp
         };
-    ou.exports = Sp
+    su.exports = Tp
 });
-var lu = W((Y2, su) => {
+var uu = W((t5, cu) => {
     "use strict";
-    su.exports = {
+    cu.exports = {
         options: {
             html: !1,
             xhtmlOut: !1,
             breaks: !1,
             langPrefix: "language-",
             linkify: !1,
             typographer: !1,
@@ -5482,17 +5482,17 @@
         components: {
             core: {},
             block: {},
             inline: {}
         }
     }
 });
-var uu = W((Z2, cu) => {
+var du = W((r5, hu) => {
     "use strict";
-    cu.exports = {
+    hu.exports = {
         options: {
             html: !1,
             xhtmlOut: !1,
             breaks: !1,
             langPrefix: "language-",
             linkify: !1,
             typographer: !1,
@@ -5510,17 +5510,17 @@
             inline: {
                 rules: ["text"],
                 rules2: ["balance_pairs", "fragments_join"]
             }
         }
     }
 });
-var du = W((Q2, hu) => {
+var pu = W((n5, mu) => {
     "use strict";
-    hu.exports = {
+    mu.exports = {
         options: {
             html: !0,
             xhtmlOut: !0,
             breaks: !1,
             langPrefix: "language-",
             linkify: !1,
             typographer: !1,
@@ -5538,66 +5538,66 @@
             inline: {
                 rules: ["autolink", "backticks", "emphasis", "entity", "escape", "html_inline", "image", "link", "newline", "text"],
                 rules2: ["balance_pairs", "emphasis", "fragments_join"]
             }
         }
     }
 });
-var gu = W((X2, fu) => {
+var yu = W((i5, bu) => {
     "use strict";
     var Ir = Se(),
-        Cp = Qs(),
-        Tp = Js(),
-        Ap = Cl(),
-        qp = sc(),
-        Mp = Vc(),
-        Ep = Xc(),
-        ar = ii(),
-        mu = au(),
-        Dp = {
-            default: lu(),
-            zero: uu(),
-            commonmark: du()
+        Ap = Js(),
+        qp = el(),
+        Mp = Al(),
+        Ep = cc(),
+        Dp = Uc(),
+        zp = Kc(),
+        ar = ai(),
+        fu = lu(),
+        Rp = {
+            default: uu(),
+            zero: du(),
+            commonmark: pu()
         },
-        zp = /^(vbscript|javascript|file|data):/,
-        Rp = /^data:image\/(gif|png|jpeg|webp);/;
+        Fp = /^(vbscript|javascript|file|data):/,
+        Bp = /^data:image\/(gif|png|jpeg|webp);/;
 
-    function Fp(r) {
+    function Np(r) {
         var e = r.trim().toLowerCase();
-        return zp.test(e) ? !!Rp.test(e) : !0
+        return Fp.test(e) ? !!Bp.test(e) : !0
     }
-    var pu = ["http:", "https:", "mailto:"];
+    var gu = ["http:", "https:", "mailto:"];
 
-    function Bp(r) {
+    function Lp(r) {
         var e = ar.parse(r, !0);
-        if (e.hostname && (!e.protocol || pu.indexOf(e.protocol) >= 0)) try {
-            e.hostname = mu.toASCII(e.hostname)
+        if (e.hostname && (!e.protocol || gu.indexOf(e.protocol) >= 0)) try {
+            e.hostname = fu.toASCII(e.hostname)
         } catch {}
         return ar.encode(ar.format(e))
     }
 
-    function Np(r) {
+    function Pp(r) {
         var e = ar.parse(r, !0);
-        if (e.hostname && (!e.protocol || pu.indexOf(e.protocol) >= 0)) try {
-            e.hostname = mu.toUnicode(e.hostname)
+        if (e.hostname && (!e.protocol || gu.indexOf(e.protocol) >= 0)) try {
+            e.hostname = fu.toUnicode(e.hostname)
         } catch {}
         return ar.decode(ar.format(e), ar.decode.defaultChars + "%")
     }
 
     function bt(r, e) {
         if (!(this instanceof bt)) return new bt(r, e);
-        e || Ir.isString(r) || (e = r || {}, r = "default"), this.inline = new Mp, this.block = new qp, this.core = new Ap, this.renderer = new Tp, this.linkify = new Ep, this.validateLink = Fp, this.normalizeLink = Bp, this.normalizeLinkText = Np, this.utils = Ir, this.helpers = Ir.assign({}, Cp), this.options = {}, this.configure(r), e && this.set(e)
+        e || Ir.isString(r) || (e = r || {}, r = "default"), this.inline = new Dp, this.block = new Ep, this.core = new Mp, this.renderer = new qp, this.linkify = new zp, this.validateLink = Np, this.normalizeLink = Lp, this.normalizeLinkText = Pp, this.utils = Ir, this.helpers = Ir.assign({}, Ap), this.options = {}, this.configure(r), e && this.set(e)
     }
     bt.prototype.set = function(r) {
         return Ir.assign(this.options, r), this
     };
     bt.prototype.configure = function(r) {
         var e = this,
             i;
-        if (Ir.isString(r) && (i = r, r = Dp[i], !r)) throw new Error('Wrong `markdown-it` preset "' + i + '", check name');
+        if (Ir.isString(r) && (i = r, r = Rp[i], !r)) throw new Error('Wrong `markdown-it` preset "' + i + '", check name');
         if (!r) throw new Error("Wrong `markdown-it` preset, can't be empty");
         return r.options && e.set(r.options), r.components && Object.keys(r.components).forEach(function(a) {
             r.components[a].rules && e[a].ruler.enableOnly(r.components[a].rules), r.components[a].rules2 && e[a].ruler2.enableOnly(r.components[a].rules2)
         }), this
     };
     bt.prototype.enable = function(r, e) {
         var i = [];
@@ -5636,23 +5636,23 @@
     bt.prototype.parseInline = function(r, e) {
         var i = new this.core.State(r, this, e);
         return i.inlineMode = !0, this.core.process(i), i.tokens
     };
     bt.prototype.renderInline = function(r, e) {
         return e = e || {}, this.renderer.render(this.parseInline(r, e), this.options, e)
     };
-    fu.exports = bt
+    bu.exports = bt
 });
-var yu = W((J2, bu) => {
+var vu = W((o5, xu) => {
     "use strict";
-    bu.exports = gu()
+    xu.exports = yu()
 });
-var xu = W((Or, Mi) => {
+var wu = W((Or, Di) => {
     (function(e, i) {
-        typeof Or == "object" && typeof Mi == "object" ? Mi.exports = i() : typeof define == "function" && define.amd ? define([], i) : typeof Or == "object" ? Or.katex = i() : e.katex = i()
+        typeof Or == "object" && typeof Di == "object" ? Di.exports = i() : typeof define == "function" && define.amd ? define([], i) : typeof Or == "object" ? Or.katex = i() : e.katex = i()
     })(typeof self < "u" ? self : Or, function() {
         return function() {
             "use strict";
             var r = {};
             (function() {
                 r.d = function(n, t) {
                     for (var o in t) r.o(t, o) && !r.o(n, o) && Object.defineProperty(n, o, {
@@ -5665,15 +5665,15 @@
                 r.o = function(n, t) {
                     return Object.prototype.hasOwnProperty.call(n, t)
                 }
             }();
             var e = {};
             r.d(e, {
                 default: function() {
-                    return K1
+                    return th
                 }
             });
             class i {
                 constructor(t, o) {
                     this.name = void 0, this.position = void 0, this.length = void 0, this.rawMessage = void 0;
                     let s = "KaTeX parse error: " + t,
                         u, p, b = o && o.loc;
@@ -6004,86 +6004,86 @@
 H40000v` + (40 + n) + `H1012.3
 s-271.3,567,-271.3,567c-38.7,80.7,-84,175,-136,283c-52,108,-89.167,185.3,-111.5,232
 c-22.3,46.7,-33.8,70.3,-34.5,71c-4.7,4.7,-12.3,7,-23,7s-12,-1,-12,-1
 s-109,-253,-109,-253c-72.7,-168,-109.3,-252,-110,-252c-10.7,8,-22,16.7,-34,26
 c-22,17.3,-33.3,26,-34,26s-26,-26,-26,-26s76,-59,76,-59s76,-60,76,-60z
 M` + (1001 + n) + " " + t + "h400000v" + (40 + n) + "h-400000z"
                 },
-                H0 = function(n, t) {
+                $0 = function(n, t) {
                     return "M983 " + (10 + n + t) + `
 l` + n / 3.13 + " -" + n + `
 c4,-6.7,10,-10,18,-10 H400000v` + (40 + n) + `
 H1013.1s-83.4,268,-264.1,840c-180.7,572,-277,876.3,-289,913c-4.7,4.7,-12.7,7,-24,7
 s-12,0,-12,0c-1.3,-3.3,-3.7,-11.7,-7,-25c-35.3,-125.3,-106.7,-373.3,-214,-744
 c-10,12,-21,25,-33,39s-32,39,-32,39c-6,-5.3,-15,-14,-27,-26s25,-30,25,-30
 c26.7,-32.7,52,-63,76,-91s52,-60,52,-60s208,722,208,722
 c56,-175.3,126.3,-397.3,211,-666c84.7,-268.7,153.8,-488.2,207.5,-658.5
 c53.7,-170.3,84.5,-266.8,92.5,-289.5z
 M` + (1001 + n) + " " + t + "h400000v" + (40 + n) + "h-400000z"
                 },
-                $0 = function(n, t) {
+                G0 = function(n, t) {
                     return "M424," + (2398 + n + t) + `
 c-1.3,-0.7,-38.5,-172,-111.5,-514c-73,-342,-109.8,-513.3,-110.5,-514
 c0,-2,-10.7,14.3,-32,49c-4.7,7.3,-9.8,15.7,-15.5,25c-5.7,9.3,-9.8,16,-12.5,20
 s-5,7,-5,7c-4,-3.3,-8.3,-7.7,-13,-13s-13,-13,-13,-13s76,-122,76,-122s77,-121,77,-121
 s209,968,209,968c0,-2,84.7,-361.7,254,-1079c169.3,-717.3,254.7,-1077.7,256,-1081
 l` + n / 4.223 + " -" + n + `c4,-6.7,10,-10,18,-10 H400000
 v` + (40 + n) + `H1014.6
 s-87.3,378.7,-272.6,1166c-185.3,787.3,-279.3,1182.3,-282,1185
 c-2,6,-10,9,-24,9
 c-8,0,-12,-0.7,-12,-2z M` + (1001 + n) + " " + t + `
 h400000v` + (40 + n) + "h-400000z"
                 },
-                G0 = function(n, t) {
+                V0 = function(n, t) {
                     return "M473," + (2713 + n + t) + `
 c339.3,-1799.3,509.3,-2700,510,-2702 l` + n / 5.298 + " -" + n + `
 c3.3,-7.3,9.3,-11,18,-11 H400000v` + (40 + n) + `H1017.7
 s-90.5,478,-276.2,1466c-185.7,988,-279.5,1483,-281.5,1485c-2,6,-10,9,-24,9
 c-8,0,-12,-0.7,-12,-2c0,-1.3,-5.3,-32,-16,-92c-50.7,-293.3,-119.7,-693.3,-207,-1200
 c0,-1.3,-5.3,8.7,-16,30c-10.7,21.3,-21.3,42.7,-32,64s-16,33,-16,33s-26,-26,-26,-26
 s76,-153,76,-153s77,-151,77,-151c0.7,0.7,35.7,202,105,604c67.3,400.7,102,602.7,104,
 606zM` + (1001 + n) + " " + t + "h400000v" + (40 + n) + "H1017.7z"
                 },
-                zu = function(n) {
+                Fu = function(n) {
                     let t = n / 2;
                     return "M400000 " + n + " H0 L" + t + " 0 l65 45 L145 " + (n - 80) + " H400000z"
                 },
-                Ru = function(n, t, o) {
+                Bu = function(n, t, o) {
                     let s = o - 54 - t - n;
                     return "M702 " + (n + t) + "H400000" + (40 + n) + `
 H742v` + s + `l-4 4-4 4c-.667.7 -2 1.5-4 2.5s-4.167 1.833-6.5 2.5-5.5 1-9.5 1
 h-12l-28-84c-16.667-52-96.667 -294.333-240-727l-212 -643 -85 170
 c-4-3.333-8.333-7.667-13 -13l-13-13l77-155 77-156c66 199.333 139 419.667
 219 661 l218 661zM702 ` + t + "H400000v" + (40 + n) + "H742z"
                 },
-                Fu = function(n, t, o) {
+                Nu = function(n, t, o) {
                     t = 1e3 * t;
                     let s = "";
                     switch (n) {
                         case "sqrtMain":
                             s = Pt(t, ct);
                             break;
                         case "sqrtSize1":
                             s = yr(t, ct);
                             break;
                         case "sqrtSize2":
-                            s = H0(t, ct);
+                            s = $0(t, ct);
                             break;
                         case "sqrtSize3":
-                            s = $0(t, ct);
+                            s = G0(t, ct);
                             break;
                         case "sqrtSize4":
-                            s = G0(t, ct);
+                            s = V0(t, ct);
                             break;
                         case "sqrtTall":
-                            s = Ru(t, ct, o)
+                            s = Bu(t, ct, o)
                     }
                     return s
                 },
-                Bu = function(n, t) {
+                Lu = function(n, t) {
                     switch (n) {
                         case "\u239C":
                             return "M291 0 H417 V" + t + " H291z M291 0 H417 V" + t + " H291z";
                         case "\u2223":
                             return "M145 0 H188 V" + t + " H145z M145 0 H188 V" + t + " H145z";
                         case "\u2225":
                             return "M145 0 H188 V" + t + " H145z M145 0 H188 V" + t + " H145z" + ("M367 0 H410 V" + t + " H367z M367 0 H410 V" + t + " H367z");
@@ -6099,15 +6099,15 @@
                             return "M312 0 H355 V" + t + " H312z M312 0 H355 V" + t + " H312z";
                         case "\u2016":
                             return "M257 0 H300 V" + t + " H257z M257 0 H300 V" + t + " H257z" + ("M478 0 H521 V" + t + " H478z M478 0 H521 V" + t + " H478z");
                         default:
                             return ""
                     }
                 },
-                Ei = {
+                zi = {
                     doubleleftarrow: `M262 157
 l10-10c34-36 62.7-77 86-123 3.3-8 5-13.3 5-16 0-5.3-6.7-8-20-8-7.3
  0-12.2.5-14.5 1.5-2.3 1-4.8 4.5-7.5 10.5-49.3 97.3-121.7 169.3-217 216-28
  14-57.3 25-88 33-6.7 2-11 3.8-13 5.5-2 1.7-3 4.2-3 7.5s1 5.8 3 7.5
 c2 1.7 6.3 3.5 13 5.5 68 17.3 128.2 47.8 180.5 91.5 52.3 43.7 93.8 96.2 124.5
  157.5 9.3 8 15.3 12.3 18 13h6c12-.7 18-4 18-10 0-2-1.7-7-5-15-23.3-46-52-87
 -86-123l-10-10h399738v-40H218c328 0 0 0 0 0l-10-8c-26.7-20-65.7-43-117-69 2.7
@@ -6331,15 +6331,15 @@
 M93 435 v40 H400000 v-40z M500 241 v40 H400000 v-40z M500 241 v40 H400000 v-40z`,
                     shortrightharpoonabovebar: `M53,241l0,40c398570,0,399437,0,399437,0
 c4.7,-4.7,7,-9.3,7,-14c0,-9.3,-3.7,-15.3,-11,-18c-92.7,-56.7,-159,-133.7,-199,
 -231c-3.3,-9.3,-6,-14.7,-8,-16c-2,-1.3,-7,-2,-15,-2c-10.7,0,-16.7,2,-18,6
 c-2,2.7,-1,9.7,3,21c15.3,42,36.7,81.8,64,119.5c27.3,37.7,58,69.2,92,94.5z
 M500 241 v40 H399408 v-40z M500 435 v40 H400000 v-40z`
                 },
-                Nu = function(n, t) {
+                Pu = function(n, t) {
                     switch (n) {
                         case "lbrack":
                             return "M403 1759 V84 H666 V0 H319 V1759 v" + t + ` v1759 h347 v-84
 H403z M403 1759 V0 H319 V1759 v` + t + " v1759 h84z";
                         case "rbrack":
                             return "M347 1759 V0 H0 V84 H263 V1759 v" + t + ` v1759 H0 v84 H347z
 M347 1759 V0 H263 V1759 v` + t + " v1759 h84z";
@@ -8519,15 +8519,15 @@
                     sqrtRuleThickness: [.04, .04, .04],
                     ptPerEm: [10, 10, 10],
                     doubleRuleSep: [.2, .2, .2],
                     arrayRuleWidth: [.04, .04, .04],
                     fboxsep: [.3, .3, .3],
                     fboxrule: [.04, .04, .04]
                 },
-                Di = {
+                Ri = {
                     \u00C5: "A",
                     \u00D0: "D",
                     \u00DE: "o",
                     \u00E5: "a",
                     \u00F0: "d",
                     \u00FE: "o",
                     \u0410: "A",
@@ -8592,62 +8592,62 @@
                     \u044B: "m",
                     \u044C: "a",
                     \u044D: "e",
                     \u044E: "m",
                     \u044F: "r"
                 };
 
-            function Lu(n, t) {
+            function Iu(n, t) {
                 vt[n] = t
             }
 
-            function V0(n, t, o) {
+            function j0(n, t, o) {
                 if (!vt[t]) throw new Error("Font metrics not found for font: " + t + ".");
                 let s = n.charCodeAt(0),
                     u = vt[t][s];
-                if (!u && n[0] in Di && (s = Di[n[0]].charCodeAt(0), u = vt[t][s]), !u && o === "text" && qt(s) && (u = vt[t][77]), u) return {
+                if (!u && n[0] in Ri && (s = Ri[n[0]].charCodeAt(0), u = vt[t][s]), !u && o === "text" && qt(s) && (u = vt[t][77]), u) return {
                     depth: u[0],
                     height: u[1],
                     italic: u[2],
                     skew: u[3],
                     width: u[4]
                 }
             }
-            let j0 = {};
+            let U0 = {};
 
-            function Pu(n) {
+            function Ou(n) {
                 let t;
-                if (n >= 5 ? t = 0 : n >= 3 ? t = 1 : t = 2, !j0[t]) {
-                    let o = j0[t] = {
+                if (n >= 5 ? t = 0 : n >= 3 ? t = 1 : t = 2, !U0[t]) {
+                    let o = U0[t] = {
                         cssEmPerMu: $r.quad[t] / 18
                     };
                     for (let s in $r) $r.hasOwnProperty(s) && (o[s] = $r[s][t])
                 }
-                return j0[t]
+                return U0[t]
             }
-            let Iu = [
+            let Hu = [
                     [1, 1, 1],
                     [2, 1, 1],
                     [3, 1, 1],
                     [4, 2, 1],
                     [5, 2, 1],
                     [6, 3, 1],
                     [7, 4, 2],
                     [8, 6, 3],
                     [9, 7, 6],
                     [10, 8, 7],
                     [11, 10, 9]
                 ],
-                zi = [.5, .6, .7, .8, .9, 1, 1.2, 1.44, 1.728, 2.074, 2.488],
-                Ri = function(n, t) {
-                    return t.size < 2 ? n : Iu[n - 1][t.size - 1]
+                Fi = [.5, .6, .7, .8, .9, 1, 1.2, 1.44, 1.728, 2.074, 2.488],
+                Bi = function(n, t) {
+                    return t.size < 2 ? n : Hu[n - 1][t.size - 1]
                 };
             class Mt {
                 constructor(t) {
-                    this.style = void 0, this.color = void 0, this.size = void 0, this.textSize = void 0, this.phantom = void 0, this.font = void 0, this.fontFamily = void 0, this.fontWeight = void 0, this.fontShape = void 0, this.sizeMultiplier = void 0, this.maxSize = void 0, this.minRuleThickness = void 0, this._fontMetrics = void 0, this.style = t.style, this.color = t.color, this.size = t.size || Mt.BASESIZE, this.textSize = t.textSize || this.size, this.phantom = !!t.phantom, this.font = t.font || "", this.fontFamily = t.fontFamily || "", this.fontWeight = t.fontWeight || "", this.fontShape = t.fontShape || "", this.sizeMultiplier = zi[this.size - 1], this.maxSize = t.maxSize, this.minRuleThickness = t.minRuleThickness, this._fontMetrics = void 0
+                    this.style = void 0, this.color = void 0, this.size = void 0, this.textSize = void 0, this.phantom = void 0, this.font = void 0, this.fontFamily = void 0, this.fontWeight = void 0, this.fontShape = void 0, this.sizeMultiplier = void 0, this.maxSize = void 0, this.minRuleThickness = void 0, this._fontMetrics = void 0, this.style = t.style, this.color = t.color, this.size = t.size || Mt.BASESIZE, this.textSize = t.textSize || this.size, this.phantom = !!t.phantom, this.font = t.font || "", this.fontFamily = t.fontFamily || "", this.fontWeight = t.fontWeight || "", this.fontShape = t.fontShape || "", this.sizeMultiplier = Fi[this.size - 1], this.maxSize = t.maxSize, this.minRuleThickness = t.minRuleThickness, this._fontMetrics = void 0
                 }
                 extend(t) {
                     let o = {
                         style: this.style,
                         size: this.size,
                         textSize: this.textSize,
                         color: this.color,
@@ -8661,31 +8661,31 @@
                     };
                     for (let s in t) t.hasOwnProperty(s) && (o[s] = t[s]);
                     return new Mt(o)
                 }
                 havingStyle(t) {
                     return this.style === t ? this : this.extend({
                         style: t,
-                        size: Ri(this.textSize, t)
+                        size: Bi(this.textSize, t)
                     })
                 }
                 havingCrampedStyle() {
                     return this.havingStyle(this.style.cramp())
                 }
                 havingSize(t) {
                     return this.size === t && this.textSize === t ? this : this.extend({
                         style: this.style.text(),
                         size: t,
                         textSize: t,
-                        sizeMultiplier: zi[t - 1]
+                        sizeMultiplier: Fi[t - 1]
                     })
                 }
                 havingBaseStyle(t) {
                     t = t || this.style.text();
-                    let o = Ri(Mt.BASESIZE, t);
+                    let o = Bi(Mt.BASESIZE, t);
                     return this.size === o && this.textSize === Mt.BASESIZE && this.style === t ? this : this.extend({
                         style: t,
                         size: o
                     })
                 }
                 havingBaseSizing() {
                     let t;
@@ -8742,47 +8742,47 @@
                 sizingClasses(t) {
                     return t.size !== this.size ? ["sizing", "reset-size" + t.size, "size" + this.size] : []
                 }
                 baseSizingClasses() {
                     return this.size !== Mt.BASESIZE ? ["sizing", "reset-size" + this.size, "size" + Mt.BASESIZE] : []
                 }
                 fontMetrics() {
-                    return this._fontMetrics || (this._fontMetrics = Pu(this.size)), this._fontMetrics
+                    return this._fontMetrics || (this._fontMetrics = Ou(this.size)), this._fontMetrics
                 }
                 getColor() {
                     return this.phantom ? "transparent" : this.color
                 }
             }
             Mt.BASESIZE = 6;
-            var Ou = Mt;
-            let U0 = {
+            var $u = Mt;
+            let W0 = {
                     pt: 1,
                     mm: 7227 / 2540,
                     cm: 7227 / 254,
                     in: 72.27,
                     bp: 803 / 800,
                     pc: 12,
                     dd: 1238 / 1157,
                     cc: 14856 / 1157,
                     nd: 685 / 642,
                     nc: 1370 / 107,
                     sp: 1 / 65536,
                     px: 803 / 800
                 },
-                Hu = {
+                Gu = {
                     ex: !0,
                     em: !0,
                     mu: !0
                 },
-                Fi = function(n) {
-                    return typeof n != "string" && (n = n.unit), n in U0 || n in Hu || n === "ex"
+                Ni = function(n) {
+                    return typeof n != "string" && (n = n.unit), n in W0 || n in Gu || n === "ex"
                 },
                 Ie = function(n, t) {
                     let o;
-                    if (n.unit in U0) o = U0[n.unit] / t.fontMetrics().ptPerEm / t.sizeMultiplier;
+                    if (n.unit in W0) o = W0[n.unit] / t.fontMetrics().ptPerEm / t.sizeMultiplier;
                     else if (n.unit === "mu") o = t.fontMetrics().cssEmPerMu;
                     else {
                         let s;
                         if (t.style.isTight() ? s = t.havingStyle(t.style.text()) : s = t, n.unit === "ex") o = s.fontMetrics().xHeight;
                         else if (n.unit === "em") o = s.fontMetrics().quad;
                         else throw new a("Invalid unit: '" + n.unit + "'");
                         s !== t && (o *= s.sizeMultiplier / t.sizeMultiplier)
@@ -8791,75 +8791,75 @@
                 },
                 Z = function(n) {
                     return +n.toFixed(4) + "em"
                 },
                 It = function(n) {
                     return n.filter(t => t).join(" ")
                 },
-                Bi = function(n, t, o) {
+                Li = function(n, t, o) {
                     if (this.classes = n || [], this.attributes = {}, this.height = 0, this.depth = 0, this.maxFontSize = 0, this.style = o || {}, t) {
                         t.style.isTight() && this.classes.push("mtight");
                         let s = t.getColor();
                         s && (this.style.color = s)
                     }
                 },
-                Ni = function(n) {
+                Pi = function(n) {
                     let t = document.createElement(n);
                     t.className = It(this.classes);
                     for (let o in this.style) this.style.hasOwnProperty(o) && (t.style[o] = this.style[o]);
                     for (let o in this.attributes) this.attributes.hasOwnProperty(o) && t.setAttribute(o, this.attributes[o]);
                     for (let o = 0; o < this.children.length; o++) t.appendChild(this.children[o].toNode());
                     return t
                 },
-                Li = function(n) {
+                Ii = function(n) {
                     let t = "<" + n;
                     this.classes.length && (t += ' class="' + R.escape(It(this.classes)) + '"');
                     let o = "";
                     for (let s in this.style) this.style.hasOwnProperty(s) && (o += R.hyphenate(s) + ":" + this.style[s] + ";");
                     o && (t += ' style="' + R.escape(o) + '"');
                     for (let s in this.attributes) this.attributes.hasOwnProperty(s) && (t += " " + s + '="' + R.escape(this.attributes[s]) + '"');
                     t += ">";
                     for (let s = 0; s < this.children.length; s++) t += this.children[s].toMarkup();
                     return t += "</" + n + ">", t
                 };
             class vr {
                 constructor(t, o, s, u) {
-                    this.children = void 0, this.attributes = void 0, this.classes = void 0, this.height = void 0, this.depth = void 0, this.width = void 0, this.maxFontSize = void 0, this.style = void 0, Bi.call(this, t, s, u), this.children = o || []
+                    this.children = void 0, this.attributes = void 0, this.classes = void 0, this.height = void 0, this.depth = void 0, this.width = void 0, this.maxFontSize = void 0, this.style = void 0, Li.call(this, t, s, u), this.children = o || []
                 }
                 setAttribute(t, o) {
                     this.attributes[t] = o
                 }
                 hasClass(t) {
                     return R.contains(this.classes, t)
                 }
                 toNode() {
-                    return Ni.call(this, "span")
+                    return Pi.call(this, "span")
                 }
                 toMarkup() {
-                    return Li.call(this, "span")
+                    return Ii.call(this, "span")
                 }
             }
-            class W0 {
+            class Y0 {
                 constructor(t, o, s, u) {
-                    this.children = void 0, this.attributes = void 0, this.classes = void 0, this.height = void 0, this.depth = void 0, this.maxFontSize = void 0, this.style = void 0, Bi.call(this, o, u), this.children = s || [], this.setAttribute("href", t)
+                    this.children = void 0, this.attributes = void 0, this.classes = void 0, this.height = void 0, this.depth = void 0, this.maxFontSize = void 0, this.style = void 0, Li.call(this, o, u), this.children = s || [], this.setAttribute("href", t)
                 }
                 setAttribute(t, o) {
                     this.attributes[t] = o
                 }
                 hasClass(t) {
                     return R.contains(this.classes, t)
                 }
                 toNode() {
-                    return Ni.call(this, "a")
+                    return Pi.call(this, "a")
                 }
                 toMarkup() {
-                    return Li.call(this, "a")
+                    return Ii.call(this, "a")
                 }
             }
-            class $u {
+            class Vu {
                 constructor(t, o, s) {
                     this.src = void 0, this.alt = void 0, this.classes = void 0, this.height = void 0, this.depth = void 0, this.maxFontSize = void 0, this.style = void 0, this.alt = o, this.src = t, this.classes = ["mord"], this.style = s
                 }
                 hasClass(t) {
                     return R.contains(this.classes, t)
                 }
                 toNode() {
@@ -8871,25 +8871,25 @@
                 toMarkup() {
                     let t = '<img src="' + R.escape(this.src) + '"' + (' alt="' + R.escape(this.alt) + '"'),
                         o = "";
                     for (let s in this.style) this.style.hasOwnProperty(s) && (o += R.hyphenate(s) + ":" + this.style[s] + ";");
                     return o && (t += ' style="' + R.escape(o) + '"'), t += "'/>", t
                 }
             }
-            let Gu = {
+            let ju = {
                 \u00EE: "\u0131\u0302",
                 \u00EF: "\u0131\u0308",
                 \u00ED: "\u0131\u0301",
                 \u00EC: "\u0131\u0300"
             };
             class ut {
                 constructor(t, o, s, u, p, b, v, S) {
                     this.text = void 0, this.height = void 0, this.depth = void 0, this.italic = void 0, this.skew = void 0, this.width = void 0, this.maxFontSize = void 0, this.classes = void 0, this.style = void 0, this.text = t, this.height = o || 0, this.depth = s || 0, this.italic = u || 0, this.skew = p || 0, this.width = b || 0, this.classes = v || [], this.style = S || {}, this.maxFontSize = 0;
                     let E = Te(this.text.charCodeAt(0));
-                    E && this.classes.push(E + "_fallback"), /[îïíì]/.test(this.text) && (this.text = Gu[this.text])
+                    E && this.classes.push(E + "_fallback"), /[îïíì]/.test(this.text) && (this.text = ju[this.text])
                 }
                 hasClass(t) {
                     return R.contains(this.classes, t)
                 }
                 toNode() {
                     let t = document.createTextNode(this.text),
                         o = null;
@@ -8929,21 +8929,21 @@
             }
             class Ot {
                 constructor(t, o) {
                     this.pathName = void 0, this.alternate = void 0, this.pathName = t, this.alternate = o
                 }
                 toNode() {
                     let o = document.createElementNS("http://www.w3.org/2000/svg", "path");
-                    return this.alternate ? o.setAttribute("d", this.alternate) : o.setAttribute("d", Ei[this.pathName]), o
+                    return this.alternate ? o.setAttribute("d", this.alternate) : o.setAttribute("d", zi[this.pathName]), o
                 }
                 toMarkup() {
-                    return this.alternate ? '<path d="' + R.escape(this.alternate) + '"/>' : '<path d="' + R.escape(Ei[this.pathName]) + '"/>'
+                    return this.alternate ? '<path d="' + R.escape(this.alternate) + '"/>' : '<path d="' + R.escape(zi[this.pathName]) + '"/>'
                 }
             }
-            class Y0 {
+            class Z0 {
                 constructor(t) {
                     this.attributes = void 0, this.attributes = t || {}
                 }
                 toNode() {
                     let o = document.createElementNS("http://www.w3.org/2000/svg", "line");
                     for (let s in this.attributes) Object.prototype.hasOwnProperty.call(this.attributes, s) && o.setAttribute(s, this.attributes[s]);
                     return o
@@ -8951,32 +8951,32 @@
                 toMarkup() {
                     let t = "<line";
                     for (let o in this.attributes) Object.prototype.hasOwnProperty.call(this.attributes, o) && (t += " " + o + '="' + R.escape(this.attributes[o]) + '"');
                     return t += "/>", t
                 }
             }
 
-            function Pi(n) {
+            function Oi(n) {
                 if (n instanceof ut) return n;
                 throw new Error("Expected symbolNode but got " + String(n) + ".")
             }
 
-            function Vu(n) {
+            function Uu(n) {
                 if (n instanceof vr) return n;
                 throw new Error("Expected span<HtmlDomNode> but got " + String(n) + ".")
             }
-            let ju = {
+            let Wu = {
                     bin: 1,
                     close: 1,
                     inner: 1,
                     open: 1,
                     punct: 1,
                     rel: 1
                 },
-                Uu = {
+                Yu = {
                     "accent-token": 1,
                     mathord: 1,
                     "op-token": 1,
                     spacing: 1,
                     textord: 1
                 },
                 Gr = {
@@ -9004,29 +9004,29 @@
                 We = "op-token",
                 at = "open",
                 Vr = "punct",
                 q = "rel",
                 Dt = "spacing",
                 D = "textord";
             h(m, x, q, "\u2261", "\\equiv", !0), h(m, x, q, "\u227A", "\\prec", !0), h(m, x, q, "\u227B", "\\succ", !0), h(m, x, q, "\u223C", "\\sim", !0), h(m, x, q, "\u22A5", "\\perp"), h(m, x, q, "\u2AAF", "\\preceq", !0), h(m, x, q, "\u2AB0", "\\succeq", !0), h(m, x, q, "\u2243", "\\simeq", !0), h(m, x, q, "\u2223", "\\mid", !0), h(m, x, q, "\u226A", "\\ll", !0), h(m, x, q, "\u226B", "\\gg", !0), h(m, x, q, "\u224D", "\\asymp", !0), h(m, x, q, "\u2225", "\\parallel"), h(m, x, q, "\u22C8", "\\bowtie", !0), h(m, x, q, "\u2323", "\\smile", !0), h(m, x, q, "\u2291", "\\sqsubseteq", !0), h(m, x, q, "\u2292", "\\sqsupseteq", !0), h(m, x, q, "\u2250", "\\doteq", !0), h(m, x, q, "\u2322", "\\frown", !0), h(m, x, q, "\u220B", "\\ni", !0), h(m, x, q, "\u221D", "\\propto", !0), h(m, x, q, "\u22A2", "\\vdash", !0), h(m, x, q, "\u22A3", "\\dashv", !0), h(m, x, q, "\u220B", "\\owns"), h(m, x, Vr, ".", "\\ldotp"), h(m, x, Vr, "\u22C5", "\\cdotp"), h(m, x, D, "#", "\\#"), h($, x, D, "#", "\\#"), h(m, x, D, "&", "\\&"), h($, x, D, "&", "\\&"), h(m, x, D, "\u2135", "\\aleph", !0), h(m, x, D, "\u2200", "\\forall", !0), h(m, x, D, "\u210F", "\\hbar", !0), h(m, x, D, "\u2203", "\\exists", !0), h(m, x, D, "\u2207", "\\nabla", !0), h(m, x, D, "\u266D", "\\flat", !0), h(m, x, D, "\u2113", "\\ell", !0), h(m, x, D, "\u266E", "\\natural", !0), h(m, x, D, "\u2663", "\\clubsuit", !0), h(m, x, D, "\u2118", "\\wp", !0), h(m, x, D, "\u266F", "\\sharp", !0), h(m, x, D, "\u2662", "\\diamondsuit", !0), h(m, x, D, "\u211C", "\\Re", !0), h(m, x, D, "\u2661", "\\heartsuit", !0), h(m, x, D, "\u2111", "\\Im", !0), h(m, x, D, "\u2660", "\\spadesuit", !0), h(m, x, D, "\xA7", "\\S", !0), h($, x, D, "\xA7", "\\S"), h(m, x, D, "\xB6", "\\P", !0), h($, x, D, "\xB6", "\\P"), h(m, x, D, "\u2020", "\\dag"), h($, x, D, "\u2020", "\\dag"), h($, x, D, "\u2020", "\\textdagger"), h(m, x, D, "\u2021", "\\ddag"), h($, x, D, "\u2021", "\\ddag"), h($, x, D, "\u2021", "\\textdaggerdbl"), h(m, x, et, "\u23B1", "\\rmoustache", !0), h(m, x, at, "\u23B0", "\\lmoustache", !0), h(m, x, et, "\u27EF", "\\rgroup", !0), h(m, x, at, "\u27EE", "\\lgroup", !0), h(m, x, J, "\u2213", "\\mp", !0), h(m, x, J, "\u2296", "\\ominus", !0), h(m, x, J, "\u228E", "\\uplus", !0), h(m, x, J, "\u2293", "\\sqcap", !0), h(m, x, J, "\u2217", "\\ast"), h(m, x, J, "\u2294", "\\sqcup", !0), h(m, x, J, "\u25EF", "\\bigcirc", !0), h(m, x, J, "\u2219", "\\bullet", !0), h(m, x, J, "\u2021", "\\ddagger"), h(m, x, J, "\u2240", "\\wr", !0), h(m, x, J, "\u2A3F", "\\amalg"), h(m, x, J, "&", "\\And"), h(m, x, q, "\u27F5", "\\longleftarrow", !0), h(m, x, q, "\u21D0", "\\Leftarrow", !0), h(m, x, q, "\u27F8", "\\Longleftarrow", !0), h(m, x, q, "\u27F6", "\\longrightarrow", !0), h(m, x, q, "\u21D2", "\\Rightarrow", !0), h(m, x, q, "\u27F9", "\\Longrightarrow", !0), h(m, x, q, "\u2194", "\\leftrightarrow", !0), h(m, x, q, "\u27F7", "\\longleftrightarrow", !0), h(m, x, q, "\u21D4", "\\Leftrightarrow", !0), h(m, x, q, "\u27FA", "\\Longleftrightarrow", !0), h(m, x, q, "\u21A6", "\\mapsto", !0), h(m, x, q, "\u27FC", "\\longmapsto", !0), h(m, x, q, "\u2197", "\\nearrow", !0), h(m, x, q, "\u21A9", "\\hookleftarrow", !0), h(m, x, q, "\u21AA", "\\hookrightarrow", !0), h(m, x, q, "\u2198", "\\searrow", !0), h(m, x, q, "\u21BC", "\\leftharpoonup", !0), h(m, x, q, "\u21C0", "\\rightharpoonup", !0), h(m, x, q, "\u2199", "\\swarrow", !0), h(m, x, q, "\u21BD", "\\leftharpoondown", !0), h(m, x, q, "\u21C1", "\\rightharpoondown", !0), h(m, x, q, "\u2196", "\\nwarrow", !0), h(m, x, q, "\u21CC", "\\rightleftharpoons", !0), h(m, C, q, "\u226E", "\\nless", !0), h(m, C, q, "\uE010", "\\@nleqslant"), h(m, C, q, "\uE011", "\\@nleqq"), h(m, C, q, "\u2A87", "\\lneq", !0), h(m, C, q, "\u2268", "\\lneqq", !0), h(m, C, q, "\uE00C", "\\@lvertneqq"), h(m, C, q, "\u22E6", "\\lnsim", !0), h(m, C, q, "\u2A89", "\\lnapprox", !0), h(m, C, q, "\u2280", "\\nprec", !0), h(m, C, q, "\u22E0", "\\npreceq", !0), h(m, C, q, "\u22E8", "\\precnsim", !0), h(m, C, q, "\u2AB9", "\\precnapprox", !0), h(m, C, q, "\u2241", "\\nsim", !0), h(m, C, q, "\uE006", "\\@nshortmid"), h(m, C, q, "\u2224", "\\nmid", !0), h(m, C, q, "\u22AC", "\\nvdash", !0), h(m, C, q, "\u22AD", "\\nvDash", !0), h(m, C, q, "\u22EA", "\\ntriangleleft"), h(m, C, q, "\u22EC", "\\ntrianglelefteq", !0), h(m, C, q, "\u228A", "\\subsetneq", !0), h(m, C, q, "\uE01A", "\\@varsubsetneq"), h(m, C, q, "\u2ACB", "\\subsetneqq", !0), h(m, C, q, "\uE017", "\\@varsubsetneqq"), h(m, C, q, "\u226F", "\\ngtr", !0), h(m, C, q, "\uE00F", "\\@ngeqslant"), h(m, C, q, "\uE00E", "\\@ngeqq"), h(m, C, q, "\u2A88", "\\gneq", !0), h(m, C, q, "\u2269", "\\gneqq", !0), h(m, C, q, "\uE00D", "\\@gvertneqq"), h(m, C, q, "\u22E7", "\\gnsim", !0), h(m, C, q, "\u2A8A", "\\gnapprox", !0), h(m, C, q, "\u2281", "\\nsucc", !0), h(m, C, q, "\u22E1", "\\nsucceq", !0), h(m, C, q, "\u22E9", "\\succnsim", !0), h(m, C, q, "\u2ABA", "\\succnapprox", !0), h(m, C, q, "\u2246", "\\ncong", !0), h(m, C, q, "\uE007", "\\@nshortparallel"), h(m, C, q, "\u2226", "\\nparallel", !0), h(m, C, q, "\u22AF", "\\nVDash", !0), h(m, C, q, "\u22EB", "\\ntriangleright"), h(m, C, q, "\u22ED", "\\ntrianglerighteq", !0), h(m, C, q, "\uE018", "\\@nsupseteqq"), h(m, C, q, "\u228B", "\\supsetneq", !0), h(m, C, q, "\uE01B", "\\@varsupsetneq"), h(m, C, q, "\u2ACC", "\\supsetneqq", !0), h(m, C, q, "\uE019", "\\@varsupsetneqq"), h(m, C, q, "\u22AE", "\\nVdash", !0), h(m, C, q, "\u2AB5", "\\precneqq", !0), h(m, C, q, "\u2AB6", "\\succneqq", !0), h(m, C, q, "\uE016", "\\@nsubseteqq"), h(m, C, J, "\u22B4", "\\unlhd"), h(m, C, J, "\u22B5", "\\unrhd"), h(m, C, q, "\u219A", "\\nleftarrow", !0), h(m, C, q, "\u219B", "\\nrightarrow", !0), h(m, C, q, "\u21CD", "\\nLeftarrow", !0), h(m, C, q, "\u21CF", "\\nRightarrow", !0), h(m, C, q, "\u21AE", "\\nleftrightarrow", !0), h(m, C, q, "\u21CE", "\\nLeftrightarrow", !0), h(m, C, q, "\u25B3", "\\vartriangle"), h(m, C, D, "\u210F", "\\hslash"), h(m, C, D, "\u25BD", "\\triangledown"), h(m, C, D, "\u25CA", "\\lozenge"), h(m, C, D, "\u24C8", "\\circledS"), h(m, C, D, "\xAE", "\\circledR"), h($, C, D, "\xAE", "\\circledR"), h(m, C, D, "\u2221", "\\measuredangle", !0), h(m, C, D, "\u2204", "\\nexists"), h(m, C, D, "\u2127", "\\mho"), h(m, C, D, "\u2132", "\\Finv", !0), h(m, C, D, "\u2141", "\\Game", !0), h(m, C, D, "\u2035", "\\backprime"), h(m, C, D, "\u25B2", "\\blacktriangle"), h(m, C, D, "\u25BC", "\\blacktriangledown"), h(m, C, D, "\u25A0", "\\blacksquare"), h(m, C, D, "\u29EB", "\\blacklozenge"), h(m, C, D, "\u2605", "\\bigstar"), h(m, C, D, "\u2222", "\\sphericalangle", !0), h(m, C, D, "\u2201", "\\complement", !0), h(m, C, D, "\xF0", "\\eth", !0), h($, x, D, "\xF0", "\xF0"), h(m, C, D, "\u2571", "\\diagup"), h(m, C, D, "\u2572", "\\diagdown"), h(m, C, D, "\u25A1", "\\square"), h(m, C, D, "\u25A1", "\\Box"), h(m, C, D, "\u25CA", "\\Diamond"), h(m, C, D, "\xA5", "\\yen", !0), h($, C, D, "\xA5", "\\yen", !0), h(m, C, D, "\u2713", "\\checkmark", !0), h($, C, D, "\u2713", "\\checkmark"), h(m, C, D, "\u2136", "\\beth", !0), h(m, C, D, "\u2138", "\\daleth", !0), h(m, C, D, "\u2137", "\\gimel", !0), h(m, C, D, "\u03DD", "\\digamma", !0), h(m, C, D, "\u03F0", "\\varkappa"), h(m, C, at, "\u250C", "\\@ulcorner", !0), h(m, C, et, "\u2510", "\\@urcorner", !0), h(m, C, at, "\u2514", "\\@llcorner", !0), h(m, C, et, "\u2518", "\\@lrcorner", !0), h(m, C, q, "\u2266", "\\leqq", !0), h(m, C, q, "\u2A7D", "\\leqslant", !0), h(m, C, q, "\u2A95", "\\eqslantless", !0), h(m, C, q, "\u2272", "\\lesssim", !0), h(m, C, q, "\u2A85", "\\lessapprox", !0), h(m, C, q, "\u224A", "\\approxeq", !0), h(m, C, J, "\u22D6", "\\lessdot"), h(m, C, q, "\u22D8", "\\lll", !0), h(m, C, q, "\u2276", "\\lessgtr", !0), h(m, C, q, "\u22DA", "\\lesseqgtr", !0), h(m, C, q, "\u2A8B", "\\lesseqqgtr", !0), h(m, C, q, "\u2251", "\\doteqdot"), h(m, C, q, "\u2253", "\\risingdotseq", !0), h(m, C, q, "\u2252", "\\fallingdotseq", !0), h(m, C, q, "\u223D", "\\backsim", !0), h(m, C, q, "\u22CD", "\\backsimeq", !0), h(m, C, q, "\u2AC5", "\\subseteqq", !0), h(m, C, q, "\u22D0", "\\Subset", !0), h(m, C, q, "\u228F", "\\sqsubset", !0), h(m, C, q, "\u227C", "\\preccurlyeq", !0), h(m, C, q, "\u22DE", "\\curlyeqprec", !0), h(m, C, q, "\u227E", "\\precsim", !0), h(m, C, q, "\u2AB7", "\\precapprox", !0), h(m, C, q, "\u22B2", "\\vartriangleleft"), h(m, C, q, "\u22B4", "\\trianglelefteq"), h(m, C, q, "\u22A8", "\\vDash", !0), h(m, C, q, "\u22AA", "\\Vvdash", !0), h(m, C, q, "\u2323", "\\smallsmile"), h(m, C, q, "\u2322", "\\smallfrown"), h(m, C, q, "\u224F", "\\bumpeq", !0), h(m, C, q, "\u224E", "\\Bumpeq", !0), h(m, C, q, "\u2267", "\\geqq", !0), h(m, C, q, "\u2A7E", "\\geqslant", !0), h(m, C, q, "\u2A96", "\\eqslantgtr", !0), h(m, C, q, "\u2273", "\\gtrsim", !0), h(m, C, q, "\u2A86", "\\gtrapprox", !0), h(m, C, J, "\u22D7", "\\gtrdot"), h(m, C, q, "\u22D9", "\\ggg", !0), h(m, C, q, "\u2277", "\\gtrless", !0), h(m, C, q, "\u22DB", "\\gtreqless", !0), h(m, C, q, "\u2A8C", "\\gtreqqless", !0), h(m, C, q, "\u2256", "\\eqcirc", !0), h(m, C, q, "\u2257", "\\circeq", !0), h(m, C, q, "\u225C", "\\triangleq", !0), h(m, C, q, "\u223C", "\\thicksim"), h(m, C, q, "\u2248", "\\thickapprox"), h(m, C, q, "\u2AC6", "\\supseteqq", !0), h(m, C, q, "\u22D1", "\\Supset", !0), h(m, C, q, "\u2290", "\\sqsupset", !0), h(m, C, q, "\u227D", "\\succcurlyeq", !0), h(m, C, q, "\u22DF", "\\curlyeqsucc", !0), h(m, C, q, "\u227F", "\\succsim", !0), h(m, C, q, "\u2AB8", "\\succapprox", !0), h(m, C, q, "\u22B3", "\\vartriangleright"), h(m, C, q, "\u22B5", "\\trianglerighteq"), h(m, C, q, "\u22A9", "\\Vdash", !0), h(m, C, q, "\u2223", "\\shortmid"), h(m, C, q, "\u2225", "\\shortparallel"), h(m, C, q, "\u226C", "\\between", !0), h(m, C, q, "\u22D4", "\\pitchfork", !0), h(m, C, q, "\u221D", "\\varpropto"), h(m, C, q, "\u25C0", "\\blacktriangleleft"), h(m, C, q, "\u2234", "\\therefore", !0), h(m, C, q, "\u220D", "\\backepsilon"), h(m, C, q, "\u25B6", "\\blacktriangleright"), h(m, C, q, "\u2235", "\\because", !0), h(m, C, q, "\u22D8", "\\llless"), h(m, C, q, "\u22D9", "\\gggtr"), h(m, C, J, "\u22B2", "\\lhd"), h(m, C, J, "\u22B3", "\\rhd"), h(m, C, q, "\u2242", "\\eqsim", !0), h(m, x, q, "\u22C8", "\\Join"), h(m, C, q, "\u2251", "\\Doteq", !0), h(m, C, J, "\u2214", "\\dotplus", !0), h(m, C, J, "\u2216", "\\smallsetminus"), h(m, C, J, "\u22D2", "\\Cap", !0), h(m, C, J, "\u22D3", "\\Cup", !0), h(m, C, J, "\u2A5E", "\\doublebarwedge", !0), h(m, C, J, "\u229F", "\\boxminus", !0), h(m, C, J, "\u229E", "\\boxplus", !0), h(m, C, J, "\u22C7", "\\divideontimes", !0), h(m, C, J, "\u22C9", "\\ltimes", !0), h(m, C, J, "\u22CA", "\\rtimes", !0), h(m, C, J, "\u22CB", "\\leftthreetimes", !0), h(m, C, J, "\u22CC", "\\rightthreetimes", !0), h(m, C, J, "\u22CF", "\\curlywedge", !0), h(m, C, J, "\u22CE", "\\curlyvee", !0), h(m, C, J, "\u229D", "\\circleddash", !0), h(m, C, J, "\u229B", "\\circledast", !0), h(m, C, J, "\u22C5", "\\centerdot"), h(m, C, J, "\u22BA", "\\intercal", !0), h(m, C, J, "\u22D2", "\\doublecap"), h(m, C, J, "\u22D3", "\\doublecup"), h(m, C, J, "\u22A0", "\\boxtimes", !0), h(m, C, q, "\u21E2", "\\dashrightarrow", !0), h(m, C, q, "\u21E0", "\\dashleftarrow", !0), h(m, C, q, "\u21C7", "\\leftleftarrows", !0), h(m, C, q, "\u21C6", "\\leftrightarrows", !0), h(m, C, q, "\u21DA", "\\Lleftarrow", !0), h(m, C, q, "\u219E", "\\twoheadleftarrow", !0), h(m, C, q, "\u21A2", "\\leftarrowtail", !0), h(m, C, q, "\u21AB", "\\looparrowleft", !0), h(m, C, q, "\u21CB", "\\leftrightharpoons", !0), h(m, C, q, "\u21B6", "\\curvearrowleft", !0), h(m, C, q, "\u21BA", "\\circlearrowleft", !0), h(m, C, q, "\u21B0", "\\Lsh", !0), h(m, C, q, "\u21C8", "\\upuparrows", !0), h(m, C, q, "\u21BF", "\\upharpoonleft", !0), h(m, C, q, "\u21C3", "\\downharpoonleft", !0), h(m, x, q, "\u22B6", "\\origof", !0), h(m, x, q, "\u22B7", "\\imageof", !0), h(m, C, q, "\u22B8", "\\multimap", !0), h(m, C, q, "\u21AD", "\\leftrightsquigarrow", !0), h(m, C, q, "\u21C9", "\\rightrightarrows", !0), h(m, C, q, "\u21C4", "\\rightleftarrows", !0), h(m, C, q, "\u21A0", "\\twoheadrightarrow", !0), h(m, C, q, "\u21A3", "\\rightarrowtail", !0), h(m, C, q, "\u21AC", "\\looparrowright", !0), h(m, C, q, "\u21B7", "\\curvearrowright", !0), h(m, C, q, "\u21BB", "\\circlearrowright", !0), h(m, C, q, "\u21B1", "\\Rsh", !0), h(m, C, q, "\u21CA", "\\downdownarrows", !0), h(m, C, q, "\u21BE", "\\upharpoonright", !0), h(m, C, q, "\u21C2", "\\downharpoonright", !0), h(m, C, q, "\u21DD", "\\rightsquigarrow", !0), h(m, C, q, "\u21DD", "\\leadsto"), h(m, C, q, "\u21DB", "\\Rrightarrow", !0), h(m, C, q, "\u21BE", "\\restriction"), h(m, x, D, "\u2018", "`"), h(m, x, D, "$", "\\$"), h($, x, D, "$", "\\$"), h($, x, D, "$", "\\textdollar"), h(m, x, D, "%", "\\%"), h($, x, D, "%", "\\%"), h(m, x, D, "_", "\\_"), h($, x, D, "_", "\\_"), h($, x, D, "_", "\\textunderscore"), h(m, x, D, "\u2220", "\\angle", !0), h(m, x, D, "\u221E", "\\infty", !0), h(m, x, D, "\u2032", "\\prime"), h(m, x, D, "\u25B3", "\\triangle"), h(m, x, D, "\u0393", "\\Gamma", !0), h(m, x, D, "\u0394", "\\Delta", !0), h(m, x, D, "\u0398", "\\Theta", !0), h(m, x, D, "\u039B", "\\Lambda", !0), h(m, x, D, "\u039E", "\\Xi", !0), h(m, x, D, "\u03A0", "\\Pi", !0), h(m, x, D, "\u03A3", "\\Sigma", !0), h(m, x, D, "\u03A5", "\\Upsilon", !0), h(m, x, D, "\u03A6", "\\Phi", !0), h(m, x, D, "\u03A8", "\\Psi", !0), h(m, x, D, "\u03A9", "\\Omega", !0), h(m, x, D, "A", "\u0391"), h(m, x, D, "B", "\u0392"), h(m, x, D, "E", "\u0395"), h(m, x, D, "Z", "\u0396"), h(m, x, D, "H", "\u0397"), h(m, x, D, "I", "\u0399"), h(m, x, D, "K", "\u039A"), h(m, x, D, "M", "\u039C"), h(m, x, D, "N", "\u039D"), h(m, x, D, "O", "\u039F"), h(m, x, D, "P", "\u03A1"), h(m, x, D, "T", "\u03A4"), h(m, x, D, "X", "\u03A7"), h(m, x, D, "\xAC", "\\neg", !0), h(m, x, D, "\xAC", "\\lnot"), h(m, x, D, "\u22A4", "\\top"), h(m, x, D, "\u22A5", "\\bot"), h(m, x, D, "\u2205", "\\emptyset"), h(m, C, D, "\u2205", "\\varnothing"), h(m, x, se, "\u03B1", "\\alpha", !0), h(m, x, se, "\u03B2", "\\beta", !0), h(m, x, se, "\u03B3", "\\gamma", !0), h(m, x, se, "\u03B4", "\\delta", !0), h(m, x, se, "\u03F5", "\\epsilon", !0), h(m, x, se, "\u03B6", "\\zeta", !0), h(m, x, se, "\u03B7", "\\eta", !0), h(m, x, se, "\u03B8", "\\theta", !0), h(m, x, se, "\u03B9", "\\iota", !0), h(m, x, se, "\u03BA", "\\kappa", !0), h(m, x, se, "\u03BB", "\\lambda", !0), h(m, x, se, "\u03BC", "\\mu", !0), h(m, x, se, "\u03BD", "\\nu", !0), h(m, x, se, "\u03BE", "\\xi", !0), h(m, x, se, "\u03BF", "\\omicron", !0), h(m, x, se, "\u03C0", "\\pi", !0), h(m, x, se, "\u03C1", "\\rho", !0), h(m, x, se, "\u03C3", "\\sigma", !0), h(m, x, se, "\u03C4", "\\tau", !0), h(m, x, se, "\u03C5", "\\upsilon", !0), h(m, x, se, "\u03D5", "\\phi", !0), h(m, x, se, "\u03C7", "\\chi", !0), h(m, x, se, "\u03C8", "\\psi", !0), h(m, x, se, "\u03C9", "\\omega", !0), h(m, x, se, "\u03B5", "\\varepsilon", !0), h(m, x, se, "\u03D1", "\\vartheta", !0), h(m, x, se, "\u03D6", "\\varpi", !0), h(m, x, se, "\u03F1", "\\varrho", !0), h(m, x, se, "\u03C2", "\\varsigma", !0), h(m, x, se, "\u03C6", "\\varphi", !0), h(m, x, J, "\u2217", "*", !0), h(m, x, J, "+", "+"), h(m, x, J, "\u2212", "-", !0), h(m, x, J, "\u22C5", "\\cdot", !0), h(m, x, J, "\u2218", "\\circ", !0), h(m, x, J, "\xF7", "\\div", !0), h(m, x, J, "\xB1", "\\pm", !0), h(m, x, J, "\xD7", "\\times", !0), h(m, x, J, "\u2229", "\\cap", !0), h(m, x, J, "\u222A", "\\cup", !0), h(m, x, J, "\u2216", "\\setminus", !0), h(m, x, J, "\u2227", "\\land"), h(m, x, J, "\u2228", "\\lor"), h(m, x, J, "\u2227", "\\wedge", !0), h(m, x, J, "\u2228", "\\vee", !0), h(m, x, D, "\u221A", "\\surd"), h(m, x, at, "\u27E8", "\\langle", !0), h(m, x, at, "\u2223", "\\lvert"), h(m, x, at, "\u2225", "\\lVert"), h(m, x, et, "?", "?"), h(m, x, et, "!", "!"), h(m, x, et, "\u27E9", "\\rangle", !0), h(m, x, et, "\u2223", "\\rvert"), h(m, x, et, "\u2225", "\\rVert"), h(m, x, q, "=", "="), h(m, x, q, ":", ":"), h(m, x, q, "\u2248", "\\approx", !0), h(m, x, q, "\u2245", "\\cong", !0), h(m, x, q, "\u2265", "\\ge"), h(m, x, q, "\u2265", "\\geq", !0), h(m, x, q, "\u2190", "\\gets"), h(m, x, q, ">", "\\gt", !0), h(m, x, q, "\u2208", "\\in", !0), h(m, x, q, "\uE020", "\\@not"), h(m, x, q, "\u2282", "\\subset", !0), h(m, x, q, "\u2283", "\\supset", !0), h(m, x, q, "\u2286", "\\subseteq", !0), h(m, x, q, "\u2287", "\\supseteq", !0), h(m, C, q, "\u2288", "\\nsubseteq", !0), h(m, C, q, "\u2289", "\\nsupseteq", !0), h(m, x, q, "\u22A8", "\\models"), h(m, x, q, "\u2190", "\\leftarrow", !0), h(m, x, q, "\u2264", "\\le"), h(m, x, q, "\u2264", "\\leq", !0), h(m, x, q, "<", "\\lt", !0), h(m, x, q, "\u2192", "\\rightarrow", !0), h(m, x, q, "\u2192", "\\to"), h(m, C, q, "\u2271", "\\ngeq", !0), h(m, C, q, "\u2270", "\\nleq", !0), h(m, x, Dt, "\xA0", "\\ "), h(m, x, Dt, "\xA0", "\\space"), h(m, x, Dt, "\xA0", "\\nobreakspace"), h($, x, Dt, "\xA0", "\\ "), h($, x, Dt, "\xA0", " "), h($, x, Dt, "\xA0", "\\space"), h($, x, Dt, "\xA0", "\\nobreakspace"), h(m, x, Dt, null, "\\nobreak"), h(m, x, Dt, null, "\\allowbreak"), h(m, x, Vr, ",", ","), h(m, x, Vr, ";", ";"), h(m, C, J, "\u22BC", "\\barwedge", !0), h(m, C, J, "\u22BB", "\\veebar", !0), h(m, x, J, "\u2299", "\\odot", !0), h(m, x, J, "\u2295", "\\oplus", !0), h(m, x, J, "\u2297", "\\otimes", !0), h(m, x, D, "\u2202", "\\partial", !0), h(m, x, J, "\u2298", "\\oslash", !0), h(m, C, J, "\u229A", "\\circledcirc", !0), h(m, C, J, "\u22A1", "\\boxdot", !0), h(m, x, J, "\u25B3", "\\bigtriangleup"), h(m, x, J, "\u25BD", "\\bigtriangledown"), h(m, x, J, "\u2020", "\\dagger"), h(m, x, J, "\u22C4", "\\diamond"), h(m, x, J, "\u22C6", "\\star"), h(m, x, J, "\u25C3", "\\triangleleft"), h(m, x, J, "\u25B9", "\\triangleright"), h(m, x, at, "{", "\\{"), h($, x, D, "{", "\\{"), h($, x, D, "{", "\\textbraceleft"), h(m, x, et, "}", "\\}"), h($, x, D, "}", "\\}"), h($, x, D, "}", "\\textbraceright"), h(m, x, at, "{", "\\lbrace"), h(m, x, et, "}", "\\rbrace"), h(m, x, at, "[", "\\lbrack", !0), h($, x, D, "[", "\\lbrack", !0), h(m, x, et, "]", "\\rbrack", !0), h($, x, D, "]", "\\rbrack", !0), h(m, x, at, "(", "\\lparen", !0), h(m, x, et, ")", "\\rparen", !0), h($, x, D, "<", "\\textless", !0), h($, x, D, ">", "\\textgreater", !0), h(m, x, at, "\u230A", "\\lfloor", !0), h(m, x, et, "\u230B", "\\rfloor", !0), h(m, x, at, "\u2308", "\\lceil", !0), h(m, x, et, "\u2309", "\\rceil", !0), h(m, x, D, "\\", "\\backslash"), h(m, x, D, "\u2223", "|"), h(m, x, D, "\u2223", "\\vert"), h($, x, D, "|", "\\textbar", !0), h(m, x, D, "\u2225", "\\|"), h(m, x, D, "\u2225", "\\Vert"), h($, x, D, "\u2225", "\\textbardbl"), h($, x, D, "~", "\\textasciitilde"), h($, x, D, "\\", "\\textbackslash"), h($, x, D, "^", "\\textasciicircum"), h(m, x, q, "\u2191", "\\uparrow", !0), h(m, x, q, "\u21D1", "\\Uparrow", !0), h(m, x, q, "\u2193", "\\downarrow", !0), h(m, x, q, "\u21D3", "\\Downarrow", !0), h(m, x, q, "\u2195", "\\updownarrow", !0), h(m, x, q, "\u21D5", "\\Updownarrow", !0), h(m, x, We, "\u2210", "\\coprod"), h(m, x, We, "\u22C1", "\\bigvee"), h(m, x, We, "\u22C0", "\\bigwedge"), h(m, x, We, "\u2A04", "\\biguplus"), h(m, x, We, "\u22C2", "\\bigcap"), h(m, x, We, "\u22C3", "\\bigcup"), h(m, x, We, "\u222B", "\\int"), h(m, x, We, "\u222B", "\\intop"), h(m, x, We, "\u222C", "\\iint"), h(m, x, We, "\u222D", "\\iiint"), h(m, x, We, "\u220F", "\\prod"), h(m, x, We, "\u2211", "\\sum"), h(m, x, We, "\u2A02", "\\bigotimes"), h(m, x, We, "\u2A01", "\\bigoplus"), h(m, x, We, "\u2A00", "\\bigodot"), h(m, x, We, "\u222E", "\\oint"), h(m, x, We, "\u222F", "\\oiint"), h(m, x, We, "\u2230", "\\oiiint"), h(m, x, We, "\u2A06", "\\bigsqcup"), h(m, x, We, "\u222B", "\\smallint"), h($, x, sr, "\u2026", "\\textellipsis"), h(m, x, sr, "\u2026", "\\mathellipsis"), h($, x, sr, "\u2026", "\\ldots", !0), h(m, x, sr, "\u2026", "\\ldots", !0), h(m, x, sr, "\u22EF", "\\@cdots", !0), h(m, x, sr, "\u22F1", "\\ddots", !0), h(m, x, D, "\u22EE", "\\varvdots"), h(m, x, Be, "\u02CA", "\\acute"), h(m, x, Be, "\u02CB", "\\grave"), h(m, x, Be, "\xA8", "\\ddot"), h(m, x, Be, "~", "\\tilde"), h(m, x, Be, "\u02C9", "\\bar"), h(m, x, Be, "\u02D8", "\\breve"), h(m, x, Be, "\u02C7", "\\check"), h(m, x, Be, "^", "\\hat"), h(m, x, Be, "\u20D7", "\\vec"), h(m, x, Be, "\u02D9", "\\dot"), h(m, x, Be, "\u02DA", "\\mathring"), h(m, x, se, "\uE131", "\\@imath"), h(m, x, se, "\uE237", "\\@jmath"), h(m, x, D, "\u0131", "\u0131"), h(m, x, D, "\u0237", "\u0237"), h($, x, D, "\u0131", "\\i", !0), h($, x, D, "\u0237", "\\j", !0), h($, x, D, "\xDF", "\\ss", !0), h($, x, D, "\xE6", "\\ae", !0), h($, x, D, "\u0153", "\\oe", !0), h($, x, D, "\xF8", "\\o", !0), h($, x, D, "\xC6", "\\AE", !0), h($, x, D, "\u0152", "\\OE", !0), h($, x, D, "\xD8", "\\O", !0), h($, x, Be, "\u02CA", "\\'"), h($, x, Be, "\u02CB", "\\`"), h($, x, Be, "\u02C6", "\\^"), h($, x, Be, "\u02DC", "\\~"), h($, x, Be, "\u02C9", "\\="), h($, x, Be, "\u02D8", "\\u"), h($, x, Be, "\u02D9", "\\."), h($, x, Be, "\xB8", "\\c"), h($, x, Be, "\u02DA", "\\r"), h($, x, Be, "\u02C7", "\\v"), h($, x, Be, "\xA8", '\\"'), h($, x, Be, "\u02DD", "\\H"), h($, x, Be, "\u25EF", "\\textcircled");
-            let Ii = {
+            let Hi = {
                 "--": !0,
                 "---": !0,
                 "``": !0,
                 "''": !0
             };
             h($, x, D, "\u2013", "--", !0), h($, x, D, "\u2013", "\\textendash"), h($, x, D, "\u2014", "---", !0), h($, x, D, "\u2014", "\\textemdash"), h($, x, D, "\u2018", "`", !0), h($, x, D, "\u2018", "\\textquoteleft"), h($, x, D, "\u2019", "'", !0), h($, x, D, "\u2019", "\\textquoteright"), h($, x, D, "\u201C", "``", !0), h($, x, D, "\u201C", "\\textquotedblleft"), h($, x, D, "\u201D", "''", !0), h($, x, D, "\u201D", "\\textquotedblright"), h(m, x, D, "\xB0", "\\degree", !0), h($, x, D, "\xB0", "\\degree"), h($, x, D, "\xB0", "\\textdegree", !0), h(m, x, D, "\xA3", "\\pounds"), h(m, x, D, "\xA3", "\\mathsterling", !0), h($, x, D, "\xA3", "\\pounds"), h($, x, D, "\xA3", "\\textsterling", !0), h(m, C, D, "\u2720", "\\maltese"), h($, C, D, "\u2720", "\\maltese");
-            let Oi = '0123456789/@."';
-            for (let n = 0; n < Oi.length; n++) {
-                let t = Oi.charAt(n);
+            let $i = '0123456789/@."';
+            for (let n = 0; n < $i.length; n++) {
+                let t = $i.charAt(n);
                 h(m, x, D, t, t)
             }
-            let Hi = '0123456789!@*()-=+";:?/.,';
-            for (let n = 0; n < Hi.length; n++) {
-                let t = Hi.charAt(n);
+            let Gi = '0123456789!@*()-=+";:?/.,';
+            for (let n = 0; n < Gi.length; n++) {
+                let t = Gi.charAt(n);
                 h($, x, D, t, t)
             }
             let jr = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz";
             for (let n = 0; n < jr.length; n++) {
                 let t = jr.charAt(n);
                 h(m, x, se, t, t), h($, x, D, t, t)
             }
@@ -9037,17 +9037,17 @@
                 le = String.fromCharCode(55349, 56320 + n), h(m, x, se, t, le), h($, x, D, t, le), le = String.fromCharCode(55349, 56372 + n), h(m, x, se, t, le), h($, x, D, t, le), le = String.fromCharCode(55349, 56424 + n), h(m, x, se, t, le), h($, x, D, t, le), le = String.fromCharCode(55349, 56580 + n), h(m, x, se, t, le), h($, x, D, t, le), le = String.fromCharCode(55349, 56684 + n), h(m, x, se, t, le), h($, x, D, t, le), le = String.fromCharCode(55349, 56736 + n), h(m, x, se, t, le), h($, x, D, t, le), le = String.fromCharCode(55349, 56788 + n), h(m, x, se, t, le), h($, x, D, t, le), le = String.fromCharCode(55349, 56840 + n), h(m, x, se, t, le), h($, x, D, t, le), le = String.fromCharCode(55349, 56944 + n), h(m, x, se, t, le), h($, x, D, t, le), n < 26 && (le = String.fromCharCode(55349, 56632 + n), h(m, x, se, t, le), h($, x, D, t, le), le = String.fromCharCode(55349, 56476 + n), h(m, x, se, t, le), h($, x, D, t, le))
             }
             le = "\u{1D55C}", h(m, x, se, "k", le), h($, x, D, "k", le);
             for (let n = 0; n < 10; n++) {
                 let t = n.toString();
                 le = String.fromCharCode(55349, 57294 + n), h(m, x, se, t, le), h($, x, D, t, le), le = String.fromCharCode(55349, 57314 + n), h(m, x, se, t, le), h($, x, D, t, le), le = String.fromCharCode(55349, 57324 + n), h(m, x, se, t, le), h($, x, D, t, le), le = String.fromCharCode(55349, 57334 + n), h(m, x, se, t, le), h($, x, D, t, le)
             }
-            let Z0 = "\xD0\xDE\xFE";
-            for (let n = 0; n < Z0.length; n++) {
-                let t = Z0.charAt(n);
+            let Q0 = "\xD0\xDE\xFE";
+            for (let n = 0; n < Q0.length; n++) {
+                let t = Q0.charAt(n);
                 h(m, x, se, t, t), h($, x, D, t, t)
             }
             let Ur = [
                     ["mathbf", "textbf", "Main-Bold"],
                     ["mathbf", "textbf", "Main-Bold"],
                     ["mathnormal", "textit", "Math-Italic"],
                     ["mathnormal", "textit", "Math-Italic"],
@@ -9070,42 +9070,42 @@
                     ["mathitsf", "textitsf", "SansSerif-Italic"],
                     ["mathitsf", "textitsf", "SansSerif-Italic"],
                     ["", "", ""],
                     ["", "", ""],
                     ["mathtt", "texttt", "Typewriter-Regular"],
                     ["mathtt", "texttt", "Typewriter-Regular"]
                 ],
-                $i = [
+                Vi = [
                     ["mathbf", "textbf", "Main-Bold"],
                     ["", "", ""],
                     ["mathsf", "textsf", "SansSerif-Regular"],
                     ["mathboldsf", "textboldsf", "SansSerif-Bold"],
                     ["mathtt", "texttt", "Typewriter-Regular"]
                 ],
-                Wu = function(n, t) {
+                Zu = function(n, t) {
                     let o = n.charCodeAt(0),
                         s = n.charCodeAt(1),
                         u = (o - 55296) * 1024 + (s - 56320) + 65536,
                         p = t === "math" ? 0 : 1;
                     if (119808 <= u && u < 120484) {
                         let b = Math.floor((u - 119808) / 26);
                         return [Ur[b][2], Ur[b][p]]
                     } else if (120782 <= u && u <= 120831) {
                         let b = Math.floor((u - 120782) / 10);
-                        return [$i[b][2], $i[b][p]]
+                        return [Vi[b][2], Vi[b][p]]
                     } else {
                         if (u === 120485 || u === 120486) return [Ur[0][2], Ur[0][p]];
                         if (120486 < u && u < 120782) return ["", ""];
                         throw new a("Unsupported character: " + n)
                     }
                 },
                 Wr = function(n, t, o) {
                     return Oe[o][n] && Oe[o][n].replace && (n = Oe[o][n].replace), {
                         value: n,
-                        metrics: V0(n, t, o)
+                        metrics: j0(n, t, o)
                     }
                 },
                 yt = function(n, t, o, s, u) {
                     let p = Wr(n, t, o),
                         b = p.metrics;
                     n = p.value;
                     let v;
@@ -9116,46 +9116,46 @@
                     if (s) {
                         v.maxFontSize = s.sizeMultiplier, s.style.isTight() && v.classes.push("mtight");
                         let S = s.getColor();
                         S && (v.style.color = S)
                     }
                     return v
                 },
-                Yu = function(n, t, o, s) {
+                Qu = function(n, t, o, s) {
                     return s === void 0 && (s = []), o.font === "boldsymbol" && Wr(n, "Main-Bold", t).metrics ? yt(n, "Main-Bold", t, o, s.concat(["mathbf"])) : n === "\\" || Oe[t][n].font === "main" ? yt(n, "Main-Regular", t, o, s) : yt(n, "AMS-Regular", t, o, s.concat(["amsrm"]))
                 },
-                Zu = function(n, t, o, s, u) {
+                Xu = function(n, t, o, s, u) {
                     return u !== "textord" && Wr(n, "Math-BoldItalic", t).metrics ? {
                         fontName: "Math-BoldItalic",
                         fontClass: "boldsymbol"
                     } : {
                         fontName: "Main-Bold",
                         fontClass: "mathbf"
                     }
                 },
-                Qu = function(n, t, o) {
+                Ju = function(n, t, o) {
                     let s = n.mode,
                         u = n.text,
                         p = ["mord"],
                         b = s === "math" || s === "text" && t.font,
                         v = b ? t.font : t.fontFamily,
                         S = "",
                         E = "";
-                    if (u.charCodeAt(0) === 55349 && ([S, E] = Wu(u, s)), S.length > 0) return yt(u, S, s, t, p.concat(E));
+                    if (u.charCodeAt(0) === 55349 && ([S, E] = Zu(u, s)), S.length > 0) return yt(u, S, s, t, p.concat(E));
                     if (v) {
                         let z, F;
                         if (v === "boldsymbol") {
-                            let N = Zu(u, s, t, p, o);
+                            let N = Xu(u, s, t, p, o);
                             z = N.fontName, F = [N.fontClass]
-                        } else b ? (z = ji[v].fontName, F = [v]) : (z = Yr(v, t.fontWeight, t.fontShape), F = [v, t.fontWeight, t.fontShape]);
+                        } else b ? (z = Wi[v].fontName, F = [v]) : (z = Yr(v, t.fontWeight, t.fontShape), F = [v, t.fontWeight, t.fontShape]);
                         if (Wr(u, z, s).metrics) return yt(u, z, s, t, p.concat(F));
-                        if (Ii.hasOwnProperty(u) && z.slice(0, 10) === "Typewriter") {
+                        if (Hi.hasOwnProperty(u) && z.slice(0, 10) === "Typewriter") {
                             let N = [];
                             for (let H = 0; H < u.length; H++) N.push(yt(u[H], z, s, t, p.concat(F)));
-                            return Vi(N)
+                            return Ui(N)
                         }
                     }
                     if (o === "mathord") return yt(u, "Math-Italic", s, t, p.concat(["mathnormal"]));
                     if (o === "textord") {
                         let z = Oe[s][u] && Oe[s][u].font;
                         if (z === "ams") {
                             let F = Yr("amsrm", t.fontWeight, t.fontShape);
@@ -9165,65 +9165,65 @@
                             return yt(u, F, s, t, p.concat(t.fontWeight, t.fontShape))
                         } else {
                             let F = Yr(z, t.fontWeight, t.fontShape);
                             return yt(u, F, s, t, p.concat(F, t.fontWeight, t.fontShape))
                         }
                     } else throw new Error("unexpected type: " + o + " in makeOrd")
                 },
-                Xu = (n, t) => {
+                Ku = (n, t) => {
                     if (It(n.classes) !== It(t.classes) || n.skew !== t.skew || n.maxFontSize !== t.maxFontSize) return !1;
                     if (n.classes.length === 1) {
                         let o = n.classes[0];
                         if (o === "mbin" || o === "mord") return !1
                     }
                     for (let o in n.style)
                         if (n.style.hasOwnProperty(o) && n.style[o] !== t.style[o]) return !1;
                     for (let o in t.style)
                         if (t.style.hasOwnProperty(o) && n.style[o] !== t.style[o]) return !1;
                     return !0
                 },
-                Ju = n => {
+                e1 = n => {
                     for (let t = 0; t < n.length - 1; t++) {
                         let o = n[t],
                             s = n[t + 1];
-                        o instanceof ut && s instanceof ut && Xu(o, s) && (o.text += s.text, o.height = Math.max(o.height, s.height), o.depth = Math.max(o.depth, s.depth), o.italic = s.italic, n.splice(t + 1, 1), t--)
+                        o instanceof ut && s instanceof ut && Ku(o, s) && (o.text += s.text, o.height = Math.max(o.height, s.height), o.depth = Math.max(o.depth, s.depth), o.italic = s.italic, n.splice(t + 1, 1), t--)
                     }
                     return n
                 },
-                Q0 = function(n) {
+                X0 = function(n) {
                     let t = 0,
                         o = 0,
                         s = 0;
                     for (let u = 0; u < n.children.length; u++) {
                         let p = n.children[u];
                         p.height > t && (t = p.height), p.depth > o && (o = p.depth), p.maxFontSize > s && (s = p.maxFontSize)
                     }
                     n.height = t, n.depth = o, n.maxFontSize = s
                 },
                 nt = function(n, t, o, s) {
                     let u = new vr(n, t, o, s);
-                    return Q0(u), u
+                    return X0(u), u
                 },
-                Gi = (n, t, o, s) => new vr(n, t, o, s),
-                Ku = function(n, t, o) {
+                ji = (n, t, o, s) => new vr(n, t, o, s),
+                t1 = function(n, t, o) {
                     let s = nt([n], [], t);
                     return s.height = Math.max(o || t.fontMetrics().defaultRuleThickness, t.minRuleThickness), s.style.borderBottomWidth = Z(s.height), s.maxFontSize = 1, s
                 },
-                e1 = function(n, t, o, s) {
-                    let u = new W0(n, t, o, s);
-                    return Q0(u), u
+                r1 = function(n, t, o, s) {
+                    let u = new Y0(n, t, o, s);
+                    return X0(u), u
                 },
-                Vi = function(n) {
+                Ui = function(n) {
                     let t = new xr(n);
-                    return Q0(t), t
+                    return X0(t), t
                 },
-                t1 = function(n, t) {
+                n1 = function(n, t) {
                     return n instanceof xr ? nt([], [n], t) : n
                 },
-                r1 = function(n) {
+                i1 = function(n) {
                     if (n.positionType === "individualShift") {
                         let o = n.children,
                             s = [o[0]],
                             u = -o[0].shift - o[0].elem.depth,
                             p = u;
                         for (let b = 1; b < o.length; b++) {
                             let v = -o[b].shift - p - o[b].elem.depth,
@@ -9255,19 +9255,19 @@
                         else throw new Error("Invalid positionType " + n.positionType + ".")
                     }
                     return {
                         children: n.children,
                         depth: t
                     }
                 },
-                n1 = function(n, t) {
+                o1 = function(n, t) {
                     let {
                         children: o,
                         depth: s
-                    } = r1(n), u = 0;
+                    } = i1(n), u = 0;
                     for (let H = 0; H < o.length; H++) {
                         let K = o[H];
                         if (K.type === "elem") {
                             let ie = K.elem;
                             u = Math.max(u, ie.maxFontSize, ie.height)
                         }
                     }
@@ -9299,15 +9299,15 @@
                         K.style.height = Z(-v);
                         let ie = nt(["vlist-s"], [new ut("\u200B")]);
                         F = [nt(["vlist-r"], [z, ie]), nt(["vlist-r"], [K])]
                     } else F = [nt(["vlist-r"], [z])];
                     let N = nt(["vlist-t"], F);
                     return F.length === 2 && N.classes.push("vlist-t2"), N.height = S, N.depth = -v, N
                 },
-                i1 = (n, t) => {
+                a1 = (n, t) => {
                     let o = nt(["mspace"], [], t),
                         s = Ie(n, t);
                     return o.style.marginRight = Z(s), o
                 },
                 Yr = function(n, t, o) {
                     let s = "";
                     switch (n) {
@@ -9325,15 +9325,15 @@
                             break;
                         default:
                             s = n
                     }
                     let u;
                     return t === "textbf" && o === "textit" ? u = "BoldItalic" : t === "textbf" ? u = "Bold" : t === "textit" ? u = "Italic" : u = "Regular", s + "-" + u
                 },
-                ji = {
+                Wi = {
                     mathbf: {
                         variant: "bold",
                         fontName: "Main-Bold"
                     },
                     mathrm: {
                         variant: "normal",
                         fontName: "Main-Regular"
@@ -9371,60 +9371,60 @@
                         fontName: "SansSerif-Regular"
                     },
                     mathtt: {
                         variant: "monospace",
                         fontName: "Typewriter-Regular"
                     }
                 },
-                Ui = {
+                Yi = {
                     vec: ["vec", .471, .714],
                     oiintSize1: ["oiintSize1", .957, .499],
                     oiintSize2: ["oiintSize2", 1.472, .659],
                     oiiintSize1: ["oiiintSize1", 1.304, .499],
                     oiiintSize2: ["oiiintSize2", 1.98, .659]
                 };
             var B = {
-                fontMap: ji,
+                fontMap: Wi,
                 makeSymbol: yt,
-                mathsym: Yu,
+                mathsym: Qu,
                 makeSpan: nt,
-                makeSvgSpan: Gi,
-                makeLineSpan: Ku,
-                makeAnchor: e1,
-                makeFragment: Vi,
-                wrapFragment: t1,
-                makeVList: n1,
-                makeOrd: Qu,
-                makeGlue: i1,
+                makeSvgSpan: ji,
+                makeLineSpan: t1,
+                makeAnchor: r1,
+                makeFragment: Ui,
+                wrapFragment: n1,
+                makeVList: o1,
+                makeOrd: Ju,
+                makeGlue: a1,
                 staticSvg: function(n, t) {
-                    let [o, s, u] = Ui[n], p = new Ot(o), b = new Et([p], {
+                    let [o, s, u] = Yi[n], p = new Ot(o), b = new Et([p], {
                         width: Z(s),
                         height: Z(u),
                         style: "width:" + Z(s),
                         viewBox: "0 0 " + 1e3 * s + " " + 1e3 * u,
                         preserveAspectRatio: "xMinYMin"
-                    }), v = Gi(["overlay"], [b], t);
+                    }), v = ji(["overlay"], [b], t);
                     return v.height = u, v.style.height = Z(u), v.style.width = Z(s), v
                 },
-                svgData: Ui,
-                tryCombineChars: Ju
+                svgData: Yi,
+                tryCombineChars: e1
             };
             let He = {
                     number: 3,
                     unit: "mu"
                 },
                 Jt = {
                     number: 4,
                     unit: "mu"
                 },
                 zt = {
                     number: 5,
                     unit: "mu"
                 },
-                o1 = {
+                s1 = {
                     mord: {
                         mop: He,
                         mbin: Jt,
                         mrel: zt,
                         minner: He
                     },
                     mop: {
@@ -9467,15 +9467,15 @@
                         mbin: Jt,
                         mrel: zt,
                         mopen: He,
                         mpunct: He,
                         minner: He
                     }
                 },
-                a1 = {
+                l1 = {
                     mord: {
                         mop: He
                     },
                     mop: {
                         mord: He,
                         mop: He
                     },
@@ -9486,15 +9486,15 @@
                         mop: He
                     },
                     mpunct: {},
                     minner: {
                         mop: He
                     }
                 },
-                Wi = {},
+                Zi = {},
                 Zr = {},
                 Qr = {};
 
             function Q(n) {
                 let {
                     type: t,
                     names: o,
@@ -9510,15 +9510,15 @@
                     allowedInText: !!s.allowedInText,
                     allowedInMath: s.allowedInMath === void 0 ? !0 : s.allowedInMath,
                     numOptionalArgs: s.numOptionalArgs || 0,
                     infix: !!s.infix,
                     primitive: !!s.primitive,
                     handler: u
                 };
-                for (let S = 0; S < o.length; ++S) Wi[o[S]] = v;
+                for (let S = 0; S < o.length; ++S) Zi[o[S]] = v;
                 t && (p && (Zr[t] = p), b && (Qr[t] = b))
             }
 
             function Kt(n) {
                 let {
                     type: t,
                     htmlBuilder: o,
@@ -9540,23 +9540,23 @@
             let Xr = function(n) {
                     return n.type === "ordgroup" && n.body.length === 1 ? n.body[0] : n
                 },
                 je = function(n) {
                     return n.type === "ordgroup" ? n.body : [n]
                 },
                 Rt = B.makeSpan,
-                s1 = ["leftmost", "mbin", "mopen", "mrel", "mop", "mpunct"],
-                l1 = ["rightmost", "mrel", "mclose", "mpunct"],
-                c1 = {
+                c1 = ["leftmost", "mbin", "mopen", "mrel", "mop", "mpunct"],
+                u1 = ["rightmost", "mrel", "mclose", "mpunct"],
+                h1 = {
                     display: G.DISPLAY,
                     text: G.TEXT,
                     script: G.SCRIPT,
                     scriptscript: G.SCRIPTSCRIPT
                 },
-                u1 = {
+                d1 = {
                     mord: "mord",
                     mop: "mop",
                     mbin: "mbin",
                     mrel: "mrel",
                     mopen: "mopen",
                     mclose: "mclose",
                     mpunct: "mpunct",
@@ -9572,71 +9572,71 @@
                             u.push(...F)
                         } else u.push(z)
                     }
                     if (B.tryCombineChars(u), !o) return u;
                     let p = t;
                     if (n.length === 1) {
                         let E = n[0];
-                        E.type === "sizing" ? p = t.havingSize(E.size) : E.type === "styling" && (p = t.havingStyle(c1[E.style]))
+                        E.type === "sizing" ? p = t.havingSize(E.size) : E.type === "styling" && (p = t.havingStyle(h1[E.style]))
                     }
                     let b = Rt([s[0] || "leftmost"], [], t),
                         v = Rt([s[1] || "rightmost"], [], t),
                         S = o === "root";
-                    return X0(u, (E, z) => {
+                    return J0(u, (E, z) => {
                         let F = z.classes[0],
                             N = E.classes[0];
-                        F === "mbin" && R.contains(l1, N) ? z.classes[0] = "mord" : N === "mbin" && R.contains(s1, F) && (E.classes[0] = "mord")
+                        F === "mbin" && R.contains(u1, N) ? z.classes[0] = "mord" : N === "mbin" && R.contains(c1, F) && (E.classes[0] = "mord")
                     }, {
                         node: b
-                    }, v, S), X0(u, (E, z) => {
-                        let F = K0(z),
-                            N = K0(E),
-                            H = F && N ? E.hasClass("mtight") ? a1[F][N] : o1[F][N] : null;
+                    }, v, S), J0(u, (E, z) => {
+                        let F = en(z),
+                            N = en(E),
+                            H = F && N ? E.hasClass("mtight") ? l1[F][N] : s1[F][N] : null;
                         if (H) return B.makeGlue(H, p)
                     }, {
                         node: b
                     }, v, S), u
                 },
-                X0 = function(n, t, o, s, u) {
+                J0 = function(n, t, o, s, u) {
                     s && n.push(s);
                     let p = 0;
                     for (; p < n.length; p++) {
                         let b = n[p],
-                            v = Yi(b);
+                            v = Qi(b);
                         if (v) {
-                            X0(v.children, t, o, null, u);
+                            J0(v.children, t, o, null, u);
                             continue
                         }
                         let S = !b.hasClass("mspace");
                         if (S) {
                             let E = t(b, o.node);
                             E && (o.insertAfter ? o.insertAfter(E) : (n.unshift(E), p++))
                         }
                         S ? o.node = b : u && b.hasClass("newline") && (o.node = Rt(["leftmost"])), o.insertAfter = (E => z => {
                             n.splice(E + 1, 0, z), p++
                         })(p)
                     }
                     s && n.pop()
                 },
-                Yi = function(n) {
-                    return n instanceof xr || n instanceof W0 || n instanceof vr && n.hasClass("enclosing") ? n : null
+                Qi = function(n) {
+                    return n instanceof xr || n instanceof Y0 || n instanceof vr && n.hasClass("enclosing") ? n : null
                 },
-                J0 = function(n, t) {
-                    let o = Yi(n);
+                K0 = function(n, t) {
+                    let o = Qi(n);
                     if (o) {
                         let s = o.children;
                         if (s.length) {
-                            if (t === "right") return J0(s[s.length - 1], "right");
-                            if (t === "left") return J0(s[0], "left")
+                            if (t === "right") return K0(s[s.length - 1], "right");
+                            if (t === "left") return K0(s[0], "left")
                         }
                     }
                     return n
                 },
-                K0 = function(n, t) {
-                    return n ? (t && (n = J0(n, t)), u1[n.classes[0]] || null) : null
+                en = function(n, t) {
+                    return n ? (t && (n = K0(n, t)), d1[n.classes[0]] || null) : null
                 },
                 wr = function(n, t) {
                     let o = ["nulldelimiter"].concat(n.baseSizingClasses());
                     return Rt(t.concat(o))
                 },
                 ve = function(n, t, o) {
                     if (!n) return Rt();
@@ -9653,15 +9653,15 @@
 
             function Jr(n, t) {
                 let o = Rt(["base"], n, t),
                     s = Rt(["strut"]);
                 return s.style.height = Z(o.height + o.depth), o.depth && (s.style.verticalAlign = Z(-o.depth)), o.children.unshift(s), o
             }
 
-            function en(n, t) {
+            function tn(n, t) {
                 let o = null;
                 n.length === 1 && n[0].type === "tag" && (o = n[0].tag, n = n[0].body);
                 let s = Ze(n, t, "root"),
                     u;
                 s.length === 2 && s[1].hasClass("tag") && (u = s.pop());
                 let p = [],
                     b = [];
@@ -9678,15 +9678,15 @@
                 if (S.setAttribute("aria-hidden", "true"), v) {
                     let E = v.children[0];
                     E.style.height = Z(S.height + S.depth), S.depth && (E.style.verticalAlign = Z(-S.depth))
                 }
                 return S
             }
 
-            function Zi(n) {
+            function Xi(n) {
                 return new xr(n)
             }
             class ht {
                 constructor(t, o, s) {
                     this.type = void 0, this.attributes = void 0, this.children = void 0, this.classes = void 0, this.type = t, this.attributes = {}, this.children = o || [], this.classes = s || []
                 }
                 setAttribute(t, o) {
@@ -9723,15 +9723,15 @@
                 toMarkup() {
                     return R.escape(this.toText())
                 }
                 toText() {
                     return this.text
                 }
             }
-            class h1 {
+            class m1 {
                 constructor(t) {
                     this.width = void 0, this.character = void 0, this.width = t, t >= .05555 && t <= .05556 ? this.character = "\u200A" : t >= .1666 && t <= .1667 ? this.character = "\u2009" : t >= .2222 && t <= .2223 ? this.character = "\u2005" : t >= .2777 && t <= .2778 ? this.character = "\u2005\u200A" : t >= -.05556 && t <= -.05555 ? this.character = "\u200A\u2063" : t >= -.1667 && t <= -.1666 ? this.character = "\u2009\u2063" : t >= -.2223 && t <= -.2222 ? this.character = "\u205F\u2063" : t >= -.2778 && t <= -.2777 ? this.character = "\u2005\u2063" : this.character = null
                 }
                 toNode() {
                     if (this.character) return document.createTextNode(this.character);
                     {
                         let t = document.createElementNS("http://www.w3.org/1998/Math/MathML", "mspace");
@@ -9744,24 +9744,24 @@
                 toText() {
                     return this.character ? this.character : " "
                 }
             }
             var V = {
                 MathNode: ht,
                 TextNode: kr,
-                SpaceNode: h1,
-                newDocumentFragment: Zi
+                SpaceNode: m1,
+                newDocumentFragment: Xi
             };
             let dt = function(n, t, o) {
-                    return Oe[t][n] && Oe[t][n].replace && n.charCodeAt(0) !== 55349 && !(Ii.hasOwnProperty(n) && o && (o.fontFamily && o.fontFamily.slice(4, 6) === "tt" || o.font && o.font.slice(4, 6) === "tt")) && (n = Oe[t][n].replace), new V.TextNode(n)
+                    return Oe[t][n] && Oe[t][n].replace && n.charCodeAt(0) !== 55349 && !(Hi.hasOwnProperty(n) && o && (o.fontFamily && o.fontFamily.slice(4, 6) === "tt" || o.font && o.font.slice(4, 6) === "tt")) && (n = Oe[t][n].replace), new V.TextNode(n)
                 },
-                tn = function(n) {
+                rn = function(n) {
                     return n.length === 1 ? n[0] : new V.MathNode("mrow", n)
                 },
-                rn = function(n, t) {
+                nn = function(n, t) {
                     if (t.fontFamily === "texttt") return "monospace";
                     if (t.fontFamily === "textsf") return t.fontShape === "textit" && t.fontWeight === "textbf" ? "sans-serif-bold-italic" : t.fontShape === "textit" ? "sans-serif-italic" : t.fontWeight === "textbf" ? "bold-sans-serif" : "sans-serif";
                     if (t.fontShape === "textit" && t.fontWeight === "textbf") return "bold-italic";
                     if (t.fontShape === "textit") return "italic";
                     if (t.fontWeight === "textbf") return "bold";
                     let o = t.font;
                     if (!o || o === "mathnormal") return null;
@@ -9774,15 +9774,15 @@
                     if (o === "mathscr" || o === "mathcal") return "script";
                     if (o === "mathsf") return "sans-serif";
                     if (o === "mathtt") return "monospace";
                     let u = n.text;
                     if (R.contains(["\\imath", "\\jmath"], u)) return null;
                     Oe[s][u] && Oe[s][u].replace && (u = Oe[s][u].replace);
                     let p = B.fontMap[o].fontName;
-                    return V0(u, p, s) ? B.fontMap[o].variant : null
+                    return j0(u, p, s) ? B.fontMap[o].variant : null
                 },
                 it = function(n, t, o) {
                     if (n.length === 1) {
                         let p = Ee(n[0], t);
                         return o && p instanceof ht && p.type === "mo" && (p.setAttribute("lspace", "0em"), p.setAttribute("rspace", "0em")), [p]
                     }
                     let s = [],
@@ -9811,70 +9811,70 @@
                             }
                         }
                         s.push(b), u = b
                     }
                     return s
                 },
                 Ht = function(n, t, o) {
-                    return tn(it(n, t, o))
+                    return rn(it(n, t, o))
                 },
                 Ee = function(n, t) {
                     if (!n) return new V.MathNode("mrow");
                     if (Qr[n.type]) return Qr[n.type](n, t);
                     throw new a("Got group of unknown type: '" + n.type + "'")
                 };
 
-            function Qi(n, t, o, s, u) {
+            function Ji(n, t, o, s, u) {
                 let p = it(n, o),
                     b;
                 p.length === 1 && p[0] instanceof ht && R.contains(["mrow", "mtable"], p[0].type) ? b = p[0] : b = new V.MathNode("mrow", p);
                 let v = new V.MathNode("annotation", [new V.TextNode(t)]);
                 v.setAttribute("encoding", "application/x-tex");
                 let S = new V.MathNode("semantics", [b, v]),
                     E = new V.MathNode("math", [S]);
                 E.setAttribute("xmlns", "http://www.w3.org/1998/Math/MathML"), s && E.setAttribute("display", "block");
                 let z = u ? "katex" : "katex-mathml";
                 return B.makeSpan([z], [E])
             }
-            let Xi = function(n) {
-                    return new Ou({
+            let Ki = function(n) {
+                    return new $u({
                         style: n.displayMode ? G.DISPLAY : G.TEXT,
                         maxSize: n.maxSize,
                         minRuleThickness: n.minRuleThickness
                     })
                 },
-                Ji = function(n, t) {
+                eo = function(n, t) {
                     if (t.displayMode) {
                         let o = ["katex-display"];
                         t.leqno && o.push("leqno"), t.fleqn && o.push("fleqn"), n = B.makeSpan(o, [n])
                     }
                     return n
                 },
-                d1 = function(n, t, o) {
-                    let s = Xi(o),
+                p1 = function(n, t, o) {
+                    let s = Ki(o),
                         u;
-                    if (o.output === "mathml") return Qi(n, t, s, o.displayMode, !0);
+                    if (o.output === "mathml") return Ji(n, t, s, o.displayMode, !0);
                     if (o.output === "html") {
-                        let p = en(n, s);
+                        let p = tn(n, s);
                         u = B.makeSpan(["katex"], [p])
                     } else {
-                        let p = Qi(n, t, s, o.displayMode, !1),
-                            b = en(n, s);
+                        let p = Ji(n, t, s, o.displayMode, !1),
+                            b = tn(n, s);
                         u = B.makeSpan(["katex"], [p, b])
                     }
-                    return Ji(u, o)
+                    return eo(u, o)
                 },
-                m1 = function(n, t, o) {
-                    let s = Xi(o),
-                        u = en(n, s),
+                f1 = function(n, t, o) {
+                    let s = Ki(o),
+                        u = tn(n, s),
                         p = B.makeSpan(["katex"], [u]);
-                    return Ji(p, o)
+                    return eo(p, o)
                 };
-            var Xp = null;
-            let p1 = {
+            var Kp = null;
+            let g1 = {
                     widehat: "^",
                     widecheck: "\u02C7",
                     widetilde: "~",
                     utilde: "~",
                     overleftarrow: "\u2190",
                     underleftarrow: "\u2190",
                     xleftarrow: "\u2190",
@@ -9910,19 +9910,19 @@
                     xrightleftarrows: "\u21C4",
                     xrightequilibrium: "\u21CC",
                     xleftequilibrium: "\u21CB",
                     "\\cdrightarrow": "\u2192",
                     "\\cdleftarrow": "\u2190",
                     "\\cdlongequal": "="
                 },
-                f1 = function(n) {
-                    let t = new V.MathNode("mo", [new V.TextNode(p1[n.replace(/^\\/, "")])]);
+                b1 = function(n) {
+                    let t = new V.MathNode("mo", [new V.TextNode(g1[n.replace(/^\\/, "")])]);
                     return t.setAttribute("stretchy", "true"), t
                 },
-                g1 = {
+                y1 = {
                     overrightarrow: [
                         ["rightarrow"], .888, 522, "xMaxYMin"
                     ],
                     overleftarrow: [
                         ["leftarrow"], .888, 522, "xMinYMin"
                     ],
                     underrightarrow: [
@@ -10036,55 +10036,55 @@
                     xrightequilibrium: [
                         ["baraboveshortleftharpoon", "rightharpoonaboveshortbar"], 1.75, 716
                     ],
                     xleftequilibrium: [
                         ["shortbaraboveleftharpoon", "shortrightharpoonabovebar"], 1.75, 716
                     ]
                 },
-                b1 = function(n) {
+                x1 = function(n) {
                     return n.type === "ordgroup" ? n.body.length : 1
                 };
             var Ft = {
                 encloseSpan: function(n, t, o, s, u) {
                     let p, b = n.height + n.depth + o + s;
                     if (/fbox|color|angl/.test(t)) {
                         if (p = B.makeSpan(["stretchy", t], [], u), t === "fbox") {
                             let v = u.color && u.getColor();
                             v && (p.style.borderColor = v)
                         }
                     } else {
                         let v = [];
-                        /^[bx]cancel$/.test(t) && v.push(new Y0({
+                        /^[bx]cancel$/.test(t) && v.push(new Z0({
                             x1: "0",
                             y1: "0",
                             x2: "100%",
                             y2: "100%",
                             "stroke-width": "0.046em"
-                        })), /^x?cancel$/.test(t) && v.push(new Y0({
+                        })), /^x?cancel$/.test(t) && v.push(new Z0({
                             x1: "0",
                             y1: "100%",
                             x2: "100%",
                             y2: "0",
                             "stroke-width": "0.046em"
                         }));
                         let S = new Et(v, {
                             width: "100%",
                             height: Z(b)
                         });
                         p = B.makeSvgSpan([], [S], u)
                     }
                     return p.height = b, p.style.height = Z(b), p
                 },
-                mathMLnode: f1,
+                mathMLnode: b1,
                 svgSpan: function(n, t) {
                     function o() {
                         let b = 4e5,
                             v = n.label.slice(1);
                         if (R.contains(["widehat", "widecheck", "widetilde", "utilde"], v)) {
-                            let E = b1(n.base),
+                            let E = x1(n.base),
                                 z, F, N;
                             if (E > 5) v === "widehat" || v === "widecheck" ? (z = 420, b = 2364, N = .42, F = v + "4") : (z = 312, b = 2340, N = .34, F = "tilde4");
                             else {
                                 let ie = [1, 1, 2, 2, 3, 3][E];
                                 v === "widehat" || v === "widecheck" ? (b = [0, 1062, 2364, 2364, 2364][ie], z = [0, 239, 300, 360, 420][ie], N = [0, .24, .3, .3, .36, .42][ie], F = v + ie) : (b = [0, 600, 1033, 2339, 2340][ie], z = [0, 260, 286, 306, 312][ie], N = [0, .26, .286, .3, .306, .34][ie], F = "tilde" + ie)
                             }
                             let H = new Ot(F),
@@ -10097,15 +10097,15 @@
                             return {
                                 span: B.makeSvgSpan([], [K], t),
                                 minWidth: 0,
                                 height: N
                             }
                         } else {
                             let S = [],
-                                E = g1[v],
+                                E = y1[v],
                                 [z, F, N] = E,
                                 H = N / 1e3,
                                 K = z.length,
                                 ie, ye;
                             if (K === 1) {
                                 let ge = E[3];
                                 ie = ["hide-tail"], ye = [ge]
@@ -10146,33 +10146,33 @@
             };
 
             function de(n, t) {
                 if (!n || n.type !== t) throw new Error("Expected node of type " + t + ", but got " + (n ? "node of type " + n.type : String(n)));
                 return n
             }
 
-            function nn(n) {
+            function on(n) {
                 let t = Kr(n);
                 if (!t) throw new Error("Expected node of symbol group type, but got " + (n ? "node of type " + n.type : String(n)));
                 return t
             }
 
             function Kr(n) {
-                return n && (n.type === "atom" || Uu.hasOwnProperty(n.type)) ? n : null
+                return n && (n.type === "atom" || Yu.hasOwnProperty(n.type)) ? n : null
             }
-            let on = (n, t) => {
+            let an = (n, t) => {
                     let o, s, u;
-                    n && n.type === "supsub" ? (s = de(n.base, "accent"), o = s.base, n.base = o, u = Vu(ve(n, t)), n.base = s) : (s = de(n, "accent"), o = s.base);
+                    n && n.type === "supsub" ? (s = de(n.base, "accent"), o = s.base, n.base = o, u = Uu(ve(n, t)), n.base = s) : (s = de(n, "accent"), o = s.base);
                     let p = ve(o, t.havingCrampedStyle()),
                         b = s.isShifty && R.isCharacterBox(o),
                         v = 0;
                     if (b) {
                         let N = R.getBaseElem(o),
                             H = ve(N, t.havingCrampedStyle());
-                        v = Pi(H).skew
+                        v = Oi(H).skew
                     }
                     let S = s.label === "\\c",
                         E = S ? p.height + p.depth : Math.min(p.height, t.fontMetrics().xHeight),
                         z;
                     if (s.isStretchy) z = Ft.svgSpan(s, t), z = B.makeVList({
                         positionType: "firstBaseline",
                         children: [{
@@ -10189,15 +10189,15 @@
                         }]
                     }, t);
                     else {
                         let N, H;
                         s.label === "\\vec" ? (N = B.staticSvg("vec", t), H = B.svgData.vec[1]) : (N = B.makeOrd({
                             mode: s.mode,
                             text: s.label
-                        }, t, "textord"), N = Pi(N), N.italic = 0, H = N.width, S && (E += N.depth)), z = B.makeSpan(["accent-body"], [N]);
+                        }, t, "textord"), N = Oi(N), N.italic = 0, H = N.width, S && (E += N.depth)), z = B.makeSpan(["accent-body"], [N]);
                         let K = s.label === "\\textcircled";
                         K && (z.classes.push("accent-full"), E = p.height);
                         let ie = v;
                         K || (ie -= H / 2), z.style.left = Z(ie), s.label === "\\textcircled" && (z.style.top = ".2em"), z = B.makeVList({
                             positionType: "firstBaseline",
                             children: [{
                                 type: "elem",
@@ -10210,41 +10210,41 @@
                                 elem: z
                             }]
                         }, t)
                     }
                     let F = B.makeSpan(["mord", "accent"], [z], t);
                     return u ? (u.children[0] = F, u.height = Math.max(F.height, u.height), u.classes[0] = "mord", u) : F
                 },
-                Ki = (n, t) => {
+                to = (n, t) => {
                     let o = n.isStretchy ? Ft.mathMLnode(n.label) : new V.MathNode("mo", [dt(n.label, n.mode)]),
                         s = new V.MathNode("mover", [Ee(n.base, t), o]);
                     return s.setAttribute("accent", "true"), s
                 },
-                y1 = new RegExp(["\\acute", "\\grave", "\\ddot", "\\tilde", "\\bar", "\\breve", "\\check", "\\hat", "\\vec", "\\dot", "\\mathring"].map(n => "\\" + n).join("|"));
+                v1 = new RegExp(["\\acute", "\\grave", "\\ddot", "\\tilde", "\\bar", "\\breve", "\\check", "\\hat", "\\vec", "\\dot", "\\mathring"].map(n => "\\" + n).join("|"));
             Q({
                 type: "accent",
                 names: ["\\acute", "\\grave", "\\ddot", "\\tilde", "\\bar", "\\breve", "\\check", "\\hat", "\\vec", "\\dot", "\\mathring", "\\widecheck", "\\widehat", "\\widetilde", "\\overrightarrow", "\\overleftarrow", "\\Overrightarrow", "\\overleftrightarrow", "\\overgroup", "\\overlinesegment", "\\overleftharpoon", "\\overrightharpoon"],
                 props: {
                     numArgs: 1
                 },
                 handler: (n, t) => {
                     let o = Xr(t[0]),
-                        s = !y1.test(n.funcName),
+                        s = !v1.test(n.funcName),
                         u = !s || n.funcName === "\\widehat" || n.funcName === "\\widetilde" || n.funcName === "\\widecheck";
                     return {
                         type: "accent",
                         mode: n.parser.mode,
                         label: n.funcName,
                         isStretchy: s,
                         isShifty: u,
                         base: o
                     }
                 },
-                htmlBuilder: on,
-                mathmlBuilder: Ki
+                htmlBuilder: an,
+                mathmlBuilder: to
             }), Q({
                 type: "accent",
                 names: ["\\'", "\\`", "\\^", "\\~", "\\=", "\\u", "\\.", '\\"', "\\c", "\\r", "\\H", "\\v", "\\textcircled"],
                 props: {
                     numArgs: 1,
                     allowedInText: !0,
                     allowedInMath: !0,
@@ -10258,16 +10258,16 @@
                         mode: s,
                         label: n.funcName,
                         isStretchy: !1,
                         isShifty: !0,
                         base: o
                     }
                 },
-                htmlBuilder: on,
-                mathmlBuilder: Ki
+                htmlBuilder: an,
+                mathmlBuilder: to
             }), Q({
                 type: "accentUnder",
                 names: ["\\underleftarrow", "\\underrightarrow", "\\underleftrightarrow", "\\undergroup", "\\underlinesegment", "\\utilde"],
                 props: {
                     numArgs: 1
                 },
                 handler: (n, t) => {
@@ -10391,22 +10391,22 @@
                     } else if (n.below) {
                         let u = e0(Ee(n.below, t));
                         s = new V.MathNode("munder", [o, u])
                     } else s = e0(), s = new V.MathNode("mover", [o, s]);
                     return s
                 }
             });
-            let x1 = B.makeSpan;
+            let w1 = B.makeSpan;
 
-            function eo(n, t) {
+            function ro(n, t) {
                 let o = Ze(n.body, t, !0);
-                return x1([n.mclass], o, t)
+                return w1([n.mclass], o, t)
             }
 
-            function to(n, t) {
+            function no(n, t) {
                 let o, s = it(n.body, t);
                 return n.mclass === "minner" ? o = new V.MathNode("mpadded", s) : n.mclass === "mord" ? n.isCharacterBox ? (o = s[0], o.type = "mi") : o = new V.MathNode("mi", s) : (n.isCharacterBox ? (o = s[0], o.type = "mo") : o = new V.MathNode("mo", s), n.mclass === "mbin" ? (o.attributes.lspace = "0.22em", o.attributes.rspace = "0.22em") : n.mclass === "mpunct" ? (o.attributes.lspace = "0em", o.attributes.rspace = "0.17em") : n.mclass === "mopen" || n.mclass === "mclose" ? (o.attributes.lspace = "0em", o.attributes.rspace = "0em") : n.mclass === "minner" && (o.attributes.lspace = "0.0556em", o.attributes.width = "+0.1111em")), o
             }
             Q({
                 type: "mclass",
                 names: ["\\mathord", "\\mathbin", "\\mathrel", "\\mathopen", "\\mathclose", "\\mathpunct", "\\mathinner"],
                 props: {
@@ -10422,16 +10422,16 @@
                         type: "mclass",
                         mode: o.mode,
                         mclass: "m" + s.slice(5),
                         body: je(u),
                         isCharacterBox: R.isCharacterBox(u)
                     }
                 },
-                htmlBuilder: eo,
-                mathmlBuilder: to
+                htmlBuilder: ro,
+                mathmlBuilder: no
             });
             let t0 = n => {
                 let t = n.type === "ordgroup" && n.body.length ? n.body[0] : n;
                 return t.type === "atom" && (t.family === "bin" || t.family === "rel") ? "m" + t.family : "mord"
             };
             Q({
                 type: "mclass",
@@ -10484,16 +10484,16 @@
                         type: "mclass",
                         mode: o.mode,
                         mclass: b,
                         body: [S],
                         isCharacterBox: R.isCharacterBox(S)
                     }
                 },
-                htmlBuilder: eo,
-                mathmlBuilder: to
+                htmlBuilder: ro,
+                mathmlBuilder: no
             }), Q({
                 type: "pmb",
                 names: ["\\pmb"],
                 props: {
                     numArgs: 1,
                     allowedInText: !0
                 },
@@ -10515,34 +10515,34 @@
                 },
                 mathmlBuilder(n, t) {
                     let o = it(n.body, t),
                         s = new V.MathNode("mstyle", o);
                     return s.setAttribute("style", "text-shadow: 0.02em 0.01em 0.04px"), s
                 }
             });
-            let v1 = {
+            let k1 = {
                     ">": "\\\\cdrightarrow",
                     "<": "\\\\cdleftarrow",
                     "=": "\\\\cdlongequal",
                     A: "\\uparrow",
                     V: "\\downarrow",
                     "|": "\\Vert",
                     ".": "no arrow"
                 },
-                ro = () => ({
+                io = () => ({
                     type: "styling",
                     body: [],
                     mode: "math",
                     style: "display"
                 }),
-                no = n => n.type === "textord" && n.text === "@",
-                w1 = (n, t) => (n.type === "mathord" || n.type === "atom") && n.text === t;
+                oo = n => n.type === "textord" && n.text === "@",
+                _1 = (n, t) => (n.type === "mathord" || n.type === "atom") && n.text === t;
 
-            function k1(n, t, o) {
-                let s = v1[n];
+            function S1(n, t, o) {
+                let s = k1[n];
                 switch (s) {
                     case "\\\\cdrightarrow":
                     case "\\\\cdleftarrow":
                         return o.callFunction(s, [t[0]], [t[1]]);
                     case "\\uparrow":
                     case "\\downarrow": {
                         let u = o.callFunction("\\\\cdleft", [t[0]], []),
@@ -10574,65 +10574,65 @@
                     default:
                         return {
                             type: "textord", text: " ", mode: "math"
                         }
                 }
             }
 
-            function _1(n) {
+            function C1(n) {
                 let t = [];
                 for (n.gullet.beginGroup(), n.gullet.macros.set("\\cr", "\\\\\\relax"), n.gullet.beginGroup();;) {
                     t.push(n.parseExpression(!1, "\\\\")), n.gullet.endGroup(), n.gullet.beginGroup();
                     let p = n.fetch().text;
                     if (p === "&" || p === "\\\\") n.consume();
                     else if (p === "\\end") {
                         t[t.length - 1].length === 0 && t.pop();
                         break
                     } else throw new a("Expected \\\\ or \\cr or \\end", n.nextToken)
                 }
                 let o = [],
                     s = [o];
                 for (let p = 0; p < t.length; p++) {
                     let b = t[p],
-                        v = ro();
+                        v = io();
                     for (let S = 0; S < b.length; S++)
-                        if (!no(b[S])) v.body.push(b[S]);
+                        if (!oo(b[S])) v.body.push(b[S]);
                         else {
                             o.push(v), S += 1;
-                            let E = nn(b[S]).text,
+                            let E = on(b[S]).text,
                                 z = new Array(2);
                             if (z[0] = {
                                     type: "ordgroup",
                                     mode: "math",
                                     body: []
                                 }, z[1] = {
                                     type: "ordgroup",
                                     mode: "math",
                                     body: []
                                 }, !("=|.".indexOf(E) > -1))
                                 if ("<>AV".indexOf(E) > -1)
                                     for (let H = 0; H < 2; H++) {
                                         let K = !0;
                                         for (let ie = S + 1; ie < b.length; ie++) {
-                                            if (w1(b[ie], E)) {
+                                            if (_1(b[ie], E)) {
                                                 K = !1, S = ie;
                                                 break
                                             }
-                                            if (no(b[ie])) throw new a("Missing a " + E + " character to complete a CD arrow.", b[ie]);
+                                            if (oo(b[ie])) throw new a("Missing a " + E + " character to complete a CD arrow.", b[ie]);
                                             z[H].body.push(b[ie])
                                         }
                                         if (K) throw new a("Missing a " + E + " character to complete a CD arrow.", b[S])
                                     } else throw new a('Expected one of "<>AV=|." after @', b[S]);
                             let N = {
                                 type: "styling",
-                                body: [k1(E, z, n)],
+                                body: [S1(E, z, n)],
                                 mode: "math",
                                 style: "display"
                             };
-                            o.push(N), v = ro()
+                            o.push(N), v = io()
                         } p % 2 === 0 ? o.push(v) : o.shift(), o = [], s.push(o)
                 }
                 n.gullet.endGroup(), n.gullet.endGroup();
                 let u = new Array(s[0].length).fill({
                     type: "align",
                     align: "c",
                     pregap: .25,
@@ -10722,19 +10722,19 @@
                     return b <= 65535 ? v = String.fromCharCode(b) : (b -= 65536, v = String.fromCharCode((b >> 10) + 55296, (b & 1023) + 56320)), {
                         type: "textord",
                         mode: o.mode,
                         text: v
                     }
                 }
             });
-            let io = (n, t) => {
+            let ao = (n, t) => {
                     let o = Ze(n.body, t.withColor(n.color), !1);
                     return B.makeFragment(o)
                 },
-                oo = (n, t) => {
+                so = (n, t) => {
                     let o = it(n.body, t.withColor(n.color)),
                         s = new V.MathNode("mstyle", o);
                     return s.setAttribute("mathcolor", n.color), s
                 };
             Q({
                 type: "color",
                 names: ["\\textcolor"],
@@ -10750,16 +10750,16 @@
                     return {
                         type: "color",
                         mode: o.mode,
                         color: s,
                         body: je(u)
                     }
                 },
-                htmlBuilder: io,
-                mathmlBuilder: oo
+                htmlBuilder: ao,
+                mathmlBuilder: so
             }), Q({
                 type: "color",
                 names: ["\\color"],
                 props: {
                     numArgs: 1,
                     allowedInText: !0,
                     argTypes: ["color"]
@@ -10774,16 +10774,16 @@
                     return {
                         type: "color",
                         mode: o.mode,
                         color: u,
                         body: p
                     }
                 },
-                htmlBuilder: io,
-                mathmlBuilder: oo
+                htmlBuilder: ao,
+                mathmlBuilder: so
             }), Q({
                 type: "cr",
                 names: ["\\\\"],
                 props: {
                     numArgs: 0,
                     numOptionalArgs: 0,
                     allowedInText: !0
@@ -10804,35 +10804,35 @@
                     return n.newLine && (o.classes.push("newline"), n.size && (o.style.marginTop = Z(Ie(n.size, t)))), o
                 },
                 mathmlBuilder(n, t) {
                     let o = new V.MathNode("mspace");
                     return n.newLine && (o.setAttribute("linebreak", "newline"), n.size && o.setAttribute("height", Z(Ie(n.size, t)))), o
                 }
             });
-            let an = {
+            let sn = {
                     "\\global": "\\global",
                     "\\long": "\\\\globallong",
                     "\\\\globallong": "\\\\globallong",
                     "\\def": "\\gdef",
                     "\\gdef": "\\gdef",
                     "\\edef": "\\xdef",
                     "\\xdef": "\\xdef",
                     "\\let": "\\\\globallet",
                     "\\futurelet": "\\\\globalfuture"
                 },
-                ao = n => {
+                lo = n => {
                     let t = n.text;
                     if (/^(?:[\\{}$&#^_]|EOF)$/.test(t)) throw new a("Expected a control sequence", n);
                     return t
                 },
-                S1 = n => {
+                T1 = n => {
                     let t = n.gullet.popToken();
                     return t.text === "=" && (t = n.gullet.popToken(), t.text === " " && (t = n.gullet.popToken())), t
                 },
-                so = (n, t, o, s) => {
+                co = (n, t, o, s) => {
                     let u = n.gullet.macros.get(o.text);
                     u == null && (o.noexpand = !0, u = {
                         tokens: [o],
                         numArgs: 0,
                         unexpandable: !n.gullet.isExpandable(o.text)
                     }), n.gullet.macros.set(t, u, s)
                 };
@@ -10846,15 +10846,15 @@
                 handler(n) {
                     let {
                         parser: t,
                         funcName: o
                     } = n;
                     t.consumeSpaces();
                     let s = t.fetch();
-                    if (an[s.text]) return (o === "\\global" || o === "\\\\globallong") && (s.text = an[s.text]), de(t.parseFunction(), "internal");
+                    if (sn[s.text]) return (o === "\\global" || o === "\\\\globallong") && (s.text = sn[s.text]), de(t.parseFunction(), "internal");
                     throw new a("Invalid token after macro prefix", s)
                 }
             }), Q({
                 type: "internal",
                 names: ["\\def", "\\gdef", "\\edef", "\\xdef"],
                 props: {
                     numArgs: 0,
@@ -10886,15 +10886,15 @@
                         } let {
                         tokens: S
                     } = t.gullet.consumeArg();
                     return b && S.unshift(b), (o === "\\edef" || o === "\\xdef") && (S = t.gullet.expandTokens(S), S.reverse()), t.gullet.macros.set(u, {
                         tokens: S,
                         numArgs: p,
                         delimiters: v
-                    }, o === an[o]), {
+                    }, o === sn[o]), {
                         type: "internal",
                         mode: t.mode
                     }
                 }
             }), Q({
                 type: "internal",
                 names: ["\\let", "\\\\globallet"],
@@ -10903,18 +10903,18 @@
                     allowedInText: !0,
                     primitive: !0
                 },
                 handler(n) {
                     let {
                         parser: t,
                         funcName: o
-                    } = n, s = ao(t.gullet.popToken());
+                    } = n, s = lo(t.gullet.popToken());
                     t.gullet.consumeSpaces();
-                    let u = S1(t);
-                    return so(t, s, u, o === "\\\\globallet"), {
+                    let u = T1(t);
+                    return co(t, s, u, o === "\\\\globallet"), {
                         type: "internal",
                         mode: t.mode
                     }
                 }
             }), Q({
                 type: "internal",
                 names: ["\\futurelet", "\\\\globalfuture"],
@@ -10923,87 +10923,87 @@
                     allowedInText: !0,
                     primitive: !0
                 },
                 handler(n) {
                     let {
                         parser: t,
                         funcName: o
-                    } = n, s = ao(t.gullet.popToken()), u = t.gullet.popToken(), p = t.gullet.popToken();
-                    return so(t, s, p, o === "\\\\globalfuture"), t.gullet.pushToken(p), t.gullet.pushToken(u), {
+                    } = n, s = lo(t.gullet.popToken()), u = t.gullet.popToken(), p = t.gullet.popToken();
+                    return co(t, s, p, o === "\\\\globalfuture"), t.gullet.pushToken(p), t.gullet.pushToken(u), {
                         type: "internal",
                         mode: t.mode
                     }
                 }
             });
             let _r = function(n, t, o) {
                     let s = Oe.math[n] && Oe.math[n].replace,
-                        u = V0(s || n, t, o);
+                        u = j0(s || n, t, o);
                     if (!u) throw new Error("Unsupported symbol " + n + " and font size " + t + ".");
                     return u
                 },
-                sn = function(n, t, o, s) {
+                ln = function(n, t, o, s) {
                     let u = o.havingBaseStyle(t),
                         p = B.makeSpan(s.concat(u.sizingClasses(o)), [n], o),
                         b = u.sizeMultiplier / o.sizeMultiplier;
                     return p.height *= b, p.depth *= b, p.maxFontSize = u.sizeMultiplier, p
                 },
-                lo = function(n, t, o) {
+                uo = function(n, t, o) {
                     let s = t.havingBaseStyle(o),
                         u = (1 - t.sizeMultiplier / s.sizeMultiplier) * t.fontMetrics().axisHeight;
                     n.classes.push("delimcenter"), n.style.top = Z(u), n.height -= u, n.depth += u
                 },
-                C1 = function(n, t, o, s, u, p) {
+                A1 = function(n, t, o, s, u, p) {
                     let b = B.makeSymbol(n, "Main-Regular", u, s),
-                        v = sn(b, t, s, p);
-                    return o && lo(v, s, t), v
+                        v = ln(b, t, s, p);
+                    return o && uo(v, s, t), v
                 },
-                T1 = function(n, t, o, s) {
+                q1 = function(n, t, o, s) {
                     return B.makeSymbol(n, "Size" + t + "-Regular", o, s)
                 },
-                co = function(n, t, o, s, u, p) {
-                    let b = T1(n, t, u, s),
-                        v = sn(B.makeSpan(["delimsizing", "size" + t], [b], s), G.TEXT, s, p);
-                    return o && lo(v, s, G.TEXT), v
+                ho = function(n, t, o, s, u, p) {
+                    let b = q1(n, t, u, s),
+                        v = ln(B.makeSpan(["delimsizing", "size" + t], [b], s), G.TEXT, s, p);
+                    return o && uo(v, s, G.TEXT), v
                 },
-                ln = function(n, t, o) {
+                cn = function(n, t, o) {
                     let s;
                     return t === "Size1-Regular" ? s = "delim-size1" : s = "delim-size4", {
                         type: "elem",
                         elem: B.makeSpan(["delimsizinginner", s], [B.makeSpan([], [B.makeSymbol(n, t, o)])])
                     }
                 },
-                cn = function(n, t, o) {
+                un = function(n, t, o) {
                     let s = vt["Size4-Regular"][n.charCodeAt(0)] ? vt["Size4-Regular"][n.charCodeAt(0)][4] : vt["Size1-Regular"][n.charCodeAt(0)][4],
-                        u = new Ot("inner", Bu(n, Math.round(1e3 * t))),
+                        u = new Ot("inner", Lu(n, Math.round(1e3 * t))),
                         p = new Et([u], {
                             width: Z(s),
                             height: Z(t),
                             style: "width:" + Z(s),
                             viewBox: "0 0 " + 1e3 * s + " " + Math.round(1e3 * t),
                             preserveAspectRatio: "xMinYMin"
                         }),
                         b = B.makeSvgSpan([], [p], o);
                     return b.height = t, b.style.height = Z(t), b.style.width = Z(s), {
                         type: "elem",
                         elem: b
                     }
                 },
-                un = .008,
+                hn = .008,
                 r0 = {
                     type: "kern",
-                    size: -1 * un
+                    size: -1 * hn
                 },
-                A1 = ["|", "\\lvert", "\\rvert", "\\vert"],
-                q1 = ["\\|", "\\lVert", "\\rVert", "\\Vert"],
-                uo = function(n, t, o, s, u, p) {
+                M1 = ["|", "\\lvert", "\\rvert", "\\vert"],
+                E1 = ["\\|", "\\lVert", "\\rVert", "\\Vert"],
+                mo = function(n, t, o, s, u, p) {
                     let b, v, S, E, z = "",
                         F = 0;
                     b = S = E = n, v = null;
                     let N = "Size1-Regular";
-                    n === "\\uparrow" ? S = E = "\u23D0" : n === "\\Uparrow" ? S = E = "\u2016" : n === "\\downarrow" ? b = S = "\u23D0" : n === "\\Downarrow" ? b = S = "\u2016" : n === "\\updownarrow" ? (b = "\\uparrow", S = "\u23D0", E = "\\downarrow") : n === "\\Updownarrow" ? (b = "\\Uparrow", S = "\u2016", E = "\\Downarrow") : R.contains(A1, n) ? (S = "\u2223", z = "vert", F = 333) : R.contains(q1, n) ? (S = "\u2225", z = "doublevert", F = 556) : n === "[" || n === "\\lbrack" ? (b = "\u23A1", S = "\u23A2", E = "\u23A3", N = "Size4-Regular", z = "lbrack", F = 667) : n === "]" || n === "\\rbrack" ? (b = "\u23A4", S = "\u23A5", E = "\u23A6", N = "Size4-Regular", z = "rbrack", F = 667) : n === "\\lfloor" || n === "\u230A" ? (S = b = "\u23A2", E = "\u23A3", N = "Size4-Regular", z = "lfloor", F = 667) : n === "\\lceil" || n === "\u2308" ? (b = "\u23A1", S = E = "\u23A2", N = "Size4-Regular", z = "lceil", F = 667) : n === "\\rfloor" || n === "\u230B" ? (S = b = "\u23A5", E = "\u23A6", N = "Size4-Regular", z = "rfloor", F = 667) : n === "\\rceil" || n === "\u2309" ? (b = "\u23A4", S = E = "\u23A5", N = "Size4-Regular", z = "rceil", F = 667) : n === "(" || n === "\\lparen" ? (b = "\u239B", S = "\u239C", E = "\u239D", N = "Size4-Regular", z = "lparen", F = 875) : n === ")" || n === "\\rparen" ? (b = "\u239E", S = "\u239F", E = "\u23A0", N = "Size4-Regular", z = "rparen", F = 875) : n === "\\{" || n === "\\lbrace" ? (b = "\u23A7", v = "\u23A8", E = "\u23A9", S = "\u23AA", N = "Size4-Regular") : n === "\\}" || n === "\\rbrace" ? (b = "\u23AB", v = "\u23AC", E = "\u23AD", S = "\u23AA", N = "Size4-Regular") : n === "\\lgroup" || n === "\u27EE" ? (b = "\u23A7", E = "\u23A9", S = "\u23AA", N = "Size4-Regular") : n === "\\rgroup" || n === "\u27EF" ? (b = "\u23AB", E = "\u23AD", S = "\u23AA", N = "Size4-Regular") : n === "\\lmoustache" || n === "\u23B0" ? (b = "\u23A7", E = "\u23AD", S = "\u23AA", N = "Size4-Regular") : (n === "\\rmoustache" || n === "\u23B1") && (b = "\u23AB", E = "\u23A9", S = "\u23AA", N = "Size4-Regular");
+                    n === "\\uparrow" ? S = E = "\u23D0" : n === "\\Uparrow" ? S = E = "\u2016" : n === "\\downarrow" ? b = S = "\u23D0" : n === "\\Downarrow" ? b = S = "\u2016" : n === "\\updownarrow" ? (b = "\\uparrow", S = "\u23D0", E = "\\downarrow") : n === "\\Updownarrow" ? (b = "\\Uparrow", S = "\u2016", E = "\\Downarrow") : R.contains(M1, n) ? (S = "\u2223", z = "vert", F = 333) : R.contains(E1, n) ? (S = "\u2225", z = "doublevert", F = 556) : n === "[" || n === "\\lbrack" ? (b = "\u23A1", S = "\u23A2", E = "\u23A3", N = "Size4-Regular", z = "lbrack", F = 667) : n === "]" || n === "\\rbrack" ? (b = "\u23A4", S = "\u23A5", E = "\u23A6", N = "Size4-Regular", z = "rbrack", F = 667) : n === "\\lfloor" || n === "\u230A" ? (S = b = "\u23A2", E = "\u23A3", N = "Size4-Regular", z = "lfloor", F = 667) : n === "\\lceil" || n === "\u2308" ? (b = "\u23A1", S = E = "\u23A2", N = "Size4-Regular", z = "lceil", F = 667) : n === "\\rfloor" || n === "\u230B" ? (S = b = "\u23A5", E = "\u23A6", N = "Size4-Regular", z = "rfloor", F = 667) : n === "\\rceil" || n === "\u2309" ? (b = "\u23A4", S = E = "\u23A5", N = "Size4-Regular", z = "rceil", F = 667) : n === "(" || n === "\\lparen" ? (b = "\u239B", S = "\u239C", E = "\u239D", N = "Size4-Regular", z = "lparen", F = 875) : n === ")" || n === "\\rparen" ? (b = "\u239E", S = "\u239F", E = "\u23A0", N = "Size4-Regular", z = "rparen", F = 875) : n === "\\{" || n === "\\lbrace" ? (b = "\u23A7", v = "\u23A8", E = "\u23A9", S = "\u23AA", N = "Size4-Regular") : n === "\\}" || n === "\\rbrace" ? (b = "\u23AB", v = "\u23AC", E = "\u23AD", S = "\u23AA", N = "Size4-Regular") : n === "\\lgroup" || n === "\u27EE" ? (b = "\u23A7", E = "\u23A9", S = "\u23AA", N = "Size4-Regular") : n === "\\rgroup" || n === "\u27EF" ? (b = "\u23AB", E = "\u23AD", S = "\u23AA", N = "Size4-Regular") : n === "\\lmoustache" || n === "\u23B0" ? (b = "\u23A7", E = "\u23AD", S = "\u23AA", N = "Size4-Regular") : (n === "\\rmoustache" || n === "\u23B1") && (b = "\u23AB", E = "\u23A9", S = "\u23AA", N = "Size4-Regular");
                     let H = _r(b, N, u),
                         K = H.height + H.depth,
                         ie = _r(S, N, u),
                         ye = ie.height + ie.depth,
                         ge = _r(E, N, u),
                         xe = ge.height + ge.depth,
                         ke = 0,
@@ -11018,84 +11018,84 @@
                         cr = s.fontMetrics().axisHeight;
                     o && (cr *= s.sizeMultiplier);
                     let we = pt / 2 - cr,
                         qe = [];
                     if (z.length > 0) {
                         let Ve = pt - K - xe,
                             $e = Math.round(pt * 1e3),
-                            ft = Nu(z, Math.round(Ve * 1e3)),
-                            eh = new Ot(z, ft),
-                            ta = (F / 1e3).toFixed(3) + "em",
-                            ra = ($e / 1e3).toFixed(3) + "em",
-                            th = new Et([eh], {
-                                width: ta,
-                                height: ra,
+                            ft = Pu(z, Math.round(Ve * 1e3)),
+                            rh = new Ot(z, ft),
+                            na = (F / 1e3).toFixed(3) + "em",
+                            ia = ($e / 1e3).toFixed(3) + "em",
+                            nh = new Et([rh], {
+                                width: na,
+                                height: ia,
                                 viewBox: "0 0 " + F + " " + $e
                             }),
-                            s0 = B.makeSvgSpan([], [th], s);
-                        s0.height = $e / 1e3, s0.style.width = ta, s0.style.height = ra, qe.push({
+                            s0 = B.makeSvgSpan([], [nh], s);
+                        s0.height = $e / 1e3, s0.style.width = na, s0.style.height = ia, qe.push({
                             type: "elem",
                             elem: s0
                         })
                     } else {
-                        if (qe.push(ln(E, N, u)), qe.push(r0), v === null) {
-                            let Ve = pt - K - xe + 2 * un;
-                            qe.push(cn(S, Ve, s))
+                        if (qe.push(cn(E, N, u)), qe.push(r0), v === null) {
+                            let Ve = pt - K - xe + 2 * hn;
+                            qe.push(un(S, Ve, s))
                         } else {
-                            let Ve = (pt - K - xe - ke) / 2 + 2 * un;
-                            qe.push(cn(S, Ve, s)), qe.push(r0), qe.push(ln(v, N, u)), qe.push(r0), qe.push(cn(S, Ve, s))
+                            let Ve = (pt - K - xe - ke) / 2 + 2 * hn;
+                            qe.push(un(S, Ve, s)), qe.push(r0), qe.push(cn(v, N, u)), qe.push(r0), qe.push(un(S, Ve, s))
                         }
-                        qe.push(r0), qe.push(ln(b, N, u))
+                        qe.push(r0), qe.push(cn(b, N, u))
                     }
                     let Fe = s.havingBaseStyle(G.TEXT),
                         Ne = B.makeVList({
                             positionType: "bottom",
                             positionData: we,
                             children: qe
                         }, Fe);
-                    return sn(B.makeSpan(["delimsizing", "mult"], [Ne], Fe), G.TEXT, s, p)
+                    return ln(B.makeSpan(["delimsizing", "mult"], [Ne], Fe), G.TEXT, s, p)
                 },
-                hn = 80,
-                dn = .08,
-                mn = function(n, t, o, s, u) {
-                    let p = Fu(n, s, o),
+                dn = 80,
+                mn = .08,
+                pn = function(n, t, o, s, u) {
+                    let p = Nu(n, s, o),
                         b = new Ot(n, p),
                         v = new Et([b], {
                             width: "400em",
                             height: Z(t),
                             viewBox: "0 0 400000 " + o,
                             preserveAspectRatio: "xMinYMin slice"
                         });
                     return B.makeSvgSpan(["hide-tail"], [v], u)
                 },
-                M1 = function(n, t) {
+                D1 = function(n, t) {
                     let o = t.havingBaseSizing(),
-                        s = fo("\\surd", n * o.sizeMultiplier, po, o),
+                        s = bo("\\surd", n * o.sizeMultiplier, go, o),
                         u = o.sizeMultiplier,
                         p = Math.max(0, t.minRuleThickness - t.fontMetrics().sqrtRuleThickness),
                         b, v = 0,
                         S = 0,
                         E = 0,
                         z;
-                    return s.type === "small" ? (E = 1e3 + 1e3 * p + hn, n < 1 ? u = 1 : n < 1.4 && (u = .7), v = (1 + p + dn) / u, S = (1 + p) / u, b = mn("sqrtMain", v, E, p, t), b.style.minWidth = "0.853em", z = .833 / u) : s.type === "large" ? (E = (1e3 + hn) * Sr[s.size], S = (Sr[s.size] + p) / u, v = (Sr[s.size] + p + dn) / u, b = mn("sqrtSize" + s.size, v, E, p, t), b.style.minWidth = "1.02em", z = 1 / u) : (v = n + p + dn, S = n + p, E = Math.floor(1e3 * n + p) + hn, b = mn("sqrtTall", v, E, p, t), b.style.minWidth = "0.742em", z = 1.056), b.height = S, b.style.height = Z(v), {
+                    return s.type === "small" ? (E = 1e3 + 1e3 * p + dn, n < 1 ? u = 1 : n < 1.4 && (u = .7), v = (1 + p + mn) / u, S = (1 + p) / u, b = pn("sqrtMain", v, E, p, t), b.style.minWidth = "0.853em", z = .833 / u) : s.type === "large" ? (E = (1e3 + dn) * Sr[s.size], S = (Sr[s.size] + p) / u, v = (Sr[s.size] + p + mn) / u, b = pn("sqrtSize" + s.size, v, E, p, t), b.style.minWidth = "1.02em", z = 1 / u) : (v = n + p + mn, S = n + p, E = Math.floor(1e3 * n + p) + dn, b = pn("sqrtTall", v, E, p, t), b.style.minWidth = "0.742em", z = 1.056), b.height = S, b.style.height = Z(v), {
                         span: b,
                         advanceWidth: z,
                         ruleWidth: (t.fontMetrics().sqrtRuleThickness + p) * u
                     }
                 },
-                ho = ["(", "\\lparen", ")", "\\rparen", "[", "\\lbrack", "]", "\\rbrack", "\\{", "\\lbrace", "\\}", "\\rbrace", "\\lfloor", "\\rfloor", "\u230A", "\u230B", "\\lceil", "\\rceil", "\u2308", "\u2309", "\\surd"],
-                E1 = ["\\uparrow", "\\downarrow", "\\updownarrow", "\\Uparrow", "\\Downarrow", "\\Updownarrow", "|", "\\|", "\\vert", "\\Vert", "\\lvert", "\\rvert", "\\lVert", "\\rVert", "\\lgroup", "\\rgroup", "\u27EE", "\u27EF", "\\lmoustache", "\\rmoustache", "\u23B0", "\u23B1"],
-                mo = ["<", ">", "\\langle", "\\rangle", "/", "\\backslash", "\\lt", "\\gt"],
+                po = ["(", "\\lparen", ")", "\\rparen", "[", "\\lbrack", "]", "\\rbrack", "\\{", "\\lbrace", "\\}", "\\rbrace", "\\lfloor", "\\rfloor", "\u230A", "\u230B", "\\lceil", "\\rceil", "\u2308", "\u2309", "\\surd"],
+                z1 = ["\\uparrow", "\\downarrow", "\\updownarrow", "\\Uparrow", "\\Downarrow", "\\Updownarrow", "|", "\\|", "\\vert", "\\Vert", "\\lvert", "\\rvert", "\\lVert", "\\rVert", "\\lgroup", "\\rgroup", "\u27EE", "\u27EF", "\\lmoustache", "\\rmoustache", "\u23B0", "\u23B1"],
+                fo = ["<", ">", "\\langle", "\\rangle", "/", "\\backslash", "\\lt", "\\gt"],
                 Sr = [0, 1.2, 1.8, 2.4, 3],
-                D1 = function(n, t, o, s, u) {
-                    if (n === "<" || n === "\\lt" || n === "\u27E8" ? n = "\\langle" : (n === ">" || n === "\\gt" || n === "\u27E9") && (n = "\\rangle"), R.contains(ho, n) || R.contains(mo, n)) return co(n, t, !1, o, s, u);
-                    if (R.contains(E1, n)) return uo(n, Sr[t], !1, o, s, u);
+                R1 = function(n, t, o, s, u) {
+                    if (n === "<" || n === "\\lt" || n === "\u27E8" ? n = "\\langle" : (n === ">" || n === "\\gt" || n === "\u27E9") && (n = "\\rangle"), R.contains(po, n) || R.contains(fo, n)) return ho(n, t, !1, o, s, u);
+                    if (R.contains(z1, n)) return mo(n, Sr[t], !1, o, s, u);
                     throw new a("Illegal delimiter: '" + n + "'")
                 },
-                z1 = [{
+                F1 = [{
                     type: "small",
                     style: G.SCRIPTSCRIPT
                 }, {
                     type: "small",
                     style: G.SCRIPT
                 }, {
                     type: "small",
@@ -11109,27 +11109,27 @@
                 }, {
                     type: "large",
                     size: 3
                 }, {
                     type: "large",
                     size: 4
                 }],
-                R1 = [{
+                B1 = [{
                     type: "small",
                     style: G.SCRIPTSCRIPT
                 }, {
                     type: "small",
                     style: G.SCRIPT
                 }, {
                     type: "small",
                     style: G.TEXT
                 }, {
                     type: "stack"
                 }],
-                po = [{
+                go = [{
                     type: "small",
                     style: G.SCRIPTSCRIPT
                 }, {
                     type: "small",
                     style: G.SCRIPT
                 }, {
                     type: "small",
@@ -11145,55 +11145,55 @@
                     size: 3
                 }, {
                     type: "large",
                     size: 4
                 }, {
                     type: "stack"
                 }],
-                F1 = function(n) {
+                N1 = function(n) {
                     if (n.type === "small") return "Main-Regular";
                     if (n.type === "large") return "Size" + n.size + "-Regular";
                     if (n.type === "stack") return "Size4-Regular";
                     throw new Error("Add support for delim type '" + n.type + "' here.")
                 },
-                fo = function(n, t, o, s) {
+                bo = function(n, t, o, s) {
                     let u = Math.min(2, 3 - s.style.size);
                     for (let p = u; p < o.length && o[p].type !== "stack"; p++) {
-                        let b = _r(n, F1(o[p]), "math"),
+                        let b = _r(n, N1(o[p]), "math"),
                             v = b.height + b.depth;
                         if (o[p].type === "small") {
                             let S = s.havingBaseStyle(o[p].style);
                             v *= S.sizeMultiplier
                         }
                         if (v > t) return o[p]
                     }
                     return o[o.length - 1]
                 },
-                go = function(n, t, o, s, u, p) {
+                yo = function(n, t, o, s, u, p) {
                     n === "<" || n === "\\lt" || n === "\u27E8" ? n = "\\langle" : (n === ">" || n === "\\gt" || n === "\u27E9") && (n = "\\rangle");
                     let b;
-                    R.contains(mo, n) ? b = z1 : R.contains(ho, n) ? b = po : b = R1;
-                    let v = fo(n, t, b, s);
-                    return v.type === "small" ? C1(n, v.style, o, s, u, p) : v.type === "large" ? co(n, v.size, o, s, u, p) : uo(n, t, o, s, u, p)
+                    R.contains(fo, n) ? b = F1 : R.contains(po, n) ? b = go : b = B1;
+                    let v = bo(n, t, b, s);
+                    return v.type === "small" ? A1(n, v.style, o, s, u, p) : v.type === "large" ? ho(n, v.size, o, s, u, p) : mo(n, t, o, s, u, p)
                 };
             var Bt = {
-                sqrtImage: M1,
-                sizedDelim: D1,
+                sqrtImage: D1,
+                sizedDelim: R1,
                 sizeToMaxHeight: Sr,
-                customSizedDelim: go,
+                customSizedDelim: yo,
                 leftRightDelim: function(n, t, o, s, u, p) {
                     let b = s.fontMetrics().axisHeight * s.sizeMultiplier,
                         v = 901,
                         S = 5 / s.fontMetrics().ptPerEm,
                         E = Math.max(t - b, o + b),
                         z = Math.max(E / 500 * v, 2 * E - S);
-                    return go(n, z, !0, s, u, p)
+                    return yo(n, z, !0, s, u, p)
                 }
             };
-            let bo = {
+            let xo = {
                     "\\bigl": {
                         mclass: "mopen",
                         size: 1
                     },
                     "\\Bigl": {
                         mclass: "mopen",
                         size: 2
@@ -11251,50 +11251,50 @@
                         size: 3
                     },
                     "\\Bigg": {
                         mclass: "mord",
                         size: 4
                     }
                 },
-                B1 = ["(", "\\lparen", ")", "\\rparen", "[", "\\lbrack", "]", "\\rbrack", "\\{", "\\lbrace", "\\}", "\\rbrace", "\\lfloor", "\\rfloor", "\u230A", "\u230B", "\\lceil", "\\rceil", "\u2308", "\u2309", "<", ">", "\\langle", "\u27E8", "\\rangle", "\u27E9", "\\lt", "\\gt", "\\lvert", "\\rvert", "\\lVert", "\\rVert", "\\lgroup", "\\rgroup", "\u27EE", "\u27EF", "\\lmoustache", "\\rmoustache", "\u23B0", "\u23B1", "/", "\\backslash", "|", "\\vert", "\\|", "\\Vert", "\\uparrow", "\\Uparrow", "\\downarrow", "\\Downarrow", "\\updownarrow", "\\Updownarrow", "."];
+                L1 = ["(", "\\lparen", ")", "\\rparen", "[", "\\lbrack", "]", "\\rbrack", "\\{", "\\lbrace", "\\}", "\\rbrace", "\\lfloor", "\\rfloor", "\u230A", "\u230B", "\\lceil", "\\rceil", "\u2308", "\u2309", "<", ">", "\\langle", "\u27E8", "\\rangle", "\u27E9", "\\lt", "\\gt", "\\lvert", "\\rvert", "\\lVert", "\\rVert", "\\lgroup", "\\rgroup", "\u27EE", "\u27EF", "\\lmoustache", "\\rmoustache", "\u23B0", "\u23B1", "/", "\\backslash", "|", "\\vert", "\\|", "\\Vert", "\\uparrow", "\\Uparrow", "\\downarrow", "\\Downarrow", "\\updownarrow", "\\Updownarrow", "."];
 
             function n0(n, t) {
                 let o = Kr(n);
-                if (o && R.contains(B1, o.text)) return o;
+                if (o && R.contains(L1, o.text)) return o;
                 throw o ? new a("Invalid delimiter '" + o.text + "' after '" + t.funcName + "'", n) : new a("Invalid delimiter type '" + n.type + "'", n)
             }
             Q({
                 type: "delimsizing",
                 names: ["\\bigl", "\\Bigl", "\\biggl", "\\Biggl", "\\bigr", "\\Bigr", "\\biggr", "\\Biggr", "\\bigm", "\\Bigm", "\\biggm", "\\Biggm", "\\big", "\\Big", "\\bigg", "\\Bigg"],
                 props: {
                     numArgs: 1,
                     argTypes: ["primitive"]
                 },
                 handler: (n, t) => {
                     let o = n0(t[0], n);
                     return {
                         type: "delimsizing",
                         mode: n.parser.mode,
-                        size: bo[n.funcName].size,
-                        mclass: bo[n.funcName].mclass,
+                        size: xo[n.funcName].size,
+                        mclass: xo[n.funcName].mclass,
                         delim: o.text
                     }
                 },
                 htmlBuilder: (n, t) => n.delim === "." ? B.makeSpan([n.mclass]) : Bt.sizedDelim(n.delim, n.size, t, n.mode, [n.mclass]),
                 mathmlBuilder: n => {
                     let t = [];
                     n.delim !== "." && t.push(dt(n.delim, n.mode));
                     let o = new V.MathNode("mo", t);
                     n.mclass === "mopen" || n.mclass === "mclose" ? o.setAttribute("fence", "true") : o.setAttribute("fence", "false"), o.setAttribute("stretchy", "true");
                     let s = Z(Bt.sizeToMaxHeight[n.size]);
                     return o.setAttribute("minsize", s), o.setAttribute("maxsize", s), o
                 }
             });
 
-            function yo(n) {
+            function vo(n) {
                 if (!n.body) throw new Error("Bug: The leftright ParseNode wasn't fully parsed.")
             }
             Q({
                 type: "leftright-right",
                 names: ["\\right"],
                 props: {
                     numArgs: 1,
@@ -11330,15 +11330,15 @@
                         body: u,
                         left: o.text,
                         right: p.delim,
                         rightColor: p.color
                     }
                 },
                 htmlBuilder: (n, t) => {
-                    yo(n);
+                    vo(n);
                     let o = Ze(n.body, t, !0, ["mopen", "mclose"]),
                         s = 0,
                         u = 0,
                         p = !1;
                     for (let S = 0; S < o.length; S++) o[S].isMiddle ? p = !0 : (s = Math.max(o[S].height, s), u = Math.max(o[S].depth, u));
                     s *= t.sizeMultiplier, u *= t.sizeMultiplier;
                     let b;
@@ -11352,25 +11352,25 @@
                     else {
                         let S = n.rightColor ? t.withColor(n.rightColor) : t;
                         v = Bt.leftRightDelim(n.right, s, u, S, n.mode, ["mclose"])
                     }
                     return o.push(v), B.makeSpan(["minner"], o, t)
                 },
                 mathmlBuilder: (n, t) => {
-                    yo(n);
+                    vo(n);
                     let o = it(n.body, t);
                     if (n.left !== ".") {
                         let s = new V.MathNode("mo", [dt(n.left, n.mode)]);
                         s.setAttribute("fence", "true"), o.unshift(s)
                     }
                     if (n.right !== ".") {
                         let s = new V.MathNode("mo", [dt(n.right, n.mode)]);
                         s.setAttribute("fence", "true"), n.rightColor && s.setAttribute("mathcolor", n.rightColor), o.push(s)
                     }
-                    return tn(o)
+                    return rn(o)
                 }
             }), Q({
                 type: "middle",
                 names: ["\\middle"],
                 props: {
                     numArgs: 1,
                     primitive: !0
@@ -11399,15 +11399,15 @@
                 },
                 mathmlBuilder: (n, t) => {
                     let o = n.delim === "\\vert" || n.delim === "|" ? dt("|", "text") : dt(n.delim, n.mode),
                         s = new V.MathNode("mo", [o]);
                     return s.setAttribute("fence", "true"), s.setAttribute("lspace", "0.05em"), s.setAttribute("rspace", "0.05em"), s
                 }
             });
-            let pn = (n, t) => {
+            let fn = (n, t) => {
                     let o = B.wrapFragment(ve(n.body, t), t),
                         s = n.label.slice(1),
                         u = t.sizeMultiplier,
                         p, b = 0,
                         v = R.isCharacterBox(n.body);
                     if (s === "sout") p = B.makeSpan(["stretchy", "sout"]), p.height = t.fontMetrics().defaultRuleThickness / u, b = -.5 * t.fontMetrics().xHeight;
                     else if (s === "phase") {
@@ -11420,15 +11420,15 @@
                                 unit: "ex"
                             }, t),
                             F = t.havingBaseSizing();
                         u = u / F.sizeMultiplier;
                         let N = o.height + o.depth + E + z;
                         o.style.paddingLeft = Z(N / 2 + E);
                         let H = Math.floor(1e3 * N * u),
-                            K = zu(H),
+                            K = Fu(H),
                             ie = new Et([new Ot("phase", K)], {
                                 width: "400em",
                                 height: Z(H / 1e3),
                                 viewBox: "0 0 400000 " + H,
                                 preserveAspectRatio: "xMinYMin slice"
                             });
                         p = B.makeSvgSpan(["hide-tail"], [ie], t), p.style.height = Z(N), b = o.depth + E + z
@@ -11466,15 +11466,15 @@
                                 shift: b,
                                 wrapperClasses: E
                             }]
                         }, t)
                     }
                     return /cancel/.test(s) && (S.height = o.height, S.depth = o.depth), /cancel/.test(s) && !v ? B.makeSpan(["mord", "cancel-lap"], [S], t) : B.makeSpan(["mord"], [S], t)
                 },
-                fn = (n, t) => {
+                gn = (n, t) => {
                     let o = 0,
                         s = new V.MathNode(n.label.indexOf("colorbox") > -1 ? "mpadded" : "menclose", [Ee(n.body, t)]);
                     switch (n.label) {
                         case "\\cancel":
                             s.setAttribute("notation", "updiagonalstrike");
                             break;
                         case "\\bcancel":
@@ -11522,16 +11522,16 @@
                         type: "enclose",
                         mode: s.mode,
                         label: u,
                         backgroundColor: p,
                         body: b
                     }
                 },
-                htmlBuilder: pn,
-                mathmlBuilder: fn
+                htmlBuilder: fn,
+                mathmlBuilder: gn
             }), Q({
                 type: "enclose",
                 names: ["\\fcolorbox"],
                 props: {
                     numArgs: 3,
                     allowedInText: !0,
                     argTypes: ["color", "color", "text"]
@@ -11546,16 +11546,16 @@
                         mode: s.mode,
                         label: u,
                         backgroundColor: b,
                         borderColor: p,
                         body: v
                     }
                 },
-                htmlBuilder: pn,
-                mathmlBuilder: fn
+                htmlBuilder: fn,
+                mathmlBuilder: gn
             }), Q({
                 type: "enclose",
                 names: ["\\fbox"],
                 props: {
                     numArgs: 1,
                     argTypes: ["hbox"],
                     allowedInText: !0
@@ -11585,16 +11585,16 @@
                     return {
                         type: "enclose",
                         mode: o.mode,
                         label: s,
                         body: u
                     }
                 },
-                htmlBuilder: pn,
-                mathmlBuilder: fn
+                htmlBuilder: fn,
+                mathmlBuilder: gn
             }), Q({
                 type: "enclose",
                 names: ["\\angl"],
                 props: {
                     numArgs: 1,
                     argTypes: ["hbox"],
                     allowedInText: !1
@@ -11607,15 +11607,15 @@
                         type: "enclose",
                         mode: o.mode,
                         label: "\\angl",
                         body: t[0]
                     }
                 }
             });
-            let xo = {};
+            let wo = {};
 
             function wt(n) {
                 let {
                     type: t,
                     names: o,
                     props: s,
                     handler: u,
@@ -11624,21 +11624,21 @@
                 } = n, v = {
                     type: t,
                     numArgs: s.numArgs || 0,
                     allowedInText: !1,
                     numOptionalArgs: 0,
                     handler: u
                 };
-                for (let S = 0; S < o.length; ++S) xo[o[S]] = v;
+                for (let S = 0; S < o.length; ++S) wo[o[S]] = v;
                 p && (Zr[t] = p), b && (Qr[t] = b)
             }
-            let vo = {};
+            let ko = {};
 
             function k(n, t) {
-                vo[n] = t
+                ko[n] = t
             }
             class st {
                 constructor(t, o, s) {
                     this.lexer = void 0, this.start = void 0, this.end = void 0, this.lexer = t, this.start = o, this.end = s
                 }
                 static range(t, o) {
                     return o ? !t || !t.loc || !o.loc || t.loc.lexer !== o.loc.lexer ? null : new st(t.loc.lexer, t.loc.start, o.loc.end) : t && t.loc
@@ -11649,26 +11649,26 @@
                     this.text = void 0, this.loc = void 0, this.noexpand = void 0, this.treatAsRelax = void 0, this.text = t, this.loc = o
                 }
                 range(t, o) {
                     return new mt(o, st.range(this, t))
                 }
             }
 
-            function wo(n) {
+            function _o(n) {
                 let t = [];
                 n.consumeSpaces();
                 let o = n.fetch().text;
                 for (o === "\\relax" && (n.consume(), n.consumeSpaces(), o = n.fetch().text); o === "\\hline" || o === "\\hdashline";) n.consume(), t.push(o === "\\hdashline"), n.consumeSpaces(), o = n.fetch().text;
                 return t
             }
             let i0 = n => {
                 if (!n.parser.settings.displayMode) throw new a("{" + n.envName + "} can be used only in display mode.")
             };
 
-            function gn(n) {
+            function bn(n) {
                 if (n.indexOf("ed") === -1) return n.indexOf("*") === -1
             }
 
             function $t(n, t, o) {
                 let {
                     hskipBeforeAndAfter: s,
                     addJot: u,
@@ -11696,15 +11696,15 @@
                 function xe() {
                     S && n.gullet.macros.set("\\@eqnsw", "1", !0)
                 }
 
                 function ke() {
                     ge && (n.gullet.macros.get("\\df@tag") ? (ge.push(n.subparse([new mt("\\df@tag")])), n.gullet.macros.set("\\df@tag", void 0, !0)) : ge.push(!!S && n.gullet.macros.get("\\@eqnsw") === "1"))
                 }
-                for (xe(), ye.push(wo(n));;) {
+                for (xe(), ye.push(_o(n));;) {
                     let ze = n.parseExpression(!1, E ? "\\end" : "\\\\");
                     n.gullet.endGroup(), n.gullet.beginGroup(), ze = {
                         type: "ordgroup",
                         mode: n.mode,
                         body: ze
                     }, o && (ze = {
                         type: "styling",
@@ -11721,15 +11721,15 @@
                         n.consume()
                     } else if (tt === "\\end") {
                         ke(), H.length === 1 && ze.type === "styling" && ze.body[0].body.length === 0 && (K.length > 1 || !z) && K.pop(), ye.length < K.length + 1 && ye.push([]);
                         break
                     } else if (tt === "\\\\") {
                         n.consume();
                         let Qe;
-                        n.gullet.future().text !== " " && (Qe = n.parseSizeGroup(!0)), ie.push(Qe ? Qe.value : null), ke(), ye.push(wo(n)), H = [], K.push(H), xe()
+                        n.gullet.future().text !== " " && (Qe = n.parseSizeGroup(!0)), ie.push(Qe ? Qe.value : null), ke(), ye.push(_o(n)), H = [], K.push(H), xe()
                     } else throw new a("Expected & or \\\\ or \\cr or \\end", n.nextToken)
                 }
                 return n.gullet.endGroup(), n.gullet.endGroup(), {
                     type: "array",
                     mode: n.mode,
                     addJot: u,
                     arraystretch: b,
@@ -11740,15 +11740,15 @@
                     hLinesBeforeRow: ye,
                     colSeparationType: v,
                     tags: ge,
                     leqno: N
                 }
             }
 
-            function bn(n) {
+            function yn(n) {
                 return n.slice(0, 1) === "d" ? "display" : "text"
             }
             let kt = function(n, t) {
                     let o, s, u = n.body.length,
                         p = n.hLinesBeforeRow,
                         b = 0,
                         v = new Array(u),
@@ -11867,15 +11867,15 @@
                         let we = B.makeVList({
                             positionType: "individualShift",
                             children: cr
                         }, t);
                         return we = B.makeSpan(["tag"], [we], t), B.makeFragment([v, we])
                     }
                 },
-                N1 = {
+                P1 = {
                     c: "center ",
                     l: "left ",
                     r: "right "
                 },
                 _t = function(n, t) {
                     let o = [],
                         s = new V.MathNode("mtd", [], ["mtr-glue"]),
@@ -11894,38 +11894,38 @@
                     if (n.cols && n.cols.length > 0) {
                         let F = n.cols,
                             N = "",
                             H = !1,
                             K = 0,
                             ie = F.length;
                         F[0].type === "separator" && (v += "top ", K = 1), F[F.length - 1].type === "separator" && (v += "bottom ", ie -= 1);
-                        for (let ye = K; ye < ie; ye++) F[ye].type === "align" ? (S += N1[F[ye].align], H && (N += "none "), H = !0) : F[ye].type === "separator" && H && (N += F[ye].separator === "|" ? "solid " : "dashed ", H = !1);
+                        for (let ye = K; ye < ie; ye++) F[ye].type === "align" ? (S += P1[F[ye].align], H && (N += "none "), H = !0) : F[ye].type === "separator" && H && (N += F[ye].separator === "|" ? "solid " : "dashed ", H = !1);
                         p.setAttribute("columnalign", S.trim()), /[sd]/.test(N) && p.setAttribute("columnlines", N.trim())
                     }
                     if (n.colSeparationType === "align") {
                         let F = n.cols || [],
                             N = "";
                         for (let H = 1; H < F.length; H++) N += H % 2 ? "0em " : "1em ";
                         p.setAttribute("columnspacing", N.trim())
                     } else n.colSeparationType === "alignat" || n.colSeparationType === "gather" ? p.setAttribute("columnspacing", "0em") : n.colSeparationType === "small" ? p.setAttribute("columnspacing", "0.2778em") : n.colSeparationType === "CD" ? p.setAttribute("columnspacing", "0.5em") : p.setAttribute("columnspacing", "1em");
                     let E = "",
                         z = n.hLinesBeforeRow;
                     v += z[0].length > 0 ? "left " : "", v += z[z.length - 1].length > 0 ? "right " : "";
                     for (let F = 1; F < z.length - 1; F++) E += z[F].length === 0 ? "none " : z[F][0] ? "dashed " : "solid ";
                     return /[sd]/.test(E) && p.setAttribute("rowlines", E.trim()), v !== "" && (p = new V.MathNode("menclose", [p]), p.setAttribute("notation", v.trim())), n.arraystretch && n.arraystretch < 1 && (p = new V.MathNode("mstyle", [p]), p.setAttribute("scriptlevel", "1")), p
                 },
-                ko = function(n, t) {
+                So = function(n, t) {
                     n.envName.indexOf("ed") === -1 && i0(n);
                     let o = [],
                         s = n.envName.indexOf("at") > -1 ? "alignat" : "align",
                         u = n.envName === "split",
                         p = $t(n.parser, {
                             cols: o,
                             addJot: !0,
-                            autoTag: u ? void 0 : gn(n.envName),
+                            autoTag: u ? void 0 : bn(n.envName),
                             emptySingleRow: !0,
                             colSeparationType: s,
                             maxNumCols: u ? 2 : void 0,
                             leqno: n.parser.settings.leqno
                         }, "display"),
                         b, v = 0,
                         S = {
@@ -11969,15 +11969,15 @@
                 type: "array",
                 names: ["array", "darray"],
                 props: {
                     numArgs: 1
                 },
                 handler(n, t) {
                     let u = (Kr(t[0]) ? [t[0]] : de(t[0], "ordgroup").body).map(function(b) {
-                            let S = nn(b).text;
+                            let S = on(b).text;
                             if ("lcr".indexOf(S) !== -1) return {
                                 type: "align",
                                 align: S
                             };
                             if (S === "|") return {
                                 type: "separator",
                                 separator: "|"
@@ -11989,15 +11989,15 @@
                             throw new a("Unknown column alignment: " + S, b)
                         }),
                         p = {
                             cols: u,
                             hskipBeforeAndAfter: !0,
                             maxNumCols: u.length
                         };
-                    return $t(n.parser, p, bn(n.envName))
+                    return $t(n.parser, p, yn(n.envName))
                 },
                 htmlBuilder: kt,
                 mathmlBuilder: _t
             }), wt({
                 type: "array",
                 names: ["matrix", "pmatrix", "bmatrix", "Bmatrix", "vmatrix", "Vmatrix", "matrix*", "pmatrix*", "bmatrix*", "Bmatrix*", "vmatrix*", "Vmatrix*"],
                 props: {
@@ -12026,15 +12026,15 @@
                             if (b.consume(), b.consumeSpaces(), o = b.fetch().text, "lcr".indexOf(o) === -1) throw new a("Expected l or c or r", b.nextToken);
                             b.consume(), b.consumeSpaces(), b.expect("]"), b.consume(), s.cols = [{
                                 type: "align",
                                 align: o
                             }]
                         }
                     }
-                    let u = $t(n.parser, s, bn(n.envName)),
+                    let u = $t(n.parser, s, yn(n.envName)),
                         p = Math.max(0, ...u.body.map(b => b.length));
                     return u.cols = new Array(p).fill({
                         type: "align",
                         align: o
                     }), t ? {
                         type: "leftright",
                         mode: n.mode,
@@ -12065,15 +12065,15 @@
                 type: "array",
                 names: ["subarray"],
                 props: {
                     numArgs: 1
                 },
                 handler(n, t) {
                     let u = (Kr(t[0]) ? [t[0]] : de(t[0], "ordgroup").body).map(function(b) {
-                        let S = nn(b).text;
+                        let S = on(b).text;
                         if ("lc".indexOf(S) !== -1) return {
                             type: "align",
                             align: S
                         };
                         throw new a("Unknown column alignment: " + S, b)
                     });
                     if (u.length > 1) throw new a("{subarray} can contain only one column");
@@ -12104,15 +12104,15 @@
                             }, {
                                 type: "align",
                                 align: "l",
                                 pregap: 0,
                                 postgap: 0
                             }]
                         },
-                        o = $t(n.parser, t, bn(n.envName));
+                        o = $t(n.parser, t, yn(n.envName));
                     return {
                         type: "leftright",
                         mode: n.mode,
                         body: [o],
                         left: n.envName.indexOf("r") > -1 ? "." : "\\{",
                         right: n.envName.indexOf("r") > -1 ? "\\}" : ".",
                         rightColor: void 0
@@ -12122,15 +12122,15 @@
                 mathmlBuilder: _t
             }), wt({
                 type: "array",
                 names: ["align", "align*", "aligned", "split"],
                 props: {
                     numArgs: 0
                 },
-                handler: ko,
+                handler: So,
                 htmlBuilder: kt,
                 mathmlBuilder: _t
             }), wt({
                 type: "array",
                 names: ["gathered", "gather", "gather*"],
                 props: {
                     numArgs: 0
@@ -12140,41 +12140,41 @@
                     let t = {
                         cols: [{
                             type: "align",
                             align: "c"
                         }],
                         addJot: !0,
                         colSeparationType: "gather",
-                        autoTag: gn(n.envName),
+                        autoTag: bn(n.envName),
                         emptySingleRow: !0,
                         leqno: n.parser.settings.leqno
                     };
                     return $t(n.parser, t, "display")
                 },
                 htmlBuilder: kt,
                 mathmlBuilder: _t
             }), wt({
                 type: "array",
                 names: ["alignat", "alignat*", "alignedat"],
                 props: {
                     numArgs: 1
                 },
-                handler: ko,
+                handler: So,
                 htmlBuilder: kt,
                 mathmlBuilder: _t
             }), wt({
                 type: "array",
                 names: ["equation", "equation*"],
                 props: {
                     numArgs: 0
                 },
                 handler(n) {
                     i0(n);
                     let t = {
-                        autoTag: gn(n.envName),
+                        autoTag: bn(n.envName),
                         emptySingleRow: !0,
                         singleRow: !0,
                         maxNumCols: 1,
                         leqno: n.parser.settings.leqno
                     };
                     return $t(n.parser, t, "display")
                 },
@@ -12183,15 +12183,15 @@
             }), wt({
                 type: "array",
                 names: ["CD"],
                 props: {
                     numArgs: 0
                 },
                 handler(n) {
-                    return i0(n), _1(n.parser)
+                    return i0(n), C1(n.parser)
                 },
                 htmlBuilder: kt,
                 mathmlBuilder: _t
             }), k("\\nonumber", "\\gdef\\@eqnsw{0}"), k("\\notag", "\\nonumber"), Q({
                 type: "text",
                 names: ["\\hline", "\\hdashline"],
                 props: {
@@ -12199,15 +12199,15 @@
                     allowedInText: !0,
                     allowedInMath: !0
                 },
                 handler(n, t) {
                     throw new a(n.funcName + " valid only within array environment")
                 }
             });
-            var _o = xo;
+            var Co = wo;
             Q({
                 type: "environment",
                 names: ["\\begin", "\\end"],
                 props: {
                     numArgs: 1,
                     argTypes: ["text"]
                 },
@@ -12216,16 +12216,16 @@
                         parser: o,
                         funcName: s
                     } = n, u = t[0];
                     if (u.type !== "ordgroup") throw new a("Invalid environment name", u);
                     let p = "";
                     for (let b = 0; b < u.body.length; ++b) p += de(u.body[b], "textord").text;
                     if (s === "\\begin") {
-                        if (!_o.hasOwnProperty(p)) throw new a("No such environment: " + p, u);
-                        let b = _o[p],
+                        if (!Co.hasOwnProperty(p)) throw new a("No such environment: " + p, u);
+                        let b = Co[p],
                             {
                                 args: v,
                                 optArgs: S
                             } = o.parseArguments("\\begin{" + p + "}", b),
                             E = {
                                 mode: o.mode,
                                 envName: p,
@@ -12242,25 +12242,25 @@
                         type: "environment",
                         mode: o.mode,
                         name: p,
                         nameGroup: u
                     }
                 }
             });
-            let So = (n, t) => {
+            let To = (n, t) => {
                     let o = n.font,
                         s = t.withFont(o);
                     return ve(n.body, s)
                 },
-                Co = (n, t) => {
+                Ao = (n, t) => {
                     let o = n.font,
                         s = t.withFont(o);
                     return Ee(n.body, s)
                 },
-                To = {
+                qo = {
                     "\\Bbb": "\\mathbb",
                     "\\bold": "\\mathbf",
                     "\\frak": "\\mathfrak",
                     "\\bm": "\\boldsymbol"
                 };
             Q({
                 type: "font",
@@ -12270,23 +12270,23 @@
                     allowedInArgument: !0
                 },
                 handler: (n, t) => {
                     let {
                         parser: o,
                         funcName: s
                     } = n, u = Xr(t[0]), p = s;
-                    return p in To && (p = To[p]), {
+                    return p in qo && (p = qo[p]), {
                         type: "font",
                         mode: o.mode,
                         font: p.slice(1),
                         body: u
                     }
                 },
-                htmlBuilder: So,
-                mathmlBuilder: Co
+                htmlBuilder: To,
+                mathmlBuilder: Ao
             }), Q({
                 type: "mclass",
                 names: ["\\boldsymbol", "\\bm"],
                 props: {
                     numArgs: 1
                 },
                 handler: (n, t) => {
@@ -12328,23 +12328,23 @@
                         body: {
                             type: "ordgroup",
                             mode: o.mode,
                             body: b
                         }
                     }
                 },
-                htmlBuilder: So,
-                mathmlBuilder: Co
+                htmlBuilder: To,
+                mathmlBuilder: Ao
             });
-            let Ao = (n, t) => {
+            let Mo = (n, t) => {
                     let o = t;
                     return n === "display" ? o = o.id >= G.SCRIPT.id ? o.text() : G.DISPLAY : n === "text" && o.size === G.DISPLAY.size ? o = G.TEXT : n === "script" ? o = G.SCRIPT : n === "scriptscript" && (o = G.SCRIPTSCRIPT), o
                 },
-                yn = (n, t) => {
-                    let o = Ao(n.size, t.style),
+                xn = (n, t) => {
+                    let o = Mo(n.size, t.style),
                         s = o.fracNum(),
                         u = o.fracDen(),
                         p;
                     p = t.havingStyle(s);
                     let b = ve(n.numer, p, t);
                     if (n.continued) {
                         let xe = 8.5 / t.fontMetrics().ptPerEm,
@@ -12395,22 +12395,22 @@
                     }
                     p = t.havingStyle(o), K.height *= p.sizeMultiplier / t.sizeMultiplier, K.depth *= p.sizeMultiplier / t.sizeMultiplier;
                     let ie;
                     o.size === G.DISPLAY.size ? ie = t.fontMetrics().delim1 : o.size === G.SCRIPTSCRIPT.size ? ie = t.havingStyle(G.SCRIPT).fontMetrics().delim2 : ie = t.fontMetrics().delim2;
                     let ye, ge;
                     return n.leftDelim == null ? ye = wr(t, ["mopen"]) : ye = Bt.customSizedDelim(n.leftDelim, ie, !0, t.havingStyle(o), n.mode, ["mopen"]), n.continued ? ge = B.makeSpan([]) : n.rightDelim == null ? ge = wr(t, ["mclose"]) : ge = Bt.customSizedDelim(n.rightDelim, ie, !0, t.havingStyle(o), n.mode, ["mclose"]), B.makeSpan(["mord"].concat(p.sizingClasses(t)), [ye, B.makeSpan(["mfrac"], [K]), ge], t)
                 },
-                xn = (n, t) => {
+                vn = (n, t) => {
                     let o = new V.MathNode("mfrac", [Ee(n.numer, t), Ee(n.denom, t)]);
                     if (!n.hasBarLine) o.setAttribute("linethickness", "0px");
                     else if (n.barSize) {
                         let u = Ie(n.barSize, t);
                         o.setAttribute("linethickness", Z(u))
                     }
-                    let s = Ao(n.size, t.style);
+                    let s = Mo(n.size, t.style);
                     if (s.size !== t.style.size) {
                         o = new V.MathNode("mstyle", [o]);
                         let u = s.size === G.DISPLAY.size ? "true" : "false";
                         o.setAttribute("displaystyle", u), o.setAttribute("scriptlevel", "0")
                     }
                     if (n.leftDelim != null || n.rightDelim != null) {
                         let u = [];
@@ -12418,15 +12418,15 @@
                             let p = new V.MathNode("mo", [new V.TextNode(n.leftDelim.replace("\\", ""))]);
                             p.setAttribute("fence", "true"), u.push(p)
                         }
                         if (u.push(o), n.rightDelim != null) {
                             let p = new V.MathNode("mo", [new V.TextNode(n.rightDelim.replace("\\", ""))]);
                             p.setAttribute("fence", "true"), u.push(p)
                         }
-                        return tn(u)
+                        return rn(u)
                     }
                     return o
                 };
             Q({
                 type: "genfrac",
                 names: ["\\dfrac", "\\frac", "\\tfrac", "\\dbinom", "\\binom", "\\tbinom", "\\\\atopfrac", "\\\\bracefrac", "\\\\brackfrac"],
                 props: {
@@ -12480,16 +12480,16 @@
                         hasBarLine: b,
                         leftDelim: v,
                         rightDelim: S,
                         size: E,
                         barSize: null
                     }
                 },
-                htmlBuilder: yn,
-                mathmlBuilder: xn
+                htmlBuilder: xn,
+                mathmlBuilder: vn
             }), Q({
                 type: "genfrac",
                 names: ["\\cfrac"],
                 props: {
                     numArgs: 2
                 },
                 handler: (n, t) => {
@@ -12546,55 +12546,55 @@
                         type: "infix",
                         mode: t.mode,
                         replaceWith: u,
                         token: s
                     }
                 }
             });
-            let qo = ["display", "text", "script", "scriptscript"],
-                Mo = function(n) {
+            let Eo = ["display", "text", "script", "scriptscript"],
+                Do = function(n) {
                     let t = null;
                     return n.length > 0 && (t = n, t = t === "." ? null : t), t
                 };
             Q({
                 type: "genfrac",
                 names: ["\\genfrac"],
                 props: {
                     numArgs: 6,
                     allowedInArgument: !0,
                     argTypes: ["math", "math", "size", "text", "math", "math"]
                 },
                 handler(n, t) {
                     let {
                         parser: o
-                    } = n, s = t[4], u = t[5], p = Xr(t[0]), b = p.type === "atom" && p.family === "open" ? Mo(p.text) : null, v = Xr(t[1]), S = v.type === "atom" && v.family === "close" ? Mo(v.text) : null, E = de(t[2], "size"), z, F = null;
+                    } = n, s = t[4], u = t[5], p = Xr(t[0]), b = p.type === "atom" && p.family === "open" ? Do(p.text) : null, v = Xr(t[1]), S = v.type === "atom" && v.family === "close" ? Do(v.text) : null, E = de(t[2], "size"), z, F = null;
                     E.isBlank ? z = !0 : (F = E.value, z = F.number > 0);
                     let N = "auto",
                         H = t[3];
                     if (H.type === "ordgroup") {
                         if (H.body.length > 0) {
                             let K = de(H.body[0], "textord");
-                            N = qo[Number(K.text)]
+                            N = Eo[Number(K.text)]
                         }
-                    } else H = de(H, "textord"), N = qo[Number(H.text)];
+                    } else H = de(H, "textord"), N = Eo[Number(H.text)];
                     return {
                         type: "genfrac",
                         mode: o.mode,
                         numer: s,
                         denom: u,
                         continued: !1,
                         hasBarLine: z,
                         barSize: F,
                         leftDelim: b,
                         rightDelim: S,
                         size: N
                     }
                 },
-                htmlBuilder: yn,
-                mathmlBuilder: xn
+                htmlBuilder: xn,
+                mathmlBuilder: vn
             }), Q({
                 type: "infix",
                 names: ["\\above"],
                 props: {
                     numArgs: 1,
                     argTypes: ["size"],
                     infix: !0
@@ -12634,18 +12634,18 @@
                         hasBarLine: v,
                         barSize: p,
                         leftDelim: null,
                         rightDelim: null,
                         size: "auto"
                     }
                 },
-                htmlBuilder: yn,
-                mathmlBuilder: xn
+                htmlBuilder: xn,
+                mathmlBuilder: vn
             });
-            let Eo = (n, t) => {
+            let zo = (n, t) => {
                 let o = t.style,
                     s, u;
                 n.type === "supsub" ? (s = n.sup ? ve(n.sup, t.havingStyle(o.sup()), t) : ve(n.sub, t.havingStyle(o.sub()), t), u = de(n.base, "horizBrace")) : u = de(n, "horizBrace");
                 let p = ve(u.base, t.havingBaseStyle(G.DISPLAY)),
                     b = Ft.svgSpan(u, t),
                     v;
                 if (u.isOver ? (v = B.makeVList({
@@ -12719,15 +12719,15 @@
                         type: "horizBrace",
                         mode: o.mode,
                         label: s,
                         isOver: /^\\over/.test(s),
                         base: t[0]
                     }
                 },
-                htmlBuilder: Eo,
+                htmlBuilder: zo,
                 mathmlBuilder: (n, t) => {
                     let o = Ft.mathMLnode(n.label);
                     return new V.MathNode(n.isOver ? "mover" : "munder", [Ee(n.base, t), o])
                 }
             }), Q({
                 type: "href",
                 names: ["\\href"],
@@ -12909,27 +12909,27 @@
                 },
                 htmlBuilder: (n, t) => {
                     let o = Ze(n.html, t, !1);
                     return B.makeFragment(o)
                 },
                 mathmlBuilder: (n, t) => Ht(n.mathml, t)
             });
-            let vn = function(n) {
+            let wn = function(n) {
                 if (/^[-+]? *(\d+(\.\d*)?|\.\d+)$/.test(n)) return {
                     number: +n,
                     unit: "bp"
                 };
                 {
                     let t = /([-+]?) *(\d+(?:\.\d*)?|\.\d+) *([a-z]{2})/.exec(n);
                     if (!t) throw new a("Invalid size: '" + n + "' in \\includegraphics");
                     let o = {
                         number: +(t[1] + t[2]),
                         unit: t[3]
                     };
-                    if (!Fi(o)) throw new a("Invalid unit: '" + o.unit + "' in \\includegraphics.");
+                    if (!Ni(o)) throw new a("Invalid unit: '" + o.unit + "' in \\includegraphics.");
                     return o
                 }
             };
             Q({
                 type: "includegraphics",
                 names: ["\\includegraphics"],
                 props: {
@@ -12958,21 +12958,21 @@
                             if (N.length === 2) {
                                 let H = N[1].trim();
                                 switch (N[0].trim()) {
                                     case "alt":
                                         v = H;
                                         break;
                                     case "width":
-                                        u = vn(H);
+                                        u = wn(H);
                                         break;
                                     case "height":
-                                        p = vn(H);
+                                        p = wn(H);
                                         break;
                                     case "totalheight":
-                                        b = vn(H);
+                                        b = wn(H);
                                         break;
                                     default:
                                         throw new a("Invalid key: '" + N[0] + "' in \\includegraphics.")
                                 }
                             }
                         }
                     }
@@ -12996,15 +12996,15 @@
                     n.totalheight.number > 0 && (s = Ie(n.totalheight, t) - o);
                     let u = 0;
                     n.width.number > 0 && (u = Ie(n.width, t));
                     let p = {
                         height: Z(o + s)
                     };
                     u > 0 && (p.width = Z(u)), s > 0 && (p.verticalAlign = Z(-s));
-                    let b = new $u(n.src, n.alt, p);
+                    let b = new Vu(n.src, n.alt, p);
                     return b.height = o, b.depth = s, b
                 },
                 mathmlBuilder: (n, t) => {
                     let o = new V.MathNode("mglyph", []);
                     o.setAttribute("alt", n.alt);
                     let s = Ie(n.height, t),
                         u = 0;
@@ -13112,15 +13112,15 @@
                     allowedInText: !0,
                     allowedInMath: !1
                 },
                 handler(n, t) {
                     throw new a("Mismatched " + n.funcName)
                 }
             });
-            let Do = (n, t) => {
+            let Ro = (n, t) => {
                 switch (t.style.size) {
                     case G.DISPLAY.size:
                         return n.display;
                     case G.TEXT.size:
                         return n.text;
                     case G.SCRIPT.size:
                         return n.script;
@@ -13147,24 +13147,24 @@
                         display: je(t[0]),
                         text: je(t[1]),
                         script: je(t[2]),
                         scriptscript: je(t[3])
                     }
                 },
                 htmlBuilder: (n, t) => {
-                    let o = Do(n, t),
+                    let o = Ro(n, t),
                         s = Ze(o, t, !1);
                     return B.makeFragment(s)
                 },
                 mathmlBuilder: (n, t) => {
-                    let o = Do(n, t);
+                    let o = Ro(n, t);
                     return Ht(o, t)
                 }
             });
-            let zo = (n, t, o, s, u, p, b) => {
+            let Fo = (n, t, o, s, u, p, b) => {
                     n = B.makeSpan([], [n]);
                     let v = o && R.isCharacterBox(o),
                         S, E;
                     if (t) {
                         let N = ve(t, s.havingStyle(u.sup()), s);
                         E = {
                             elem: N,
@@ -13253,22 +13253,22 @@
                     let F = [z];
                     if (S && p !== 0 && !v) {
                         let N = B.makeSpan(["mspace"], [], s);
                         N.style.marginRight = Z(p), F.unshift(N)
                     }
                     return B.makeSpan(["mop", "op-limits"], F, s)
                 },
-                Ro = ["\\smallint"],
+                Bo = ["\\smallint"],
                 lr = (n, t) => {
                     let o, s, u = !1,
                         p;
                     n.type === "supsub" ? (o = n.sup, s = n.sub, p = de(n.base, "op"), u = !0) : p = de(n, "op");
                     let b = t.style,
                         v = !1;
-                    b.size === G.DISPLAY.size && p.symbol && !R.contains(Ro, p.name) && (v = !0);
+                    b.size === G.DISPLAY.size && p.symbol && !R.contains(Bo, p.name) && (v = !0);
                     let S;
                     if (p.symbol) {
                         let F = v ? "Size2-Regular" : "Size1-Regular",
                             N = "";
                         if ((p.name === "\\oiint" || p.name === "\\oiiint") && (N = p.name.slice(1), p.name = N === "oiint" ? "\\iint" : "\\iiint"), S = B.makeSymbol(p.name, F, "math", t, ["mop", "op-symbol", v ? "large-op" : "small-op"]), N.length > 0) {
                             let H = S.italic,
                                 K = B.staticSvg(N + "Size" + (v ? "2" : "1"), t);
@@ -13291,28 +13291,28 @@
                     } else {
                         let F = [];
                         for (let N = 1; N < p.name.length; N++) F.push(B.mathsym(p.name[N], p.mode, t));
                         S = B.makeSpan(["mop"], F, t)
                     }
                     let E = 0,
                         z = 0;
-                    return (S instanceof ut || p.name === "\\oiint" || p.name === "\\oiiint") && !p.suppressBaseShift && (E = (S.height - S.depth) / 2 - t.fontMetrics().axisHeight, z = S.italic), u ? zo(S, o, s, t, b, z, E) : (E && (S.style.position = "relative", S.style.top = Z(E)), S)
+                    return (S instanceof ut || p.name === "\\oiint" || p.name === "\\oiiint") && !p.suppressBaseShift && (E = (S.height - S.depth) / 2 - t.fontMetrics().axisHeight, z = S.italic), u ? Fo(S, o, s, t, b, z, E) : (E && (S.style.position = "relative", S.style.top = Z(E)), S)
                 },
                 Cr = (n, t) => {
                     let o;
-                    if (n.symbol) o = new ht("mo", [dt(n.name, n.mode)]), R.contains(Ro, n.name) && o.setAttribute("largeop", "false");
+                    if (n.symbol) o = new ht("mo", [dt(n.name, n.mode)]), R.contains(Bo, n.name) && o.setAttribute("largeop", "false");
                     else if (n.body) o = new ht("mo", it(n.body, t));
                     else {
                         o = new ht("mi", [new kr(n.name.slice(1))]);
                         let s = new ht("mo", [dt("\u2061", "text")]);
-                        n.parentIsSupSub ? o = new ht("mrow", [o, s]) : o = Zi([o, s])
+                        n.parentIsSupSub ? o = new ht("mrow", [o, s]) : o = Xi([o, s])
                     }
                     return o
                 },
-                L1 = {
+                I1 = {
                     "\u220F": "\\prod",
                     "\u2210": "\\coprod",
                     "\u2211": "\\sum",
                     "\u22C0": "\\bigwedge",
                     "\u22C1": "\\bigvee",
                     "\u22C2": "\\bigcap",
                     "\u22C3": "\\bigcup",
@@ -13329,15 +13329,15 @@
                     numArgs: 0
                 },
                 handler: (n, t) => {
                     let {
                         parser: o,
                         funcName: s
                     } = n, u = s;
-                    return u.length === 1 && (u = L1[u]), {
+                    return u.length === 1 && (u = I1[u]), {
                         type: "op",
                         mode: o.mode,
                         limits: !0,
                         parentIsSupSub: !1,
                         symbol: !0,
                         name: u
                     }
@@ -13363,15 +13363,15 @@
                         symbol: !1,
                         body: je(s)
                     }
                 },
                 htmlBuilder: lr,
                 mathmlBuilder: Cr
             });
-            let P1 = {
+            let O1 = {
                 "\u222B": "\\int",
                 "\u222C": "\\iint",
                 "\u222D": "\\iiint",
                 "\u222E": "\\oint",
                 "\u222F": "\\oiint",
                 "\u2230": "\\oiiint"
             };
@@ -13426,27 +13426,27 @@
                     numArgs: 0
                 },
                 handler(n) {
                     let {
                         parser: t,
                         funcName: o
                     } = n, s = o;
-                    return s.length === 1 && (s = P1[s]), {
+                    return s.length === 1 && (s = O1[s]), {
                         type: "op",
                         mode: t.mode,
                         limits: !1,
                         parentIsSupSub: !1,
                         symbol: !0,
                         name: s
                     }
                 },
                 htmlBuilder: lr,
                 mathmlBuilder: Cr
             });
-            let Fo = (n, t) => {
+            let No = (n, t) => {
                 let o, s, u = !1,
                     p;
                 n.type === "supsub" ? (o = n.sup, s = n.sub, p = de(n.base, "operatorname"), u = !0) : p = de(n, "operatorname");
                 let b;
                 if (p.body.length > 0) {
                     let v = p.body.map(E => {
                             let z = E.text;
@@ -13459,15 +13459,15 @@
                         S = Ze(v, t.withFont("mathrm"), !0);
                     for (let E = 0; E < S.length; E++) {
                         let z = S[E];
                         z instanceof ut && (z.text = z.text.replace(/\u2212/, "-").replace(/\u2217/, "*"))
                     }
                     b = B.makeSpan(["mop"], S, t)
                 } else b = B.makeSpan(["mop"], [], t);
-                return u ? zo(b, o, s, t, t.style, 0, 0) : b
+                return u ? Fo(b, o, s, t, t.style, 0, 0) : b
             };
             Q({
                 type: "operatorname",
                 names: ["\\operatorname@", "\\operatornamewithlimits"],
                 props: {
                     numArgs: 1
                 },
@@ -13481,15 +13481,15 @@
                         mode: o.mode,
                         body: je(u),
                         alwaysHandleSupSub: s === "\\operatornamewithlimits",
                         limits: !1,
                         parentIsSupSub: !1
                     }
                 },
-                htmlBuilder: Fo,
+                htmlBuilder: No,
                 mathmlBuilder: (n, t) => {
                     let o = it(n.body, t.withFont("mathrm")),
                         s = !0;
                     for (let b = 0; b < o.length; b++) {
                         let v = o[b];
                         if (!(v instanceof V.SpaceNode))
                             if (v instanceof V.MathNode) switch (v.type) {
@@ -13744,47 +13744,47 @@
                         b = new V.MathNode("mspace");
                     b.setAttribute("mathbackground", p), b.setAttribute("width", Z(o)), b.setAttribute("height", Z(s));
                     let v = new V.MathNode("mpadded", [b]);
                     return u >= 0 ? v.setAttribute("height", Z(u)) : (v.setAttribute("height", Z(u)), v.setAttribute("depth", Z(-u))), v.setAttribute("voffset", Z(u)), v
                 }
             });
 
-            function Bo(n, t, o) {
+            function Lo(n, t, o) {
                 let s = Ze(n, t, !1),
                     u = t.sizeMultiplier / o.sizeMultiplier;
                 for (let p = 0; p < s.length; p++) {
                     let b = s[p].classes.indexOf("sizing");
                     b < 0 ? Array.prototype.push.apply(s[p].classes, t.sizingClasses(o)) : s[p].classes[b + 1] === "reset-size" + t.size && (s[p].classes[b + 1] = "reset-size" + o.size), s[p].height *= u, s[p].depth *= u
                 }
                 return B.makeFragment(s)
             }
-            let No = ["\\tiny", "\\sixptsize", "\\scriptsize", "\\footnotesize", "\\small", "\\normalsize", "\\large", "\\Large", "\\LARGE", "\\huge", "\\Huge"];
+            let Po = ["\\tiny", "\\sixptsize", "\\scriptsize", "\\footnotesize", "\\small", "\\normalsize", "\\large", "\\Large", "\\LARGE", "\\huge", "\\Huge"];
             Q({
                 type: "sizing",
-                names: No,
+                names: Po,
                 props: {
                     numArgs: 0,
                     allowedInText: !0
                 },
                 handler: (n, t) => {
                     let {
                         breakOnTokenText: o,
                         funcName: s,
                         parser: u
                     } = n, p = u.parseExpression(!1, o);
                     return {
                         type: "sizing",
                         mode: u.mode,
-                        size: No.indexOf(s) + 1,
+                        size: Po.indexOf(s) + 1,
                         body: p
                     }
                 },
                 htmlBuilder: (n, t) => {
                     let o = t.havingSize(n.size);
-                    return Bo(n.body, o, t)
+                    return Lo(n.body, o, t)
                 },
                 mathmlBuilder: (n, t) => {
                     let o = t.havingSize(n.size),
                         s = it(n.body, o),
                         u = new V.MathNode("mstyle", s);
                     return u.setAttribute("mathsize", Z(o.sizeMultiplier)), u
                 }
@@ -13911,15 +13911,15 @@
                     let {
                         body: o,
                         index: s
                     } = n;
                     return s ? new V.MathNode("mroot", [Ee(o, t), Ee(s, t)]) : new V.MathNode("msqrt", [Ee(o, t)])
                 }
             });
-            let Lo = {
+            let Io = {
                 display: G.DISPLAY,
                 text: G.TEXT,
                 script: G.SCRIPT,
                 scriptscript: G.SCRIPTSCRIPT
             };
             Q({
                 type: "styling",
@@ -13939,40 +13939,40 @@
                         type: "styling",
                         mode: u.mode,
                         style: b,
                         body: p
                     }
                 },
                 htmlBuilder(n, t) {
-                    let o = Lo[n.style],
+                    let o = Io[n.style],
                         s = t.havingStyle(o).withFont("");
-                    return Bo(n.body, s, t)
+                    return Lo(n.body, s, t)
                 },
                 mathmlBuilder(n, t) {
-                    let o = Lo[n.style],
+                    let o = Io[n.style],
                         s = t.havingStyle(o),
                         u = it(n.body, s),
                         p = new V.MathNode("mstyle", u),
                         v = {
                             display: ["0", "true"],
                             text: ["0", "false"],
                             script: ["1", "false"],
                             scriptscript: ["2", "false"]
                         } [n.style];
                     return p.setAttribute("scriptlevel", v[0]), p.setAttribute("displaystyle", v[1]), p
                 }
             });
-            let I1 = function(n, t) {
+            let H1 = function(n, t) {
                 let o = n.base;
-                return o ? o.type === "op" ? o.limits && (t.style.size === G.DISPLAY.size || o.alwaysHandleSupSub) ? lr : null : o.type === "operatorname" ? o.alwaysHandleSupSub && (t.style.size === G.DISPLAY.size || o.limits) ? Fo : null : o.type === "accent" ? R.isCharacterBox(o.base) ? on : null : o.type === "horizBrace" && !n.sub === o.isOver ? Eo : null : null
+                return o ? o.type === "op" ? o.limits && (t.style.size === G.DISPLAY.size || o.alwaysHandleSupSub) ? lr : null : o.type === "operatorname" ? o.alwaysHandleSupSub && (t.style.size === G.DISPLAY.size || o.limits) ? No : null : o.type === "accent" ? R.isCharacterBox(o.base) ? an : null : o.type === "horizBrace" && !n.sub === o.isOver ? zo : null : null
             };
             Kt({
                 type: "supsub",
                 htmlBuilder(n, t) {
-                    let o = I1(n, t);
+                    let o = H1(n, t);
                     if (o) return o(n, t);
                     let {
                         base: s,
                         sup: u,
                         sub: p
                     } = n, b = ve(s, t), v, S, E = t.fontMetrics(), z = 0, F = 0, N = s && R.isCharacterBox(s);
                     if (u) {
@@ -14036,15 +14036,15 @@
                         children: [{
                             type: "elem",
                             elem: v,
                             marginRight: ie
                         }]
                     }, t);
                     else throw new Error("supsub must have either sup or sub.");
-                    let xe = K0(b, "right") || "mord";
+                    let xe = en(b, "right") || "mord";
                     return B.makeSpan([xe], [b, B.makeSpan(["msupsub"], [ge])], t)
                 },
                 mathmlBuilder(n, t) {
                     let o = !1,
                         s, u;
                     n.base && n.base.type === "horizBrace" && (u = !!n.sup, u === n.base.isOver && (o = !0, s = n.base.isOver)), n.base && (n.base.type === "op" || n.base.type === "operatorname") && (n.base.parentIsSupSub = !0);
                     let p = [Ee(n.base, t)];
@@ -14069,115 +14069,115 @@
                 type: "atom",
                 htmlBuilder(n, t) {
                     return B.mathsym(n.text, n.mode, t, ["m" + n.family])
                 },
                 mathmlBuilder(n, t) {
                     let o = new V.MathNode("mo", [dt(n.text, n.mode)]);
                     if (n.family === "bin") {
-                        let s = rn(n, t);
+                        let s = nn(n, t);
                         s === "bold-italic" && o.setAttribute("mathvariant", s)
                     } else n.family === "punct" ? o.setAttribute("separator", "true") : (n.family === "open" || n.family === "close") && o.setAttribute("stretchy", "false");
                     return o
                 }
             });
-            let Po = {
+            let Oo = {
                 mi: "italic",
                 mn: "normal",
                 mtext: "normal"
             };
             Kt({
                 type: "mathord",
                 htmlBuilder(n, t) {
                     return B.makeOrd(n, t, "mathord")
                 },
                 mathmlBuilder(n, t) {
                     let o = new V.MathNode("mi", [dt(n.text, n.mode, t)]),
-                        s = rn(n, t) || "italic";
-                    return s !== Po[o.type] && o.setAttribute("mathvariant", s), o
+                        s = nn(n, t) || "italic";
+                    return s !== Oo[o.type] && o.setAttribute("mathvariant", s), o
                 }
             }), Kt({
                 type: "textord",
                 htmlBuilder(n, t) {
                     return B.makeOrd(n, t, "textord")
                 },
                 mathmlBuilder(n, t) {
                     let o = dt(n.text, n.mode, t),
-                        s = rn(n, t) || "normal",
+                        s = nn(n, t) || "normal",
                         u;
-                    return n.mode === "text" ? u = new V.MathNode("mtext", [o]) : /[0-9]/.test(n.text) ? u = new V.MathNode("mn", [o]) : n.text === "\\prime" ? u = new V.MathNode("mo", [o]) : u = new V.MathNode("mi", [o]), s !== Po[u.type] && u.setAttribute("mathvariant", s), u
+                    return n.mode === "text" ? u = new V.MathNode("mtext", [o]) : /[0-9]/.test(n.text) ? u = new V.MathNode("mn", [o]) : n.text === "\\prime" ? u = new V.MathNode("mo", [o]) : u = new V.MathNode("mi", [o]), s !== Oo[u.type] && u.setAttribute("mathvariant", s), u
                 }
             });
-            let wn = {
+            let kn = {
                     "\\nobreak": "nobreak",
                     "\\allowbreak": "allowbreak"
                 },
-                kn = {
+                _n = {
                     " ": {},
                     "\\ ": {},
                     "~": {
                         className: "nobreak"
                     },
                     "\\space": {},
                     "\\nobreakspace": {
                         className: "nobreak"
                     }
                 };
             Kt({
                 type: "spacing",
                 htmlBuilder(n, t) {
-                    if (kn.hasOwnProperty(n.text)) {
-                        let o = kn[n.text].className || "";
+                    if (_n.hasOwnProperty(n.text)) {
+                        let o = _n[n.text].className || "";
                         if (n.mode === "text") {
                             let s = B.makeOrd(n, t, "textord");
                             return s.classes.push(o), s
                         } else return B.makeSpan(["mspace", o], [B.mathsym(n.text, n.mode, t)], t)
                     } else {
-                        if (wn.hasOwnProperty(n.text)) return B.makeSpan(["mspace", wn[n.text]], [], t);
+                        if (kn.hasOwnProperty(n.text)) return B.makeSpan(["mspace", kn[n.text]], [], t);
                         throw new a('Unknown type of space "' + n.text + '"')
                     }
                 },
                 mathmlBuilder(n, t) {
                     let o;
-                    if (kn.hasOwnProperty(n.text)) o = new V.MathNode("mtext", [new V.TextNode("\xA0")]);
+                    if (_n.hasOwnProperty(n.text)) o = new V.MathNode("mtext", [new V.TextNode("\xA0")]);
                     else {
-                        if (wn.hasOwnProperty(n.text)) return new V.MathNode("mspace");
+                        if (kn.hasOwnProperty(n.text)) return new V.MathNode("mspace");
                         throw new a('Unknown type of space "' + n.text + '"')
                     }
                     return o
                 }
             });
-            let Io = () => {
+            let Ho = () => {
                 let n = new V.MathNode("mtd", []);
                 return n.setAttribute("width", "50%"), n
             };
             Kt({
                 type: "tag",
                 mathmlBuilder(n, t) {
-                    let o = new V.MathNode("mtable", [new V.MathNode("mtr", [Io(), new V.MathNode("mtd", [Ht(n.body, t)]), Io(), new V.MathNode("mtd", [Ht(n.tag, t)])])]);
+                    let o = new V.MathNode("mtable", [new V.MathNode("mtr", [Ho(), new V.MathNode("mtd", [Ht(n.body, t)]), Ho(), new V.MathNode("mtd", [Ht(n.tag, t)])])]);
                     return o.setAttribute("width", "100%"), o
                 }
             });
-            let Oo = {
+            let $o = {
                     "\\text": void 0,
                     "\\textrm": "textrm",
                     "\\textsf": "textsf",
                     "\\texttt": "texttt",
                     "\\textnormal": "textrm"
                 },
-                Ho = {
+                Go = {
                     "\\textbf": "textbf",
                     "\\textmd": "textmd"
                 },
-                O1 = {
+                $1 = {
                     "\\textit": "textit",
                     "\\textup": "textup"
                 },
-                $o = (n, t) => {
+                Vo = (n, t) => {
                     let o = n.font;
-                    return o ? Oo[o] ? t.withTextFontFamily(Oo[o]) : Ho[o] ? t.withTextFontWeight(Ho[o]) : t.withTextFontShape(O1[o]) : t
+                    return o ? $o[o] ? t.withTextFontFamily($o[o]) : Go[o] ? t.withTextFontWeight(Go[o]) : t.withTextFontShape($1[o]) : t
                 };
             Q({
                 type: "text",
                 names: ["\\text", "\\textrm", "\\textsf", "\\texttt", "\\textnormal", "\\textbf", "\\textmd", "\\textit", "\\textup"],
                 props: {
                     numArgs: 1,
                     argTypes: ["text"],
@@ -14193,20 +14193,20 @@
                         type: "text",
                         mode: o.mode,
                         body: je(u),
                         font: s
                     }
                 },
                 htmlBuilder(n, t) {
-                    let o = $o(n, t),
+                    let o = Vo(n, t),
                         s = Ze(n.body, o, !0);
                     return B.makeSpan(["mord", "text"], s, o)
                 },
                 mathmlBuilder(n, t) {
-                    let o = $o(n, t);
+                    let o = Vo(n, t);
                     return Ht(n.body, o)
                 }
             }), Q({
                 type: "underline",
                 names: ["\\underline"],
                 props: {
                     numArgs: 1,
@@ -14292,45 +14292,45 @@
                     numArgs: 0,
                     allowedInText: !0
                 },
                 handler(n, t, o) {
                     throw new a("\\verb ended by end of line instead of matching delimiter")
                 },
                 htmlBuilder(n, t) {
-                    let o = Go(n),
+                    let o = jo(n),
                         s = [],
                         u = t.havingStyle(t.style.text());
                     for (let p = 0; p < o.length; p++) {
                         let b = o[p];
                         b === "~" && (b = "\\textasciitilde"), s.push(B.makeSymbol(b, "Typewriter-Regular", n.mode, u, ["mord", "texttt"]))
                     }
                     return B.makeSpan(["mord", "text"].concat(u.sizingClasses(t)), B.tryCombineChars(s), u)
                 },
                 mathmlBuilder(n, t) {
-                    let o = new V.TextNode(Go(n)),
+                    let o = new V.TextNode(jo(n)),
                         s = new V.MathNode("mtext", [o]);
                     return s.setAttribute("mathvariant", "monospace"), s
                 }
             });
-            let Go = n => n.body.replace(/ /g, n.star ? "\u2423" : "\xA0");
-            var Gt = Wi;
-            let Vo = `[ \r
+            let jo = n => n.body.replace(/ /g, n.star ? "\u2423" : "\xA0");
+            var Gt = Zi;
+            let Uo = `[ \r
 	]`,
-                H1 = "\\\\[a-zA-Z@]+",
-                $1 = "\\\\[^\uD800-\uDFFF]",
-                G1 = "(" + H1 + ")" + Vo + "*",
-                V1 = `\\\\(
+                G1 = "\\\\[a-zA-Z@]+",
+                V1 = "\\\\[^\uD800-\uDFFF]",
+                j1 = "(" + G1 + ")" + Uo + "*",
+                U1 = `\\\\(
 |[ \r	]+
 ?)[ \r	]*`,
-                _n = "[\u0300-\u036F]",
-                j1 = new RegExp(_n + "+$"),
-                U1 = "(" + Vo + "+)|" + (V1 + "|") + "([!-\\[\\]-\u2027\u202A-\uD7FF\uF900-\uFFFF]" + (_n + "*") + "|[\uD800-\uDBFF][\uDC00-\uDFFF]" + (_n + "*") + "|\\\\verb\\*([^]).*?\\4|\\\\verb([^*a-zA-Z]).*?\\5" + ("|" + G1) + ("|" + $1 + ")");
-            class jo {
+                Sn = "[\u0300-\u036F]",
+                W1 = new RegExp(Sn + "+$"),
+                Y1 = "(" + Uo + "+)|" + (U1 + "|") + "([!-\\[\\]-\u2027\u202A-\uD7FF\uF900-\uFFFF]" + (Sn + "*") + "|[\uD800-\uDBFF][\uDC00-\uDFFF]" + (Sn + "*") + "|\\\\verb\\*([^]).*?\\4|\\\\verb([^*a-zA-Z]).*?\\5" + ("|" + j1) + ("|" + V1 + ")");
+            class Wo {
                 constructor(t, o) {
-                    this.input = void 0, this.settings = void 0, this.tokenRegex = void 0, this.catcodes = void 0, this.input = t, this.settings = o, this.tokenRegex = new RegExp(U1, "g"), this.catcodes = {
+                    this.input = void 0, this.settings = void 0, this.tokenRegex = void 0, this.catcodes = void 0, this.input = t, this.settings = o, this.tokenRegex = new RegExp(Y1, "g"), this.catcodes = {
                         "%": 14,
                         "~": 13
                     }
                 }
                 setCatcode(t, o) {
                     this.catcodes[t] = o
                 }
@@ -14345,15 +14345,15 @@
                         let p = t.indexOf(`
 `, this.tokenRegex.lastIndex);
                         return p === -1 ? (this.tokenRegex.lastIndex = t.length, this.settings.reportNonstrict("commentAtEnd", "% comment has no terminating newline; LaTeX would fail because of commenting the end of math mode (e.g. $)")) : this.tokenRegex.lastIndex = p + 1, this.lex()
                     }
                     return new mt(u, new st(this, o, this.tokenRegex.lastIndex))
                 }
             }
-            class W1 {
+            class Z1 {
                 constructor(t, o) {
                     t === void 0 && (t = {}), o === void 0 && (o = {}), this.current = void 0, this.builtins = void 0, this.undefStack = void 0, this.current = o, this.builtins = t, this.undefStack = []
                 }
                 beginGroup() {
                     this.undefStack.push({})
                 }
                 endGroup() {
@@ -14377,15 +14377,15 @@
                     } else {
                         let u = this.undefStack[this.undefStack.length - 1];
                         u && !u.hasOwnProperty(t) && (u[t] = this.current[t])
                     }
                     o == null ? delete this.current[t] : this.current[t] = o
                 }
             }
-            var Y1 = vo;
+            var Q1 = ko;
             k("\\noexpand", function(n) {
                 let t = n.popToken();
                 return n.isExpandable(t.text) && (t.noexpand = !0, t.treatAsRelax = !0), {
                     tokens: [t],
                     numArgs: 0
                 }
             }), k("\\expandafter", function(n) {
@@ -14421,15 +14421,15 @@
                     tokens: t[0],
                     numArgs: 0
                 } : {
                     tokens: t[1],
                     numArgs: 0
                 }
             });
-            let Uo = {
+            let Yo = {
                 0: 0,
                 1: 1,
                 2: 2,
                 3: 3,
                 4: 4,
                 5: 5,
                 6: 6,
@@ -14458,22 +14458,22 @@
                     if (t = n.popToken(), t.text[0] === "\\") s = t.text.charCodeAt(1);
                     else {
                         if (t.text === "EOF") throw new a("\\char` missing argument");
                         s = t.text.charCodeAt(0)
                     }
                 else o = 10;
                 if (o) {
-                    if (s = Uo[t.text], s == null || s >= o) throw new a("Invalid base-" + o + " digit " + t.text);
+                    if (s = Yo[t.text], s == null || s >= o) throw new a("Invalid base-" + o + " digit " + t.text);
                     let u;
                     for (;
-                        (u = Uo[n.future().text]) != null && u < o;) s *= o, s += u, n.popToken()
+                        (u = Yo[n.future().text]) != null && u < o;) s *= o, s += u, n.popToken()
                 }
                 return "\\@char{" + s + "}"
             });
-            let Sn = (n, t, o) => {
+            let Cn = (n, t, o) => {
                 let s = n.consumeArg().tokens;
                 if (s.length !== 1) throw new a("\\newcommand's first argument must be a macro name");
                 let u = s[0].text,
                     p = n.isDefined(u);
                 if (p && !t) throw new a("\\newcommand{" + u + "} attempting to redefine " + (u + "; use \\renewcommand"));
                 if (!p && !o) throw new a("\\renewcommand{" + u + "} when command " + u + " does not yet exist; use \\newcommand");
                 let b = 0;
@@ -14485,26 +14485,26 @@
                     b = parseInt(v), s = n.consumeArg().tokens
                 }
                 return n.macros.set(u, {
                     tokens: s,
                     numArgs: b
                 }), ""
             };
-            k("\\newcommand", n => Sn(n, !1, !0)), k("\\renewcommand", n => Sn(n, !0, !1)), k("\\providecommand", n => Sn(n, !0, !0)), k("\\message", n => {
+            k("\\newcommand", n => Cn(n, !1, !0)), k("\\renewcommand", n => Cn(n, !0, !1)), k("\\providecommand", n => Cn(n, !0, !0)), k("\\message", n => {
                 let t = n.consumeArgs(1)[0];
                 return console.log(t.reverse().map(o => o.text).join("")), ""
             }), k("\\errmessage", n => {
                 let t = n.consumeArgs(1)[0];
                 return console.error(t.reverse().map(o => o.text).join("")), ""
             }), k("\\show", n => {
                 let t = n.popToken(),
                     o = t.text;
                 return console.log(t, n.macros.get(o), Gt[o], Oe.math[o], Oe.text[o]), ""
             }), k("\\bgroup", "{"), k("\\egroup", "}"), k("~", "\\nobreakspace"), k("\\lq", "`"), k("\\rq", "'"), k("\\aa", "\\r a"), k("\\AA", "\\r A"), k("\\textcopyright", "\\html@mathml{\\textcircled{c}}{\\char`\xA9}"), k("\\copyright", "\\TextOrMath{\\textcopyright}{\\text{\\textcopyright}}"), k("\\textregistered", "\\html@mathml{\\textcircled{\\scriptsize R}}{\\char`\xAE}"), k("\u212C", "\\mathscr{B}"), k("\u2130", "\\mathscr{E}"), k("\u2131", "\\mathscr{F}"), k("\u210B", "\\mathscr{H}"), k("\u2110", "\\mathscr{I}"), k("\u2112", "\\mathscr{L}"), k("\u2133", "\\mathscr{M}"), k("\u211B", "\\mathscr{R}"), k("\u212D", "\\mathfrak{C}"), k("\u210C", "\\mathfrak{H}"), k("\u2128", "\\mathfrak{Z}"), k("\\Bbbk", "\\Bbb{k}"), k("\xB7", "\\cdotp"), k("\\llap", "\\mathllap{\\textrm{#1}}"), k("\\rlap", "\\mathrlap{\\textrm{#1}}"), k("\\clap", "\\mathclap{\\textrm{#1}}"), k("\\mathstrut", "\\vphantom{(}"), k("\\underbar", "\\underline{\\text{#1}}"), k("\\not", '\\html@mathml{\\mathrel{\\mathrlap\\@not}}{\\char"338}'), k("\\neq", "\\html@mathml{\\mathrel{\\not=}}{\\mathrel{\\char`\u2260}}"), k("\\ne", "\\neq"), k("\u2260", "\\neq"), k("\\notin", "\\html@mathml{\\mathrel{{\\in}\\mathllap{/\\mskip1mu}}}{\\mathrel{\\char`\u2209}}"), k("\u2209", "\\notin"), k("\u2258", "\\html@mathml{\\mathrel{=\\kern{-1em}\\raisebox{0.4em}{$\\scriptsize\\frown$}}}{\\mathrel{\\char`\u2258}}"), k("\u2259", "\\html@mathml{\\stackrel{\\tiny\\wedge}{=}}{\\mathrel{\\char`\u2258}}"), k("\u225A", "\\html@mathml{\\stackrel{\\tiny\\vee}{=}}{\\mathrel{\\char`\u225A}}"), k("\u225B", "\\html@mathml{\\stackrel{\\scriptsize\\star}{=}}{\\mathrel{\\char`\u225B}}"), k("\u225D", "\\html@mathml{\\stackrel{\\tiny\\mathrm{def}}{=}}{\\mathrel{\\char`\u225D}}"), k("\u225E", "\\html@mathml{\\stackrel{\\tiny\\mathrm{m}}{=}}{\\mathrel{\\char`\u225E}}"), k("\u225F", "\\html@mathml{\\stackrel{\\tiny?}{=}}{\\mathrel{\\char`\u225F}}"), k("\u27C2", "\\perp"), k("\u203C", "\\mathclose{!\\mkern-0.8mu!}"), k("\u220C", "\\notni"), k("\u231C", "\\ulcorner"), k("\u231D", "\\urcorner"), k("\u231E", "\\llcorner"), k("\u231F", "\\lrcorner"), k("\xA9", "\\copyright"), k("\xAE", "\\textregistered"), k("\uFE0F", "\\textregistered"), k("\\ulcorner", '\\html@mathml{\\@ulcorner}{\\mathop{\\char"231c}}'), k("\\urcorner", '\\html@mathml{\\@urcorner}{\\mathop{\\char"231d}}'), k("\\llcorner", '\\html@mathml{\\@llcorner}{\\mathop{\\char"231e}}'), k("\\lrcorner", '\\html@mathml{\\@lrcorner}{\\mathop{\\char"231f}}'), k("\\vdots", "\\mathord{\\varvdots\\rule{0pt}{15pt}}"), k("\u22EE", "\\vdots"), k("\\varGamma", "\\mathit{\\Gamma}"), k("\\varDelta", "\\mathit{\\Delta}"), k("\\varTheta", "\\mathit{\\Theta}"), k("\\varLambda", "\\mathit{\\Lambda}"), k("\\varXi", "\\mathit{\\Xi}"), k("\\varPi", "\\mathit{\\Pi}"), k("\\varSigma", "\\mathit{\\Sigma}"), k("\\varUpsilon", "\\mathit{\\Upsilon}"), k("\\varPhi", "\\mathit{\\Phi}"), k("\\varPsi", "\\mathit{\\Psi}"), k("\\varOmega", "\\mathit{\\Omega}"), k("\\substack", "\\begin{subarray}{c}#1\\end{subarray}"), k("\\colon", "\\nobreak\\mskip2mu\\mathpunct{}\\mathchoice{\\mkern-3mu}{\\mkern-3mu}{}{}{:}\\mskip6mu\\relax"), k("\\boxed", "\\fbox{$\\displaystyle{#1}$}"), k("\\iff", "\\DOTSB\\;\\Longleftrightarrow\\;"), k("\\implies", "\\DOTSB\\;\\Longrightarrow\\;"), k("\\impliedby", "\\DOTSB\\;\\Longleftarrow\\;");
-            let Wo = {
+            let Zo = {
                 ",": "\\dotsc",
                 "\\not": "\\dotsb",
                 "+": "\\dotsb",
                 "=": "\\dotsb",
                 "<": "\\dotsb",
                 ">": "\\dotsb",
                 "-": "\\dotsb",
@@ -14548,17 +14548,17 @@
                 "\\iiiint": "\\dotsi",
                 "\\idotsint": "\\dotsi",
                 "\\DOTSX": "\\dotsx"
             };
             k("\\dots", function(n) {
                 let t = "\\dotso",
                     o = n.expandAfterFuture().text;
-                return o in Wo ? t = Wo[o] : (o.slice(0, 4) === "\\not" || o in Oe.math && R.contains(["bin", "rel"], Oe.math[o].group)) && (t = "\\dotsb"), t
+                return o in Zo ? t = Zo[o] : (o.slice(0, 4) === "\\not" || o in Oe.math && R.contains(["bin", "rel"], Oe.math[o].group)) && (t = "\\dotsb"), t
             });
-            let Cn = {
+            let Tn = {
                 ")": !0,
                 "]": !0,
                 "\\rbrack": !0,
                 "\\}": !0,
                 "\\rbrace": !0,
                 "\\rangle": !0,
                 "\\rceil": !0,
@@ -14572,27 +14572,27 @@
                 "\\Biggr": !0,
                 $: !0,
                 ";": !0,
                 ".": !0,
                 ",": !0
             };
             k("\\dotso", function(n) {
-                return n.future().text in Cn ? "\\ldots\\," : "\\ldots"
+                return n.future().text in Tn ? "\\ldots\\," : "\\ldots"
             }), k("\\dotsc", function(n) {
                 let t = n.future().text;
-                return t in Cn && t !== "," ? "\\ldots\\," : "\\ldots"
+                return t in Tn && t !== "," ? "\\ldots\\," : "\\ldots"
             }), k("\\cdots", function(n) {
-                return n.future().text in Cn ? "\\@cdots\\," : "\\@cdots"
+                return n.future().text in Tn ? "\\@cdots\\," : "\\@cdots"
             }), k("\\dotsb", "\\cdots"), k("\\dotsm", "\\cdots"), k("\\dotsi", "\\!\\cdots"), k("\\dotsx", "\\ldots\\,"), k("\\DOTSI", "\\relax"), k("\\DOTSB", "\\relax"), k("\\DOTSX", "\\relax"), k("\\tmspace", "\\TextOrMath{\\kern#1#3}{\\mskip#1#2}\\relax"), k("\\,", "\\tmspace+{3mu}{.1667em}"), k("\\thinspace", "\\,"), k("\\>", "\\mskip{4mu}"), k("\\:", "\\tmspace+{4mu}{.2222em}"), k("\\medspace", "\\:"), k("\\;", "\\tmspace+{5mu}{.2777em}"), k("\\thickspace", "\\;"), k("\\!", "\\tmspace-{3mu}{.1667em}"), k("\\negthinspace", "\\!"), k("\\negmedspace", "\\tmspace-{4mu}{.2222em}"), k("\\negthickspace", "\\tmspace-{5mu}{.277em}"), k("\\enspace", "\\kern.5em "), k("\\enskip", "\\hskip.5em\\relax"), k("\\quad", "\\hskip1em\\relax"), k("\\qquad", "\\hskip2em\\relax"), k("\\tag", "\\@ifstar\\tag@literal\\tag@paren"), k("\\tag@paren", "\\tag@literal{({#1})}"), k("\\tag@literal", n => {
                 if (n.macros.get("\\df@tag")) throw new a("Multiple \\tag");
                 return "\\gdef\\df@tag{\\text{#1}}"
             }), k("\\bmod", "\\mathchoice{\\mskip1mu}{\\mskip1mu}{\\mskip5mu}{\\mskip5mu}\\mathbin{\\rm mod}\\mathchoice{\\mskip1mu}{\\mskip1mu}{\\mskip5mu}{\\mskip5mu}"), k("\\pod", "\\allowbreak\\mathchoice{\\mkern18mu}{\\mkern8mu}{\\mkern8mu}{\\mkern8mu}(#1)"), k("\\pmod", "\\pod{{\\rm mod}\\mkern6mu#1}"), k("\\mod", "\\allowbreak\\mathchoice{\\mkern18mu}{\\mkern12mu}{\\mkern12mu}{\\mkern12mu}{\\rm mod}\\,\\,#1"), k("\\newline", "\\\\\\relax"), k("\\TeX", "\\textrm{\\html@mathml{T\\kern-.1667em\\raisebox{-.5ex}{E}\\kern-.125emX}{TeX}}");
-            let Yo = Z(vt["Main-Regular"][84][1] - .7 * vt["Main-Regular"][65][1]);
-            k("\\LaTeX", "\\textrm{\\html@mathml{" + ("L\\kern-.36em\\raisebox{" + Yo + "}{\\scriptstyle A}") + "\\kern-.15em\\TeX}{LaTeX}}"), k("\\KaTeX", "\\textrm{\\html@mathml{" + ("K\\kern-.17em\\raisebox{" + Yo + "}{\\scriptstyle A}") + "\\kern-.15em\\TeX}{KaTeX}}"), k("\\hspace", "\\@ifstar\\@hspacer\\@hspace"), k("\\@hspace", "\\hskip #1\\relax"), k("\\@hspacer", "\\rule{0pt}{0pt}\\hskip #1\\relax"), k("\\ordinarycolon", ":"), k("\\vcentcolon", "\\mathrel{\\mathop\\ordinarycolon}"), k("\\dblcolon", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-.9mu}\\vcentcolon}}{\\mathop{\\char"2237}}'), k("\\coloneqq", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-1.2mu}=}}{\\mathop{\\char"2254}}'), k("\\Coloneqq", '\\html@mathml{\\mathrel{\\dblcolon\\mathrel{\\mkern-1.2mu}=}}{\\mathop{\\char"2237\\char"3d}}'), k("\\coloneq", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-1.2mu}\\mathrel{-}}}{\\mathop{\\char"3a\\char"2212}}'), k("\\Coloneq", '\\html@mathml{\\mathrel{\\dblcolon\\mathrel{\\mkern-1.2mu}\\mathrel{-}}}{\\mathop{\\char"2237\\char"2212}}'), k("\\eqqcolon", '\\html@mathml{\\mathrel{=\\mathrel{\\mkern-1.2mu}\\vcentcolon}}{\\mathop{\\char"2255}}'), k("\\Eqqcolon", '\\html@mathml{\\mathrel{=\\mathrel{\\mkern-1.2mu}\\dblcolon}}{\\mathop{\\char"3d\\char"2237}}'), k("\\eqcolon", '\\html@mathml{\\mathrel{\\mathrel{-}\\mathrel{\\mkern-1.2mu}\\vcentcolon}}{\\mathop{\\char"2239}}'), k("\\Eqcolon", '\\html@mathml{\\mathrel{\\mathrel{-}\\mathrel{\\mkern-1.2mu}\\dblcolon}}{\\mathop{\\char"2212\\char"2237}}'), k("\\colonapprox", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-1.2mu}\\approx}}{\\mathop{\\char"3a\\char"2248}}'), k("\\Colonapprox", '\\html@mathml{\\mathrel{\\dblcolon\\mathrel{\\mkern-1.2mu}\\approx}}{\\mathop{\\char"2237\\char"2248}}'), k("\\colonsim", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-1.2mu}\\sim}}{\\mathop{\\char"3a\\char"223c}}'), k("\\Colonsim", '\\html@mathml{\\mathrel{\\dblcolon\\mathrel{\\mkern-1.2mu}\\sim}}{\\mathop{\\char"2237\\char"223c}}'), k("\u2237", "\\dblcolon"), k("\u2239", "\\eqcolon"), k("\u2254", "\\coloneqq"), k("\u2255", "\\eqqcolon"), k("\u2A74", "\\Coloneqq"), k("\\ratio", "\\vcentcolon"), k("\\coloncolon", "\\dblcolon"), k("\\colonequals", "\\coloneqq"), k("\\coloncolonequals", "\\Coloneqq"), k("\\equalscolon", "\\eqqcolon"), k("\\equalscoloncolon", "\\Eqqcolon"), k("\\colonminus", "\\coloneq"), k("\\coloncolonminus", "\\Coloneq"), k("\\minuscolon", "\\eqcolon"), k("\\minuscoloncolon", "\\Eqcolon"), k("\\coloncolonapprox", "\\Colonapprox"), k("\\coloncolonsim", "\\Colonsim"), k("\\simcolon", "\\mathrel{\\sim\\mathrel{\\mkern-1.2mu}\\vcentcolon}"), k("\\simcoloncolon", "\\mathrel{\\sim\\mathrel{\\mkern-1.2mu}\\dblcolon}"), k("\\approxcolon", "\\mathrel{\\approx\\mathrel{\\mkern-1.2mu}\\vcentcolon}"), k("\\approxcoloncolon", "\\mathrel{\\approx\\mathrel{\\mkern-1.2mu}\\dblcolon}"), k("\\notni", "\\html@mathml{\\not\\ni}{\\mathrel{\\char`\u220C}}"), k("\\limsup", "\\DOTSB\\operatorname*{lim\\,sup}"), k("\\liminf", "\\DOTSB\\operatorname*{lim\\,inf}"), k("\\injlim", "\\DOTSB\\operatorname*{inj\\,lim}"), k("\\projlim", "\\DOTSB\\operatorname*{proj\\,lim}"), k("\\varlimsup", "\\DOTSB\\operatorname*{\\overline{lim}}"), k("\\varliminf", "\\DOTSB\\operatorname*{\\underline{lim}}"), k("\\varinjlim", "\\DOTSB\\operatorname*{\\underrightarrow{lim}}"), k("\\varprojlim", "\\DOTSB\\operatorname*{\\underleftarrow{lim}}"), k("\\gvertneqq", "\\html@mathml{\\@gvertneqq}{\u2269}"), k("\\lvertneqq", "\\html@mathml{\\@lvertneqq}{\u2268}"), k("\\ngeqq", "\\html@mathml{\\@ngeqq}{\u2271}"), k("\\ngeqslant", "\\html@mathml{\\@ngeqslant}{\u2271}"), k("\\nleqq", "\\html@mathml{\\@nleqq}{\u2270}"), k("\\nleqslant", "\\html@mathml{\\@nleqslant}{\u2270}"), k("\\nshortmid", "\\html@mathml{\\@nshortmid}{\u2224}"), k("\\nshortparallel", "\\html@mathml{\\@nshortparallel}{\u2226}"), k("\\nsubseteqq", "\\html@mathml{\\@nsubseteqq}{\u2288}"), k("\\nsupseteqq", "\\html@mathml{\\@nsupseteqq}{\u2289}"), k("\\varsubsetneq", "\\html@mathml{\\@varsubsetneq}{\u228A}"), k("\\varsubsetneqq", "\\html@mathml{\\@varsubsetneqq}{\u2ACB}"), k("\\varsupsetneq", "\\html@mathml{\\@varsupsetneq}{\u228B}"), k("\\varsupsetneqq", "\\html@mathml{\\@varsupsetneqq}{\u2ACC}"), k("\\imath", "\\html@mathml{\\@imath}{\u0131}"), k("\\jmath", "\\html@mathml{\\@jmath}{\u0237}"), k("\\llbracket", "\\html@mathml{\\mathopen{[\\mkern-3.2mu[}}{\\mathopen{\\char`\u27E6}}"), k("\\rrbracket", "\\html@mathml{\\mathclose{]\\mkern-3.2mu]}}{\\mathclose{\\char`\u27E7}}"), k("\u27E6", "\\llbracket"), k("\u27E7", "\\rrbracket"), k("\\lBrace", "\\html@mathml{\\mathopen{\\{\\mkern-3.2mu[}}{\\mathopen{\\char`\u2983}}"), k("\\rBrace", "\\html@mathml{\\mathclose{]\\mkern-3.2mu\\}}}{\\mathclose{\\char`\u2984}}"), k("\u2983", "\\lBrace"), k("\u2984", "\\rBrace"), k("\\minuso", "\\mathbin{\\html@mathml{{\\mathrlap{\\mathchoice{\\kern{0.145em}}{\\kern{0.145em}}{\\kern{0.1015em}}{\\kern{0.0725em}}\\circ}{-}}}{\\char`\u29B5}}"), k("\u29B5", "\\minuso"), k("\\darr", "\\downarrow"), k("\\dArr", "\\Downarrow"), k("\\Darr", "\\Downarrow"), k("\\lang", "\\langle"), k("\\rang", "\\rangle"), k("\\uarr", "\\uparrow"), k("\\uArr", "\\Uparrow"), k("\\Uarr", "\\Uparrow"), k("\\N", "\\mathbb{N}"), k("\\R", "\\mathbb{R}"), k("\\Z", "\\mathbb{Z}"), k("\\alef", "\\aleph"), k("\\alefsym", "\\aleph"), k("\\Alpha", "\\mathrm{A}"), k("\\Beta", "\\mathrm{B}"), k("\\bull", "\\bullet"), k("\\Chi", "\\mathrm{X}"), k("\\clubs", "\\clubsuit"), k("\\cnums", "\\mathbb{C}"), k("\\Complex", "\\mathbb{C}"), k("\\Dagger", "\\ddagger"), k("\\diamonds", "\\diamondsuit"), k("\\empty", "\\emptyset"), k("\\Epsilon", "\\mathrm{E}"), k("\\Eta", "\\mathrm{H}"), k("\\exist", "\\exists"), k("\\harr", "\\leftrightarrow"), k("\\hArr", "\\Leftrightarrow"), k("\\Harr", "\\Leftrightarrow"), k("\\hearts", "\\heartsuit"), k("\\image", "\\Im"), k("\\infin", "\\infty"), k("\\Iota", "\\mathrm{I}"), k("\\isin", "\\in"), k("\\Kappa", "\\mathrm{K}"), k("\\larr", "\\leftarrow"), k("\\lArr", "\\Leftarrow"), k("\\Larr", "\\Leftarrow"), k("\\lrarr", "\\leftrightarrow"), k("\\lrArr", "\\Leftrightarrow"), k("\\Lrarr", "\\Leftrightarrow"), k("\\Mu", "\\mathrm{M}"), k("\\natnums", "\\mathbb{N}"), k("\\Nu", "\\mathrm{N}"), k("\\Omicron", "\\mathrm{O}"), k("\\plusmn", "\\pm"), k("\\rarr", "\\rightarrow"), k("\\rArr", "\\Rightarrow"), k("\\Rarr", "\\Rightarrow"), k("\\real", "\\Re"), k("\\reals", "\\mathbb{R}"), k("\\Reals", "\\mathbb{R}"), k("\\Rho", "\\mathrm{P}"), k("\\sdot", "\\cdot"), k("\\sect", "\\S"), k("\\spades", "\\spadesuit"), k("\\sub", "\\subset"), k("\\sube", "\\subseteq"), k("\\supe", "\\supseteq"), k("\\Tau", "\\mathrm{T}"), k("\\thetasym", "\\vartheta"), k("\\weierp", "\\wp"), k("\\Zeta", "\\mathrm{Z}"), k("\\argmin", "\\DOTSB\\operatorname*{arg\\,min}"), k("\\argmax", "\\DOTSB\\operatorname*{arg\\,max}"), k("\\plim", "\\DOTSB\\mathop{\\operatorname{plim}}\\limits"), k("\\bra", "\\mathinner{\\langle{#1}|}"), k("\\ket", "\\mathinner{|{#1}\\rangle}"), k("\\braket", "\\mathinner{\\langle{#1}\\rangle}"), k("\\Bra", "\\left\\langle#1\\right|"), k("\\Ket", "\\left|#1\\right\\rangle");
-            let Zo = n => t => {
+            let Qo = Z(vt["Main-Regular"][84][1] - .7 * vt["Main-Regular"][65][1]);
+            k("\\LaTeX", "\\textrm{\\html@mathml{" + ("L\\kern-.36em\\raisebox{" + Qo + "}{\\scriptstyle A}") + "\\kern-.15em\\TeX}{LaTeX}}"), k("\\KaTeX", "\\textrm{\\html@mathml{" + ("K\\kern-.17em\\raisebox{" + Qo + "}{\\scriptstyle A}") + "\\kern-.15em\\TeX}{KaTeX}}"), k("\\hspace", "\\@ifstar\\@hspacer\\@hspace"), k("\\@hspace", "\\hskip #1\\relax"), k("\\@hspacer", "\\rule{0pt}{0pt}\\hskip #1\\relax"), k("\\ordinarycolon", ":"), k("\\vcentcolon", "\\mathrel{\\mathop\\ordinarycolon}"), k("\\dblcolon", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-.9mu}\\vcentcolon}}{\\mathop{\\char"2237}}'), k("\\coloneqq", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-1.2mu}=}}{\\mathop{\\char"2254}}'), k("\\Coloneqq", '\\html@mathml{\\mathrel{\\dblcolon\\mathrel{\\mkern-1.2mu}=}}{\\mathop{\\char"2237\\char"3d}}'), k("\\coloneq", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-1.2mu}\\mathrel{-}}}{\\mathop{\\char"3a\\char"2212}}'), k("\\Coloneq", '\\html@mathml{\\mathrel{\\dblcolon\\mathrel{\\mkern-1.2mu}\\mathrel{-}}}{\\mathop{\\char"2237\\char"2212}}'), k("\\eqqcolon", '\\html@mathml{\\mathrel{=\\mathrel{\\mkern-1.2mu}\\vcentcolon}}{\\mathop{\\char"2255}}'), k("\\Eqqcolon", '\\html@mathml{\\mathrel{=\\mathrel{\\mkern-1.2mu}\\dblcolon}}{\\mathop{\\char"3d\\char"2237}}'), k("\\eqcolon", '\\html@mathml{\\mathrel{\\mathrel{-}\\mathrel{\\mkern-1.2mu}\\vcentcolon}}{\\mathop{\\char"2239}}'), k("\\Eqcolon", '\\html@mathml{\\mathrel{\\mathrel{-}\\mathrel{\\mkern-1.2mu}\\dblcolon}}{\\mathop{\\char"2212\\char"2237}}'), k("\\colonapprox", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-1.2mu}\\approx}}{\\mathop{\\char"3a\\char"2248}}'), k("\\Colonapprox", '\\html@mathml{\\mathrel{\\dblcolon\\mathrel{\\mkern-1.2mu}\\approx}}{\\mathop{\\char"2237\\char"2248}}'), k("\\colonsim", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-1.2mu}\\sim}}{\\mathop{\\char"3a\\char"223c}}'), k("\\Colonsim", '\\html@mathml{\\mathrel{\\dblcolon\\mathrel{\\mkern-1.2mu}\\sim}}{\\mathop{\\char"2237\\char"223c}}'), k("\u2237", "\\dblcolon"), k("\u2239", "\\eqcolon"), k("\u2254", "\\coloneqq"), k("\u2255", "\\eqqcolon"), k("\u2A74", "\\Coloneqq"), k("\\ratio", "\\vcentcolon"), k("\\coloncolon", "\\dblcolon"), k("\\colonequals", "\\coloneqq"), k("\\coloncolonequals", "\\Coloneqq"), k("\\equalscolon", "\\eqqcolon"), k("\\equalscoloncolon", "\\Eqqcolon"), k("\\colonminus", "\\coloneq"), k("\\coloncolonminus", "\\Coloneq"), k("\\minuscolon", "\\eqcolon"), k("\\minuscoloncolon", "\\Eqcolon"), k("\\coloncolonapprox", "\\Colonapprox"), k("\\coloncolonsim", "\\Colonsim"), k("\\simcolon", "\\mathrel{\\sim\\mathrel{\\mkern-1.2mu}\\vcentcolon}"), k("\\simcoloncolon", "\\mathrel{\\sim\\mathrel{\\mkern-1.2mu}\\dblcolon}"), k("\\approxcolon", "\\mathrel{\\approx\\mathrel{\\mkern-1.2mu}\\vcentcolon}"), k("\\approxcoloncolon", "\\mathrel{\\approx\\mathrel{\\mkern-1.2mu}\\dblcolon}"), k("\\notni", "\\html@mathml{\\not\\ni}{\\mathrel{\\char`\u220C}}"), k("\\limsup", "\\DOTSB\\operatorname*{lim\\,sup}"), k("\\liminf", "\\DOTSB\\operatorname*{lim\\,inf}"), k("\\injlim", "\\DOTSB\\operatorname*{inj\\,lim}"), k("\\projlim", "\\DOTSB\\operatorname*{proj\\,lim}"), k("\\varlimsup", "\\DOTSB\\operatorname*{\\overline{lim}}"), k("\\varliminf", "\\DOTSB\\operatorname*{\\underline{lim}}"), k("\\varinjlim", "\\DOTSB\\operatorname*{\\underrightarrow{lim}}"), k("\\varprojlim", "\\DOTSB\\operatorname*{\\underleftarrow{lim}}"), k("\\gvertneqq", "\\html@mathml{\\@gvertneqq}{\u2269}"), k("\\lvertneqq", "\\html@mathml{\\@lvertneqq}{\u2268}"), k("\\ngeqq", "\\html@mathml{\\@ngeqq}{\u2271}"), k("\\ngeqslant", "\\html@mathml{\\@ngeqslant}{\u2271}"), k("\\nleqq", "\\html@mathml{\\@nleqq}{\u2270}"), k("\\nleqslant", "\\html@mathml{\\@nleqslant}{\u2270}"), k("\\nshortmid", "\\html@mathml{\\@nshortmid}{\u2224}"), k("\\nshortparallel", "\\html@mathml{\\@nshortparallel}{\u2226}"), k("\\nsubseteqq", "\\html@mathml{\\@nsubseteqq}{\u2288}"), k("\\nsupseteqq", "\\html@mathml{\\@nsupseteqq}{\u2289}"), k("\\varsubsetneq", "\\html@mathml{\\@varsubsetneq}{\u228A}"), k("\\varsubsetneqq", "\\html@mathml{\\@varsubsetneqq}{\u2ACB}"), k("\\varsupsetneq", "\\html@mathml{\\@varsupsetneq}{\u228B}"), k("\\varsupsetneqq", "\\html@mathml{\\@varsupsetneqq}{\u2ACC}"), k("\\imath", "\\html@mathml{\\@imath}{\u0131}"), k("\\jmath", "\\html@mathml{\\@jmath}{\u0237}"), k("\\llbracket", "\\html@mathml{\\mathopen{[\\mkern-3.2mu[}}{\\mathopen{\\char`\u27E6}}"), k("\\rrbracket", "\\html@mathml{\\mathclose{]\\mkern-3.2mu]}}{\\mathclose{\\char`\u27E7}}"), k("\u27E6", "\\llbracket"), k("\u27E7", "\\rrbracket"), k("\\lBrace", "\\html@mathml{\\mathopen{\\{\\mkern-3.2mu[}}{\\mathopen{\\char`\u2983}}"), k("\\rBrace", "\\html@mathml{\\mathclose{]\\mkern-3.2mu\\}}}{\\mathclose{\\char`\u2984}}"), k("\u2983", "\\lBrace"), k("\u2984", "\\rBrace"), k("\\minuso", "\\mathbin{\\html@mathml{{\\mathrlap{\\mathchoice{\\kern{0.145em}}{\\kern{0.145em}}{\\kern{0.1015em}}{\\kern{0.0725em}}\\circ}{-}}}{\\char`\u29B5}}"), k("\u29B5", "\\minuso"), k("\\darr", "\\downarrow"), k("\\dArr", "\\Downarrow"), k("\\Darr", "\\Downarrow"), k("\\lang", "\\langle"), k("\\rang", "\\rangle"), k("\\uarr", "\\uparrow"), k("\\uArr", "\\Uparrow"), k("\\Uarr", "\\Uparrow"), k("\\N", "\\mathbb{N}"), k("\\R", "\\mathbb{R}"), k("\\Z", "\\mathbb{Z}"), k("\\alef", "\\aleph"), k("\\alefsym", "\\aleph"), k("\\Alpha", "\\mathrm{A}"), k("\\Beta", "\\mathrm{B}"), k("\\bull", "\\bullet"), k("\\Chi", "\\mathrm{X}"), k("\\clubs", "\\clubsuit"), k("\\cnums", "\\mathbb{C}"), k("\\Complex", "\\mathbb{C}"), k("\\Dagger", "\\ddagger"), k("\\diamonds", "\\diamondsuit"), k("\\empty", "\\emptyset"), k("\\Epsilon", "\\mathrm{E}"), k("\\Eta", "\\mathrm{H}"), k("\\exist", "\\exists"), k("\\harr", "\\leftrightarrow"), k("\\hArr", "\\Leftrightarrow"), k("\\Harr", "\\Leftrightarrow"), k("\\hearts", "\\heartsuit"), k("\\image", "\\Im"), k("\\infin", "\\infty"), k("\\Iota", "\\mathrm{I}"), k("\\isin", "\\in"), k("\\Kappa", "\\mathrm{K}"), k("\\larr", "\\leftarrow"), k("\\lArr", "\\Leftarrow"), k("\\Larr", "\\Leftarrow"), k("\\lrarr", "\\leftrightarrow"), k("\\lrArr", "\\Leftrightarrow"), k("\\Lrarr", "\\Leftrightarrow"), k("\\Mu", "\\mathrm{M}"), k("\\natnums", "\\mathbb{N}"), k("\\Nu", "\\mathrm{N}"), k("\\Omicron", "\\mathrm{O}"), k("\\plusmn", "\\pm"), k("\\rarr", "\\rightarrow"), k("\\rArr", "\\Rightarrow"), k("\\Rarr", "\\Rightarrow"), k("\\real", "\\Re"), k("\\reals", "\\mathbb{R}"), k("\\Reals", "\\mathbb{R}"), k("\\Rho", "\\mathrm{P}"), k("\\sdot", "\\cdot"), k("\\sect", "\\S"), k("\\spades", "\\spadesuit"), k("\\sub", "\\subset"), k("\\sube", "\\subseteq"), k("\\supe", "\\supseteq"), k("\\Tau", "\\mathrm{T}"), k("\\thetasym", "\\vartheta"), k("\\weierp", "\\wp"), k("\\Zeta", "\\mathrm{Z}"), k("\\argmin", "\\DOTSB\\operatorname*{arg\\,min}"), k("\\argmax", "\\DOTSB\\operatorname*{arg\\,max}"), k("\\plim", "\\DOTSB\\mathop{\\operatorname{plim}}\\limits"), k("\\bra", "\\mathinner{\\langle{#1}|}"), k("\\ket", "\\mathinner{|{#1}\\rangle}"), k("\\braket", "\\mathinner{\\langle{#1}\\rangle}"), k("\\Bra", "\\left\\langle#1\\right|"), k("\\Ket", "\\left|#1\\right\\rangle");
+            let Xo = n => t => {
                 let o = t.consumeArg().tokens,
                     s = t.consumeArg().tokens,
                     u = t.consumeArg().tokens,
                     p = t.consumeArg().tokens,
                     b = t.macros.get("|"),
                     v = t.macros.get("\\|");
                 t.macros.beginGroup();
@@ -14608,27 +14608,27 @@
                 let E = t.consumeArg().tokens,
                     z = t.expandTokens([...p, ...E, ...o]);
                 return t.macros.endGroup(), {
                     tokens: z.reverse(),
                     numArgs: 0
                 }
             };
-            k("\\bra@ket", Zo(!1)), k("\\bra@set", Zo(!0)), k("\\Braket", "\\bra@ket{\\left\\langle}{\\,\\middle\\vert\\,}{\\,\\middle\\vert\\,}{\\right\\rangle}"), k("\\Set", "\\bra@set{\\left\\{\\:}{\\;\\middle\\vert\\;}{\\;\\middle\\Vert\\;}{\\:\\right\\}}"), k("\\set", "\\bra@set{\\{\\,}{\\mid}{}{\\,\\}}"), k("\\angln", "{\\angl n}"), k("\\blue", "\\textcolor{##6495ed}{#1}"), k("\\orange", "\\textcolor{##ffa500}{#1}"), k("\\pink", "\\textcolor{##ff00af}{#1}"), k("\\red", "\\textcolor{##df0030}{#1}"), k("\\green", "\\textcolor{##28ae7b}{#1}"), k("\\gray", "\\textcolor{gray}{#1}"), k("\\purple", "\\textcolor{##9d38bd}{#1}"), k("\\blueA", "\\textcolor{##ccfaff}{#1}"), k("\\blueB", "\\textcolor{##80f6ff}{#1}"), k("\\blueC", "\\textcolor{##63d9ea}{#1}"), k("\\blueD", "\\textcolor{##11accd}{#1}"), k("\\blueE", "\\textcolor{##0c7f99}{#1}"), k("\\tealA", "\\textcolor{##94fff5}{#1}"), k("\\tealB", "\\textcolor{##26edd5}{#1}"), k("\\tealC", "\\textcolor{##01d1c1}{#1}"), k("\\tealD", "\\textcolor{##01a995}{#1}"), k("\\tealE", "\\textcolor{##208170}{#1}"), k("\\greenA", "\\textcolor{##b6ffb0}{#1}"), k("\\greenB", "\\textcolor{##8af281}{#1}"), k("\\greenC", "\\textcolor{##74cf70}{#1}"), k("\\greenD", "\\textcolor{##1fab54}{#1}"), k("\\greenE", "\\textcolor{##0d923f}{#1}"), k("\\goldA", "\\textcolor{##ffd0a9}{#1}"), k("\\goldB", "\\textcolor{##ffbb71}{#1}"), k("\\goldC", "\\textcolor{##ff9c39}{#1}"), k("\\goldD", "\\textcolor{##e07d10}{#1}"), k("\\goldE", "\\textcolor{##a75a05}{#1}"), k("\\redA", "\\textcolor{##fca9a9}{#1}"), k("\\redB", "\\textcolor{##ff8482}{#1}"), k("\\redC", "\\textcolor{##f9685d}{#1}"), k("\\redD", "\\textcolor{##e84d39}{#1}"), k("\\redE", "\\textcolor{##bc2612}{#1}"), k("\\maroonA", "\\textcolor{##ffbde0}{#1}"), k("\\maroonB", "\\textcolor{##ff92c6}{#1}"), k("\\maroonC", "\\textcolor{##ed5fa6}{#1}"), k("\\maroonD", "\\textcolor{##ca337c}{#1}"), k("\\maroonE", "\\textcolor{##9e034e}{#1}"), k("\\purpleA", "\\textcolor{##ddd7ff}{#1}"), k("\\purpleB", "\\textcolor{##c6b9fc}{#1}"), k("\\purpleC", "\\textcolor{##aa87ff}{#1}"), k("\\purpleD", "\\textcolor{##7854ab}{#1}"), k("\\purpleE", "\\textcolor{##543b78}{#1}"), k("\\mintA", "\\textcolor{##f5f9e8}{#1}"), k("\\mintB", "\\textcolor{##edf2df}{#1}"), k("\\mintC", "\\textcolor{##e0e5cc}{#1}"), k("\\grayA", "\\textcolor{##f6f7f7}{#1}"), k("\\grayB", "\\textcolor{##f0f1f2}{#1}"), k("\\grayC", "\\textcolor{##e3e5e6}{#1}"), k("\\grayD", "\\textcolor{##d6d8da}{#1}"), k("\\grayE", "\\textcolor{##babec2}{#1}"), k("\\grayF", "\\textcolor{##888d93}{#1}"), k("\\grayG", "\\textcolor{##626569}{#1}"), k("\\grayH", "\\textcolor{##3b3e40}{#1}"), k("\\grayI", "\\textcolor{##21242c}{#1}"), k("\\kaBlue", "\\textcolor{##314453}{#1}"), k("\\kaGreen", "\\textcolor{##71B307}{#1}");
-            let Qo = {
+            k("\\bra@ket", Xo(!1)), k("\\bra@set", Xo(!0)), k("\\Braket", "\\bra@ket{\\left\\langle}{\\,\\middle\\vert\\,}{\\,\\middle\\vert\\,}{\\right\\rangle}"), k("\\Set", "\\bra@set{\\left\\{\\:}{\\;\\middle\\vert\\;}{\\;\\middle\\Vert\\;}{\\:\\right\\}}"), k("\\set", "\\bra@set{\\{\\,}{\\mid}{}{\\,\\}}"), k("\\angln", "{\\angl n}"), k("\\blue", "\\textcolor{##6495ed}{#1}"), k("\\orange", "\\textcolor{##ffa500}{#1}"), k("\\pink", "\\textcolor{##ff00af}{#1}"), k("\\red", "\\textcolor{##df0030}{#1}"), k("\\green", "\\textcolor{##28ae7b}{#1}"), k("\\gray", "\\textcolor{gray}{#1}"), k("\\purple", "\\textcolor{##9d38bd}{#1}"), k("\\blueA", "\\textcolor{##ccfaff}{#1}"), k("\\blueB", "\\textcolor{##80f6ff}{#1}"), k("\\blueC", "\\textcolor{##63d9ea}{#1}"), k("\\blueD", "\\textcolor{##11accd}{#1}"), k("\\blueE", "\\textcolor{##0c7f99}{#1}"), k("\\tealA", "\\textcolor{##94fff5}{#1}"), k("\\tealB", "\\textcolor{##26edd5}{#1}"), k("\\tealC", "\\textcolor{##01d1c1}{#1}"), k("\\tealD", "\\textcolor{##01a995}{#1}"), k("\\tealE", "\\textcolor{##208170}{#1}"), k("\\greenA", "\\textcolor{##b6ffb0}{#1}"), k("\\greenB", "\\textcolor{##8af281}{#1}"), k("\\greenC", "\\textcolor{##74cf70}{#1}"), k("\\greenD", "\\textcolor{##1fab54}{#1}"), k("\\greenE", "\\textcolor{##0d923f}{#1}"), k("\\goldA", "\\textcolor{##ffd0a9}{#1}"), k("\\goldB", "\\textcolor{##ffbb71}{#1}"), k("\\goldC", "\\textcolor{##ff9c39}{#1}"), k("\\goldD", "\\textcolor{##e07d10}{#1}"), k("\\goldE", "\\textcolor{##a75a05}{#1}"), k("\\redA", "\\textcolor{##fca9a9}{#1}"), k("\\redB", "\\textcolor{##ff8482}{#1}"), k("\\redC", "\\textcolor{##f9685d}{#1}"), k("\\redD", "\\textcolor{##e84d39}{#1}"), k("\\redE", "\\textcolor{##bc2612}{#1}"), k("\\maroonA", "\\textcolor{##ffbde0}{#1}"), k("\\maroonB", "\\textcolor{##ff92c6}{#1}"), k("\\maroonC", "\\textcolor{##ed5fa6}{#1}"), k("\\maroonD", "\\textcolor{##ca337c}{#1}"), k("\\maroonE", "\\textcolor{##9e034e}{#1}"), k("\\purpleA", "\\textcolor{##ddd7ff}{#1}"), k("\\purpleB", "\\textcolor{##c6b9fc}{#1}"), k("\\purpleC", "\\textcolor{##aa87ff}{#1}"), k("\\purpleD", "\\textcolor{##7854ab}{#1}"), k("\\purpleE", "\\textcolor{##543b78}{#1}"), k("\\mintA", "\\textcolor{##f5f9e8}{#1}"), k("\\mintB", "\\textcolor{##edf2df}{#1}"), k("\\mintC", "\\textcolor{##e0e5cc}{#1}"), k("\\grayA", "\\textcolor{##f6f7f7}{#1}"), k("\\grayB", "\\textcolor{##f0f1f2}{#1}"), k("\\grayC", "\\textcolor{##e3e5e6}{#1}"), k("\\grayD", "\\textcolor{##d6d8da}{#1}"), k("\\grayE", "\\textcolor{##babec2}{#1}"), k("\\grayF", "\\textcolor{##888d93}{#1}"), k("\\grayG", "\\textcolor{##626569}{#1}"), k("\\grayH", "\\textcolor{##3b3e40}{#1}"), k("\\grayI", "\\textcolor{##21242c}{#1}"), k("\\kaBlue", "\\textcolor{##314453}{#1}"), k("\\kaGreen", "\\textcolor{##71B307}{#1}");
+            let Jo = {
                 "^": !0,
                 _: !0,
                 "\\limits": !0,
                 "\\nolimits": !0
             };
-            class Z1 {
+            class X1 {
                 constructor(t, o, s) {
-                    this.settings = void 0, this.expansionCount = void 0, this.lexer = void 0, this.macros = void 0, this.stack = void 0, this.mode = void 0, this.settings = o, this.expansionCount = 0, this.feed(t), this.macros = new W1(Y1, o.macros), this.mode = s, this.stack = []
+                    this.settings = void 0, this.expansionCount = void 0, this.lexer = void 0, this.macros = void 0, this.stack = void 0, this.mode = void 0, this.settings = o, this.expansionCount = 0, this.feed(t), this.macros = new Z1(Q1, o.macros), this.mode = s, this.stack = []
                 }
                 feed(t) {
-                    this.lexer = new jo(t, this.settings)
+                    this.lexer = new Wo(t, this.settings)
                 }
                 switchMode(t) {
                     this.mode = t
                 }
                 beginGroup() {
                     this.macros.beginGroup()
                 }
@@ -14771,34 +14771,34 @@
                     let s = typeof o == "function" ? o(this) : o;
                     if (typeof s == "string") {
                         let u = 0;
                         if (s.indexOf("#") !== -1) {
                             let E = s.replace(/##/g, "");
                             for (; E.indexOf("#" + (u + 1)) !== -1;) ++u
                         }
-                        let p = new jo(s, this.settings),
+                        let p = new Wo(s, this.settings),
                             b = [],
                             v = p.lex();
                         for (; v.text !== "EOF";) b.push(v), v = p.lex();
                         return b.reverse(), {
                             tokens: b,
                             numArgs: u
                         }
                     }
                     return s
                 }
                 isDefined(t) {
-                    return this.macros.has(t) || Gt.hasOwnProperty(t) || Oe.math.hasOwnProperty(t) || Oe.text.hasOwnProperty(t) || Qo.hasOwnProperty(t)
+                    return this.macros.has(t) || Gt.hasOwnProperty(t) || Oe.math.hasOwnProperty(t) || Oe.text.hasOwnProperty(t) || Jo.hasOwnProperty(t)
                 }
                 isExpandable(t) {
                     let o = this.macros.get(t);
                     return o != null ? typeof o == "string" || typeof o == "function" || !o.unexpandable : Gt.hasOwnProperty(t) && !Gt[t].primitive
                 }
             }
-            let Xo = /^[₊₋₌₍₎₀₁₂₃₄₅₆₇₈₉ₐₑₕᵢⱼₖₗₘₙₒₚᵣₛₜᵤᵥₓᵦᵧᵨᵩᵪ]/,
+            let Ko = /^[₊₋₌₍₎₀₁₂₃₄₅₆₇₈₉ₐₑₕᵢⱼₖₗₘₙₒₚᵣₛₜᵤᵥₓᵦᵧᵨᵩᵪ]/,
                 o0 = Object.freeze({
                     "\u208A": "+",
                     "\u208B": "-",
                     "\u208C": "=",
                     "\u208D": "(",
                     "\u208E": ")",
                     "\u2080": "0",
@@ -14895,15 +14895,15 @@
                     "\u1D5D": "\u03B2",
                     "\u1D5E": "\u03B3",
                     "\u1D5F": "\u03B4",
                     "\u1D60": "\u03D5",
                     "\u1D61": "\u03C7",
                     "\u1DBF": "\u03B8"
                 }),
-                Tn = {
+                An = {
                     "\u0301": {
                         text: "\\'",
                         math: "\\acute"
                     },
                     "\u0300": {
                         text: "\\`",
                         math: "\\grave"
@@ -14943,15 +14943,15 @@
                     "\u030B": {
                         text: "\\H"
                     },
                     "\u0327": {
                         text: "\\c"
                     }
                 },
-                Jo = {
+                ea = {
                     \u00E1: "a\u0301",
                     \u00E0: "a\u0300",
                     \u00E4: "a\u0308",
                     \u01DF: "a\u0308\u0304",
                     \u00E3: "a\u0303",
                     \u0101: "a\u0304",
                     \u0103: "a\u0306",
@@ -15291,15 +15291,15 @@
                     \u1FE9: "\u03A5\u0304",
                     \u1FE8: "\u03A5\u0306",
                     \u038F: "\u03A9\u0301",
                     \u1FFA: "\u03A9\u0300"
                 };
             class a0 {
                 constructor(t, o) {
-                    this.mode = void 0, this.gullet = void 0, this.settings = void 0, this.leftrightDepth = void 0, this.nextToken = void 0, this.mode = "math", this.gullet = new Z1(t, o, this.mode), this.settings = o, this.leftrightDepth = 0
+                    this.mode = void 0, this.gullet = void 0, this.settings = void 0, this.leftrightDepth = void 0, this.nextToken = void 0, this.mode = "math", this.gullet = new X1(t, o, this.mode), this.settings = o, this.leftrightDepth = 0
                 }
                 expect(t, o) {
                     if (o === void 0 && (o = !0), this.fetch().text !== t) throw new a("Expected '" + t + "', got '" + this.fetch().text + "'", this.fetch());
                     o && this.consume()
                 }
                 consume() {
                     this.nextToken = null
@@ -15420,19 +15420,19 @@
                             for (this.consume(); this.fetch().text === "'";) v.push(b), this.consume();
                             this.fetch().text === "^" && v.push(this.handleSupSubscript("superscript")), s = {
                                 type: "ordgroup",
                                 mode: this.mode,
                                 body: v
                             }
                         } else if (o0[p.text]) {
-                            let b = Xo.test(p.text),
+                            let b = Ko.test(p.text),
                                 v = [];
                             for (v.push(new mt(o0[p.text])), this.consume();;) {
                                 let E = this.fetch().text;
-                                if (!o0[E] || Xo.test(E) !== b) break;
+                                if (!o0[E] || Ko.test(E) !== b) break;
                                 v.unshift(new mt(o0[E])), this.consume()
                             }
                             let S = this.subparse(v);
                             b ? u = {
                                 type: "ordgroup",
                                 mode: "math",
                                 body: S
@@ -15580,15 +15580,15 @@
                     !t && o.text.length === 0 && (o.text = "0pt", s = !0);
                     let u = /([-+]?) *(\d+(?:\.\d*)?|\.\d+) *([a-z]{2})/.exec(o.text);
                     if (!u) throw new a("Invalid size: '" + o.text + "'", o);
                     let p = {
                         number: +(u[1] + u[2]),
                         unit: u[3]
                     };
-                    if (!Fi(p)) throw new a("Invalid unit: '" + p.unit + "'", o);
+                    if (!Ni(p)) throw new a("Invalid unit: '" + p.unit + "'", o);
                     return {
                         type: "size",
                         mode: this.mode,
                         value: p,
                         isBlank: s
                     }
                 }
@@ -15631,15 +15631,15 @@
                         this.expect(b), this.gullet.endGroup(), p = {
                             type: "ordgroup",
                             mode: this.mode,
                             loc: st.range(s, S),
                             body: v,
                             semisimple: u === "\\begingroup" || void 0
                         }
-                    } else if (p = this.parseFunction(o, t) || this.parseSymbol(), p == null && u[0] === "\\" && !Qo.hasOwnProperty(u)) {
+                    } else if (p = this.parseFunction(o, t) || this.parseSymbol(), p == null && u[0] === "\\" && !Jo.hasOwnProperty(u)) {
                         if (this.settings.throwOnError) throw new a("Undefined control sequence: " + u, s);
                         p = this.formatUnsupportedCmd(u), this.consume()
                     }
                     return p
                 }
                 formLigatures(t) {
                     let o = t.length - 1;
@@ -15676,24 +15676,24 @@
                         return p = p.slice(1, -1), {
                             type: "verb",
                             mode: "text",
                             body: p,
                             star: b
                         }
                     }
-                    Jo.hasOwnProperty(o[0]) && !Oe[this.mode][o[0]] && (this.settings.strict && this.mode === "math" && this.settings.reportNonstrict("unicodeTextInMathMode", 'Accented Unicode text character "' + o[0] + '" used in math mode', t), o = Jo[o[0]] + o.slice(1));
-                    let s = j1.exec(o);
+                    ea.hasOwnProperty(o[0]) && !Oe[this.mode][o[0]] && (this.settings.strict && this.mode === "math" && this.settings.reportNonstrict("unicodeTextInMathMode", 'Accented Unicode text character "' + o[0] + '" used in math mode', t), o = ea[o[0]] + o.slice(1));
+                    let s = W1.exec(o);
                     s && (o = o.substring(0, s.index), o === "i" ? o = "\u0131" : o === "j" && (o = "\u0237"));
                     let u;
                     if (Oe[this.mode][o]) {
-                        this.settings.strict && this.mode === "math" && Z0.indexOf(o) >= 0 && this.settings.reportNonstrict("unicodeTextInMathMode", 'Latin-1/Unicode text character "' + o[0] + '" used in math mode', t);
+                        this.settings.strict && this.mode === "math" && Q0.indexOf(o) >= 0 && this.settings.reportNonstrict("unicodeTextInMathMode", 'Latin-1/Unicode text character "' + o[0] + '" used in math mode', t);
                         let p = Oe[this.mode][o].group,
                             b = st.range(t),
                             v;
-                        if (ju.hasOwnProperty(p)) {
+                        if (Wu.hasOwnProperty(p)) {
                             let S = p;
                             v = {
                                 type: "atom",
                                 mode: this.mode,
                                 family: S,
                                 loc: b,
                                 text: o
@@ -15711,16 +15711,16 @@
                         loc: st.range(t),
                         text: o
                     };
                     else return null;
                     if (this.consume(), s)
                         for (let p = 0; p < s[0].length; p++) {
                             let b = s[0][p];
-                            if (!Tn[b]) throw new a("Unknown accent ' " + b + "'", t);
-                            let v = Tn[b][this.mode] || Tn[b].text;
+                            if (!An[b]) throw new a("Unknown accent ' " + b + "'", t);
+                            let v = An[b][this.mode] || An[b].text;
                             if (!v) throw new a("Accent " + b + " unsupported in " + this.mode + " mode", t);
                             u = {
                                 type: "accent",
                                 mode: this.mode,
                                 loc: st.range(t),
                                 label: v,
                                 isStretchy: !1,
@@ -15728,15 +15728,15 @@
                                 base: u
                             }
                         }
                     return u
                 }
             }
             a0.endOfExpression = ["}", "\\endgroup", "\\end", "\\right", "&"];
-            var An = function(n, t) {
+            var qn = function(n, t) {
                 if (!(typeof n == "string" || n instanceof String)) throw new TypeError("KaTeX can only parse string typed expression");
                 let o = new a0(n, t);
                 delete o.gullet.macros.current["\\df@tag"];
                 let s = o.parse();
                 if (delete o.gullet.macros.current["\\current@color"], delete o.gullet.macros.current["\\color"], o.gullet.macros.get("\\df@tag")) {
                     if (!t.displayMode) throw new a("\\tag works only in display equations");
                     s = [{
@@ -15744,167 +15744,167 @@
                         mode: "text",
                         body: s,
                         tag: o.subparse([new mt("\\df@tag")])
                     }]
                 }
                 return s
             };
-            let Ko = function(n, t, o) {
+            let ta = function(n, t, o) {
                 t.textContent = "";
-                let s = qn(n, o).toNode();
+                let s = Mn(n, o).toNode();
                 t.appendChild(s)
             };
-            typeof document < "u" && document.compatMode !== "CSS1Compat" && (typeof console < "u" && console.warn("Warning: KaTeX doesn't work in quirks mode. Make sure your website has a suitable doctype."), Ko = function() {
+            typeof document < "u" && document.compatMode !== "CSS1Compat" && (typeof console < "u" && console.warn("Warning: KaTeX doesn't work in quirks mode. Make sure your website has a suitable doctype."), ta = function() {
                 throw new a("KaTeX doesn't work in quirks mode.")
             });
-            let Q1 = function(n, t) {
-                    return qn(n, t).toMarkup()
+            let J1 = function(n, t) {
+                    return Mn(n, t).toMarkup()
                 },
-                X1 = function(n, t) {
+                K1 = function(n, t) {
                     let o = new I(t);
-                    return An(n, o)
+                    return qn(n, o)
                 },
-                ea = function(n, t, o) {
+                ra = function(n, t, o) {
                     if (o.throwOnError || !(n instanceof a)) throw n;
                     let s = B.makeSpan(["katex-error"], [new ut(t)]);
                     return s.setAttribute("title", n.toString()), s.setAttribute("style", "color:" + o.errorColor), s
                 },
-                qn = function(n, t) {
+                Mn = function(n, t) {
                     let o = new I(t);
                     try {
-                        let s = An(n, o);
-                        return d1(s, n, o)
+                        let s = qn(n, o);
+                        return p1(s, n, o)
                     } catch (s) {
-                        return ea(s, n, o)
+                        return ra(s, n, o)
                     }
                 };
-            var J1 = {
+            var eh = {
                     version: "0.16.10",
-                    render: Ko,
-                    renderToString: Q1,
+                    render: ta,
+                    renderToString: J1,
                     ParseError: a,
                     SETTINGS_SCHEMA: O,
-                    __parse: X1,
-                    __renderToDomTree: qn,
+                    __parse: K1,
+                    __renderToDomTree: Mn,
                     __renderToHTMLTree: function(n, t) {
                         let o = new I(t);
                         try {
-                            let s = An(n, o);
-                            return m1(s, n, o)
+                            let s = qn(n, o);
+                            return f1(s, n, o)
                         } catch (s) {
-                            return ea(s, n, o)
+                            return ra(s, n, o)
                         }
                     },
-                    __setFontMetrics: Lu,
+                    __setFontMetrics: Iu,
                     __defineSymbol: h,
                     __defineFunction: Q,
                     __defineMacro: k,
                     __domTree: {
                         Span: vr,
-                        Anchor: W0,
+                        Anchor: Y0,
                         SymbolNode: ut,
                         SvgNode: Et,
                         PathNode: Ot,
-                        LineNode: Y0
+                        LineNode: Z0
                     }
                 },
-                K1 = J1;
+                th = eh;
             return e = e.default, e
         }()
     })
 });
-var Tu = W(Hr => {
+var qu = W(Hr => {
     "use strict";
-    var Lp = Hr && Hr.__importDefault || function(r) {
+    var Ip = Hr && Hr.__importDefault || function(r) {
         return r && r.__esModule ? r : {
             default: r
         }
     };
     Object.defineProperty(Hr, "__esModule", {
         value: !0
     });
-    var vu = Lp(xu());
+    var ku = Ip(wu());
 
-    function wu(r, e) {
+    function _u(r, e) {
         let i = r.src[e - 1],
             a = r.src[e],
             l = r.src[e + 1];
         if (a !== "$") return {
             can_open: !1,
             can_close: !1
         };
         let c = !1,
             d = !1;
-        return i !== "$" && i !== "\\" && (i === void 0 || ku(i) || !_u(i)) && (c = !0), l !== "$" && (l == null || ku(l) || !_u(l)) && (d = !0), {
+        return i !== "$" && i !== "\\" && (i === void 0 || Su(i) || !Cu(i)) && (c = !0), l !== "$" && (l == null || Su(l) || !Cu(l)) && (d = !0), {
             can_open: c,
             can_close: d
         }
     }
 
-    function ku(r) {
+    function Su(r) {
         return /^\s$/u.test(r)
     }
 
-    function _u(r) {
+    function Cu(r) {
         return /^[\w\d]$/u.test(r)
     }
 
-    function Su(r, e) {
+    function Tu(r, e) {
         let i = r.src[e - 1],
             a = r.src[e],
             l = r.src[e + 1],
             c = r.src[e + 2];
         return a === "$" && i !== "$" && i !== "\\" && l === "$" && c !== "$" ? {
             can_open: !0,
             can_close: !0
         } : {
             can_open: !1,
             can_close: !1
         }
     }
 
-    function Pp(r, e) {
+    function Op(r, e) {
         if (r.src[r.pos] !== "$") return !1;
         let i = r.tokens.at(-1);
         if (i?.type === "html_inline" && /^<\w+.+[^/]>$/.test(i.content)) return !1;
-        let a = wu(r, r.pos);
+        let a = _u(r, r.pos);
         if (!a.can_open) return e || (r.pending += "$"), r.pos += 1, !0;
         let l = r.pos + 1,
             c = l,
             d;
         for (;
             (c = r.src.indexOf("$", c)) !== -1;) {
             for (d = c - 1; r.src[d] === "\\";) d -= 1;
             if ((c - d) % 2 == 1) break;
             c += 1
         }
         if (c === -1) return e || (r.pending += "$"), r.pos = l, !0;
         if (c - l === 0) return e || (r.pending += "$$"), r.pos = l + 1, !0;
-        if (a = wu(r, c), !a.can_close) return e || (r.pending += "$"), r.pos = l, !0;
+        if (a = _u(r, c), !a.can_close) return e || (r.pending += "$"), r.pos = l, !0;
         if (!e) {
             let f = r.push("math_inline", "math", 0);
             f.markup = "$", f.content = r.src.slice(l, c)
         }
         return r.pos = c + 1, !0
     }
 
-    function Ip(r, e, i, a) {
+    function Hp(r, e, i, a) {
         var l, c, d, f = !1,
             g, y = r.bMarks[e] + r.tShift[e],
             _ = r.eMarks[e];
         if (y + 2 > _ || r.src.slice(y, y + 2) !== "$$") return !1;
         y += 2;
         let w = r.src.slice(y, _);
         if (a) return !0;
         for (w.trim().slice(-2) === "$$" && (w = w.trim().slice(0, -2), f = !0), c = e; !f && (c++, !(c >= i || (y = r.bMarks[c] + r.tShift[c], _ = r.eMarks[c], y < _ && r.tShift[c] < r.blkIndent)));) r.src.slice(y, _).trim().slice(-2) === "$$" ? (d = r.src.slice(0, _).lastIndexOf("$$"), l = r.src.slice(y, d), f = !0) : r.src.slice(y, _).trim().includes("$$") && (d = r.src.slice(0, _).trim().indexOf("$$"), l = r.src.slice(y, d), f = !0);
         return r.line = c + 1, g = r.push("math_block", "math", 0), g.block = !0, g.content = (w && w.trim() ? w + `
 ` : "") + r.getLines(e + 1, c, r.tShift[e], !0) + (l && l.trim() ? l : ""), g.map = [e, r.line], g.markup = "$$", !0
     }
 
-    function Op(r, e, i, a) {
+    function $p(r, e, i, a) {
         let l = r.bMarks[e] + r.tShift[e],
             c = r.eMarks[e];
         if (!r.src.slice(l, c).match(/^\s*\\begin\s*\{([^{}]+)\}/)) return !1;
         if (e > 0) {
             let A = r.bMarks[e - 1] + r.tShift[e - 1],
                 L = r.eMarks[e - 1],
                 R = r.src.slice(A, L);
@@ -15927,28 +15927,28 @@
             }
         }
         r.line = y + 1;
         let T = r.push("math_block", "math", 0);
         return T.block = !0, T.content = (r.getLines(e, y, r.tShift[e], !0) + (_ ?? "")).trim(), T.map = [e, r.line], T.markup = "$$", !0
     }
 
-    function Hp(r, e) {
+    function Gp(r, e) {
         var i, a, l, c, d;
         if (r.src.slice(r.pos, r.pos + 2) !== "$$") return !1;
-        if (c = Su(r, r.pos), !c.can_open) return e || (r.pending += "$$"), r.pos += 2, !0;
+        if (c = Tu(r, r.pos), !c.can_open) return e || (r.pending += "$$"), r.pos += 2, !0;
         for (i = r.pos + 2, a = i;
             (a = r.src.indexOf("$$", a)) !== -1;) {
             for (d = a - 1; r.src[d] === "\\";) d -= 1;
             if ((a - d) % 2 == 1) break;
             a += 2
         }
-        return a === -1 ? (e || (r.pending += "$$"), r.pos = i, !0) : a - i === 0 ? (e || (r.pending += "$$$$"), r.pos = i + 2, !0) : (c = Su(r, a), c.can_close ? (e || (l = r.push("math_block", "math", 0), l.block = !0, l.markup = "$$", l.content = r.src.slice(i, a)), r.pos = a + 2, !0) : (e || (r.pending += "$$"), r.pos = i, !0))
+        return a === -1 ? (e || (r.pending += "$$"), r.pos = i, !0) : a - i === 0 ? (e || (r.pending += "$$$$"), r.pos = i + 2, !0) : (c = Tu(r, a), c.can_close ? (e || (l = r.push("math_block", "math", 0), l.block = !0, l.markup = "$$", l.content = r.src.slice(i, a)), r.pos = a + 2, !0) : (e || (r.pending += "$$"), r.pos = i, !0))
     }
 
-    function $p(r, e) {
+    function Vp(r, e) {
         let i = r.src.slice(r.pos);
         if (!/^\n\\begin/.test(i)) return !1;
         if (r.pos += 1, e) return !0;
         let a = i.split(/\n/g).slice(1),
             l, c = [];
         e: for (var d = 0; d < a.length; ++d) {
             let y = a[d];
@@ -15961,15 +15961,15 @@
         }
         if (typeof l > "u") return !1;
         let f = a.slice(0, l + 1).reduce((y, _) => y + _.length, 0) + l + 1,
             g = r.push("math_inline_bare_block", "math", 0);
         return g.block = !0, g.markup = "$$", g.content = i.slice(1, f), r.pos = r.pos + f, !0
     }
 
-    function Cu(r, e, i, a) {
+    function Au(r, e, i, a) {
         let l = r.tokens;
         for (let c = l.length - 1; c >= 0; c--) {
             let d = l[c],
                 f = [];
             if (d.type !== "html_block") continue;
             let g = d.content;
             for (let y of g.matchAll(a)) {
@@ -15998,68 +15998,68 @@
                 })
             }
             f.length > 0 && l.splice(c, 1, ...f)
         }
         return !0
     }
 
-    function O0(r) {
+    function H0(r) {
         return r.replace(/&/g, "&amp;").replace(/</g, "&lt;").replace(/>/g, "&gt;").replace(/"/g, "&quot;").replace(/'/g, "&#039;")
     }
 
-    function Gp(r, e) {
+    function jp(r, e) {
         let i = e?.enableBareBlocks,
             a = e?.enableMathBlockInHtml,
             l = e?.enableMathInlineInHtml,
             c = w => {
                 let T = /\\begin\{(align|equation|gather|cd|alignat)\}/ig.test(w);
                 try {
-                    return vu.default.renderToString(w, {
+                    return ku.default.renderToString(w, {
                         ...e,
                         displayMode: T
                     })
                 } catch (A) {
-                    return e?.throwOnError && console.log(A), `<span class="katex-error" title="${O0(w)}">${O0(A+"")}</span>`
+                    return e?.throwOnError && console.log(A), `<span class="katex-error" title="${H0(w)}">${H0(A+"")}</span>`
                 }
             },
             d = (w, T) => c(w[T].content),
             f = w => {
                 try {
-                    return `<p class="katex-block">${vu.default.renderToString(w,{...e,displayMode:!0})}</p>`
+                    return `<p class="katex-block">${ku.default.renderToString(w,{...e,displayMode:!0})}</p>`
                 } catch (T) {
-                    return e?.throwOnError && console.log(T), `<p class="katex-block katex-error" title="${O0(w)}">${O0(T+"")}</p>`
+                    return e?.throwOnError && console.log(T), `<p class="katex-block katex-error" title="${H0(w)}">${H0(T+"")}</p>`
                 }
             },
             g = (w, T) => f(w[T].content) + `
 `;
-        r.inline.ruler.after("escape", "math_inline", Pp), r.inline.ruler.after("escape", "math_inline_block", Hp), i && r.inline.ruler.before("text", "math_inline_bare_block", $p), r.block.ruler.after("blockquote", "math_block", (w, T, A, L) => i && Op(w, T, A, L) ? !0 : Ip(w, T, A, L), {
+        r.inline.ruler.after("escape", "math_inline", Op), r.inline.ruler.after("escape", "math_inline_block", Gp), i && r.inline.ruler.before("text", "math_inline_bare_block", Vp), r.block.ruler.after("blockquote", "math_block", (w, T, A, L) => i && $p(w, T, A, L) ? !0 : Hp(w, T, A, L), {
             alt: ["paragraph", "reference", "blockquote", "list"]
         });
         let y = /(?<html_before_math>[\s\S]*?)\$\$(?<math>[\s\S]+?)\$\$(?<html_after_math>(?:(?!\$\$[\s\S]+?\$\$)[\s\S])*)/gm,
             _ = /(?<html_before_math>[\s\S]*?)\$(?<math>.*?)\$(?<html_after_math>(?:(?!\$.*?\$)[\s\S])*)/gm;
-        a && r.core.ruler.push("math_block_in_html_block", w => Cu(w, "math_block", "$$", y)), l && r.core.ruler.push("math_inline_in_html_block", w => Cu(w, "math_inline", "$", _)), r.renderer.rules.math_inline = d, r.renderer.rules.math_inline_block = g, r.renderer.rules.math_inline_bare_block = g, r.renderer.rules.math_block = g
+        a && r.core.ruler.push("math_block_in_html_block", w => Au(w, "math_block", "$$", y)), l && r.core.ruler.push("math_inline_in_html_block", w => Au(w, "math_inline", "$", _)), r.renderer.rules.math_inline = d, r.renderer.rules.math_inline_block = g, r.renderer.rules.math_inline_bare_block = g, r.renderer.rules.math_block = g
     }
-    Hr.default = Gp
+    Hr.default = jp
 });
-var d0, Me, ca, lh, er, ia, ua, En, ch, Tr = {},
-    ha = [],
-    uh = /acit|ex(?:s|g|n|p|$)|rph|grid|ows|mnc|ntw|ine[ch]|zoo|^ord|itera/i,
-    zn = Array.isArray;
+var d0, Me, ha, uh, er, aa, da, Dn, hh, Tr = {},
+    ma = [],
+    dh = /acit|ex(?:s|g|n|p|$)|rph|grid|ows|mnc|ntw|ine[ch]|zoo|^ord|itera/i,
+    Rn = Array.isArray;
 
 function Vt(r, e) {
     for (var i in e) r[i] = e[i];
     return r
 }
 
-function da(r) {
+function pa(r) {
     var e = r.parentNode;
     e && e.removeChild(r)
 }
 
-function hh(r, e, i) {
+function Fn(r, e, i) {
     var a, l, c, d = {};
     for (c in e) c == "key" ? a = e[c] : c == "ref" ? l = e[c] : d[c] = e[c];
     if (arguments.length > 2 && (d.children = arguments.length > 3 ? d0.call(arguments, 2) : i), typeof r == "function" && r.defaultProps != null)
         for (c in r.defaultProps) d[c] === void 0 && (d[c] = r.defaultProps[c]);
     return c0(r, d, a, l, null)
 }
 
@@ -16072,15 +16072,15 @@
         __k: null,
         __: null,
         __b: 0,
         __e: null,
         __d: void 0,
         __c: null,
         constructor: void 0,
-        __v: l ?? ++ca,
+        __v: l ?? ++ha,
         __i: -1,
         __u: 0
     };
     return l == null && Me.vnode != null && Me.vnode(c), c
 }
 
 function Ge(r) {
@@ -16094,66 +16094,66 @@
 function tr(r, e) {
     if (e == null) return r.__ ? tr(r.__, r.__i + 1) : null;
     for (var i; e < r.__k.length; e++)
         if ((i = r.__k[e]) != null && i.__e != null) return i.__e;
     return typeof r.type == "function" ? tr(r) : null
 }
 
-function ma(r) {
+function fa(r) {
     var e, i;
     if ((r = r.__) != null && r.__c != null) {
         for (r.__e = r.__c.base = null, e = 0; e < r.__k.length; e++)
             if ((i = r.__k[e]) != null && i.__e != null) {
                 r.__e = r.__c.base = i.__e;
                 break
-            } return ma(r)
+            } return fa(r)
     }
 }
 
-function oa(r) {
-    (!r.__d && (r.__d = !0) && er.push(r) && !h0.__r++ || ia !== Me.debounceRendering) && ((ia = Me.debounceRendering) || ua)(h0)
+function sa(r) {
+    (!r.__d && (r.__d = !0) && er.push(r) && !h0.__r++ || aa !== Me.debounceRendering) && ((aa = Me.debounceRendering) || da)(h0)
 }
 
 function h0() {
     var r, e, i, a, l, c, d, f, g;
-    for (er.sort(En); r = er.shift();) r.__d && (e = er.length, a = void 0, c = (l = (i = r).__v).__e, f = [], g = [], (d = i.__P) && ((a = Vt({}, l)).__v = l.__v + 1, Me.vnode && Me.vnode(a), Rn(d, a, l, i.__n, d.ownerSVGElement !== void 0, 32 & l.__u ? [c] : null, f, c ?? tr(l), !!(32 & l.__u), g), a.__v = l.__v, a.__.__k[a.__i] = a, ga(f, a, g), a.__e != c && ma(a)), er.length > e && er.sort(En));
+    for (er.sort(Dn); r = er.shift();) r.__d && (e = er.length, a = void 0, c = (l = (i = r).__v).__e, f = [], g = [], (d = i.__P) && ((a = Vt({}, l)).__v = l.__v + 1, Me.vnode && Me.vnode(a), Bn(d, a, l, i.__n, d.ownerSVGElement !== void 0, 32 & l.__u ? [c] : null, f, c ?? tr(l), !!(32 & l.__u), g), a.__v = l.__v, a.__.__k[a.__i] = a, ya(f, a, g), a.__e != c && fa(a)), er.length > e && er.sort(Dn));
     h0.__r = 0
 }
 
-function pa(r, e, i, a, l, c, d, f, g, y, _) {
-    var w, T, A, L, R, O = a && a.__k || ha,
+function ga(r, e, i, a, l, c, d, f, g, y, _) {
+    var w, T, A, L, R, O = a && a.__k || ma,
         P = e.length;
-    for (i.__d = g, dh(i, e, O), g = i.__d, w = 0; w < P; w++)(A = i.__k[w]) != null && typeof A != "boolean" && typeof A != "function" && (T = A.__i === -1 ? Tr : O[A.__i] || Tr, A.__i = w, Rn(r, A, T, l, c, d, f, g, y, _), L = A.__e, A.ref && T.ref != A.ref && (T.ref && Fn(T.ref, null, A), _.push(A.ref, A.__c || L, A)), R == null && L != null && (R = L), 65536 & A.__u || T.__k === A.__k ? (L || T.__e != g || (g = tr(T)), g = fa(A, g, r)) : typeof A.type == "function" && A.__d !== void 0 ? g = A.__d : L && (g = L.nextSibling), A.__d = void 0, A.__u &= -196609);
+    for (i.__d = g, mh(i, e, O), g = i.__d, w = 0; w < P; w++)(A = i.__k[w]) != null && typeof A != "boolean" && typeof A != "function" && (T = A.__i === -1 ? Tr : O[A.__i] || Tr, A.__i = w, Bn(r, A, T, l, c, d, f, g, y, _), L = A.__e, A.ref && T.ref != A.ref && (T.ref && Nn(T.ref, null, A), _.push(A.ref, A.__c || L, A)), R == null && L != null && (R = L), 65536 & A.__u || T.__k === A.__k ? (L || T.__e != g || (g = tr(T)), g = ba(A, g, r)) : typeof A.type == "function" && A.__d !== void 0 ? g = A.__d : L && (g = L.nextSibling), A.__d = void 0, A.__u &= -196609);
     i.__d = g, i.__e = R
 }
 
-function dh(r, e, i) {
+function mh(r, e, i) {
     var a, l, c, d, f, g = e.length,
         y = i.length,
         _ = y,
         w = 0;
-    for (r.__k = [], a = 0; a < g; a++) d = a + w, (l = r.__k[a] = (l = e[a]) == null || typeof l == "boolean" || typeof l == "function" ? null : typeof l == "string" || typeof l == "number" || typeof l == "bigint" || l.constructor == String ? c0(null, l, null, null, null) : zn(l) ? c0(Ge, {
+    for (r.__k = [], a = 0; a < g; a++) d = a + w, (l = r.__k[a] = (l = e[a]) == null || typeof l == "boolean" || typeof l == "function" ? null : typeof l == "string" || typeof l == "number" || typeof l == "bigint" || l.constructor == String ? c0(null, l, null, null, null) : Rn(l) ? c0(Ge, {
         children: l
-    }, null, null, null) : l.constructor === void 0 && l.__b > 0 ? c0(l.type, l.props, l.key, l.ref ? l.ref : null, l.__v) : l) != null ? (l.__ = r, l.__b = r.__b + 1, f = mh(l, i, d, _), l.__i = f, c = null, f !== -1 && (_--, (c = i[f]) && (c.__u |= 131072)), c == null || c.__v === null ? (f == -1 && w--, typeof l.type != "function" && (l.__u |= 65536)) : f !== d && (f === d + 1 ? w++ : f > d ? _ > g - d ? w += f - d : w-- : f < d ? f == d - 1 && (w = f - d) : w = 0, f !== a + w && (l.__u |= 65536))) : (c = i[d]) && c.key == null && c.__e && !(131072 & c.__u) && (c.__e == r.__d && (r.__d = tr(c)), Dn(c, c, !1), i[d] = null, _--);
+    }, null, null, null) : l.constructor === void 0 && l.__b > 0 ? c0(l.type, l.props, l.key, l.ref ? l.ref : null, l.__v) : l) != null ? (l.__ = r, l.__b = r.__b + 1, f = ph(l, i, d, _), l.__i = f, c = null, f !== -1 && (_--, (c = i[f]) && (c.__u |= 131072)), c == null || c.__v === null ? (f == -1 && w--, typeof l.type != "function" && (l.__u |= 65536)) : f !== d && (f === d + 1 ? w++ : f > d ? _ > g - d ? w += f - d : w-- : f < d ? f == d - 1 && (w = f - d) : w = 0, f !== a + w && (l.__u |= 65536))) : (c = i[d]) && c.key == null && c.__e && !(131072 & c.__u) && (c.__e == r.__d && (r.__d = tr(c)), zn(c, c, !1), i[d] = null, _--);
     if (_)
-        for (a = 0; a < y; a++)(c = i[a]) != null && !(131072 & c.__u) && (c.__e == r.__d && (r.__d = tr(c)), Dn(c, c))
+        for (a = 0; a < y; a++)(c = i[a]) != null && !(131072 & c.__u) && (c.__e == r.__d && (r.__d = tr(c)), zn(c, c))
 }
 
-function fa(r, e, i) {
+function ba(r, e, i) {
     var a, l;
     if (typeof r.type == "function") {
-        for (a = r.__k, l = 0; a && l < a.length; l++) a[l] && (a[l].__ = r, e = fa(a[l], e, i));
+        for (a = r.__k, l = 0; a && l < a.length; l++) a[l] && (a[l].__ = r, e = ba(a[l], e, i));
         return e
     }
     r.__e != e && (i.insertBefore(r.__e, e || null), e = r.__e);
     do e = e && e.nextSibling; while (e != null && e.nodeType === 8);
     return e
 }
 
-function mh(r, e, i, a) {
+function ph(r, e, i, a) {
     var l = r.key,
         c = r.type,
         d = i - 1,
         f = i + 1,
         g = e[i];
     if (g === null || g && l == g.key && c === g.type && !(131072 & g.__u)) return i;
     if (a > (g != null && !(131072 & g.__u) ? 1 : 0))
@@ -16166,59 +16166,59 @@
                 if ((g = e[f]) && !(131072 & g.__u) && l == g.key && c === g.type) return f;
                 f++
             }
         }
     return -1
 }
 
-function aa(r, e, i) {
-    e[0] === "-" ? r.setProperty(e, i ?? "") : r[e] = i == null ? "" : typeof i != "number" || uh.test(e) ? i : i + "px"
+function la(r, e, i) {
+    e[0] === "-" ? r.setProperty(e, i ?? "") : r[e] = i == null ? "" : typeof i != "number" || dh.test(e) ? i : i + "px"
 }
 
 function l0(r, e, i, a, l) {
     var c;
     e: if (e === "style")
         if (typeof i == "string") r.style.cssText = i;
         else {
             if (typeof a == "string" && (r.style.cssText = a = ""), a)
-                for (e in a) i && e in i || aa(r.style, e, "");
+                for (e in a) i && e in i || la(r.style, e, "");
             if (i)
-                for (e in i) a && i[e] === a[e] || aa(r.style, e, i[e])
+                for (e in i) a && i[e] === a[e] || la(r.style, e, i[e])
         }
-    else if (e[0] === "o" && e[1] === "n") c = e !== (e = e.replace(/(PointerCapture)$|Capture$/i, "$1")), e = e.toLowerCase() in r || e === "onFocusOut" || e === "onFocusIn" ? e.toLowerCase().slice(2) : e.slice(2), r.l || (r.l = {}), r.l[e + c] = i, i ? a ? i.u = a.u : (i.u = Date.now(), r.addEventListener(e, c ? la : sa, c)) : r.removeEventListener(e, c ? la : sa, c);
+    else if (e[0] === "o" && e[1] === "n") c = e !== (e = e.replace(/(PointerCapture)$|Capture$/i, "$1")), e = e.toLowerCase() in r || e === "onFocusOut" || e === "onFocusIn" ? e.toLowerCase().slice(2) : e.slice(2), r.l || (r.l = {}), r.l[e + c] = i, i ? a ? i.u = a.u : (i.u = Date.now(), r.addEventListener(e, c ? ua : ca, c)) : r.removeEventListener(e, c ? ua : ca, c);
     else {
         if (l) e = e.replace(/xlink(H|:h)/, "h").replace(/sName$/, "s");
         else if (e !== "width" && e !== "height" && e !== "href" && e !== "list" && e !== "form" && e !== "tabIndex" && e !== "download" && e !== "rowSpan" && e !== "colSpan" && e !== "role" && e in r) try {
             r[e] = i ?? "";
             break e
         } catch {}
         typeof i == "function" || (i == null || i === !1 && e[4] !== "-" ? r.removeAttribute(e) : r.setAttribute(e, i))
     }
 }
 
-function sa(r) {
+function ca(r) {
     if (this.l) {
         var e = this.l[r.type + !1];
         if (r.t) {
             if (r.t <= e.u) return
         } else r.t = Date.now();
         return e(Me.event ? Me.event(r) : r)
     }
 }
 
-function la(r) {
+function ua(r) {
     if (this.l) return this.l[r.type + !0](Me.event ? Me.event(r) : r)
 }
 
-function Rn(r, e, i, a, l, c, d, f, g, y) {
+function Bn(r, e, i, a, l, c, d, f, g, y) {
     var _, w, T, A, L, R, O, P, I, Y, re, te, j, ne, pe, ue = e.type;
     if (e.constructor !== void 0) return null;
     128 & i.__u && (g = !!(32 & i.__u), c = [f = e.__e = i.__e]), (_ = Me.__b) && _(e);
     e: if (typeof ue == "function") try {
-        if (P = e.props, I = (_ = ue.contextType) && a[_.__c], Y = _ ? I ? I.props.value : _.__ : a, i.__c ? O = (w = e.__c = i.__c).__ = w.__E : ("prototype" in ue && ue.prototype.render ? e.__c = w = new ue(P, Y) : (e.__c = w = new u0(P, Y), w.constructor = ue, w.render = fh), I && I.sub(w), w.props = P, w.state || (w.state = {}), w.context = Y, w.__n = a, T = w.__d = !0, w.__h = [], w._sb = []), w.__s == null && (w.__s = w.state), ue.getDerivedStateFromProps != null && (w.__s == w.state && (w.__s = Vt({}, w.__s)), Vt(w.__s, ue.getDerivedStateFromProps(P, w.__s))), A = w.props, L = w.state, w.__v = e, T) ue.getDerivedStateFromProps == null && w.componentWillMount != null && w.componentWillMount(), w.componentDidMount != null && w.__h.push(w.componentDidMount);
+        if (P = e.props, I = (_ = ue.contextType) && a[_.__c], Y = _ ? I ? I.props.value : _.__ : a, i.__c ? O = (w = e.__c = i.__c).__ = w.__E : ("prototype" in ue && ue.prototype.render ? e.__c = w = new ue(P, Y) : (e.__c = w = new u0(P, Y), w.constructor = ue, w.render = gh), I && I.sub(w), w.props = P, w.state || (w.state = {}), w.context = Y, w.__n = a, T = w.__d = !0, w.__h = [], w._sb = []), w.__s == null && (w.__s = w.state), ue.getDerivedStateFromProps != null && (w.__s == w.state && (w.__s = Vt({}, w.__s)), Vt(w.__s, ue.getDerivedStateFromProps(P, w.__s))), A = w.props, L = w.state, w.__v = e, T) ue.getDerivedStateFromProps == null && w.componentWillMount != null && w.componentWillMount(), w.componentDidMount != null && w.__h.push(w.componentDidMount);
         else {
             if (ue.getDerivedStateFromProps == null && P !== A && w.componentWillReceiveProps != null && w.componentWillReceiveProps(P, Y), !w.__e && (w.shouldComponentUpdate != null && w.shouldComponentUpdate(P, w.__s, Y) === !1 || e.__v === i.__v)) {
                 for (e.__v !== i.__v && (w.props = P, w.state = w.__s, w.__d = !1), e.__e = i.__e, e.__k = i.__k, e.__k.forEach(function(ce) {
                         ce && (ce.__ = e)
                     }), re = 0; re < w._sb.length; re++) w.__h.push(w._sb[re]);
                 w._sb = [], w.__h.length && d.push(w);
                 break e
@@ -16228,36 +16228,36 @@
             })
         }
         if (w.context = Y, w.props = P, w.__P = r, w.__e = !1, te = Me.__r, j = 0, "prototype" in ue && ue.prototype.render) {
             for (w.state = w.__s, w.__d = !1, te && te(e), _ = w.render(w.props, w.state, w.context), ne = 0; ne < w._sb.length; ne++) w.__h.push(w._sb[ne]);
             w._sb = []
         } else
             do w.__d = !1, te && te(e), _ = w.render(w.props, w.state, w.context), w.state = w.__s; while (w.__d && ++j < 25);
-        w.state = w.__s, w.getChildContext != null && (a = Vt(Vt({}, a), w.getChildContext())), T || w.getSnapshotBeforeUpdate == null || (R = w.getSnapshotBeforeUpdate(A, L)), pa(r, zn(pe = _ != null && _.type === Ge && _.key == null ? _.props.children : _) ? pe : [pe], e, i, a, l, c, d, f, g, y), w.base = e.__e, e.__u &= -161, w.__h.length && d.push(w), O && (w.__E = w.__ = null)
+        w.state = w.__s, w.getChildContext != null && (a = Vt(Vt({}, a), w.getChildContext())), T || w.getSnapshotBeforeUpdate == null || (R = w.getSnapshotBeforeUpdate(A, L)), ga(r, Rn(pe = _ != null && _.type === Ge && _.key == null ? _.props.children : _) ? pe : [pe], e, i, a, l, c, d, f, g, y), w.base = e.__e, e.__u &= -161, w.__h.length && d.push(w), O && (w.__E = w.__ = null)
     } catch (ce) {
         e.__v = null, g || c != null ? (e.__e = f, e.__u |= g ? 160 : 32, c[c.indexOf(f)] = null) : (e.__e = i.__e, e.__k = i.__k), Me.__e(ce, e, i)
-    } else c == null && e.__v === i.__v ? (e.__k = i.__k, e.__e = i.__e) : e.__e = ph(i.__e, e, i, a, l, c, d, g, y);
+    } else c == null && e.__v === i.__v ? (e.__k = i.__k, e.__e = i.__e) : e.__e = fh(i.__e, e, i, a, l, c, d, g, y);
     (_ = Me.diffed) && _(e)
 }
 
-function ga(r, e, i) {
+function ya(r, e, i) {
     e.__d = void 0;
-    for (var a = 0; a < i.length; a++) Fn(i[a], i[++a], i[++a]);
+    for (var a = 0; a < i.length; a++) Nn(i[a], i[++a], i[++a]);
     Me.__c && Me.__c(e, r), r.some(function(l) {
         try {
             r = l.__h, l.__h = [], r.some(function(c) {
                 c.call(l)
             })
         } catch (c) {
             Me.__e(c, l.__v)
         }
     })
 }
 
-function ph(r, e, i, a, l, c, d, f, g) {
+function fh(r, e, i, a, l, c, d, f, g) {
     var y, _, w, T, A, L, R, O = i.props,
         P = e.props,
         I = e.type;
     if (I === "svg" && (l = !0), c != null) {
         for (y = 0; y < c.length; y++)
             if ((A = c[y]) && "setAttribute" in A == !!I && (I ? A.localName === I : A.nodeType === 3)) {
                 r = A, c[y] = null;
@@ -16271,72 +16271,72 @@
     if (I === null) O === P || f && r.data === P || (r.data = P);
     else {
         if (c = c && d0.call(r.childNodes), O = i.props || Tr, !f && c != null)
             for (O = {}, y = 0; y < r.attributes.length; y++) O[(A = r.attributes[y]).name] = A.value;
         for (y in O) A = O[y], y == "children" || (y == "dangerouslySetInnerHTML" ? w = A : y === "key" || y in P || l0(r, y, null, A, l));
         for (y in P) A = P[y], y == "children" ? T = A : y == "dangerouslySetInnerHTML" ? _ = A : y == "value" ? L = A : y == "checked" ? R = A : y === "key" || f && typeof A != "function" || O[y] === A || l0(r, y, A, O[y], l);
         if (_) f || w && (_.__html === w.__html || _.__html === r.innerHTML) || (r.innerHTML = _.__html), e.__k = [];
-        else if (w && (r.innerHTML = ""), pa(r, zn(T) ? T : [T], e, i, a, l && I !== "foreignObject", c, d, c ? c[0] : i.__k && tr(i, 0), f, g), c != null)
-            for (y = c.length; y--;) c[y] != null && da(c[y]);
+        else if (w && (r.innerHTML = ""), ga(r, Rn(T) ? T : [T], e, i, a, l && I !== "foreignObject", c, d, c ? c[0] : i.__k && tr(i, 0), f, g), c != null)
+            for (y = c.length; y--;) c[y] != null && pa(c[y]);
         f || (y = "value", L !== void 0 && (L !== r[y] || I === "progress" && !L || I === "option" && L !== O[y]) && l0(r, y, L, O[y], !1), y = "checked", R !== void 0 && R !== r[y] && l0(r, y, R, O[y], !1))
     }
     return r
 }
 
-function Fn(r, e, i) {
+function Nn(r, e, i) {
     try {
         typeof r == "function" ? r(e) : r.current = e
     } catch (a) {
         Me.__e(a, i)
     }
 }
 
-function Dn(r, e, i) {
+function zn(r, e, i) {
     var a, l;
-    if (Me.unmount && Me.unmount(r), (a = r.ref) && (a.current && a.current !== r.__e || Fn(a, null, e)), (a = r.__c) != null) {
+    if (Me.unmount && Me.unmount(r), (a = r.ref) && (a.current && a.current !== r.__e || Nn(a, null, e)), (a = r.__c) != null) {
         if (a.componentWillUnmount) try {
             a.componentWillUnmount()
         } catch (c) {
             Me.__e(c, e)
         }
         a.base = a.__P = null, r.__c = void 0
     }
     if (a = r.__k)
-        for (l = 0; l < a.length; l++) a[l] && Dn(a[l], e, i || typeof r.type != "function");
-    i || r.__e == null || da(r.__e), r.__ = r.__e = r.__d = void 0
+        for (l = 0; l < a.length; l++) a[l] && zn(a[l], e, i || typeof r.type != "function");
+    i || r.__e == null || pa(r.__e), r.__ = r.__e = r.__d = void 0
 }
 
-function fh(r, e, i) {
+function gh(r, e, i) {
     return this.constructor(r, i)
 }
 
 function rr(r, e, i) {
     var a, l, c, d;
-    Me.__ && Me.__(r, e), l = (a = typeof i == "function") ? null : i && i.__k || e.__k, c = [], d = [], Rn(e, r = (!a && i || e).__k = hh(Ge, null, [r]), l || Tr, Tr, e.ownerSVGElement !== void 0, !a && i ? [i] : l ? null : e.firstChild ? d0.call(e.childNodes) : null, c, !a && i ? i : l ? l.__e : e.firstChild, a, d), ga(c, r, d)
+    Me.__ && Me.__(r, e), l = (a = typeof i == "function") ? null : i && i.__k || e.__k, c = [], d = [], Bn(e, r = (!a && i || e).__k = Fn(Ge, null, [r]), l || Tr, Tr, e.ownerSVGElement !== void 0, !a && i ? [i] : l ? null : e.firstChild ? d0.call(e.childNodes) : null, c, !a && i ? i : l ? l.__e : e.firstChild, a, d), ya(c, r, d)
 }
-d0 = ha.slice, Me = {
+d0 = ma.slice, Me = {
     __e: function(r, e, i, a) {
         for (var l, c, d; e = e.__;)
             if ((l = e.__c) && !l.__) try {
                 if ((c = l.constructor) && c.getDerivedStateFromError != null && (l.setState(c.getDerivedStateFromError(r)), d = l.__d), l.componentDidCatch != null && (l.componentDidCatch(r, a || {}), d = l.__d), d) return l.__E = l
             } catch (f) {
                 r = f
             }
         throw r
     }
-}, ca = 0, lh = function(r) {
+}, ha = 0, uh = function(r) {
     return r != null && r.constructor == null
 }, u0.prototype.setState = function(r, e) {
     var i;
-    i = this.__s != null && this.__s !== this.state ? this.__s : this.__s = Vt({}, this.state), typeof r == "function" && (r = r(Vt({}, i), this.props)), r && Vt(i, r), r != null && this.__v && (e && this._sb.push(e), oa(this))
+    i = this.__s != null && this.__s !== this.state ? this.__s : this.__s = Vt({}, this.state), typeof r == "function" && (r = r(Vt({}, i), this.props)), r && Vt(i, r), r != null && this.__v && (e && this._sb.push(e), sa(this))
 }, u0.prototype.forceUpdate = function(r) {
-    this.__v && (this.__e = !0, r && this.__h.push(r), oa(this))
-}, u0.prototype.render = Ge, er = [], ua = typeof Promise == "function" ? Promise.prototype.then.bind(Promise.resolve()) : setTimeout, En = function(r, e) {
+    this.__v && (this.__e = !0, r && this.__h.push(r), sa(this))
+}, u0.prototype.render = Ge, er = [], da = typeof Promise == "function" ? Promise.prototype.then.bind(Promise.resolve()) : setTimeout, Dn = function(r, e) {
     return r.__v.__b - e.__v.__b
-}, h0.__r = 0, ch = 0;
+}, h0.__r = 0, hh = 0;
 
 function jt(r, e) {
     if (e == null || r.frontierEntries == null || r.frontierEntries.length === 0) return r;
     {
         (e < 0 || e >= r.frontierEntries.length) && (e = 0);
         let i = r.frontierEntries[e];
         return {
@@ -16347,43 +16347,43 @@
             logicalQubit: i.logicalQubit,
             tfactory: i.tfactory,
             errorBudget: i.errorBudget,
             logicalCounts: r.logicalCounts
         }
     }
 }
-var Ar, Ue, Bn, ba, f0 = 0,
-    Ca = [],
+var Ar, Ue, Ln, xa, f0 = 0,
+    Aa = [],
     m0 = [],
     Ye = Me,
-    ya = Ye.__b,
-    xa = Ye.__r,
-    va = Ye.diffed,
-    wa = Ye.__c,
-    ka = Ye.unmount,
-    _a = Ye.__;
+    va = Ye.__b,
+    wa = Ye.__r,
+    ka = Ye.diffed,
+    _a = Ye.__c,
+    Sa = Ye.unmount,
+    Ca = Ye.__;
 
-function Ln(r, e) {
+function In(r, e) {
     Ye.__h && Ye.__h(Ue, r, f0 || e), f0 = 0;
     var i = Ue.__H || (Ue.__H = {
         __: [],
         __h: []
     });
     return r >= i.__.length && i.__.push({
         __V: m0
     }), i.__[r]
 }
 
 function Xe(r) {
-    return f0 = 1, gh(Aa, r)
+    return f0 = 1, bh(Ma, r)
 }
 
-function gh(r, e, i) {
-    var a = Ln(Ar++, 2);
-    if (a.t = r, !a.__c && (a.__ = [i ? i(e) : Aa(void 0, e), function(f) {
+function bh(r, e, i) {
+    var a = In(Ar++, 2);
+    if (a.t = r, !a.__c && (a.__ = [i ? i(e) : Ma(void 0, e), function(f) {
             var g = a.__N ? a.__N[0] : a.__[0],
                 y = a.t(g, f);
             g !== y && (a.__N = [y, a.__[1]], a.__c.setState({}))
         }], a.__c = Ue, !Ue.u)) {
         var l = function(f, g, y) {
             if (!a.__c.__H) return !0;
             var _ = a.__c.__H.__.filter(function(T) {
@@ -16411,110 +16411,110 @@
             d && d.call(this, f, g, y)
         }, Ue.shouldComponentUpdate = l
     }
     return a.__N || a.__
 }
 
 function Ut(r, e) {
-    var i = Ln(Ar++, 3);
-    !Ye.__s && Ta(i.__H, e) && (i.__ = r, i.i = e, Ue.__H.__h.push(i))
+    var i = In(Ar++, 3);
+    !Ye.__s && qa(i.__H, e) && (i.__ = r, i.i = e, Ue.__H.__h.push(i))
 }
 
 function St(r) {
-    return f0 = 5, bh(function() {
+    return f0 = 5, yh(function() {
         return {
             current: r
         }
     }, [])
 }
 
-function bh(r, e) {
-    var i = Ln(Ar++, 7);
-    return Ta(i.__H, e) ? (i.__V = r(), i.i = e, i.__h = r, i.__V) : i.__
+function yh(r, e) {
+    var i = In(Ar++, 7);
+    return qa(i.__H, e) ? (i.__V = r(), i.i = e, i.__h = r, i.__V) : i.__
 }
 
-function yh() {
-    for (var r; r = Ca.shift();)
+function xh() {
+    for (var r; r = Aa.shift();)
         if (r.__P && r.__H) try {
-            r.__H.__h.forEach(p0), r.__H.__h.forEach(Nn), r.__H.__h = []
+            r.__H.__h.forEach(p0), r.__H.__h.forEach(Pn), r.__H.__h = []
         } catch (e) {
             r.__H.__h = [], Ye.__e(e, r.__v)
         }
 }
 Ye.__b = function(r) {
-    Ue = null, ya && ya(r)
+    Ue = null, va && va(r)
 }, Ye.__ = function(r, e) {
-    r && e.__k && e.__k.__m && (r.__m = e.__k.__m), _a && _a(r, e)
+    r && e.__k && e.__k.__m && (r.__m = e.__k.__m), Ca && Ca(r, e)
 }, Ye.__r = function(r) {
-    xa && xa(r), Ar = 0;
+    wa && wa(r), Ar = 0;
     var e = (Ue = r.__c).__H;
-    e && (Bn === Ue ? (e.__h = [], Ue.__h = [], e.__.forEach(function(i) {
+    e && (Ln === Ue ? (e.__h = [], Ue.__h = [], e.__.forEach(function(i) {
         i.__N && (i.__ = i.__N), i.__V = m0, i.__N = i.i = void 0
-    })) : (e.__h.forEach(p0), e.__h.forEach(Nn), e.__h = [], Ar = 0)), Bn = Ue
+    })) : (e.__h.forEach(p0), e.__h.forEach(Pn), e.__h = [], Ar = 0)), Ln = Ue
 }, Ye.diffed = function(r) {
-    va && va(r);
+    ka && ka(r);
     var e = r.__c;
-    e && e.__H && (e.__H.__h.length && (Ca.push(e) !== 1 && ba === Ye.requestAnimationFrame || ((ba = Ye.requestAnimationFrame) || xh)(yh)), e.__H.__.forEach(function(i) {
+    e && e.__H && (e.__H.__h.length && (Aa.push(e) !== 1 && xa === Ye.requestAnimationFrame || ((xa = Ye.requestAnimationFrame) || vh)(xh)), e.__H.__.forEach(function(i) {
         i.i && (i.__H = i.i), i.__V !== m0 && (i.__ = i.__V), i.i = void 0, i.__V = m0
-    })), Bn = Ue = null
+    })), Ln = Ue = null
 }, Ye.__c = function(r, e) {
     e.some(function(i) {
         try {
             i.__h.forEach(p0), i.__h = i.__h.filter(function(a) {
-                return !a.__ || Nn(a)
+                return !a.__ || Pn(a)
             })
         } catch (a) {
             e.some(function(l) {
                 l.__h && (l.__h = [])
             }), e = [], Ye.__e(a, i.__v)
         }
-    }), wa && wa(r, e)
+    }), _a && _a(r, e)
 }, Ye.unmount = function(r) {
-    ka && ka(r);
+    Sa && Sa(r);
     var e, i = r.__c;
     i && i.__H && (i.__H.__.forEach(function(a) {
         try {
             p0(a)
         } catch (l) {
             e = l
         }
     }), i.__H = void 0, e && Ye.__e(e, i.__v))
 };
-var Sa = typeof requestAnimationFrame == "function";
+var Ta = typeof requestAnimationFrame == "function";
 
-function xh(r) {
+function vh(r) {
     var e, i = function() {
-            clearTimeout(a), Sa && cancelAnimationFrame(e), setTimeout(r)
+            clearTimeout(a), Ta && cancelAnimationFrame(e), setTimeout(r)
         },
         a = setTimeout(i, 100);
-    Sa && (e = requestAnimationFrame(i))
+    Ta && (e = requestAnimationFrame(i))
 }
 
 function p0(r) {
     var e = Ue,
         i = r.__c;
     typeof i == "function" && (r.__c = void 0, i()), Ue = e
 }
 
-function Nn(r) {
+function Pn(r) {
     var e = Ue;
     r.__c = r.__(), Ue = e
 }
 
-function Ta(r, e) {
+function qa(r, e) {
     return !r || r.length !== e.length || e.some(function(i, a) {
         return i !== r[a]
     })
 }
 
-function Aa(r, e) {
+function Ma(r, e) {
     return typeof e == "function" ? e(r) : e
 }
-var vh = 0,
-    vf = Array.isArray;
+var wh = 0,
+    kf = Array.isArray;
 
 function M(r, e, i, a, l, c) {
     var d, f, g = {};
     for (f in e) f == "ref" ? d = e[f] : g[f] = e[f];
     var y = {
         type: r,
         props: g,
@@ -16523,58 +16523,58 @@
         __k: null,
         __: null,
         __b: 0,
         __e: null,
         __d: void 0,
         __c: null,
         constructor: void 0,
-        __v: --vh,
+        __v: --wh,
         __i: -1,
         __u: 0,
         __source: l,
         __self: c
     };
     if (typeof r == "function" && (d = r.defaultProps))
         for (f in d) g[f] === void 0 && (g[f] = d[f]);
     return Me.vnode && Me.vnode(y), y
 }
-var qa = !1,
-    Ma = !0,
+var Ea = !1,
+    Da = !0,
     g0 = [{
         category: "itemCount",
         options: ["Show all", "Top 10", "Top 25"]
     }, {
         category: "sortOrder",
         options: ["Sort a-z", "High to low", "Low to high"]
     }, {
         category: "labels",
         options: ["Raw labels", "Ket labels", "No labels"]
     }],
-    Ea = 3,
-    wh = {
+    za = 3,
+    kh = {
         itemCount: 0,
         sortOrder: 0,
         labels: 0
     },
-    kh = /^\[(?:(Zero|One), *)*(Zero|One)\]$/;
+    _h = /^\[(?:(Zero|One), *)*(Zero|One)\]$/;
 
-function Da(r) {
+function Ra(r) {
     if (typeof r != "string") return "ERROR";
-    if (kh.test(r)) {
+    if (_h.test(r)) {
         let e = r.match(/(One|Zero)/g),
             i = "|";
         return e?.forEach(a => i += a == "One" ? "1" : "0"), i += "\u27E9", i
     } else return r
 }
 
-function Pn(r) {
+function On(r) {
     let [e, i] = Xe(""), [a, l] = Xe({
         zoom: 1,
         offset: 1
-    }), [c, d] = Xe(wh), f = St(null), g = St(null), y = 0;
+    }), [c, d] = Xe(kh), f = St(null), g = St(null), y = 0;
     switch (c.itemCount) {
         case 1:
             y = 10;
             break;
         case 2:
             y = 25;
             break
@@ -16583,15 +16583,15 @@
         w = [...r.data],
         T = 0,
         A = 0;
     w.forEach(ee => {
         T += ee[1], A = Math.max(ee[1], A)
     });
     let L = `${w.length} unique results`;
-    y > 0 && (w.sort((ee, G) => ee[1] < G[1] ? 1 : -1), w.length > y && (L = `Top ${y} of ${L}`, w.length = y)), r.filter && (L += `. Shot filter: ${_?Da(r.filter):r.filter}`), w.sort((ee, G) => {
+    y > 0 && (w.sort((ee, G) => ee[1] < G[1] ? 1 : -1), w.length > y && (L = `Top ${y} of ${L}`, w.length = y)), r.filter && (L += `. Shot filter: ${_?Ra(r.filter):r.filter}`), w.sort((ee, G) => {
         let fe = Number(ee[0]),
             Te = Number(G[0]);
         switch (c.sortOrder) {
             case 1:
                 return ee[1] < G[1] ? 1 : -1;
             case 2:
                 return ee[1] > G[1] ? 1 : -1;
@@ -16631,38 +16631,38 @@
 
     function re() {
         g.current && (g.current.style.display === "inline" ? g.current.style.display = "none" : g.current.style.display = "inline")
     }
     let te = 38,
         j = 11,
         ne = g0.length * te - 2,
-        pe = Ea * j + 3,
+        pe = za * j + 3,
         ue = 163,
         ce = 72,
         Ce = 1.2,
         De = ue * a.zoom / w.length,
         X = De * .1,
         he = De - 2 * X,
         oe = De > 5 && c.labels !== 2;
 
     function ae(ee) {
         ee.preventDefault();
         let G = ee.currentTarget,
             fe = new DOMPoint(ee.clientX, ee.clientY).matrixTransform(G.getScreenCTM()?.inverse()),
             Te = a.offset,
             Ae = a.zoom;
-        if (!Ma || !ee.altKey) {
+        if (!Da || !ee.altKey) {
             Ae = a.zoom + ee.deltaY * .05, Ae = Math.min(Math.max(1, Ae), 50);
             let Pt = ue * a.zoom,
-                H0 = (0 - a.offset + fe.x) / Pt,
-                $0 = Ae * ue - a.zoom * ue,
-                G0 = H0 * $0;
-            Te = a.offset - G0
+                $0 = (0 - a.offset + fe.x) / Pt,
+                G0 = Ae * ue - a.zoom * ue,
+                V0 = $0 * G0;
+            Te = a.offset - V0
         }
-        qa && (Te -= ee.deltaX), !qa && Ma && ee.altKey && (Te -= ee.deltaY);
+        Ea && (Te -= ee.deltaX), !Ea && Da && ee.altKey && (Te -= ee.deltaY);
         let qt = 1 - (ue * Ae - ue),
             ct = Math.min(Math.max(Te, qt), 1);
         l({
             zoom: Ae,
             offset: ct
         })
     }
@@ -16673,15 +16673,15 @@
         }) : null, M("svg", {
             class: "histogram",
             viewBox: "0 0 165 100",
             onWheel: ae,
             children: [M("g", {
                 transform: `translate(${a.offset},4)`,
                 children: w.map((ee, G) => {
-                    let fe = _ ? Da(ee[0]) : ee[0],
+                    let fe = _ ? Ra(ee[0]) : ee[0],
                         Te = ce * (ee[1] / A),
                         Ae = De * G + X,
                         qt = De * G + De / 2 - Ce,
                         ct = ce + 15 - Te,
                         Pt = `${fe} at ${(ee[1]/T*100).toFixed(2)}%`,
                         yr = "bar";
                     return ee[0] === r.filter && (yr += " bar-selected"), M(Ge, {
@@ -16800,15 +16800,15 @@
                         })]
                     })
                 })), g0.map((ee, G) => G >= g0.length - 1 ? null : M("line", {
                     class: "menu-separator",
                     x1: 37 + G * te,
                     y1: "2",
                     x2: 37 + G * te,
-                    y2: Ea * j + 1
+                    y2: za * j + 1
                 }))]
             }), M("g", {
                 ref: g,
                 style: "display: none;",
                 children: [M("rect", {
                     width: "155",
                     height: "76",
@@ -16851,15 +16851,15 @@
                     })]
                 })]
             })]
         })]
     })
 }
 
-function za(r) {
+function Fa(r) {
     let e = [],
         i = [],
         a = new Intl.NumberFormat,
         l = new Intl.NumberFormat(void 0, {
             maximumFractionDigits: 2,
             minimumFractionDigits: 2
         });
@@ -17206,19 +17206,34 @@
         alwaysVisible: !1,
         entries: i
     }), {
         groups: e,
         assumptions: ["_More details on the following lists of assumptions can be found in the paper [Accessing requirements for scaling quantum computers and their applications](https://aka.ms/AQ/RE/Paper)._", "**Uniform independent physical noise.** We assume that the noise on physical qubits and physical qubit operations is the standard circuit noise model. In particular we assume error events at different space-time locations are independent and that error rates are uniform across the system in time and space.", "**Efficient classical computation.** We assume that classical overhead (compilation, control, feedback, readout, decoding, etc.) does not dominate the overall cost of implementing the full quantum algorithm.", "**Extraction circuits for planar quantum ISA.** We assume that stabilizer extraction circuits with similar depth and error correction performance to those for standard surface and Hastings-Haah code patches can be constructed to implement all operations of the planar quantum ISA (instruction set architecture).", "**Uniform independent logical noise.** We assume that the error rate of a logical operation is approximately equal to its space-time volume (the number of tiles multiplied by the number of logical time steps) multiplied by the error rate of a logical qubit in a standard one-tile patch in one logical time step.", "**Negligible Clifford costs for synthesis.** We assume that the space overhead for synthesis and space and time overhead for transport of magic states within magic state factories and to synthesis qubits are all negligible.", "**Smooth magic state consumption rate.** We assume that the rate of T state consumption throughout the compiled algorithm is almost constant, or can be made almost constant without significantly increasing the number of logical time steps for the algorithm."]
     }
 }
+var Sh = function(r) {
+    let e = "ERROR: Rendered has not been set";
+    return console.error(e), e + ". " + r
+};
+
+function b0(r) {
+    let e = r.tagName || "div",
+        i = {
+            className: r.className,
+            dangerouslySetInnerHTML: {
+                __html: Sh(r.markdown)
+            }
+        };
+    return Fn(e, i)
+}
 
 function qr(r) {
     let [e, i] = Xe(!1), a = () => {
         i(!e)
-    }, l = za(r.estimatesData);
+    }, l = Fa(r.estimatesData);
     return M("div", {
         children: [M("div", {
             children: [M("input", {
                 type: "checkbox",
                 id: "showDetail",
                 checked: e,
                 onClick: a
@@ -17231,34 +17246,30 @@
             children: [M("summary", {
                 children: M("strong", {
                     children: c.title
                 })
             }), M("table", {
                 className: "estimate-table",
                 children: c.entries.map(d => {
-                    let g = d.path.split("/").reduce((_, w) => _[w], r.estimatesData);
-                    typeof g == "object" && (g = JSON.stringify(g));
-                    let y = {
-                        __html: r.mdRenderer(d.explanation)
-                    };
-                    return M("tr", {
+                    let g = d.path.split("/").reduce((y, _) => y[_], r.estimatesData);
+                    return typeof g == "object" && (g = JSON.stringify(g)), M("tr", {
                         children: [M("td", {
                             className: "estimate-cell title-cell",
                             children: d.label
                         }), M("td", {
                             className: "estimate-cell value-cell",
                             children: g
                         }), M("td", {
                             className: "estimate-cell",
                             children: e ? M(Ge, {
                                 children: [M("strong", {
                                     children: d.description
-                                }), M("hr", {}), M("div", {
+                                }), M("hr", {}), M(b0, {
                                     className: "estimate-explanation",
-                                    dangerouslySetInnerHTML: y
+                                    markdown: d.explanation
                                 })]
                             }) : M(Ge, {
                                 children: M("span", {
                                     children: d.description
                                 })
                             })
                         })]
@@ -17269,26 +17280,25 @@
             className: "estimate-details",
             children: [M("summary", {
                 children: M("strong", {
                     children: "Assumptions"
                 })
             }), M("ul", {
                 className: "estimate-table",
-                children: l.assumptions.map(c => M("li", {
+                children: l.assumptions.map(c => M(b0, {
                     className: "estimate-assumption",
-                    dangerouslySetInnerHTML: {
-                        __html: r.mdRenderer(c)
-                    }
+                    markdown: c,
+                    tagName: "li"
                 }))
             })]
         })]
     })
 }
 
-function Ra(r, e, i, a, l, c) {
+function Ba(r, e, i, a, l, c) {
     let d = l - a <= 180 ? "0" : "1",
         f = r + i * Math.cos(Math.PI * a / 180),
         g = e + i * Math.sin(Math.PI * a / 180),
         y = r + i * Math.cos(Math.PI * l / 180),
         _ = e + i * Math.sin(Math.PI * l / 180),
         w = r + c * Math.cos(Math.PI * a / 180),
         T = e + c * Math.sin(Math.PI * a / 180),
@@ -17310,19 +17320,19 @@
         children: [M("svg", {
             class: "qs-widget-spaceChart",
             width: "400",
             height: "400",
             viewBox: "50 0 450 450",
             id: "pieChart",
             children: [M("path", {
-                d: Ra(250, 185, 180, 0, d, 120),
+                d: Ba(250, 185, 180, 0, d, 120),
                 fill: "var(--vscode-charts-orange, orange)",
                 stroke: "white"
             }), M("path", {
-                d: Ra(250, 185, 180, d, 360, 120),
+                d: Ba(250, 185, 180, d, 360, 120),
                 fill: "var(--vscode-charts-blue, blue)",
                 stroke: "white"
             }), M("text", {
                 x: "250",
                 y: "180",
                 "text-anchor": "middle",
                 "font-size": "16",
@@ -17445,15 +17455,15 @@
                     children: r.estimatesData.logicalQubit.physicalQubits.toLocaleString()
                 })]
             })]
         })]
     })
 }
 
-function Fa(r, e) {
+function Na(r, e) {
     if (e < r || r <= 0) return [];
     let i = new Intl.NumberFormat,
         a = Math.round(10 ** Math.floor(Math.log10(r))),
         l = Math.round(10 ** Math.ceil(Math.log10(e))),
         c = [];
     for (let d = a; d <= l; d *= 10) d >= r && d <= e && c.push({
         value: d,
@@ -17543,15 +17553,15 @@
     tick: {
         value: 31536e14,
         label: "1 century"
     },
     plural: "centuries"
 }];
 
-function Ba(r, e) {
+function La(r, e) {
     if (e < r || r <= 0) return [];
     let i = 0;
     for (; i < Je.length && Je[i].tick.value <= r;) i++;
     let a = i;
     for (i > 0 && i--, a >= Je.length && (a = Je.length - 1); a < Je.length - 1 && Je[a].tick.value <= e;) a++;
     let l = [];
     for (let c = i; c <= a; c++) Je[c].tick.value >= r && Je[c].tick.value <= e && l.push(Je[c].tick);
@@ -17581,41 +17591,41 @@
                     d /= 10
                 } while (l.length < 1 && d >= 1);
                 c--
             } while (l.length < 1 && c >= 0)
         } return l
 }
 
-function _h(r) {
+function Ch(r) {
     return r.reduce((e, i) => i.items.reduce((a, l) => [Math.min(a[0], l.x), Math.max(a[1], l.x), Math.min(a[2], l.y), Math.max(a[3], l.y)], e), [Number.MAX_VALUE, Number.MIN_VALUE, Number.MAX_VALUE, Number.MIN_VALUE])
 }
 
-function Na(r, e) {
-    let [i, a, l, c] = _h(r), d = {
+function Pa(r, e) {
+    let [i, a, l, c] = Ch(r), d = {
         min: i / e,
         max: a * e
     }, f = {
         min: l / e,
         max: c * e
     };
     return {
         rangeX: d,
         rangeY: f
     }
 }
 
-function In(r) {
+function Hn(r) {
     let e = St(null),
         {
             rangeX: i,
             rangeY: a
-        } = Na(r.data, 2);
+        } = Pa(r.data, 2);
 
     function l(ae, ee) {
-        return ee ? Ba(ae.min, ae.max) : Fa(ae.min, ae.max)
+        return ee ? La(ae.min, ae.max) : Na(ae.min, ae.max)
     }
     let c = l(i, r.xAxis.isTime),
         d = l(a, r.yAxis.isTime);
 
     function f(ae, ee) {
         return (Math.log(ae) - Math.log(ee.min)) / (Math.log(ee.max) - Math.log(ee.min))
     }
@@ -17798,47 +17808,47 @@
             ref: e
         }), M("div", {
             class: "qs-scatterChart-tooltip"
         })]
     })
 }
 
-function La(r) {
+function Ia(r) {
     let e = [],
         i = 1.4142135623730951,
         a = .618033988749895,
         l = 2.718281828459045;
     for (let c = 0; c < r; c++) {
         let d = c * a % 1,
             f = (1 - c * i % 1) * .5 + .5,
             g = c * l % 1 * .3 + .35,
-            y = Ch(d, f, g),
-            _ = Th(y[0], y[1], y[2]);
+            y = Ah(d, f, g),
+            _ = qh(y[0], y[1], y[2]);
         e.push(_)
     }
     return e
 }
 
-function Ch(r, e, i) {
+function Ah(r, e, i) {
     let a, l, c;
     if (e === 0) a = l = c = i;
     else {
         let d = (y, _, w) => (w < 0 && (w += 1), w > 1 && (w -= 1), w < .16666666666666666 ? y + (_ - y) * 6 * w : w < .5 ? _ : w < .6666666666666666 ? y + (_ - y) * (.6666666666666666 - w) * 6 : y),
             f = i < .5 ? i * (1 + e) : i + e - i * e,
             g = 2 * i - f;
         a = d(g, f, r + 1 / 3), l = d(g, f, r), c = d(g, f, r - 1 / 3)
     }
     return [Math.round(a * 255), Math.round(l * 255), Math.round(c * 255)]
 }
 
-function Th(r, e, i) {
+function qh(r, e, i) {
     return `#${(1<<24|r<<16|e<<8|i).toString(16).slice(1).toUpperCase()}`
 }
 
-function Pa(r) {
+function Oa(r) {
     let [e, i] = Xe(r.initialColumns), [a, l] = Xe(null), [c, d] = Xe(!1), [f, g] = Xe(""), y = St(""), _ = St(null);
 
     function w(U) {
         if (!(U.target instanceof HTMLElement)) return;
         let X = U.target.closest("th")?.dataset.colid;
         y.current = X, U.dataTransfer.dropEffect = "move"
     }
@@ -18070,78 +18080,78 @@
                         children: te(U.cells[he])
                     }))]
                 })
             })
         })]
     })
 }
-var Ah = ["Run name", "Estimate type", "Qubit type", "QEC scheme", "Error budget", "Logical qubits", "Logical depth", "Code distance", "T states", "T factories", "T factory fraction", "Runtime", "rQOPS", "Physical qubits"],
-    qh = [0, 10, 13, 11, 12],
-    Mh = {
+var Mh = ["Run name", "Estimate type", "Qubit type", "QEC scheme", "Error budget", "Logical qubits", "Logical depth", "Code distance", "T states", "T factories", "T factory fraction", "Runtime", "rQOPS", "Physical qubits"],
+    Eh = [0, 10, 13, 11, 12],
+    Dh = {
         isTime: !0,
         label: "Runtime"
     },
-    Eh = {
+    zh = {
         isTime: !1,
         label: "Physical qubits"
     };
 
-function Dh(r, e) {
+function Rh(r, e) {
     let i = jt(r, 0),
         a = r.frontierEntries == null ? "Single" : "Frontier (" + r.frontierEntries.length + "  items)";
     return {
         cells: [i.jobParams.runName, a, i.jobParams.qubitParams.name, i.jobParams.qecScheme.name, i.jobParams.errorBudget, i.physicalCounts.breakdown.algorithmicLogicalQubits, i.physicalCounts.breakdown.algorithmicLogicalDepth, i.logicalQubit.codeDistance, i.physicalCounts.breakdown.numTstates, i.physicalCounts.breakdown.numTfactories, i.physicalCountsFormatted.physicalQubitsForTfactoriesPercentage, {
             value: i.physicalCountsFormatted.runtime,
             sortBy: i.physicalCounts.runtime
         }, i.physicalCounts.rqops, i.physicalCounts.physicalQubits],
         color: e
     }
 }
 
-function zh(r) {
+function Fh(r) {
     return {
         x: r.physicalCounts.runtime,
         y: r.physicalCounts.physicalQubits,
         label: r.physicalCountsFormatted.runtime + ", physical qubits: " + r.physicalCountsFormatted.physicalQubits + ", code distance: " + r.logicalQubit.codeDistance
     }
 }
 
-function Rh(r, e) {
+function Bh(r, e) {
     return r.frontierEntries == null || r.frontierEntries.length === 0 ? {
         color: e,
         items: [{
             x: r.physicalCounts.runtime,
             y: r.physicalCounts.physicalQubits,
             label: r.physicalCountsFormatted.runtime + ", physical qubits: " + r.physicalCountsFormatted.physicalQubits + ", code distance: " + r.logicalQubit.codeDistance
         }]
     } : {
         color: e,
-        items: r.frontierEntries.map(zh)
+        items: r.frontierEntries.map(Fh)
     }
 }
 
-function Fh(r) {
+function Nh(r) {
     if (r.length === 1) return [r[0].jobParams.sharedRunName ?? r[0].jobParams.qubitParams.name ?? r[0].jobParams.qecScheme.name ?? "estimate"];
     let e = [];
     r.forEach(() => {
         e.push([])
-    }), b0(e, r, a => a.jobParams.sharedRunName), b0(e, r, a => a.jobParams.qubitParams.name), b0(e, r, a => a.jobParams.qecScheme.name), b0(e, r, a => String(a.jobParams.errorBudget));
+    }), y0(e, r, a => a.jobParams.sharedRunName), y0(e, r, a => a.jobParams.qubitParams.name), y0(e, r, a => a.jobParams.qecScheme.name), y0(e, r, a => String(a.jobParams.errorBudget));
     let i = e.map(a => a.join(", "));
     return new Set(i).size != i.length ? i.map((a, l) => a + " (" + l + ")") : i
 }
 
-function b0(r, e, i) {
+function y0(r, e, i) {
     let a = e.map(i);
     new Set(a).size > 1 && a.forEach((c, d) => {
         r[d].push(c)
     })
 }
 
 function Er(r) {
-    let [e, i] = Xe(null), [a, l] = Xe(), c = r.runNames != null && r.runNames.length > 0 && r.runNames.length != r.estimatesData.length ? "Warning: The number of runNames does not match the number of estimates. Ignoring provided runNames." : "", d = r.runNames != null && r.runNames.length == r.estimatesData.length ? r.runNames : Fh(r.estimatesData);
+    let [e, i] = Xe(null), [a, l] = Xe(), c = r.runNames != null && r.runNames.length > 0 && r.runNames.length != r.estimatesData.length ? "Warning: The number of runNames does not match the number of estimates. Ignoring provided runNames." : "", d = r.runNames != null && r.runNames.length == r.estimatesData.length ? r.runNames : Nh(r.estimatesData);
     r.estimatesData.forEach((A, L) => {
         A.jobParams.runName = d[L]
     });
 
     function f(A, L) {
         if (A < 0) {
             g("");
@@ -18161,32 +18171,32 @@
             else {
                 let R = r.estimatesData[L];
                 l([L, 0]), r.setEstimate(jt(R, 0))
             }
         }
     }
     let y = r.colors != null && r.colors.length > 0 && r.colors.length != r.estimatesData.length ? "Warning: The number of colors does not match the number of estimates. Ignoring provided colors." : "",
-        _ = r.colors != null && r.colors.length == r.estimatesData.length ? r.colors : La(r.estimatesData.length);
+        _ = r.colors != null && r.colors.length == r.estimatesData.length ? r.colors : Ia(r.estimatesData.length);
 
     function w() {
-        return M(Pa, {
-            columnNames: Ah,
-            rows: r.estimatesData.map((A, L) => Dh(A, _[L])),
-            initialColumns: qh,
+        return M(Oa, {
+            columnNames: Mh,
+            rows: r.estimatesData.map((A, L) => Rh(A, _[L])),
+            initialColumns: Eh,
             selectedRow: e,
             onRowSelected: g,
             onRowDeleted: r.onRowDeleted
         })
     }
 
     function T() {
-        return M(In, {
-            xAxis: Mh,
-            yAxis: Eh,
-            data: r.estimatesData.map((A, L) => Rh(A, _[L])),
+        return M(Hn, {
+            xAxis: Dh,
+            yAxis: zh,
+            data: r.estimatesData.map((A, L) => Bh(A, _[L])),
             onPointSelected: f,
             selectedPoint: a
         })
     }
     return M("div", {
         className: "qs-estimatesOverview",
         children: [c != "" && M("div", {
@@ -18211,29 +18221,29 @@
                     children: "Space-time diagram"
                 }), T()]
             })]
         })]
     })
 }
 
-function On(r) {
+function $n(r) {
     return M("svg", {
         width: "40",
         height: "40",
         viewBox: "0 0 16 16",
         xmlns: "http://www.w3.org/2000/svg",
         class: "codicon-modifier-spin",
         style: r.style,
         children: M("path", {
             d: "M2.006 8.267L.78 9.5 0 8.73l2.09-2.07.76.01 2.09 2.12-.76.76-1.167-1.18a5 5 0 0 0 9.4 1.983l.813.597a6 6 0 0 1-11.22-2.683zm10.99-.466L11.76 6.55l-.76.76 2.09 2.11.76.01 2.09-2.07-.75-.76-1.194 1.18a6 6 0 0 0-11.11-2.92l.81.594a5 5 0 0 1 9.3 2.346z"
         })
     })
 }
 
-function Hn(r) {
+function Gn(r) {
     let [e, i] = Xe(null);
     return M(Ge, {
         children: [M("div", {
             style: "display:flex; height:64px; align-items: center; position: relative",
             children: [M("svg", {
                 width: "48",
                 height: "48",
@@ -18285,15 +18295,15 @@
                         d: "M 665 845 L 816 758"
                     }), M("path", {
                         d: "M 433 801 L 820 577"
                     }), M("path", {
                         d: "M 820 489 L 360 755"
                     })]
                 })
-            }), r.calculating ? M(On, {
+            }), r.calculating ? M($n, {
                 style: "position: absolute; top: 11px; left: 4px;"
             }) : null, M("h1", {
                 children: "Azure Quantum Resource Estimator"
             })]
         }), M(Er, {
             estimatesData: r.estimatesData,
             isSimplifiedView: !1,
@@ -18312,39 +18322,38 @@
                 })]
             }), M("details", {
                 open: !0,
                 children: [M("summary", {
                     style: "font-size: 1.5em; font-weight: bold; margin: 24px 8px;",
                     children: "Resource Estimates"
                 }), M(qr, {
-                    mdRenderer: r.renderer,
                     estimatesData: e
                 })]
             })]
         }) : null]
     })
 }
-var ms = Mn(ds(), 1);
-var ei = 1e4,
-    ti = 1e3;
+var fs = En(ps(), 1);
+var ri = 1e4,
+    ni = 1e3;
 
-function ri(r) {
+function ii(r) {
     let e = r.circuit,
-        i = e.qubits.length === 0 || e.operations.length > ei || e.qubits.length > ti;
+        i = e.qubits.length === 0 || e.operations.length > ri || e.qubits.length > ni;
     return M("div", {
-        children: i ? M(wd, {
+        children: i ? M(_d, {
             qubits: r.circuit.qubits.length,
             operations: r.circuit.operations.length
-        }) : M(vd, {
+        }) : M(kd, {
             circuit: r.circuit
         })
     })
 }
 
-function vd(r) {
+function kd(r) {
     let e = St(null),
         [i, a] = Xe(100),
         [l, c] = Xe(!0);
     return Ut(() => {
         c(!0);
         let y = e.current;
         y.innerHTML = ""
@@ -18355,15 +18364,15 @@
                 w = g(y, _);
             a(w), d(), c(!1)
         }
     }, [l]), Ut(() => {
         d()
     }, [i]), M("div", {
         children: [M("div", {
-            children: l ? null : M(kd, {
+            children: l ? null : M(Sd, {
                 zoom: i,
                 onChange: a
             })
         }), M("div", {
             children: l ? `Rendering diagram with ${r.circuit.operations.length} gates...` : ""
         }), M("div", {
             class: "qs-circuit",
@@ -18376,46 +18385,46 @@
         if (y) {
             let _ = y.getAttribute("width");
             y.setAttribute("style", `max-width: ${_}; width: ${parseInt(_)*(i||100)/100}; height: auto`)
         }
     }
 
     function f(y, _) {
-        return ms.draw(y, _), _.querySelectorAll("style")?.forEach(T => T.remove()), _.getElementsByClassName("qviz")[0]
+        return fs.draw(y, _), _.querySelectorAll("style")?.forEach(T => T.remove()), _.getElementsByClassName("qviz")[0]
     }
 
     function g(y, _) {
         let w = y.clientWidth,
             T = parseInt(_.getAttribute("width")),
             A = _.getAttribute("height");
         return _.setAttribute("viewBox", `0 0 ${T} ${A}`), Math.min(Math.ceil(w / T * 100), 100)
     }
 }
 
-function wd(r) {
+function _d(r) {
     let e = r.qubits === 0 ? M("div", {
         children: M("p", {
             children: "No circuit to display. No qubits have been allocated."
         })
-    }) : r.operations > ei ? M("div", {
+    }) : r.operations > ri ? M("div", {
         children: M("p", {
-            children: ["This circuit has too many gates to display. It has ", r.operations, " ", "gates, but the maximum supported is ", ei, "."]
+            children: ["This circuit has too many gates to display. It has ", r.operations, " ", "gates, but the maximum supported is ", ri, "."]
         })
-    }) : r.qubits > ti ? M("div", {
+    }) : r.qubits > ni ? M("div", {
         children: M("p", {
-            children: ["This circuit has too many qubits to display. It has ", r.qubits, " ", "qubits, but the maximum supported is ", ti, "."]
+            children: ["This circuit has too many qubits to display. It has ", r.qubits, " ", "qubits, but the maximum supported is ", ni, "."]
         })
     }) : void 0;
     return M("div", {
         class: "qs-circuit-error",
         children: e
     })
 }
 
-function kd(r) {
+function Sd(r) {
     return M("p", {
         children: [M("label", {
             htmlFor: "qs-circuit-zoom",
             children: "Zoom "
         }), M("input", {
             id: "qs-circuit-zoom",
             type: "number",
@@ -18423,190 +18432,190 @@
             max: "100",
             step: "10",
             value: r.zoom,
             onInput: e => r.onChange(parseInt(e.target.value) || 0)
         }), "%"]
     })
 }
-var Au = Mn(yu()),
-    qu = Mn(Tu());
-var Mu = (0, Au.default)();
-Mu.use(qu.default);
+var Mu = En(vu()),
+    Eu = En(qu());
+var Du = (0, Mu.default)();
+Du.use(Eu.default);
 
-function Eu(r) {
-    return Mu.render(r.replace(/\\\\/g, "\\"))
+function zu(r) {
+    return Du.render(r.replace(/\\\\/g, "\\"))
 }
 
-function n5({
+function u5({
     model: r,
     el: e
 }) {
     let i = r.get("comp");
     switch (i) {
         case "SpaceChart":
-            jp({
+            Wp({
                 model: r,
                 el: e
             });
             break;
         case "EstimatesOverview":
-            Up({
+            Yp({
                 model: r,
                 el: e
             });
             break;
         case "EstimateDetails":
-            Vp({
+            Up({
                 model: r,
                 el: e
             });
             break;
         case "Histogram":
-            Yp({
+            Qp({
                 model: r,
                 el: e
             });
             break;
         case "EstimatesPanel":
-            Wp({
+            Zp({
                 model: r,
                 el: e
             });
             break;
         case "Circuit":
-            Zp({
+            Xp({
                 model: r,
                 el: e
             });
             break;
         default:
             throw new Error(`Unknown component type ${i}`)
     }
 }
 
-function Vp({
+function Up({
     model: r,
     el: e
 }) {
     let i = () => {
         let a = r.get("estimates"),
             l = r.get("index"),
             c = jt(a, l);
         rr(M(qr, {
             estimatesData: c,
-            mdRenderer: Eu
+            mdRenderer: zu
         }), e)
     };
     i(), r.on("change:estimates", i), r.on("change:index", i)
 }
 
-function jp({
+function Wp({
     model: r,
     el: e
 }) {
     let i = () => {
         let a = r.get("estimates"),
             l = r.get("index"),
             c = jt(a, l);
         rr(M(Mr, {
             estimatesData: c
         }), e)
     };
     i(), r.on("change:estimates", i), r.on("change:index", i)
 }
 
-function Up({
+function Yp({
     model: r,
     el: e
 }) {
     let i = () => {
         let a = r.get("estimates"),
             l = r.get("colors"),
             c = r.get("runNames"),
             d = [];
         if (a[0] == null) d.push(a);
         else
             for (let g of Object.values(a)) d.push(g);
-        let f = Du(d, g => {
+        let f = Ru(d, g => {
             d = g, r.set("estimates", d)
         });
         rr(M(Er, {
             estimatesData: d,
             runNames: c,
             colors: l,
             isSimplifiedView: !0,
             onRowDeleted: f,
             setEstimate: () => {}
         }), e)
     };
     i(), r.on("change:estimates", i), r.on("change:colors", i), r.on("change:runNames", i)
 }
 
-function Wp({
+function Zp({
     model: r,
     el: e
 }) {
     let i = () => {
         let a = r.get("estimates"),
             l = r.get("colors"),
             c = r.get("runNames"),
             d = [];
         if (a[0] == null) d.push(a);
         else
             for (let g of Object.values(a)) d.push(g);
-        let f = Du(d, g => {
+        let f = Ru(d, g => {
             d = g, r.set("estimates", d)
         });
-        rr(M(Hn, {
+        rr(M(Gn, {
             estimatesData: d,
             runNames: c,
             colors: l,
-            renderer: Eu,
+            renderer: zu,
             calculating: !1,
             onRowDeleted: f
         }), e)
     };
     i(), r.on("change:estimates", i), r.on("change:colors", i), r.on("change:runNames", i)
 }
 
-function Du(r, e) {
+function Ru(r, e) {
     return i => {
         let a = JSON.parse(JSON.stringify(r)),
             l = a.findIndex(c => c.jobParams.runName === i);
         l >= 0 && a.splice(l, 1), e(a)
     }
 }
 
-function Yp({
+function Qp({
     model: r,
     el: e
 }) {
     let i = () => {
         let a = r.get("buckets"),
             l = new Map(Object.entries(a)),
             c = r.get("shot_count");
-        rr(M(Pn, {
+        rr(M(On, {
             data: l,
             shotCount: c,
             filter: "",
             onFilter: () => {},
             shotsHeader: !0
         }), e)
     };
     i(), r.on("change:buckets", i), r.on("change:shot_count", i)
 }
 
-function Zp({
+function Xp({
     model: r,
     el: e
 }) {
     let i = () => {
         let a = r.get("circuit_json");
-        rr(M(ri, {
+        rr(M(ii, {
             circuit: JSON.parse(a)
         }), e)
     };
     i(), r.on("change:circuit_json", i)
 }
 export {
-    Eu as mdRenderer, n5 as render
+    zu as mdRenderer, u5 as render
 };
```

