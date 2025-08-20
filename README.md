[FinalProject_AUSWeather.slides.html](https://github.com/user-attachments/files/21903419/FinalProject_AUSWeather.slides.html)
<!DOCTYPE html>

<html lang="en">
<head><meta charset="utf-8"/>
<meta content="chrome=1" http-equiv="X-UA-Compatible"/>
<meta content="yes" name="apple-mobile-web-app-capable"/>
<meta content="black-translucent" name="apple-mobile-web-app-status-bar-style"/>
<title>FinalProject_AUSWeather slides</title><script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/2.0.3/jquery.min.js"></script><script src="https://cdnjs.cloudflare.com/ajax/libs/require.js/2.1.10/require.min.js"></script><script type="module">
  import mermaid from 'https://cdnjs.cloudflare.com/ajax/libs/mermaid/10.7.0/mermaid.esm.min.mjs';
  mermaid.initialize({ startOnLoad: true });
</script>
<!-- General and theme style sheets -->
<link href="https://unpkg.com/reveal.js@4.0.2/dist/reveal.css" rel="stylesheet"/>
<!-- If the query includes 'print-pdf', include the PDF print sheet -->
<script>
if( window.location.search.match( /print-pdf/gi ) ) {
        var link = document.createElement( 'link' );
        link.rel = 'stylesheet';
        link.type = 'text/css';
        document.getElementsByTagName( 'head' )[0].appendChild( link );
}
</script>
<style type="text/css">
    pre { line-height: 125%; }
td.linenos .normal { color: inherit; background-color: transparent; padding-left: 5px; padding-right: 5px; }
span.linenos { color: inherit; background-color: transparent; padding-left: 5px; padding-right: 5px; }
td.linenos .special { color: #000000; background-color: #ffffc0; padding-left: 5px; padding-right: 5px; }
span.linenos.special { color: #000000; background-color: #ffffc0; padding-left: 5px; padding-right: 5px; }
.highlight .hll { background-color: var(--jp-cell-editor-active-background) }
.highlight { background: var(--jp-cell-editor-background); color: var(--jp-mirror-editor-variable-color) }
.highlight .c { color: var(--jp-mirror-editor-comment-color); font-style: italic } /* Comment */
.highlight .err { color: var(--jp-mirror-editor-error-color) } /* Error */
.highlight .k { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /* Keyword */
.highlight .o { color: var(--jp-mirror-editor-operator-color); font-weight: bold } /* Operator */
.highlight .p { color: var(--jp-mirror-editor-punctuation-color) } /* Punctuation */
.highlight .ch { color: var(--jp-mirror-editor-comment-color); font-style: italic } /* Comment.Hashbang */
.highlight .cm { color: var(--jp-mirror-editor-comment-color); font-style: italic } /* Comment.Multiline */
.highlight .cp { color: var(--jp-mirror-editor-comment-color); font-style: italic } /* Comment.Preproc */
.highlight .cpf { color: var(--jp-mirror-editor-comment-color); font-style: italic } /* Comment.PreprocFile */
.highlight .c1 { color: var(--jp-mirror-editor-comment-color); font-style: italic } /* Comment.Single */
.highlight .cs { color: var(--jp-mirror-editor-comment-color); font-style: italic } /* Comment.Special */
.highlight .kc { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /* Keyword.Constant */
.highlight .kd { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /* Keyword.Declaration */
.highlight .kn { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /* Keyword.Namespace */
.highlight .kp { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /* Keyword.Pseudo */
.highlight .kr { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /* Keyword.Reserved */
.highlight .kt { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /* Keyword.Type */
.highlight .m { color: var(--jp-mirror-editor-number-color) } /* Literal.Number */
.highlight .s { color: var(--jp-mirror-editor-string-color) } /* Literal.String */
.highlight .ow { color: var(--jp-mirror-editor-operator-color); font-weight: bold } /* Operator.Word */
.highlight .pm { color: var(--jp-mirror-editor-punctuation-color) } /* Punctuation.Marker */
.highlight .w { color: var(--jp-mirror-editor-variable-color) } /* Text.Whitespace */
.highlight .mb { color: var(--jp-mirror-editor-number-color) } /* Literal.Number.Bin */
.highlight .mf { color: var(--jp-mirror-editor-number-color) } /* Literal.Number.Float */
.highlight .mh { color: var(--jp-mirror-editor-number-color) } /* Literal.Number.Hex */
.highlight .mi { color: var(--jp-mirror-editor-number-color) } /* Literal.Number.Integer */
.highlight .mo { color: var(--jp-mirror-editor-number-color) } /* Literal.Number.Oct */
.highlight .sa { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Affix */
.highlight .sb { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Backtick */
.highlight .sc { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Char */
.highlight .dl { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Delimiter */
.highlight .sd { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Doc */
.highlight .s2 { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Double */
.highlight .se { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Escape */
.highlight .sh { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Heredoc */
.highlight .si { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Interpol */
.highlight .sx { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Other */
.highlight .sr { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Regex */
.highlight .s1 { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Single */
.highlight .ss { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Symbol */
.highlight .il { color: var(--jp-mirror-editor-number-color) } /* Literal.Number.Integer.Long */
  </style>
<style type="text/css">
/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*
 * Mozilla scrollbar styling
 */

/* use standard opaque scrollbars for most nodes */
[data-jp-theme-scrollbars='true'] {
  scrollbar-color: rgb(var(--jp-scrollbar-thumb-color))
    var(--jp-scrollbar-background-color);
}

/* for code nodes, use a transparent style of scrollbar. These selectors
 * will match lower in the tree, and so will override the above */
[data-jp-theme-scrollbars='true'] .CodeMirror-hscrollbar,
[data-jp-theme-scrollbars='true'] .CodeMirror-vscrollbar {
  scrollbar-color: rgba(var(--jp-scrollbar-thumb-color), 0.5) transparent;
}

/* tiny scrollbar */

.jp-scrollbar-tiny {
  scrollbar-color: rgba(var(--jp-scrollbar-thumb-color), 0.5) transparent;
  scrollbar-width: thin;
}

/* tiny scrollbar */

.jp-scrollbar-tiny::-webkit-scrollbar,
.jp-scrollbar-tiny::-webkit-scrollbar-corner {
  background-color: transparent;
  height: 4px;
  width: 4px;
}

.jp-scrollbar-tiny::-webkit-scrollbar-thumb {
  background: rgba(var(--jp-scrollbar-thumb-color), 0.5);
}

.jp-scrollbar-tiny::-webkit-scrollbar-track:horizontal {
  border-left: 0 solid transparent;
  border-right: 0 solid transparent;
}

.jp-scrollbar-tiny::-webkit-scrollbar-track:vertical {
  border-top: 0 solid transparent;
  border-bottom: 0 solid transparent;
}

/*
 * Lumino
 */

.lm-ScrollBar[data-orientation='horizontal'] {
  min-height: 16px;
  max-height: 16px;
  min-width: 45px;
  border-top: 1px solid #a0a0a0;
}

.lm-ScrollBar[data-orientation='vertical'] {
  min-width: 16px;
  max-width: 16px;
  min-height: 45px;
  border-left: 1px solid #a0a0a0;
}

.lm-ScrollBar-button {
  background-color: #f0f0f0;
  background-position: center center;
  min-height: 15px;
  max-height: 15px;
  min-width: 15px;
  max-width: 15px;
}

.lm-ScrollBar-button:hover {
  background-color: #dadada;
}

.lm-ScrollBar-button.lm-mod-active {
  background-color: #cdcdcd;
}

.lm-ScrollBar-track {
  background: #f0f0f0;
}

.lm-ScrollBar-thumb {
  background: #cdcdcd;
}

.lm-ScrollBar-thumb:hover {
  background: #bababa;
}

.lm-ScrollBar-thumb.lm-mod-active {
  background: #a0a0a0;
}

.lm-ScrollBar[data-orientation='horizontal'] .lm-ScrollBar-thumb {
  height: 100%;
  min-width: 15px;
  border-left: 1px solid #a0a0a0;
  border-right: 1px solid #a0a0a0;
}

.lm-ScrollBar[data-orientation='vertical'] .lm-ScrollBar-thumb {
  width: 100%;
  min-height: 15px;
  border-top: 1px solid #a0a0a0;
  border-bottom: 1px solid #a0a0a0;
}

.lm-ScrollBar[data-orientation='horizontal']
  .lm-ScrollBar-button[data-action='decrement'] {
  background-image: var(--jp-icon-caret-left);
  background-size: 17px;
}

.lm-ScrollBar[data-orientation='horizontal']
  .lm-ScrollBar-button[data-action='increment'] {
  background-image: var(--jp-icon-caret-right);
  background-size: 17px;
}

.lm-ScrollBar[data-orientation='vertical']
  .lm-ScrollBar-button[data-action='decrement'] {
  background-image: var(--jp-icon-caret-up);
  background-size: 17px;
}

.lm-ScrollBar[data-orientation='vertical']
  .lm-ScrollBar-button[data-action='increment'] {
  background-image: var(--jp-icon-caret-down);
  background-size: 17px;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-Widget {
  box-sizing: border-box;
  position: relative;
  overflow: hidden;
}

.lm-Widget.lm-mod-hidden {
  display: none !important;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

.lm-AccordionPanel[data-orientation='horizontal'] > .lm-AccordionPanel-title {
  /* Title is rotated for horizontal accordion panel using CSS */
  display: block;
  transform-origin: top left;
  transform: rotate(-90deg) translate(-100%);
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-CommandPalette {
  display: flex;
  flex-direction: column;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

.lm-CommandPalette-search {
  flex: 0 0 auto;
}

.lm-CommandPalette-content {
  flex: 1 1 auto;
  margin: 0;
  padding: 0;
  min-height: 0;
  overflow: auto;
  list-style-type: none;
}

.lm-CommandPalette-header {
  overflow: hidden;
  white-space: nowrap;
  text-overflow: ellipsis;
}

.lm-CommandPalette-item {
  display: flex;
  flex-direction: row;
}

.lm-CommandPalette-itemIcon {
  flex: 0 0 auto;
}

.lm-CommandPalette-itemContent {
  flex: 1 1 auto;
  overflow: hidden;
}

.lm-CommandPalette-itemShortcut {
  flex: 0 0 auto;
}

.lm-CommandPalette-itemLabel {
  overflow: hidden;
  white-space: nowrap;
  text-overflow: ellipsis;
}

.lm-close-icon {
  border: 1px solid transparent;
  background-color: transparent;
  position: absolute;
  z-index: 1;
  right: 3%;
  top: 0;
  bottom: 0;
  margin: auto;
  padding: 7px 0;
  display: none;
  vertical-align: middle;
  outline: 0;
  cursor: pointer;
}
.lm-close-icon:after {
  content: 'X';
  display: block;
  width: 15px;
  height: 15px;
  text-align: center;
  color: #000;
  font-weight: normal;
  font-size: 12px;
  cursor: pointer;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-DockPanel {
  z-index: 0;
}

.lm-DockPanel-widget {
  z-index: 0;
}

.lm-DockPanel-tabBar {
  z-index: 1;
}

.lm-DockPanel-handle {
  z-index: 2;
}

.lm-DockPanel-handle.lm-mod-hidden {
  display: none !important;
}

.lm-DockPanel-handle:after {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  content: '';
}

.lm-DockPanel-handle[data-orientation='horizontal'] {
  cursor: ew-resize;
}

.lm-DockPanel-handle[data-orientation='vertical'] {
  cursor: ns-resize;
}

.lm-DockPanel-handle[data-orientation='horizontal']:after {
  left: 50%;
  min-width: 8px;
  transform: translateX(-50%);
}

.lm-DockPanel-handle[data-orientation='vertical']:after {
  top: 50%;
  min-height: 8px;
  transform: translateY(-50%);
}

.lm-DockPanel-overlay {
  z-index: 3;
  box-sizing: border-box;
  pointer-events: none;
}

.lm-DockPanel-overlay.lm-mod-hidden {
  display: none !important;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-Menu {
  z-index: 10000;
  position: absolute;
  white-space: nowrap;
  overflow-x: hidden;
  overflow-y: auto;
  outline: none;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

.lm-Menu-content {
  margin: 0;
  padding: 0;
  display: table;
  list-style-type: none;
}

.lm-Menu-item {
  display: table-row;
}

.lm-Menu-item.lm-mod-hidden,
.lm-Menu-item.lm-mod-collapsed {
  display: none !important;
}

.lm-Menu-itemIcon,
.lm-Menu-itemSubmenuIcon {
  display: table-cell;
  text-align: center;
}

.lm-Menu-itemLabel {
  display: table-cell;
  text-align: left;
}

.lm-Menu-itemShortcut {
  display: table-cell;
  text-align: right;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-MenuBar {
  outline: none;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

.lm-MenuBar-content {
  margin: 0;
  padding: 0;
  display: flex;
  flex-direction: row;
  list-style-type: none;
}

.lm-MenuBar-item {
  box-sizing: border-box;
}

.lm-MenuBar-itemIcon,
.lm-MenuBar-itemLabel {
  display: inline-block;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-ScrollBar {
  display: flex;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

.lm-ScrollBar[data-orientation='horizontal'] {
  flex-direction: row;
}

.lm-ScrollBar[data-orientation='vertical'] {
  flex-direction: column;
}

.lm-ScrollBar-button {
  box-sizing: border-box;
  flex: 0 0 auto;
}

.lm-ScrollBar-track {
  box-sizing: border-box;
  position: relative;
  overflow: hidden;
  flex: 1 1 auto;
}

.lm-ScrollBar-thumb {
  box-sizing: border-box;
  position: absolute;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-SplitPanel-child {
  z-index: 0;
}

.lm-SplitPanel-handle {
  z-index: 1;
}

.lm-SplitPanel-handle.lm-mod-hidden {
  display: none !important;
}

.lm-SplitPanel-handle:after {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  content: '';
}

.lm-SplitPanel[data-orientation='horizontal'] > .lm-SplitPanel-handle {
  cursor: ew-resize;
}

.lm-SplitPanel[data-orientation='vertical'] > .lm-SplitPanel-handle {
  cursor: ns-resize;
}

.lm-SplitPanel[data-orientation='horizontal'] > .lm-SplitPanel-handle:after {
  left: 50%;
  min-width: 8px;
  transform: translateX(-50%);
}

.lm-SplitPanel[data-orientation='vertical'] > .lm-SplitPanel-handle:after {
  top: 50%;
  min-height: 8px;
  transform: translateY(-50%);
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-TabBar {
  display: flex;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

.lm-TabBar[data-orientation='horizontal'] {
  flex-direction: row;
  align-items: flex-end;
}

.lm-TabBar[data-orientation='vertical'] {
  flex-direction: column;
  align-items: flex-end;
}

.lm-TabBar-content {
  margin: 0;
  padding: 0;
  display: flex;
  flex: 1 1 auto;
  list-style-type: none;
}

.lm-TabBar[data-orientation='horizontal'] > .lm-TabBar-content {
  flex-direction: row;
}

.lm-TabBar[data-orientation='vertical'] > .lm-TabBar-content {
  flex-direction: column;
}

.lm-TabBar-tab {
  display: flex;
  flex-direction: row;
  box-sizing: border-box;
  overflow: hidden;
  touch-action: none; /* Disable native Drag/Drop */
}

.lm-TabBar-tabIcon,
.lm-TabBar-tabCloseIcon {
  flex: 0 0 auto;
}

.lm-TabBar-tabLabel {
  flex: 1 1 auto;
  overflow: hidden;
  white-space: nowrap;
}

.lm-TabBar-tabInput {
  user-select: all;
  width: 100%;
  box-sizing: border-box;
}

.lm-TabBar-tab.lm-mod-hidden {
  display: none !important;
}

.lm-TabBar-addButton.lm-mod-hidden {
  display: none !important;
}

.lm-TabBar.lm-mod-dragging .lm-TabBar-tab {
  position: relative;
}

.lm-TabBar.lm-mod-dragging[data-orientation='horizontal'] .lm-TabBar-tab {
  left: 0;
  transition: left 150ms ease;
}

.lm-TabBar.lm-mod-dragging[data-orientation='vertical'] .lm-TabBar-tab {
  top: 0;
  transition: top 150ms ease;
}

.lm-TabBar.lm-mod-dragging .lm-TabBar-tab.lm-mod-dragging {
  transition: none;
}

.lm-TabBar-tabLabel .lm-TabBar-tabInput {
  user-select: all;
  width: 100%;
  box-sizing: border-box;
  background: inherit;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-TabPanel-tabBar {
  z-index: 1;
}

.lm-TabPanel-stackedPanel {
  z-index: 0;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-Collapse {
  display: flex;
  flex-direction: column;
  align-items: stretch;
}

.jp-Collapse-header {
  padding: 1px 12px;
  background-color: var(--jp-layout-color1);
  border-bottom: solid var(--jp-border-width) var(--jp-border-color2);
  color: var(--jp-ui-font-color1);
  cursor: pointer;
  display: flex;
  align-items: center;
  font-size: var(--jp-ui-font-size0);
  font-weight: 600;
  text-transform: uppercase;
  user-select: none;
}

.jp-Collapser-icon {
  height: 16px;
}

.jp-Collapse-header-collapsed .jp-Collapser-icon {
  transform: rotate(-90deg);
  margin: auto 0;
}

.jp-Collapser-title {
  line-height: 25px;
}

.jp-Collapse-contents {
  padding: 0 12px;
  background-color: var(--jp-layout-color1);
  color: var(--jp-ui-font-color1);
  overflow: auto;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/* This file was auto-generated by ensureUiComponents() in @jupyterlab/buildutils */

/**
 * (DEPRECATED) Support for consuming icons as CSS background images
 */

/* Icons urls */

:root {
  --jp-icon-add-above: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTQiIGhlaWdodD0iMTQiIHZpZXdCb3g9IjAgMCAxNCAxNCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPGcgY2xpcC1wYXRoPSJ1cmwoI2NsaXAwXzEzN18xOTQ5MikiPgo8cGF0aCBjbGFzcz0ianAtaWNvbjMiIGQ9Ik00Ljc1IDQuOTMwNjZINi42MjVWNi44MDU2NkM2LjYyNSA3LjAxMTkxIDYuNzkzNzUgNy4xODA2NiA3IDcuMTgwNjZDNy4yMDYyNSA3LjE4MDY2IDcuMzc1IDcuMDExOTEgNy4zNzUgNi44MDU2NlY0LjkzMDY2SDkuMjVDOS40NTYyNSA0LjkzMDY2IDkuNjI1IDQuNzYxOTEgOS42MjUgNC41NTU2NkM5LjYyNSA0LjM0OTQxIDkuNDU2MjUgNC4xODA2NiA5LjI1IDQuMTgwNjZINy4zNzVWMi4zMDU2NkM3LjM3NSAyLjA5OTQxIDcuMjA2MjUgMS45MzA2NiA3IDEuOTMwNjZDNi43OTM3NSAxLjkzMDY2IDYuNjI1IDIuMDk5NDEgNi42MjUgMi4zMDU2NlY0LjE4MDY2SDQuNzVDNC41NDM3NSA0LjE4MDY2IDQuMzc1IDQuMzQ5NDEgNC4zNzUgNC41NTU2NkM0LjM3NSA0Ljc2MTkxIDQuNTQzNzUgNC45MzA2NiA0Ljc1IDQuOTMwNjZaIiBmaWxsPSIjNjE2MTYxIiBzdHJva2U9IiM2MTYxNjEiIHN0cm9rZS13aWR0aD0iMC43Ii8+CjwvZz4KPHBhdGggY2xhc3M9ImpwLWljb24zIiBmaWxsLXJ1bGU9ImV2ZW5vZGQiIGNsaXAtcnVsZT0iZXZlbm9kZCIgZD0iTTExLjUgOS41VjExLjVMMi41IDExLjVWOS41TDExLjUgOS41Wk0xMiA4QzEyLjU1MjMgOCAxMyA4LjQ0NzcyIDEzIDlWMTJDMTMgMTIuNTUyMyAxMi41NTIzIDEzIDEyIDEzTDIgMTNDMS40NDc3MiAxMyAxIDEyLjU1MjMgMSAxMlY5QzEgOC40NDc3MiAxLjQ0NzcxIDggMiA4TDEyIDhaIiBmaWxsPSIjNjE2MTYxIi8+CjxkZWZzPgo8Y2xpcFBhdGggaWQ9ImNsaXAwXzEzN18xOTQ5MiI+CjxyZWN0IGNsYXNzPSJqcC1pY29uMyIgd2lkdGg9IjYiIGhlaWdodD0iNiIgZmlsbD0id2hpdGUiIHRyYW5zZm9ybT0ibWF0cml4KC0xIDAgMCAxIDEwIDEuNTU1NjYpIi8+CjwvY2xpcFBhdGg+CjwvZGVmcz4KPC9zdmc+Cg==);
  --jp-icon-add-below: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTQiIGhlaWdodD0iMTQiIHZpZXdCb3g9IjAgMCAxNCAxNCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPGcgY2xpcC1wYXRoPSJ1cmwoI2NsaXAwXzEzN18xOTQ5OCkiPgo8cGF0aCBjbGFzcz0ianAtaWNvbjMiIGQ9Ik05LjI1IDEwLjA2OTNMNy4zNzUgMTAuMDY5M0w3LjM3NSA4LjE5NDM0QzcuMzc1IDcuOTg4MDkgNy4yMDYyNSA3LjgxOTM0IDcgNy44MTkzNEM2Ljc5Mzc1IDcuODE5MzQgNi42MjUgNy45ODgwOSA2LjYyNSA4LjE5NDM0TDYuNjI1IDEwLjA2OTNMNC43NSAxMC4wNjkzQzQuNTQzNzUgMTAuMDY5MyA0LjM3NSAxMC4yMzgxIDQuMzc1IDEwLjQ0NDNDNC4zNzUgMTAuNjUwNiA0LjU0Mzc1IDEwLjgxOTMgNC43NSAxMC44MTkzTDYuNjI1IDEwLjgxOTNMNi42MjUgMTIuNjk0M0M2LjYyNSAxMi45MDA2IDYuNzkzNzUgMTMuMDY5MyA3IDEzLjA2OTNDNy4yMDYyNSAxMy4wNjkzIDcuMzc1IDEyLjkwMDYgNy4zNzUgMTIuNjk0M0w3LjM3NSAxMC44MTkzTDkuMjUgMTAuODE5M0M5LjQ1NjI1IDEwLjgxOTMgOS42MjUgMTAuNjUwNiA5LjYyNSAxMC40NDQzQzkuNjI1IDEwLjIzODEgOS40NTYyNSAxMC4wNjkzIDkuMjUgMTAuMDY5M1oiIGZpbGw9IiM2MTYxNjEiIHN0cm9rZT0iIzYxNjE2MSIgc3Ryb2tlLXdpZHRoPSIwLjciLz4KPC9nPgo8cGF0aCBjbGFzcz0ianAtaWNvbjMiIGZpbGwtcnVsZT0iZXZlbm9kZCIgY2xpcC1ydWxlPSJldmVub2RkIiBkPSJNMi41IDUuNUwyLjUgMy41TDExLjUgMy41TDExLjUgNS41TDIuNSA1LjVaTTIgN0MxLjQ0NzcyIDcgMSA2LjU1MjI4IDEgNkwxIDNDMSAyLjQ0NzcyIDEuNDQ3NzIgMiAyIDJMMTIgMkMxMi41NTIzIDIgMTMgMi40NDc3MiAxMyAzTDEzIDZDMTMgNi41NTIyOSAxMi41NTIzIDcgMTIgN0wyIDdaIiBmaWxsPSIjNjE2MTYxIi8+CjxkZWZzPgo8Y2xpcFBhdGggaWQ9ImNsaXAwXzEzN18xOTQ5OCI+CjxyZWN0IGNsYXNzPSJqcC1pY29uMyIgd2lkdGg9IjYiIGhlaWdodD0iNiIgZmlsbD0id2hpdGUiIHRyYW5zZm9ybT0ibWF0cml4KDEgMS43NDg0NmUtMDcgMS43NDg0NmUtMDcgLTEgNCAxMy40NDQzKSIvPgo8L2NsaXBQYXRoPgo8L2RlZnM+Cjwvc3ZnPgo=);
  --jp-icon-add: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTE5IDEzaC02djZoLTJ2LTZINXYtMmg2VjVoMnY2aDZ2MnoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-bell: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE2IDE2IiB2ZXJzaW9uPSIxLjEiPgogICA8cGF0aCBjbGFzcz0ianAtaWNvbjIganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjMzMzMzMzIgogICAgICBkPSJtOCAwLjI5Yy0xLjQgMC0yLjcgMC43My0zLjYgMS44LTEuMiAxLjUtMS40IDMuNC0xLjUgNS4yLTAuMTggMi4yLTAuNDQgNC0yLjMgNS4zbDAuMjggMS4zaDVjMC4wMjYgMC42NiAwLjMyIDEuMSAwLjcxIDEuNSAwLjg0IDAuNjEgMiAwLjYxIDIuOCAwIDAuNTItMC40IDAuNi0xIDAuNzEtMS41aDVsMC4yOC0xLjNjLTEuOS0wLjk3LTIuMi0zLjMtMi4zLTUuMy0wLjEzLTEuOC0wLjI2LTMuNy0xLjUtNS4yLTAuODUtMS0yLjItMS44LTMuNi0xLjh6bTAgMS40YzAuODggMCAxLjkgMC41NSAyLjUgMS4zIDAuODggMS4xIDEuMSAyLjcgMS4yIDQuNCAwLjEzIDEuNyAwLjIzIDMuNiAxLjMgNS4yaC0xMGMxLjEtMS42IDEuMi0zLjQgMS4zLTUuMiAwLjEzLTEuNyAwLjMtMy4zIDEuMi00LjQgMC41OS0wLjcyIDEuNi0xLjMgMi41LTEuM3ptLTAuNzQgMTJoMS41Yy0wLjAwMTUgMC4yOCAwLjAxNSAwLjc5LTAuNzQgMC43OS0wLjczIDAuMDAxNi0wLjcyLTAuNTMtMC43NC0wLjc5eiIgLz4KPC9zdmc+Cg==);
  --jp-icon-bug-dot: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjQiIGhlaWdodD0iMjQiIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiM2MTYxNjEiPgogICAgICAgIDxwYXRoIGZpbGwtcnVsZT0iZXZlbm9kZCIgY2xpcC1ydWxlPSJldmVub2RkIiBkPSJNMTcuMTkgOEgyMFYxMEgxNy45MUMxNy45NiAxMC4zMyAxOCAxMC42NiAxOCAxMVYxMkgyMFYxNEgxOC41SDE4VjE0LjAyNzVDMTUuNzUgMTQuMjc2MiAxNCAxNi4xODM3IDE0IDE4LjVDMTQgMTkuMjA4IDE0LjE2MzUgMTkuODc3OSAxNC40NTQ5IDIwLjQ3MzlDMTMuNzA2MyAyMC44MTE3IDEyLjg3NTcgMjEgMTIgMjFDOS43OCAyMSA3Ljg1IDE5Ljc5IDYuODEgMThINFYxNkg2LjA5QzYuMDQgMTUuNjcgNiAxNS4zNCA2IDE1VjE0SDRWMTJINlYxMUM2IDEwLjY2IDYuMDQgMTAuMzMgNi4wOSAxMEg0VjhINi44MUM3LjI2IDcuMjIgNy44OCA2LjU1IDguNjIgNi4wNEw3IDQuNDFMOC40MSAzTDEwLjU5IDUuMTdDMTEuMDQgNS4wNiAxMS41MSA1IDEyIDVDMTIuNDkgNSAxMi45NiA1LjA2IDEzLjQyIDUuMTdMMTUuNTkgM0wxNyA0LjQxTDE1LjM3IDYuMDRDMTYuMTIgNi41NSAxNi43NCA3LjIyIDE3LjE5IDhaTTEwIDE2SDE0VjE0SDEwVjE2Wk0xMCAxMkgxNFYxMEgxMFYxMloiIGZpbGw9IiM2MTYxNjEiLz4KICAgICAgICA8cGF0aCBkPSJNMjIgMTguNUMyMiAyMC40MzMgMjAuNDMzIDIyIDE4LjUgMjJDMTYuNTY3IDIyIDE1IDIwLjQzMyAxNSAxOC41QzE1IDE2LjU2NyAxNi41NjcgMTUgMTguNSAxNUMyMC40MzMgMTUgMjIgMTYuNTY3IDIyIDE4LjVaIiBmaWxsPSIjNjE2MTYxIi8+CiAgICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-bug: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIj4KICAgIDxwYXRoIGQ9Ik0yMCA4aC0yLjgxYy0uNDUtLjc4LTEuMDctMS40NS0xLjgyLTEuOTZMMTcgNC40MSAxNS41OSAzbC0yLjE3IDIuMTdDMTIuOTYgNS4wNiAxMi40OSA1IDEyIDVjLS40OSAwLS45Ni4wNi0xLjQxLjE3TDguNDEgMyA3IDQuNDFsMS42MiAxLjYzQzcuODggNi41NSA3LjI2IDcuMjIgNi44MSA4SDR2MmgyLjA5Yy0uMDUuMzMtLjA5LjY2LS4wOSAxdjFINHYyaDJ2MWMwIC4zNC4wNC42Ny4wOSAxSDR2MmgyLjgxYzEuMDQgMS43OSAyLjk3IDMgNS4xOSAzczQuMTUtMS4yMSA1LjE5LTNIMjB2LTJoLTIuMDljLjA1LS4zMy4wOS0uNjYuMDktMXYtMWgydi0yaC0ydi0xYzAtLjM0LS4wNC0uNjctLjA5LTFIMjBWOHptLTYgOGgtNHYtMmg0djJ6bTAtNGgtNHYtMmg0djJ6Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-build: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTYiIHZpZXdCb3g9IjAgMCAyNCAyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTE0LjkgMTcuNDVDMTYuMjUgMTcuNDUgMTcuMzUgMTYuMzUgMTcuMzUgMTVDMTcuMzUgMTMuNjUgMTYuMjUgMTIuNTUgMTQuOSAxMi41NUMxMy41NCAxMi41NSAxMi40NSAxMy42NSAxMi40NSAxNUMxMi40NSAxNi4zNSAxMy41NCAxNy40NSAxNC45IDE3LjQ1Wk0yMC4xIDE1LjY4TDIxLjU4IDE2Ljg0QzIxLjcxIDE2Ljk1IDIxLjc1IDE3LjEzIDIxLjY2IDE3LjI5TDIwLjI2IDE5LjcxQzIwLjE3IDE5Ljg2IDIwIDE5LjkyIDE5LjgzIDE5Ljg2TDE4LjA5IDE5LjE2QzE3LjczIDE5LjQ0IDE3LjMzIDE5LjY3IDE2LjkxIDE5Ljg1TDE2LjY0IDIxLjdDMTYuNjIgMjEuODcgMTYuNDcgMjIgMTYuMyAyMkgxMy41QzEzLjMyIDIyIDEzLjE4IDIxLjg3IDEzLjE1IDIxLjdMMTIuODkgMTkuODVDMTIuNDYgMTkuNjcgMTIuMDcgMTkuNDQgMTEuNzEgMTkuMTZMOS45NjAwMiAxOS44NkM5LjgxMDAyIDE5LjkyIDkuNjIwMDIgMTkuODYgOS41NDAwMiAxOS43MUw4LjE0MDAyIDE3LjI5QzguMDUwMDIgMTcuMTMgOC4wOTAwMiAxNi45NSA4LjIyMDAyIDE2Ljg0TDkuNzAwMDIgMTUuNjhMOS42NTAwMSAxNUw5LjcwMDAyIDE0LjMxTDguMjIwMDIgMTMuMTZDOC4wOTAwMiAxMy4wNSA4LjA1MDAyIDEyLjg2IDguMTQwMDIgMTIuNzFMOS41NDAwMiAxMC4yOUM5LjYyMDAyIDEwLjEzIDkuODEwMDIgMTAuMDcgOS45NjAwMiAxMC4xM0wxMS43MSAxMC44NEMxMi4wNyAxMC41NiAxMi40NiAxMC4zMiAxMi44OSAxMC4xNUwxMy4xNSA4LjI4OTk4QzEzLjE4IDguMTI5OTggMTMuMzIgNy45OTk5OCAxMy41IDcuOTk5OThIMTYuM0MxNi40NyA3Ljk5OTk4IDE2LjYyIDguMTI5OTggMTYuNjQgOC4yODk5OEwxNi45MSAxMC4xNUMxNy4zMyAxMC4zMiAxNy43MyAxMC41NiAxOC4wOSAxMC44NEwxOS44MyAxMC4xM0MyMCAxMC4wNyAyMC4xNyAxMC4xMyAyMC4yNiAxMC4yOUwyMS42NiAxMi43MUMyMS43NSAxMi44NiAyMS43MSAxMy4wNSAyMS41OCAxMy4xNkwyMC4xIDE0LjMxTDIwLjE1IDE1TDIwLjEgMTUuNjhaIi8+CiAgICA8cGF0aCBkPSJNNy4zMjk2NiA3LjQ0NDU0QzguMDgzMSA3LjAwOTU0IDguMzM5MzIgNi4wNTMzMiA3LjkwNDMyIDUuMjk5ODhDNy40NjkzMiA0LjU0NjQzIDYuNTA4MSA0LjI4MTU2IDUuNzU0NjYgNC43MTY1NkM1LjM5MTc2IDQuOTI2MDggNS4xMjY5NSA1LjI3MTE4IDUuMDE4NDkgNS42NzU5NEM0LjkxMDA0IDYuMDgwNzEgNC45NjY4MiA2LjUxMTk4IDUuMTc2MzQgNi44NzQ4OEM1LjYxMTM0IDcuNjI4MzIgNi41NzYyMiA3Ljg3OTU0IDcuMzI5NjYgNy40NDQ1NFpNOS42NTcxOCA0Ljc5NTkzTDEwLjg2NzIgNC45NTE3OUMxMC45NjI4IDQuOTc3NDEgMTEuMDQwMiA1LjA3MTMzIDExLjAzODIgNS4xODc5M0wxMS4wMzg4IDYuOTg4OTNDMTEuMDQ1NSA3LjEwMDU0IDEwLjk2MTYgNy4xOTUxOCAxMC44NTUgNy4yMTA1NEw5LjY2MDAxIDcuMzgwODNMOS4yMzkxNSA4LjEzMTg4TDkuNjY5NjEgOS4yNTc0NUM5LjcwNzI5IDkuMzYyNzEgOS42NjkzNCA5LjQ3Njk5IDkuNTc0MDggOS41MzE5OUw4LjAxNTIzIDEwLjQzMkM3LjkxMTMxIDEwLjQ5MiA3Ljc5MzM3IDEwLjQ2NzcgNy43MjEwNSAxMC4zODI0TDYuOTg3NDggOS40MzE4OEw2LjEwOTMxIDkuNDMwODNMNS4zNDcwNCAxMC4zOTA1QzUuMjg5MDkgMTAuNDcwMiA1LjE3MzgzIDEwLjQ5MDUgNS4wNzE4NyAxMC40MzM5TDMuNTEyNDUgOS41MzI5M0MzLjQxMDQ5IDkuNDc2MzMgMy4zNzY0NyA5LjM1NzQxIDMuNDEwNzUgOS4yNTY3OUwzLjg2MzQ3IDguMTQwOTNMMy42MTc0OSA3Ljc3NDg4TDMuNDIzNDcgNy4zNzg4M0wyLjIzMDc1IDcuMjEyOTdDMi4xMjY0NyA3LjE5MjM1IDIuMDQwNDkgNy4xMDM0MiAyLjA0MjQ1IDYuOTg2ODJMMi4wNDE4NyA1LjE4NTgyQzIuMDQzODMgNS4wNjkyMiAyLjExOTA5IDQuOTc5NTggMi4yMTcwNCA0Ljk2OTIyTDMuNDIwNjUgNC43OTM5M0wzLjg2NzQ5IDQuMDI3ODhMMy40MTEwNSAyLjkxNzMxQzMuMzczMzcgMi44MTIwNCAzLjQxMTMxIDIuNjk3NzYgMy41MTUyMyAyLjYzNzc2TDUuMDc0MDggMS43Mzc3NkM1LjE2OTM0IDEuNjgyNzYgNS4yODcyOSAxLjcwNzA0IDUuMzU5NjEgMS43OTIzMUw2LjExOTE1IDIuNzI3ODhMNi45ODAwMSAyLjczODkzTDcuNzI0OTYgMS43ODkyMkM3Ljc5MTU2IDEuNzA0NTggNy45MTU0OCAxLjY3OTIyIDguMDA4NzkgMS43NDA4Mkw5LjU2ODIxIDIuNjQxODJDOS42NzAxNyAyLjY5ODQyIDkuNzEyODUgMi44MTIzNCA5LjY4NzIzIDIuOTA3OTdMOS4yMTcxOCA0LjAzMzgzTDkuNDYzMTYgNC4zOTk4OEw5LjY1NzE4IDQuNzk1OTNaIi8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-caret-down-empty-thin: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIwIDIwIj4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSIgc2hhcGUtcmVuZGVyaW5nPSJnZW9tZXRyaWNQcmVjaXNpb24iPgoJCTxwb2x5Z29uIGNsYXNzPSJzdDEiIHBvaW50cz0iOS45LDEzLjYgMy42LDcuNCA0LjQsNi42IDkuOSwxMi4yIDE1LjQsNi43IDE2LjEsNy40ICIvPgoJPC9nPgo8L3N2Zz4K);
  --jp-icon-caret-down-empty: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiIHNoYXBlLXJlbmRlcmluZz0iZ2VvbWV0cmljUHJlY2lzaW9uIj4KICAgIDxwYXRoIGQ9Ik01LjIsNS45TDksOS43bDMuOC0zLjhsMS4yLDEuMmwtNC45LDVsLTQuOS01TDUuMiw1Ljl6Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-caret-down: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiIHNoYXBlLXJlbmRlcmluZz0iZ2VvbWV0cmljUHJlY2lzaW9uIj4KICAgIDxwYXRoIGQ9Ik01LjIsNy41TDksMTEuMmwzLjgtMy44SDUuMnoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-caret-left: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSIgc2hhcGUtcmVuZGVyaW5nPSJnZW9tZXRyaWNQcmVjaXNpb24iPgoJCTxwYXRoIGQ9Ik0xMC44LDEyLjhMNy4xLDlsMy44LTMuOGwwLDcuNkgxMC44eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-caret-right: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiIHNoYXBlLXJlbmRlcmluZz0iZ2VvbWV0cmljUHJlY2lzaW9uIj4KICAgIDxwYXRoIGQ9Ik03LjIsNS4yTDEwLjksOWwtMy44LDMuOFY1LjJINy4yeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-caret-up-empty-thin: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIwIDIwIj4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSIgc2hhcGUtcmVuZGVyaW5nPSJnZW9tZXRyaWNQcmVjaXNpb24iPgoJCTxwb2x5Z29uIGNsYXNzPSJzdDEiIHBvaW50cz0iMTUuNCwxMy4zIDkuOSw3LjcgNC40LDEzLjIgMy42LDEyLjUgOS45LDYuMyAxNi4xLDEyLjYgIi8+Cgk8L2c+Cjwvc3ZnPgo=);
  --jp-icon-caret-up: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSIgc2hhcGUtcmVuZGVyaW5nPSJnZW9tZXRyaWNQcmVjaXNpb24iPgoJCTxwYXRoIGQ9Ik01LjIsMTAuNUw5LDYuOGwzLjgsMy44SDUuMnoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-case-sensitive: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIwIDIwIj4KICA8ZyBjbGFzcz0ianAtaWNvbjIiIGZpbGw9IiM0MTQxNDEiPgogICAgPHJlY3QgeD0iMiIgeT0iMiIgd2lkdGg9IjE2IiBoZWlnaHQ9IjE2Ii8+CiAgPC9nPgogIDxnIGNsYXNzPSJqcC1pY29uLWFjY2VudDIiIGZpbGw9IiNGRkYiPgogICAgPHBhdGggZD0iTTcuNiw4aDAuOWwzLjUsOGgtMS4xTDEwLDE0SDZsLTAuOSwySDRMNy42LDh6IE04LDkuMUw2LjQsMTNoMy4yTDgsOS4xeiIvPgogICAgPHBhdGggZD0iTTE2LjYsOS44Yy0wLjIsMC4xLTAuNCwwLjEtMC43LDAuMWMtMC4yLDAtMC40LTAuMS0wLjYtMC4yYy0wLjEtMC4xLTAuMi0wLjQtMC4yLTAuNyBjLTAuMywwLjMtMC42LDAuNS0wLjksMC43Yy0wLjMsMC4xLTAuNywwLjItMS4xLDAuMmMtMC4zLDAtMC41LDAtMC43LTAuMWMtMC4yLTAuMS0wLjQtMC4yLTAuNi0wLjNjLTAuMi0wLjEtMC4zLTAuMy0wLjQtMC41IGMtMC4xLTAuMi0wLjEtMC40LTAuMS0wLjdjMC0wLjMsMC4xLTAuNiwwLjItMC44YzAuMS0wLjIsMC4zLTAuNCwwLjQtMC41QzEyLDcsMTIuMiw2LjksMTIuNSw2LjhjMC4yLTAuMSwwLjUtMC4xLDAuNy0wLjIgYzAuMy0wLjEsMC41LTAuMSwwLjctMC4xYzAuMiwwLDAuNC0wLjEsMC42LTAuMWMwLjIsMCwwLjMtMC4xLDAuNC0wLjJjMC4xLTAuMSwwLjItMC4yLDAuMi0wLjRjMC0xLTEuMS0xLTEuMy0xIGMtMC40LDAtMS40LDAtMS40LDEuMmgtMC45YzAtMC40LDAuMS0wLjcsMC4yLTFjMC4xLTAuMiwwLjMtMC40LDAuNS0wLjZjMC4yLTAuMiwwLjUtMC4zLDAuOC0wLjNDMTMuMyw0LDEzLjYsNCwxMy45LDQgYzAuMywwLDAuNSwwLDAuOCwwLjFjMC4zLDAsMC41LDAuMSwwLjcsMC4yYzAuMiwwLjEsMC40LDAuMywwLjUsMC41QzE2LDUsMTYsNS4yLDE2LDUuNnYyLjljMCwwLjIsMCwwLjQsMCwwLjUgYzAsMC4xLDAuMSwwLjIsMC4zLDAuMmMwLjEsMCwwLjIsMCwwLjMsMFY5Ljh6IE0xNS4yLDYuOWMtMS4yLDAuNi0zLjEsMC4yLTMuMSwxLjRjMCwxLjQsMy4xLDEsMy4xLTAuNVY2Ljl6Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-check: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIj4KICAgIDxwYXRoIGQ9Ik05IDE2LjE3TDQuODMgMTJsLTEuNDIgMS40MUw5IDE5IDIxIDdsLTEuNDEtMS40MXoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-circle-empty: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTEyIDJDNi40NyAyIDIgNi40NyAyIDEyczQuNDcgMTAgMTAgMTAgMTAtNC40NyAxMC0xMFMxNy41MyAyIDEyIDJ6bTAgMThjLTQuNDEgMC04LTMuNTktOC04czMuNTktOCA4LTggOCAzLjU5IDggOC0zLjU5IDgtOCA4eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-circle: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMTggMTgiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPGNpcmNsZSBjeD0iOSIgY3k9IjkiIHI9IjgiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-clear: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8bWFzayBpZD0iZG9udXRIb2xlIj4KICAgIDxyZWN0IHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgZmlsbD0id2hpdGUiIC8+CiAgICA8Y2lyY2xlIGN4PSIxMiIgY3k9IjEyIiByPSI4IiBmaWxsPSJibGFjayIvPgogIDwvbWFzaz4KCiAgPGcgY2xhc3M9ImpwLWljb24zIiBmaWxsPSIjNjE2MTYxIj4KICAgIDxyZWN0IGhlaWdodD0iMTgiIHdpZHRoPSIyIiB4PSIxMSIgeT0iMyIgdHJhbnNmb3JtPSJyb3RhdGUoMzE1LCAxMiwgMTIpIi8+CiAgICA8Y2lyY2xlIGN4PSIxMiIgY3k9IjEyIiByPSIxMCIgbWFzaz0idXJsKCNkb251dEhvbGUpIi8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-close: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbi1ub25lIGpwLWljb24tc2VsZWN0YWJsZS1pbnZlcnNlIGpwLWljb24zLWhvdmVyIiBmaWxsPSJub25lIj4KICAgIDxjaXJjbGUgY3g9IjEyIiBjeT0iMTIiIHI9IjExIi8+CiAgPC9nPgoKICA8ZyBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIGpwLWljb24tYWNjZW50Mi1ob3ZlciIgZmlsbD0iIzYxNjE2MSI+CiAgICA8cGF0aCBkPSJNMTkgNi40MUwxNy41OSA1IDEyIDEwLjU5IDYuNDEgNSA1IDYuNDEgMTAuNTkgMTIgNSAxNy41OSA2LjQxIDE5IDEyIDEzLjQxIDE3LjU5IDE5IDE5IDE3LjU5IDEzLjQxIDEyeiIvPgogIDwvZz4KCiAgPGcgY2xhc3M9ImpwLWljb24tbm9uZSBqcC1pY29uLWJ1c3kiIGZpbGw9Im5vbmUiPgogICAgPGNpcmNsZSBjeD0iMTIiIGN5PSIxMiIgcj0iNyIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-code-check: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBzaGFwZS1yZW5kZXJpbmc9Imdlb21ldHJpY1ByZWNpc2lvbiI+CiAgICA8cGF0aCBkPSJNNi41OSwzLjQxTDIsOEw2LjU5LDEyLjZMOCwxMS4xOEw0LjgyLDhMOCw0LjgyTDYuNTksMy40MU0xMi40MSwzLjQxTDExLDQuODJMMTQuMTgsOEwxMSwxMS4xOEwxMi40MSwxMi42TDE3LDhMMTIuNDEsMy40MU0yMS41OSwxMS41OUwxMy41LDE5LjY4TDkuODMsMTZMOC40MiwxNy40MUwxMy41LDIyLjVMMjMsMTNMMjEuNTksMTEuNTlaIiAvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-code: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjIiIGhlaWdodD0iMjIiIHZpZXdCb3g9IjAgMCAyOCAyOCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CgkJPHBhdGggZD0iTTExLjQgMTguNkw2LjggMTRMMTEuNCA5LjRMMTAgOEw0IDE0TDEwIDIwTDExLjQgMTguNlpNMTYuNiAxOC42TDIxLjIgMTRMMTYuNiA5LjRMMTggOEwyNCAxNEwxOCAyMEwxNi42IDE4LjZWMTguNloiLz4KCTwvZz4KPC9zdmc+Cg==);
  --jp-icon-collapse-all: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGgKICAgICAgICAgICAgZD0iTTggMmMxIDAgMTEgMCAxMiAwczIgMSAyIDJjMCAxIDAgMTEgMCAxMnMwIDItMiAyQzIwIDE0IDIwIDQgMjAgNFMxMCA0IDYgNGMwLTIgMS0yIDItMnoiIC8+CiAgICAgICAgPHBhdGgKICAgICAgICAgICAgZD0iTTE4IDhjMC0xLTEtMi0yLTJTNSA2IDQgNnMtMiAxLTIgMmMwIDEgMCAxMSAwIDEyczEgMiAyIDJjMSAwIDExIDAgMTIgMHMyLTEgMi0yYzAtMSAwLTExIDAtMTJ6bS0yIDB2MTJINFY4eiIgLz4KICAgICAgICA8cGF0aCBkPSJNNiAxM3YyaDh2LTJ6IiAvPgogICAgPC9nPgo8L3N2Zz4K);
  --jp-icon-console: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIwMCAyMDAiPgogIDxnIGNsYXNzPSJqcC1jb25zb2xlLWljb24tYmFja2dyb3VuZC1jb2xvciBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiMwMjg4RDEiPgogICAgPHBhdGggZD0iTTIwIDE5LjhoMTYwdjE1OS45SDIweiIvPgogIDwvZz4KICA8ZyBjbGFzcz0ianAtY29uc29sZS1pY29uLWNvbG9yIGpwLWljb24tc2VsZWN0YWJsZS1pbnZlcnNlIiBmaWxsPSIjZmZmIj4KICAgIDxwYXRoIGQ9Ik0xMDUgMTI3LjNoNDB2MTIuOGgtNDB6TTUxLjEgNzdMNzQgOTkuOWwtMjMuMyAyMy4zIDEwLjUgMTAuNSAyMy4zLTIzLjNMOTUgOTkuOSA4NC41IDg5LjQgNjEuNiA2Ni41eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-copy: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMTggMTgiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTExLjksMUgzLjJDMi40LDEsMS43LDEuNywxLjcsMi41djEwLjJoMS41VjIuNWg4LjdWMXogTTE0LjEsMy45aC04Yy0wLjgsMC0xLjUsMC43LTEuNSwxLjV2MTAuMmMwLDAuOCwwLjcsMS41LDEuNSwxLjVoOCBjMC44LDAsMS41LTAuNywxLjUtMS41VjUuNEMxNS41LDQuNiwxNC45LDMuOSwxNC4xLDMuOXogTTE0LjEsMTUuNWgtOFY1LjRoOFYxNS41eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-copyright: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIGVuYWJsZS1iYWNrZ3JvdW5kPSJuZXcgMCAwIDI0IDI0IiBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCI+CiAgPGcgY2xhc3M9ImpwLWljb24zIiBmaWxsPSIjNjE2MTYxIj4KICAgIDxwYXRoIGQ9Ik0xMS44OCw5LjE0YzEuMjgsMC4wNiwxLjYxLDEuMTUsMS42MywxLjY2aDEuNzljLTAuMDgtMS45OC0xLjQ5LTMuMTktMy40NS0zLjE5QzkuNjQsNy42MSw4LDksOCwxMi4xNCBjMCwxLjk0LDAuOTMsNC4yNCwzLjg0LDQuMjRjMi4yMiwwLDMuNDEtMS42NSwzLjQ0LTIuOTVoLTEuNzljLTAuMDMsMC41OS0wLjQ1LDEuMzgtMS42MywxLjQ0QzEwLjU1LDE0LjgzLDEwLDEzLjgxLDEwLDEyLjE0IEMxMCw5LjI1LDExLjI4LDkuMTYsMTEuODgsOS4xNHogTTEyLDJDNi40OCwyLDIsNi40OCwyLDEyczQuNDgsMTAsMTAsMTBzMTAtNC40OCwxMC0xMFMxNy41MiwyLDEyLDJ6IE0xMiwyMGMtNC40MSwwLTgtMy41OS04LTggczMuNTktOCw4LThzOCwzLjU5LDgsOFMxNi40MSwyMCwxMiwyMHoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-cut: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTkuNjQgNy42NGMuMjMtLjUuMzYtMS4wNS4zNi0xLjY0IDAtMi4yMS0xLjc5LTQtNC00UzIgMy43OSAyIDZzMS43OSA0IDQgNGMuNTkgMCAxLjE0LS4xMyAxLjY0LS4zNkwxMCAxMmwtMi4zNiAyLjM2QzcuMTQgMTQuMTMgNi41OSAxNCA2IDE0Yy0yLjIxIDAtNCAxLjc5LTQgNHMxLjc5IDQgNCA0IDQtMS43OSA0LTRjMC0uNTktLjEzLTEuMTQtLjM2LTEuNjRMMTIgMTRsNyA3aDN2LTFMOS42NCA3LjY0ek02IDhjLTEuMSAwLTItLjg5LTItMnMuOS0yIDItMiAyIC44OSAyIDItLjkgMi0yIDJ6bTAgMTJjLTEuMSAwLTItLjg5LTItMnMuOS0yIDItMiAyIC44OSAyIDItLjkgMi0yIDJ6bTYtNy41Yy0uMjggMC0uNS0uMjItLjUtLjVzLjIyLS41LjUtLjUuNS4yMi41LjUtLjIyLjUtLjUuNXpNMTkgM2wtNiA2IDIgMiA3LTdWM3oiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-delete: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgd2lkdGg9IjE2cHgiIGhlaWdodD0iMTZweCI+CiAgICA8cGF0aCBkPSJNMCAwaDI0djI0SDB6IiBmaWxsPSJub25lIiAvPgogICAgPHBhdGggY2xhc3M9ImpwLWljb24zIiBmaWxsPSIjNjI2MjYyIiBkPSJNNiAxOWMwIDEuMS45IDIgMiAyaDhjMS4xIDAgMi0uOSAyLTJWN0g2djEyek0xOSA0aC0zLjVsLTEtMWgtNWwtMSAxSDV2MmgxNFY0eiIgLz4KPC9zdmc+Cg==);
  --jp-icon-download: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTE5IDloLTRWM0g5djZINWw3IDcgNy03ek01IDE4djJoMTR2LTJINXoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-duplicate: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTQiIGhlaWdodD0iMTQiIHZpZXdCb3g9IjAgMCAxNCAxNCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPHBhdGggY2xhc3M9ImpwLWljb24zIiBmaWxsLXJ1bGU9ImV2ZW5vZGQiIGNsaXAtcnVsZT0iZXZlbm9kZCIgZD0iTTIuNzk5OTggMC44NzVIOC44OTU4MkM5LjIwMDYxIDAuODc1IDkuNDQ5OTggMS4xMzkxNCA5LjQ0OTk4IDEuNDYxOThDOS40NDk5OCAxLjc4NDgyIDkuMjAwNjEgMi4wNDg5NiA4Ljg5NTgyIDIuMDQ4OTZIMy4zNTQxNUMzLjA0OTM2IDIuMDQ4OTYgMi43OTk5OCAyLjMxMzEgMi43OTk5OCAyLjYzNTk0VjkuNjc5NjlDMi43OTk5OCAxMC4wMDI1IDIuNTUwNjEgMTAuMjY2NyAyLjI0NTgyIDEwLjI2NjdDMS45NDEwMyAxMC4yNjY3IDEuNjkxNjUgMTAuMDAyNSAxLjY5MTY1IDkuNjc5NjlWMi4wNDg5NkMxLjY5MTY1IDEuNDAzMjggMi4xOTA0IDAuODc1IDIuNzk5OTggMC44NzVaTTUuMzY2NjUgMTEuOVY0LjU1SDExLjA4MzNWMTEuOUg1LjM2NjY1Wk00LjE0MTY1IDQuMTQxNjdDNC4xNDE2NSAzLjY5MDYzIDQuNTA3MjggMy4zMjUgNC45NTgzMiAzLjMyNUgxMS40OTE3QzExLjk0MjcgMy4zMjUgMTIuMzA4MyAzLjY5MDYzIDEyLjMwODMgNC4xNDE2N1YxMi4zMDgzQzEyLjMwODMgMTIuNzU5NCAxMS45NDI3IDEzLjEyNSAxMS40OTE3IDEzLjEyNUg0Ljk1ODMyQzQuNTA3MjggMTMuMTI1IDQuMTQxNjUgMTIuNzU5NCA0LjE0MTY1IDEyLjMwODNWNC4xNDE2N1oiIGZpbGw9IiM2MTYxNjEiLz4KPHBhdGggY2xhc3M9ImpwLWljb24zIiBkPSJNOS40MzU3NCA4LjI2NTA3SDguMzY0MzFWOS4zMzY1QzguMzY0MzEgOS40NTQzNSA4LjI2Nzg4IDkuNTUwNzggOC4xNTAwMiA5LjU1MDc4QzguMDMyMTcgOS41NTA3OCA3LjkzNTc0IDkuNDU0MzUgNy45MzU3NCA5LjMzNjVWOC4yNjUwN0g2Ljg2NDMxQzYuNzQ2NDUgOC4yNjUwNyA2LjY1MDAyIDguMTY4NjQgNi42NTAwMiA4LjA1MDc4QzYuNjUwMDIgNy45MzI5MiA2Ljc0NjQ1IDcuODM2NSA2Ljg2NDMxIDcuODM2NUg3LjkzNTc0VjYuNzY1MDdDNy45MzU3NCA2LjY0NzIxIDguMDMyMTcgNi41NTA3OCA4LjE1MDAyIDYuNTUwNzhDOC4yNjc4OCA2LjU1MDc4IDguMzY0MzEgNi42NDcyMSA4LjM2NDMxIDYuNzY1MDdWNy44MzY1SDkuNDM1NzRDOS41NTM2IDcuODM2NSA5LjY1MDAyIDcuOTMyOTIgOS42NTAwMiA4LjA1MDc4QzkuNjUwMDIgOC4xNjg2NCA5LjU1MzYgOC4yNjUwNyA5LjQzNTc0IDguMjY1MDdaIiBmaWxsPSIjNjE2MTYxIiBzdHJva2U9IiM2MTYxNjEiIHN0cm9rZS13aWR0aD0iMC41Ii8+Cjwvc3ZnPgo=);
  --jp-icon-edit: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTMgMTcuMjVWMjFoMy43NUwxNy44MSA5Ljk0bC0zLjc1LTMuNzVMMyAxNy4yNXpNMjAuNzEgNy4wNGMuMzktLjM5LjM5LTEuMDIgMC0xLjQxbC0yLjM0LTIuMzRjLS4zOS0uMzktMS4wMi0uMzktMS40MSAwbC0xLjgzIDEuODMgMy43NSAzLjc1IDEuODMtMS44M3oiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-ellipses: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPGNpcmNsZSBjeD0iNSIgY3k9IjEyIiByPSIyIi8+CiAgICA8Y2lyY2xlIGN4PSIxMiIgY3k9IjEyIiByPSIyIi8+CiAgICA8Y2lyY2xlIGN4PSIxOSIgY3k9IjEyIiByPSIyIi8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-error: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KPGcgY2xhc3M9ImpwLWljb24zIiBmaWxsPSIjNjE2MTYxIj48Y2lyY2xlIGN4PSIxMiIgY3k9IjE5IiByPSIyIi8+PHBhdGggZD0iTTEwIDNoNHYxMmgtNHoiLz48L2c+CjxwYXRoIGZpbGw9Im5vbmUiIGQ9Ik0wIDBoMjR2MjRIMHoiLz4KPC9zdmc+Cg==);
  --jp-icon-expand-all: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGgKICAgICAgICAgICAgZD0iTTggMmMxIDAgMTEgMCAxMiAwczIgMSAyIDJjMCAxIDAgMTEgMCAxMnMwIDItMiAyQzIwIDE0IDIwIDQgMjAgNFMxMCA0IDYgNGMwLTIgMS0yIDItMnoiIC8+CiAgICAgICAgPHBhdGgKICAgICAgICAgICAgZD0iTTE4IDhjMC0xLTEtMi0yLTJTNSA2IDQgNnMtMiAxLTIgMmMwIDEgMCAxMSAwIDEyczEgMiAyIDJjMSAwIDExIDAgMTIgMHMyLTEgMi0yYzAtMSAwLTExIDAtMTJ6bS0yIDB2MTJINFY4eiIgLz4KICAgICAgICA8cGF0aCBkPSJNMTEgMTBIOXYzSDZ2MmgzdjNoMnYtM2gzdi0yaC0zeiIgLz4KICAgIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-extension: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTIwLjUgMTFIMTlWN2MwLTEuMS0uOS0yLTItMmgtNFYzLjVDMTMgMi4xMiAxMS44OCAxIDEwLjUgMVM4IDIuMTIgOCAzLjVWNUg0Yy0xLjEgMC0xLjk5LjktMS45OSAydjMuOEgzLjVjMS40OSAwIDIuNyAxLjIxIDIuNyAyLjdzLTEuMjEgMi43LTIuNyAyLjdIMlYyMGMwIDEuMS45IDIgMiAyaDMuOHYtMS41YzAtMS40OSAxLjIxLTIuNyAyLjctMi43IDEuNDkgMCAyLjcgMS4yMSAyLjcgMi43VjIySDE3YzEuMSAwIDItLjkgMi0ydi00aDEuNWMxLjM4IDAgMi41LTEuMTIgMi41LTIuNVMyMS44OCAxMSAyMC41IDExeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-fast-forward: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTQgMThsOC41LTZMNCA2djEyem05LTEydjEybDguNS02TDEzIDZ6Ii8+CiAgICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-file-upload: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTkgMTZoNnYtNmg0bC03LTctNyA3aDR6bS00IDJoMTR2Mkg1eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-file: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMTkuMyA4LjJsLTUuNS01LjVjLS4zLS4zLS43LS41LTEuMi0uNUgzLjljLS44LjEtMS42LjktMS42IDEuOHYxNC4xYzAgLjkuNyAxLjYgMS42IDEuNmgxNC4yYy45IDAgMS42LS43IDEuNi0xLjZWOS40Yy4xLS41LS4xLS45LS40LTEuMnptLTUuOC0zLjNsMy40IDMuNmgtMy40VjQuOXptMy45IDEyLjdINC43Yy0uMSAwLS4yIDAtLjItLjJWNC43YzAtLjIuMS0uMy4yLS4zaDcuMnY0LjRzMCAuOC4zIDEuMWMuMy4zIDEuMS4zIDEuMS4zaDQuM3Y3LjJzLS4xLjItLjIuMnoiLz4KPC9zdmc+Cg==);
  --jp-icon-filter-dot: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiNGRkYiPgogICAgPHBhdGggZD0iTTE0LDEyVjE5Ljg4QzE0LjA0LDIwLjE4IDEzLjk0LDIwLjUgMTMuNzEsMjAuNzFDMTMuMzIsMjEuMSAxMi42OSwyMS4xIDEyLjMsMjAuNzFMMTAuMjksMTguN0MxMC4wNiwxOC40NyA5Ljk2LDE4LjE2IDEwLDE3Ljg3VjEySDkuOTdMNC4yMSw0LjYyQzMuODcsNC4xOSAzLjk1LDMuNTYgNC4zOCwzLjIyQzQuNTcsMy4wOCA0Ljc4LDMgNSwzVjNIMTlWM0MxOS4yMiwzIDE5LjQzLDMuMDggMTkuNjIsMy4yMkMyMC4wNSwzLjU2IDIwLjEzLDQuMTkgMTkuNzksNC42MkwxNC4wMywxMkgxNFoiIC8+CiAgPC9nPgogIDxnIGNsYXNzPSJqcC1pY29uLWRvdCIgZmlsbD0iI0ZGRiI+CiAgICA8Y2lyY2xlIGN4PSIxOCIgY3k9IjE3IiByPSIzIj48L2NpcmNsZT4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-filter-list: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTEwIDE4aDR2LTJoLTR2MnpNMyA2djJoMThWNkgzem0zIDdoMTJ2LTJINnYyeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-filter: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiNGRkYiPgogICAgPHBhdGggZD0iTTE0LDEyVjE5Ljg4QzE0LjA0LDIwLjE4IDEzLjk0LDIwLjUgMTMuNzEsMjAuNzFDMTMuMzIsMjEuMSAxMi42OSwyMS4xIDEyLjMsMjAuNzFMMTAuMjksMTguN0MxMC4wNiwxOC40NyA5Ljk2LDE4LjE2IDEwLDE3Ljg3VjEySDkuOTdMNC4yMSw0LjYyQzMuODcsNC4xOSAzLjk1LDMuNTYgNC4zOCwzLjIyQzQuNTcsMy4wOCA0Ljc4LDMgNSwzVjNIMTlWM0MxOS4yMiwzIDE5LjQzLDMuMDggMTkuNjIsMy4yMkMyMC4wNSwzLjU2IDIwLjEzLDQuMTkgMTkuNzksNC42MkwxNC4wMywxMkgxNFoiIC8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-folder-favorite: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIGhlaWdodD0iMjRweCIgdmlld0JveD0iMCAwIDI0IDI0IiB3aWR0aD0iMjRweCIgZmlsbD0iIzAwMDAwMCI+CiAgPHBhdGggZD0iTTAgMGgyNHYyNEgwVjB6IiBmaWxsPSJub25lIi8+PHBhdGggY2xhc3M9ImpwLWljb24zIGpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iIzYxNjE2MSIgZD0iTTIwIDZoLThsLTItMkg0Yy0xLjEgMC0yIC45LTIgMnYxMmMwIDEuMS45IDIgMiAyaDE2YzEuMSAwIDItLjkgMi0yVjhjMC0xLjEtLjktMi0yLTJ6bS0yLjA2IDExTDE1IDE1LjI4IDEyLjA2IDE3bC43OC0zLjMzLTIuNTktMi4yNCAzLjQxLS4yOUwxNSA4bDEuMzQgMy4xNCAzLjQxLjI5LTIuNTkgMi4yNC43OCAzLjMzeiIvPgo8L3N2Zz4K);
  --jp-icon-folder: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMTAgNEg0Yy0xLjEgMC0xLjk5LjktMS45OSAyTDIgMThjMCAxLjEuOSAyIDIgMmgxNmMxLjEgMCAyLS45IDItMlY4YzAtMS4xLS45LTItMi0yaC04bC0yLTJ6Ii8+Cjwvc3ZnPgo=);
  --jp-icon-home: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIGhlaWdodD0iMjRweCIgdmlld0JveD0iMCAwIDI0IDI0IiB3aWR0aD0iMjRweCIgZmlsbD0iIzAwMDAwMCI+CiAgPHBhdGggZD0iTTAgMGgyNHYyNEgweiIgZmlsbD0ibm9uZSIvPjxwYXRoIGNsYXNzPSJqcC1pY29uMyBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiM2MTYxNjEiIGQ9Ik0xMCAyMHYtNmg0djZoNXYtOGgzTDEyIDMgMiAxMmgzdjh6Ii8+Cjwvc3ZnPgo=);
  --jp-icon-html5: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDUxMiA1MTIiPgogIDxwYXRoIGNsYXNzPSJqcC1pY29uMCBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiMwMDAiIGQ9Ik0xMDguNCAwaDIzdjIyLjhoMjEuMlYwaDIzdjY5aC0yM1Y0NmgtMjF2MjNoLTIzLjJNMjA2IDIzaC0yMC4zVjBoNjMuN3YyM0gyMjl2NDZoLTIzbTUzLjUtNjloMjQuMWwxNC44IDI0LjNMMzEzLjIgMGgyNC4xdjY5aC0yM1YzNC44bC0xNi4xIDI0LjgtMTYuMS0yNC44VjY5aC0yMi42bTg5LjItNjloMjN2NDYuMmgzMi42VjY5aC01NS42Ii8+CiAgPHBhdGggY2xhc3M9ImpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iI2U0NGQyNiIgZD0iTTEwNy42IDQ3MWwtMzMtMzcwLjRoMzYyLjhsLTMzIDM3MC4yTDI1NS43IDUxMiIvPgogIDxwYXRoIGNsYXNzPSJqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiNmMTY1MjkiIGQ9Ik0yNTYgNDgwLjVWMTMxaDE0OC4zTDM3NiA0NDciLz4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1zZWxlY3RhYmxlLWludmVyc2UiIGZpbGw9IiNlYmViZWIiIGQ9Ik0xNDIgMTc2LjNoMTE0djQ1LjRoLTY0LjJsNC4yIDQ2LjVoNjB2NDUuM0gxNTQuNG0yIDIyLjhIMjAybDMuMiAzNi4zIDUwLjggMTMuNnY0Ny40bC05My4yLTI2Ii8+CiAgPHBhdGggY2xhc3M9ImpwLWljb24tc2VsZWN0YWJsZS1pbnZlcnNlIiBmaWxsPSIjZmZmIiBkPSJNMzY5LjYgMTc2LjNIMjU1Ljh2NDUuNGgxMDkuNm0tNC4xIDQ2LjVIMjU1Ljh2NDUuNGg1NmwtNS4zIDU5LTUwLjcgMTMuNnY0Ny4ybDkzLTI1LjgiLz4KPC9zdmc+Cg==);
  --jp-icon-image: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1icmFuZDQganAtaWNvbi1zZWxlY3RhYmxlLWludmVyc2UiIGZpbGw9IiNGRkYiIGQ9Ik0yLjIgMi4yaDE3LjV2MTcuNUgyLjJ6Ii8+CiAgPHBhdGggY2xhc3M9ImpwLWljb24tYnJhbmQwIGpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iIzNGNTFCNSIgZD0iTTIuMiAyLjJ2MTcuNWgxNy41bC4xLTE3LjVIMi4yem0xMi4xIDIuMmMxLjIgMCAyLjIgMSAyLjIgMi4ycy0xIDIuMi0yLjIgMi4yLTIuMi0xLTIuMi0yLjIgMS0yLjIgMi4yLTIuMnpNNC40IDE3LjZsMy4zLTguOCAzLjMgNi42IDIuMi0zLjIgNC40IDUuNEg0LjR6Ii8+Cjwvc3ZnPgo=);
  --jp-icon-info: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDUwLjk3OCA1MC45NzgiPgoJPGcgY2xhc3M9ImpwLWljb24zIiBmaWxsPSIjNjE2MTYxIj4KCQk8cGF0aCBkPSJNNDMuNTIsNy40NThDMzguNzExLDIuNjQ4LDMyLjMwNywwLDI1LjQ4OSwwQzE4LjY3LDAsMTIuMjY2LDIuNjQ4LDcuNDU4LDcuNDU4CgkJCWMtOS45NDMsOS45NDEtOS45NDMsMjYuMTE5LDAsMzYuMDYyYzQuODA5LDQuODA5LDExLjIxMiw3LjQ1NiwxOC4wMzEsNy40NThjMCwwLDAuMDAxLDAsMC4wMDIsMAoJCQljNi44MTYsMCwxMy4yMjEtMi42NDgsMTguMDI5LTcuNDU4YzQuODA5LTQuODA5LDcuNDU3LTExLjIxMiw3LjQ1Ny0xOC4wM0M1MC45NzcsMTguNjcsNDguMzI4LDEyLjI2Niw0My41Miw3LjQ1OHoKCQkJIE00Mi4xMDYsNDIuMTA1Yy00LjQzMiw0LjQzMS0xMC4zMzIsNi44NzItMTYuNjE1LDYuODcyaC0wLjAwMmMtNi4yODUtMC4wMDEtMTIuMTg3LTIuNDQxLTE2LjYxNy02Ljg3MgoJCQljLTkuMTYyLTkuMTYzLTkuMTYyLTI0LjA3MSwwLTMzLjIzM0MxMy4zMDMsNC40NCwxOS4yMDQsMiwyNS40ODksMmM2LjI4NCwwLDEyLjE4NiwyLjQ0LDE2LjYxNyw2Ljg3MgoJCQljNC40MzEsNC40MzEsNi44NzEsMTAuMzMyLDYuODcxLDE2LjYxN0M0OC45NzcsMzEuNzcyLDQ2LjUzNiwzNy42NzUsNDIuMTA2LDQyLjEwNXoiLz4KCQk8cGF0aCBkPSJNMjMuNTc4LDMyLjIxOGMtMC4wMjMtMS43MzQsMC4xNDMtMy4wNTksMC40OTYtMy45NzJjMC4zNTMtMC45MTMsMS4xMS0xLjk5NywyLjI3Mi0zLjI1MwoJCQljMC40NjgtMC41MzYsMC45MjMtMS4wNjIsMS4zNjctMS41NzVjMC42MjYtMC43NTMsMS4xMDQtMS40NzgsMS40MzYtMi4xNzVjMC4zMzEtMC43MDcsMC40OTUtMS41NDEsMC40OTUtMi41CgkJCWMwLTEuMDk2LTAuMjYtMi4wODgtMC43NzktMi45NzljLTAuNTY1LTAuODc5LTEuNTAxLTEuMzM2LTIuODA2LTEuMzY5Yy0xLjgwMiwwLjA1Ny0yLjk4NSwwLjY2Ny0zLjU1LDEuODMyCgkJCWMtMC4zMDEsMC41MzUtMC41MDMsMS4xNDEtMC42MDcsMS44MTRjLTAuMTM5LDAuNzA3LTAuMjA3LDEuNDMyLTAuMjA3LDIuMTc0aC0yLjkzN2MtMC4wOTEtMi4yMDgsMC40MDctNC4xMTQsMS40OTMtNS43MTkKCQkJYzEuMDYyLTEuNjQsMi44NTUtMi40ODEsNS4zNzgtMi41MjdjMi4xNiwwLjAyMywzLjg3NCwwLjYwOCw1LjE0MSwxLjc1OGMxLjI3OCwxLjE2LDEuOTI5LDIuNzY0LDEuOTUsNC44MTEKCQkJYzAsMS4xNDItMC4xMzcsMi4xMTEtMC40MSwyLjkxMWMtMC4zMDksMC44NDUtMC43MzEsMS41OTMtMS4yNjgsMi4yNDNjLTAuNDkyLDAuNjUtMS4wNjgsMS4zMTgtMS43MywyLjAwMgoJCQljLTAuNjUsMC42OTctMS4zMTMsMS40NzktMS45ODcsMi4zNDZjLTAuMjM5LDAuMzc3LTAuNDI5LDAuNzc3LTAuNTY1LDEuMTk5Yy0wLjE2LDAuOTU5LTAuMjE3LDEuOTUxLTAuMTcxLDIuOTc5CgkJCUMyNi41ODksMzIuMjE4LDIzLjU3OCwzMi4yMTgsMjMuNTc4LDMyLjIxOHogTTIzLjU3OCwzOC4yMnYtMy40ODRoMy4wNzZ2My40ODRIMjMuNTc4eiIvPgoJPC9nPgo8L3N2Zz4K);
  --jp-icon-inspector: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaW5zcGVjdG9yLWljb24tY29sb3IganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMjAgNEg0Yy0xLjEgMC0xLjk5LjktMS45OSAyTDIgMThjMCAxLjEuOSAyIDIgMmgxNmMxLjEgMCAyLS45IDItMlY2YzAtMS4xLS45LTItMi0yem0tNSAxNEg0di00aDExdjR6bTAtNUg0VjloMTF2NHptNSA1aC00VjloNHY5eiIvPgo8L3N2Zz4K);
  --jp-icon-json: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8ZyBjbGFzcz0ianAtanNvbi1pY29uLWNvbG9yIGpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iI0Y5QTgyNSI+CiAgICA8cGF0aCBkPSJNMjAuMiAxMS44Yy0xLjYgMC0xLjcuNS0xLjcgMSAwIC40LjEuOS4xIDEuMy4xLjUuMS45LjEgMS4zIDAgMS43LTEuNCAyLjMtMy41IDIuM2gtLjl2LTEuOWguNWMxLjEgMCAxLjQgMCAxLjQtLjggMC0uMyAwLS42LS4xLTEgMC0uNC0uMS0uOC0uMS0xLjIgMC0xLjMgMC0xLjggMS4zLTItMS4zLS4yLTEuMy0uNy0xLjMtMiAwLS40LjEtLjguMS0xLjIuMS0uNC4xLS43LjEtMSAwLS44LS40LS43LTEuNC0uOGgtLjVWNC4xaC45YzIuMiAwIDMuNS43IDMuNSAyLjMgMCAuNC0uMS45LS4xIDEuMy0uMS41LS4xLjktLjEgMS4zIDAgLjUuMiAxIDEuNyAxdjEuOHpNMS44IDEwLjFjMS42IDAgMS43LS41IDEuNy0xIDAtLjQtLjEtLjktLjEtMS4zLS4xLS41LS4xLS45LS4xLTEuMyAwLTEuNiAxLjQtMi4zIDMuNS0yLjNoLjl2MS45aC0uNWMtMSAwLTEuNCAwLTEuNC44IDAgLjMgMCAuNi4xIDEgMCAuMi4xLjYuMSAxIDAgMS4zIDAgMS44LTEuMyAyQzYgMTEuMiA2IDExLjcgNiAxM2MwIC40LS4xLjgtLjEgMS4yLS4xLjMtLjEuNy0uMSAxIDAgLjguMy44IDEuNC44aC41djEuOWgtLjljLTIuMSAwLTMuNS0uNi0zLjUtMi4zIDAtLjQuMS0uOS4xLTEuMy4xLS41LjEtLjkuMS0xLjMgMC0uNS0uMi0xLTEuNy0xdi0xLjl6Ii8+CiAgICA8Y2lyY2xlIGN4PSIxMSIgY3k9IjEzLjgiIHI9IjIuMSIvPgogICAgPGNpcmNsZSBjeD0iMTEiIGN5PSI4LjIiIHI9IjIuMSIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-julia: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDMyNSAzMDAiPgogIDxnIGNsYXNzPSJqcC1icmFuZDAganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjY2IzYzMzIj4KICAgIDxwYXRoIGQ9Ik0gMTUwLjg5ODQzOCAyMjUgQyAxNTAuODk4NDM4IDI2Ni40MjE4NzUgMTE3LjMyMDMxMiAzMDAgNzUuODk4NDM4IDMwMCBDIDM0LjQ3NjU2MiAzMDAgMC44OTg0MzggMjY2LjQyMTg3NSAwLjg5ODQzOCAyMjUgQyAwLjg5ODQzOCAxODMuNTc4MTI1IDM0LjQ3NjU2MiAxNTAgNzUuODk4NDM4IDE1MCBDIDExNy4zMjAzMTIgMTUwIDE1MC44OTg0MzggMTgzLjU3ODEyNSAxNTAuODk4NDM4IDIyNSIvPgogIDwvZz4KICA8ZyBjbGFzcz0ianAtYnJhbmQwIGpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iIzM4OTgyNiI+CiAgICA8cGF0aCBkPSJNIDIzNy41IDc1IEMgMjM3LjUgMTE2LjQyMTg3NSAyMDMuOTIxODc1IDE1MCAxNjIuNSAxNTAgQyAxMjEuMDc4MTI1IDE1MCA4Ny41IDExNi40MjE4NzUgODcuNSA3NSBDIDg3LjUgMzMuNTc4MTI1IDEyMS4wNzgxMjUgMCAxNjIuNSAwIEMgMjAzLjkyMTg3NSAwIDIzNy41IDMzLjU3ODEyNSAyMzcuNSA3NSIvPgogIDwvZz4KICA8ZyBjbGFzcz0ianAtYnJhbmQwIGpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iIzk1NThiMiI+CiAgICA8cGF0aCBkPSJNIDMyNC4xMDE1NjIgMjI1IEMgMzI0LjEwMTU2MiAyNjYuNDIxODc1IDI5MC41MjM0MzggMzAwIDI0OS4xMDE1NjIgMzAwIEMgMjA3LjY3OTY4OCAzMDAgMTc0LjEwMTU2MiAyNjYuNDIxODc1IDE3NC4xMDE1NjIgMjI1IEMgMTc0LjEwMTU2MiAxODMuNTc4MTI1IDIwNy42Nzk2ODggMTUwIDI0OS4xMDE1NjIgMTUwIEMgMjkwLjUyMzQzOCAxNTAgMzI0LjEwMTU2MiAxODMuNTc4MTI1IDMyNC4xMDE1NjIgMjI1Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-jupyter-favicon: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTUyIiBoZWlnaHQ9IjE2NSIgdmlld0JveD0iMCAwIDE1MiAxNjUiIHZlcnNpb249IjEuMSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgPGcgY2xhc3M9ImpwLWp1cHl0ZXItaWNvbi1jb2xvciIgZmlsbD0iI0YzNzcyNiI+CiAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgwLjA3ODk0NywgMTEwLjU4MjkyNykiIGQ9Ik03NS45NDIyODQyLDI5LjU4MDQ1NjEgQzQzLjMwMjM5NDcsMjkuNTgwNDU2MSAxNC43OTY3ODMyLDE3LjY1MzQ2MzQgMCwwIEM1LjUxMDgzMjExLDE1Ljg0MDY4MjkgMTUuNzgxNTM4OSwyOS41NjY3NzMyIDI5LjM5MDQ5NDcsMzkuMjc4NDE3MSBDNDIuOTk5Nyw0OC45ODk4NTM3IDU5LjI3MzcsNTQuMjA2NzgwNSA3NS45NjA1Nzg5LDU0LjIwNjc4MDUgQzkyLjY0NzQ1NzksNTQuMjA2NzgwNSAxMDguOTIxNDU4LDQ4Ljk4OTg1MzcgMTIyLjUzMDY2MywzOS4yNzg0MTcxIEMxMzYuMTM5NDUzLDI5LjU2Njc3MzIgMTQ2LjQxMDI4NCwxNS44NDA2ODI5IDE1MS45MjExNTgsMCBDMTM3LjA4Nzg2OCwxNy42NTM0NjM0IDEwOC41ODI1ODksMjkuNTgwNDU2MSA3NS45NDIyODQyLDI5LjU4MDQ1NjEgTDc1Ljk0MjI4NDIsMjkuNTgwNDU2MSBaIiAvPgogICAgPHBhdGggdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMC4wMzczNjgsIDAuNzA0ODc4KSIgZD0iTTc1Ljk3ODQ1NzksMjQuNjI2NDA3MyBDMTA4LjYxODc2MywyNC42MjY0MDczIDEzNy4xMjQ0NTgsMzYuNTUzNDQxNSAxNTEuOTIxMTU4LDU0LjIwNjc4MDUgQzE0Ni40MTAyODQsMzguMzY2MjIyIDEzNi4xMzk0NTMsMjQuNjQwMTMxNyAxMjIuNTMwNjYzLDE0LjkyODQ4NzggQzEwOC45MjE0NTgsNS4yMTY4NDM5IDkyLjY0NzQ1NzksMCA3NS45NjA1Nzg5LDAgQzU5LjI3MzcsMCA0Mi45OTk3LDUuMjE2ODQzOSAyOS4zOTA0OTQ3LDE0LjkyODQ4NzggQzE1Ljc4MTUzODksMjQuNjQwMTMxNyA1LjUxMDgzMjExLDM4LjM2NjIyMiAwLDU0LjIwNjc4MDUgQzE0LjgzMzA4MTYsMzYuNTg5OTI5MyA0My4zMzg1Njg0LDI0LjYyNjQwNzMgNzUuOTc4NDU3OSwyNC42MjY0MDczIEw3NS45Nzg0NTc5LDI0LjYyNjQwNzMgWiIgLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-jupyter: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMzkiIGhlaWdodD0iNTEiIHZpZXdCb3g9IjAgMCAzOSA1MSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSgtMTYzOCAtMjI4MSkiPgogICAgIDxnIGNsYXNzPSJqcC1qdXB5dGVyLWljb24tY29sb3IiIGZpbGw9IiNGMzc3MjYiPgogICAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxNjM5Ljc0IDIzMTEuOTgpIiBkPSJNIDE4LjI2NDYgNy4xMzQxMUMgMTAuNDE0NSA3LjEzNDExIDMuNTU4NzIgNC4yNTc2IDAgMEMgMS4zMjUzOSAzLjgyMDQgMy43OTU1NiA3LjEzMDgxIDcuMDY4NiA5LjQ3MzAzQyAxMC4zNDE3IDExLjgxNTIgMTQuMjU1NyAxMy4wNzM0IDE4LjI2OSAxMy4wNzM0QyAyMi4yODIzIDEzLjA3MzQgMjYuMTk2MyAxMS44MTUyIDI5LjQ2OTQgOS40NzMwM0MgMzIuNzQyNCA3LjEzMDgxIDM1LjIxMjYgMy44MjA0IDM2LjUzOCAwQyAzMi45NzA1IDQuMjU3NiAyNi4xMTQ4IDcuMTM0MTEgMTguMjY0NiA3LjEzNDExWiIvPgogICAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxNjM5LjczIDIyODUuNDgpIiBkPSJNIDE4LjI3MzMgNS45MzkzMUMgMjYuMTIzNSA1LjkzOTMxIDMyLjk3OTMgOC44MTU4MyAzNi41MzggMTMuMDczNEMgMzUuMjEyNiA5LjI1MzAzIDMyLjc0MjQgNS45NDI2MiAyOS40Njk0IDMuNjAwNEMgMjYuMTk2MyAxLjI1ODE4IDIyLjI4MjMgMCAxOC4yNjkgMEMgMTQuMjU1NyAwIDEwLjM0MTcgMS4yNTgxOCA3LjA2ODYgMy42MDA0QyAzLjc5NTU2IDUuOTQyNjIgMS4zMjUzOSA5LjI1MzAzIDAgMTMuMDczNEMgMy41Njc0NSA4LjgyNDYzIDEwLjQyMzIgNS45MzkzMSAxOC4yNzMzIDUuOTM5MzFaIi8+CiAgICA8L2c+CiAgICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxNjY5LjMgMjI4MS4zMSkiIGQ9Ik0gNS44OTM1MyAyLjg0NEMgNS45MTg4OSAzLjQzMTY1IDUuNzcwODUgNC4wMTM2NyA1LjQ2ODE1IDQuNTE2NDVDIDUuMTY1NDUgNS4wMTkyMiA0LjcyMTY4IDUuNDIwMTUgNC4xOTI5OSA1LjY2ODUxQyAzLjY2NDMgNS45MTY4OCAzLjA3NDQ0IDYuMDAxNTEgMi40OTgwNSA1LjkxMTcxQyAxLjkyMTY2IDUuODIxOSAxLjM4NDYzIDUuNTYxNyAwLjk1NDg5OCA1LjE2NDAxQyAwLjUyNTE3IDQuNzY2MzMgMC4yMjIwNTYgNC4yNDkwMyAwLjA4MzkwMzcgMy42Nzc1N0MgLTAuMDU0MjQ4MyAzLjEwNjExIC0wLjAyMTIzIDIuNTA2MTcgMC4xNzg3ODEgMS45NTM2NEMgMC4zNzg3OTMgMS40MDExIDAuNzM2ODA5IDAuOTIwODE3IDEuMjA3NTQgMC41NzM1MzhDIDEuNjc4MjYgMC4yMjYyNTkgMi4yNDA1NSAwLjAyNzU5MTkgMi44MjMyNiAwLjAwMjY3MjI5QyAzLjYwMzg5IC0wLjAzMDcxMTUgNC4zNjU3MyAwLjI0OTc4OSA0Ljk0MTQyIDAuNzgyNTUxQyA1LjUxNzExIDEuMzE1MzEgNS44NTk1NiAyLjA1Njc2IDUuODkzNTMgMi44NDRaIi8+CiAgICAgIDxwYXRoIHRyYW5zZm9ybT0idHJhbnNsYXRlKDE2MzkuOCAyMzIzLjgxKSIgZD0iTSA3LjQyNzg5IDMuNTgzMzhDIDcuNDYwMDggNC4zMjQzIDcuMjczNTUgNS4wNTgxOSA2Ljg5MTkzIDUuNjkyMTNDIDYuNTEwMzEgNi4zMjYwNyA1Ljk1MDc1IDYuODMxNTYgNS4yODQxMSA3LjE0NDZDIDQuNjE3NDcgNy40NTc2MyAzLjg3MzcxIDcuNTY0MTQgMy4xNDcwMiA3LjQ1MDYzQyAyLjQyMDMyIDcuMzM3MTIgMS43NDMzNiA3LjAwODcgMS4yMDE4NCA2LjUwNjk1QyAwLjY2MDMyOCA2LjAwNTIgMC4yNzg2MSA1LjM1MjY4IDAuMTA1MDE3IDQuNjMyMDJDIC0wLjA2ODU3NTcgMy45MTEzNSAtMC4wMjYyMzYxIDMuMTU0OTQgMC4yMjY2NzUgMi40NTg1NkMgMC40Nzk1ODcgMS43NjIxNyAwLjkzMTY5NyAxLjE1NzEzIDEuNTI1NzYgMC43MjAwMzNDIDIuMTE5ODMgMC4yODI5MzUgMi44MjkxNCAwLjAzMzQzOTUgMy41NjM4OSAwLjAwMzEzMzQ0QyA0LjU0NjY3IC0wLjAzNzQwMzMgNS41MDUyOSAwLjMxNjcwNiA2LjIyOTYxIDAuOTg3ODM1QyA2Ljk1MzkzIDEuNjU4OTYgNy4zODQ4NCAyLjU5MjM1IDcuNDI3ODkgMy41ODMzOEwgNy40Mjc4OSAzLjU4MzM4WiIvPgogICAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxNjM4LjM2IDIyODYuMDYpIiBkPSJNIDIuMjc0NzEgNC4zOTYyOUMgMS44NDM2MyA0LjQxNTA4IDEuNDE2NzEgNC4zMDQ0NSAxLjA0Nzk5IDQuMDc4NDNDIDAuNjc5MjY4IDMuODUyNCAwLjM4NTMyOCAzLjUyMTE0IDAuMjAzMzcxIDMuMTI2NTZDIDAuMDIxNDEzNiAyLjczMTk4IC0wLjA0MDM3OTggMi4yOTE4MyAwLjAyNTgxMTYgMS44NjE4MUMgMC4wOTIwMDMxIDEuNDMxOCAwLjI4MzIwNCAxLjAzMTI2IDAuNTc1MjEzIDAuNzEwODgzQyAwLjg2NzIyMiAwLjM5MDUxIDEuMjQ2OTEgMC4xNjQ3MDggMS42NjYyMiAwLjA2MjA1OTJDIDIuMDg1NTMgLTAuMDQwNTg5NyAyLjUyNTYxIC0wLjAxNTQ3MTQgMi45MzA3NiAwLjEzNDIzNUMgMy4zMzU5MSAwLjI4Mzk0MSAzLjY4NzkyIDAuNTUxNTA1IDMuOTQyMjIgMC45MDMwNkMgNC4xOTY1MiAxLjI1NDYyIDQuMzQxNjkgMS42NzQzNiA0LjM1OTM1IDIuMTA5MTZDIDQuMzgyOTkgMi42OTEwNyA0LjE3Njc4IDMuMjU4NjkgMy43ODU5NyAzLjY4NzQ2QyAzLjM5NTE2IDQuMTE2MjQgMi44NTE2NiA0LjM3MTE2IDIuMjc0NzEgNC4zOTYyOUwgMi4yNzQ3MSA0LjM5NjI5WiIvPgogICAgPC9nPgogIDwvZz4+Cjwvc3ZnPgo=);
  --jp-icon-jupyterlab-wordmark: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyMDAiIHZpZXdCb3g9IjAgMCAxODYwLjggNDc1Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjIiIGZpbGw9IiM0RTRFNEUiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDQ4MC4xMzY0MDEsIDY0LjI3MTQ5MykiPgogICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMC4wMDAwMDAsIDU4Ljg3NTU2NikiPgogICAgICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSgwLjA4NzYwMywgMC4xNDAyOTQpIj4KICAgICAgICA8cGF0aCBkPSJNLTQyNi45LDE2OS44YzAsNDguNy0zLjcsNjQuNy0xMy42LDc2LjRjLTEwLjgsMTAtMjUsMTUuNS0zOS43LDE1LjVsMy43LDI5IGMyMi44LDAuMyw0NC44LTcuOSw2MS45LTIzLjFjMTcuOC0xOC41LDI0LTQ0LjEsMjQtODMuM1YwSC00Mjd2MTcwLjFMLTQyNi45LDE2OS44TC00MjYuOSwxNjkuOHoiLz4KICAgICAgPC9nPgogICAgPC9nPgogICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMTU1LjA0NTI5NiwgNTYuODM3MTA0KSI+CiAgICAgIDxnIHRyYW5zZm9ybT0idHJhbnNsYXRlKDEuNTYyNDUzLCAxLjc5OTg0MikiPgogICAgICAgIDxwYXRoIGQ9Ik0tMzEyLDE0OGMwLDIxLDAsMzkuNSwxLjcsNTUuNGgtMzEuOGwtMi4xLTMzLjNoLTAuOGMtNi43LDExLjYtMTYuNCwyMS4zLTI4LDI3LjkgYy0xMS42LDYuNi0yNC44LDEwLTM4LjIsOS44Yy0zMS40LDAtNjktMTcuNy02OS04OVYwaDM2LjR2MTEyLjdjMCwzOC43LDExLjYsNjQuNyw0NC42LDY0LjdjMTAuMy0wLjIsMjAuNC0zLjUsMjguOS05LjQgYzguNS01LjksMTUuMS0xNC4zLDE4LjktMjMuOWMyLjItNi4xLDMuMy0xMi41LDMuMy0xOC45VjAuMmgzNi40VjE0OEgtMzEyTC0zMTIsMTQ4eiIvPgogICAgICA8L2c+CiAgICA8L2c+CiAgICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSgzOTAuMDEzMzIyLCA1My40Nzk2MzgpIj4KICAgICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMS43MDY0NTgsIDAuMjMxNDI1KSI+CiAgICAgICAgPHBhdGggZD0iTS00NzguNiw3MS40YzAtMjYtMC44LTQ3LTEuNy02Ni43aDMyLjdsMS43LDM0LjhoMC44YzcuMS0xMi41LDE3LjUtMjIuOCwzMC4xLTI5LjcgYzEyLjUtNywyNi43LTEwLjMsNDEtOS44YzQ4LjMsMCw4NC43LDQxLjcsODQuNywxMDMuM2MwLDczLjEtNDMuNywxMDkuMi05MSwxMDkuMmMtMTIuMSwwLjUtMjQuMi0yLjItMzUtNy44IGMtMTAuOC01LjYtMTkuOS0xMy45LTI2LjYtMjQuMmgtMC44VjI5MWgtMzZ2LTIyMEwtNDc4LjYsNzEuNEwtNDc4LjYsNzEuNHogTS00NDIuNiwxMjUuNmMwLjEsNS4xLDAuNiwxMC4xLDEuNywxNS4xIGMzLDEyLjMsOS45LDIzLjMsMTkuOCwzMS4xYzkuOSw3LjgsMjIuMSwxMi4xLDM0LjcsMTIuMWMzOC41LDAsNjAuNy0zMS45LDYwLjctNzguNWMwLTQwLjctMjEuMS03NS42LTU5LjUtNzUuNiBjLTEyLjksMC40LTI1LjMsNS4xLTM1LjMsMTMuNGMtOS45LDguMy0xNi45LDE5LjctMTkuNiwzMi40Yy0xLjUsNC45LTIuMywxMC0yLjUsMTUuMVYxMjUuNkwtNDQyLjYsMTI1LjZMLTQ0Mi42LDEyNS42eiIvPgogICAgICA8L2c+CiAgICA8L2c+CiAgICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSg2MDYuNzQwNzI2LCA1Ni44MzcxMDQpIj4KICAgICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMC43NTEyMjYsIDEuOTg5Mjk5KSI+CiAgICAgICAgPHBhdGggZD0iTS00NDAuOCwwbDQzLjcsMTIwLjFjNC41LDEzLjQsOS41LDI5LjQsMTIuOCw0MS43aDAuOGMzLjctMTIuMiw3LjktMjcuNywxMi44LTQyLjQgbDM5LjctMTE5LjJoMzguNUwtMzQ2LjksMTQ1Yy0yNiw2OS43LTQzLjcsMTA1LjQtNjguNiwxMjcuMmMtMTIuNSwxMS43LTI3LjksMjAtNDQuNiwyMy45bC05LjEtMzEuMSBjMTEuNy0zLjksMjIuNS0xMC4xLDMxLjgtMTguMWMxMy4yLTExLjEsMjMuNy0yNS4yLDMwLjYtNDEuMmMxLjUtMi44LDIuNS01LjcsMi45LTguOGMtMC4zLTMuMy0xLjItNi42LTIuNS05LjdMLTQ4MC4yLDAuMSBoMzkuN0wtNDQwLjgsMEwtNDQwLjgsMHoiLz4KICAgICAgPC9nPgogICAgPC9nPgogICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoODIyLjc0ODEwNCwgMC4wMDAwMDApIj4KICAgICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMS40NjQwNTAsIDAuMzc4OTE0KSI+CiAgICAgICAgPHBhdGggZD0iTS00MTMuNywwdjU4LjNoNTJ2MjguMmgtNTJWMTk2YzAsMjUsNywzOS41LDI3LjMsMzkuNWM3LjEsMC4xLDE0LjItMC43LDIxLjEtMi41IGwxLjcsMjcuN2MtMTAuMywzLjctMjEuMyw1LjQtMzIuMiw1Yy03LjMsMC40LTE0LjYtMC43LTIxLjMtMy40Yy02LjgtMi43LTEyLjktNi44LTE3LjktMTIuMWMtMTAuMy0xMC45LTE0LjEtMjktMTQuMS01Mi45IFY4Ni41aC0zMVY1OC4zaDMxVjkuNkwtNDEzLjcsMEwtNDEzLjcsMHoiLz4KICAgICAgPC9nPgogICAgPC9nPgogICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoOTc0LjQzMzI4NiwgNTMuNDc5NjM4KSI+CiAgICAgIDxnIHRyYW5zZm9ybT0idHJhbnNsYXRlKDAuOTkwMDM0LCAwLjYxMDMzOSkiPgogICAgICAgIDxwYXRoIGQ9Ik0tNDQ1LjgsMTEzYzAuOCw1MCwzMi4yLDcwLjYsNjguNiw3MC42YzE5LDAuNiwzNy45LTMsNTUuMy0xMC41bDYuMiwyNi40IGMtMjAuOSw4LjktNDMuNSwxMy4xLTY2LjIsMTIuNmMtNjEuNSwwLTk4LjMtNDEuMi05OC4zLTEwMi41Qy00ODAuMiw0OC4yLTQ0NC43LDAtMzg2LjUsMGM2NS4yLDAsODIuNyw1OC4zLDgyLjcsOTUuNyBjLTAuMSw1LjgtMC41LDExLjUtMS4yLDE3LjJoLTE0MC42SC00NDUuOEwtNDQ1LjgsMTEzeiBNLTMzOS4yLDg2LjZjMC40LTIzLjUtOS41LTYwLjEtNTAuNC02MC4xIGMtMzYuOCwwLTUyLjgsMzQuNC01NS43LDYwLjFILTMzOS4yTC0zMzkuMiw4Ni42TC0zMzkuMiw4Ni42eiIvPgogICAgICA8L2c+CiAgICA8L2c+CiAgICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxMjAxLjk2MTA1OCwgNTMuNDc5NjM4KSI+CiAgICAgIDxnIHRyYW5zZm9ybT0idHJhbnNsYXRlKDEuMTc5NjQwLCAwLjcwNTA2OCkiPgogICAgICAgIDxwYXRoIGQ9Ik0tNDc4LjYsNjhjMC0yMy45LTAuNC00NC41LTEuNy02My40aDMxLjhsMS4yLDM5LjloMS43YzkuMS0yNy4zLDMxLTQ0LjUsNTUuMy00NC41IGMzLjUtMC4xLDcsMC40LDEwLjMsMS4ydjM0LjhjLTQuMS0wLjktOC4yLTEuMy0xMi40LTEuMmMtMjUuNiwwLTQzLjcsMTkuNy00OC43LDQ3LjRjLTEsNS43LTEuNiwxMS41LTEuNywxNy4ydjEwOC4zaC0zNlY2OCBMLTQ3OC42LDY4eiIvPgogICAgICA8L2c+CiAgICA8L2c+CiAgPC9nPgoKICA8ZyBjbGFzcz0ianAtaWNvbi13YXJuMCIgZmlsbD0iI0YzNzcyNiI+CiAgICA8cGF0aCBkPSJNMTM1Mi4zLDMyNi4yaDM3VjI4aC0zN1YzMjYuMnogTTE2MDQuOCwzMjYuMmMtMi41LTEzLjktMy40LTMxLjEtMy40LTQ4Ljd2LTc2IGMwLTQwLjctMTUuMS04My4xLTc3LjMtODMuMWMtMjUuNiwwLTUwLDcuMS02Ni44LDE4LjFsOC40LDI0LjRjMTQuMy05LjIsMzQtMTUuMSw1My0xNS4xYzQxLjYsMCw0Ni4yLDMwLjIsNDYuMiw0N3Y0LjIgYy03OC42LTAuNC0xMjIuMywyNi41LTEyMi4zLDc1LjZjMCwyOS40LDIxLDU4LjQsNjIuMiw1OC40YzI5LDAsNTAuOS0xNC4zLDYyLjItMzAuMmgxLjNsMi45LDI1LjZIMTYwNC44eiBNMTU2NS43LDI1Ny43IGMwLDMuOC0wLjgsOC0yLjEsMTEuOGMtNS45LDE3LjItMjIuNywzNC00OS4yLDM0Yy0xOC45LDAtMzQuOS0xMS4zLTM0LjktMzUuM2MwLTM5LjUsNDUuOC00Ni42LDg2LjItNDUuOFYyNTcuN3ogTTE2OTguNSwzMjYuMiBsMS43LTMzLjZoMS4zYzE1LjEsMjYuOSwzOC43LDM4LjIsNjguMSwzOC4yYzQ1LjQsMCw5MS4yLTM2LjEsOTEuMi0xMDguOGMwLjQtNjEuNy0zNS4zLTEwMy43LTg1LjctMTAzLjcgYy0zMi44LDAtNTYuMywxNC43LTY5LjMsMzcuNGgtMC44VjI4aC0zNi42djI0NS43YzAsMTguMS0wLjgsMzguNi0xLjcsNTIuNUgxNjk4LjV6IE0xNzA0LjgsMjA4LjJjMC01LjksMS4zLTEwLjksMi4xLTE1LjEgYzcuNi0yOC4xLDMxLjEtNDUuNCw1Ni4zLTQ1LjRjMzkuNSwwLDYwLjUsMzQuOSw2MC41LDc1LjZjMCw0Ni42LTIzLjEsNzguMS02MS44LDc4LjFjLTI2LjksMC00OC4zLTE3LjYtNTUuNS00My4zIGMtMC44LTQuMi0xLjctOC44LTEuNy0xMy40VjIwOC4yeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-kernel: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiIgZmlsbD0iIzYxNjE2MSIgZD0iTTE1IDlIOXY2aDZWOXptLTIgNGgtMnYtMmgydjJ6bTgtMlY5aC0yVjdjMC0xLjEtLjktMi0yLTJoLTJWM2gtMnYyaC0yVjNIOXYySDdjLTEuMSAwLTIgLjktMiAydjJIM3YyaDJ2MkgzdjJoMnYyYzAgMS4xLjkgMiAyIDJoMnYyaDJ2LTJoMnYyaDJ2LTJoMmMxLjEgMCAyLS45IDItMnYtMmgydi0yaC0ydi0yaDJ6bS00IDZIN1Y3aDEwdjEweiIvPgo8L3N2Zz4K);
  --jp-icon-keyboard: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMjAgNUg0Yy0xLjEgMC0xLjk5LjktMS45OSAyTDIgMTdjMCAxLjEuOSAyIDIgMmgxNmMxLjEgMCAyLS45IDItMlY3YzAtMS4xLS45LTItMi0yem0tOSAzaDJ2MmgtMlY4em0wIDNoMnYyaC0ydi0yek04IDhoMnYySDhWOHptMCAzaDJ2Mkg4di0yem0tMSAySDV2LTJoMnYyem0wLTNINVY4aDJ2MnptOSA3SDh2LTJoOHYyem0wLTRoLTJ2LTJoMnYyem0wLTNoLTJWOGgydjJ6bTMgM2gtMnYtMmgydjJ6bTAtM2gtMlY4aDJ2MnoiLz4KPC9zdmc+Cg==);
  --jp-icon-launch: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMzIgMzIiIHdpZHRoPSIzMiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIj4KICAgIDxwYXRoIGQ9Ik0yNiwyOEg2YTIuMDAyNywyLjAwMjcsMCwwLDEtMi0yVjZBMi4wMDI3LDIuMDAyNywwLDAsMSw2LDRIMTZWNkg2VjI2SDI2VjE2aDJWMjZBMi4wMDI3LDIuMDAyNywwLDAsMSwyNiwyOFoiLz4KICAgIDxwb2x5Z29uIHBvaW50cz0iMjAgMiAyMCA0IDI2LjU4NiA0IDE4IDEyLjU4NiAxOS40MTQgMTQgMjggNS40MTQgMjggMTIgMzAgMTIgMzAgMiAyMCAyIi8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-launcher: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMTkgMTlINVY1aDdWM0g1YTIgMiAwIDAwLTIgMnYxNGEyIDIgMCAwMDIgMmgxNGMxLjEgMCAyLS45IDItMnYtN2gtMnY3ek0xNCAzdjJoMy41OWwtOS44MyA5LjgzIDEuNDEgMS40MUwxOSA2LjQxVjEwaDJWM2gtN3oiLz4KPC9zdmc+Cg==);
  --jp-icon-line-form: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxwYXRoIGZpbGw9IndoaXRlIiBkPSJNNS44OCA0LjEyTDEzLjc2IDEybC03Ljg4IDcuODhMOCAyMmwxMC0xMEw4IDJ6Ii8+Cjwvc3ZnPgo=);
  --jp-icon-link: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTMuOSAxMmMwLTEuNzEgMS4zOS0zLjEgMy4xLTMuMWg0VjdIN2MtMi43NiAwLTUgMi4yNC01IDVzMi4yNCA1IDUgNWg0di0xLjlIN2MtMS43MSAwLTMuMS0xLjM5LTMuMS0zLjF6TTggMTNoOHYtMkg4djJ6bTktNmgtNHYxLjloNGMxLjcxIDAgMy4xIDEuMzkgMy4xIDMuMXMtMS4zOSAzLjEtMy4xIDMuMWgtNFYxN2g0YzIuNzYgMCA1LTIuMjQgNS01cy0yLjI0LTUtNS01eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-list: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiM2MTYxNjEiIGQ9Ik0xOSA1djE0SDVWNWgxNG0xLjEtMkgzLjljLS41IDAtLjkuNC0uOS45djE2LjJjMCAuNC40LjkuOS45aDE2LjJjLjQgMCAuOS0uNS45LS45VjMuOWMwLS41LS41LS45LS45LS45ek0xMSA3aDZ2MmgtNlY3em0wIDRoNnYyaC02di0yem0wIDRoNnYyaC02ek03IDdoMnYySDd6bTAgNGgydjJIN3ptMCA0aDJ2Mkg3eiIvPgo8L3N2Zz4K);
  --jp-icon-markdown: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1jb250cmFzdDAganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjN0IxRkEyIiBkPSJNNSAxNC45aDEybC02LjEgNnptOS40LTYuOGMwLTEuMy0uMS0yLjktLjEtNC41LS40IDEuNC0uOSAyLjktMS4zIDQuM2wtMS4zIDQuM2gtMkw4LjUgNy45Yy0uNC0xLjMtLjctMi45LTEtNC4zLS4xIDEuNi0uMSAzLjItLjIgNC42TDcgMTIuNEg0LjhsLjctMTFoMy4zTDEwIDVjLjQgMS4yLjcgMi43IDEgMy45LjMtMS4yLjctMi42IDEtMy45bDEuMi0zLjdoMy4zbC42IDExaC0yLjRsLS4zLTQuMnoiLz4KPC9zdmc+Cg==);
  --jp-icon-move-down: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTQiIGhlaWdodD0iMTQiIHZpZXdCb3g9IjAgMCAxNCAxNCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPHBhdGggY2xhc3M9ImpwLWljb24zIiBkPSJNMTIuNDcxIDcuNTI4OTlDMTIuNzYzMiA3LjIzNjg0IDEyLjc2MzIgNi43NjMxNiAxMi40NzEgNi40NzEwMVY2LjQ3MTAxQzEyLjE3OSA2LjE3OTA1IDExLjcwNTcgNi4xNzg4NCAxMS40MTM1IDYuNDcwNTRMNy43NSAxMC4xMjc1VjEuNzVDNy43NSAxLjMzNTc5IDcuNDE0MjEgMSA3IDFWMUM2LjU4NTc5IDEgNi4yNSAxLjMzNTc5IDYuMjUgMS43NVYxMC4xMjc1TDIuNTk3MjYgNi40NjgyMkMyLjMwMzM4IDYuMTczODEgMS44MjY0MSA2LjE3MzU5IDEuNTMyMjYgNi40Njc3NFY2LjQ2Nzc0QzEuMjM4MyA2Ljc2MTcgMS4yMzgzIDcuMjM4MyAxLjUzMjI2IDcuNTMyMjZMNi4yOTI4OSAxMi4yOTI5QzYuNjgzNDIgMTIuNjgzNCA3LjMxNjU4IDEyLjY4MzQgNy43MDcxMSAxMi4yOTI5TDEyLjQ3MSA3LjUyODk5WiIgZmlsbD0iIzYxNjE2MSIvPgo8L3N2Zz4K);
  --jp-icon-move-up: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTQiIGhlaWdodD0iMTQiIHZpZXdCb3g9IjAgMCAxNCAxNCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPHBhdGggY2xhc3M9ImpwLWljb24zIiBkPSJNMS41Mjg5OSA2LjQ3MTAxQzEuMjM2ODQgNi43NjMxNiAxLjIzNjg0IDcuMjM2ODQgMS41Mjg5OSA3LjUyODk5VjcuNTI4OTlDMS44MjA5NSA3LjgyMDk1IDIuMjk0MjYgNy44MjExNiAyLjU4NjQ5IDcuNTI5NDZMNi4yNSAzLjg3MjVWMTIuMjVDNi4yNSAxMi42NjQyIDYuNTg1NzkgMTMgNyAxM1YxM0M3LjQxNDIxIDEzIDcuNzUgMTIuNjY0MiA3Ljc1IDEyLjI1VjMuODcyNUwxMS40MDI3IDcuNTMxNzhDMTEuNjk2NiA3LjgyNjE5IDEyLjE3MzYgNy44MjY0MSAxMi40Njc3IDcuNTMyMjZWNy41MzIyNkMxMi43NjE3IDcuMjM4MyAxMi43NjE3IDYuNzYxNyAxMi40Njc3IDYuNDY3NzRMNy43MDcxMSAxLjcwNzExQzcuMzE2NTggMS4zMTY1OCA2LjY4MzQyIDEuMzE2NTggNi4yOTI4OSAxLjcwNzExTDEuNTI4OTkgNi40NzEwMVoiIGZpbGw9IiM2MTYxNjEiLz4KPC9zdmc+Cg==);
  --jp-icon-new-folder: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTIwIDZoLThsLTItMkg0Yy0xLjExIDAtMS45OS44OS0xLjk5IDJMMiAxOGMwIDEuMTEuODkgMiAyIDJoMTZjMS4xMSAwIDItLjg5IDItMlY4YzAtMS4xMS0uODktMi0yLTJ6bS0xIDhoLTN2M2gtMnYtM2gtM3YtMmgzVjloMnYzaDN2MnoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-not-trusted: url(data:image/svg+xml;base64,PHN2ZyBmaWxsPSJub25lIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI1IDI1Ij4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiIgc3Ryb2tlPSIjMzMzMzMzIiBzdHJva2Utd2lkdGg9IjIiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDMgMykiIGQ9Ik0xLjg2MDk0IDExLjQ0MDlDMC44MjY0NDggOC43NzAyNyAwLjg2Mzc3OSA2LjA1NzY0IDEuMjQ5MDcgNC4xOTkzMkMyLjQ4MjA2IDMuOTMzNDcgNC4wODA2OCAzLjQwMzQ3IDUuNjAxMDIgMi44NDQ5QzcuMjM1NDkgMi4yNDQ0IDguODU2NjYgMS41ODE1IDkuOTg3NiAxLjA5NTM5QzExLjA1OTcgMS41ODM0MSAxMi42MDk0IDIuMjQ0NCAxNC4yMTggMi44NDMzOUMxNS43NTAzIDMuNDEzOTQgMTcuMzk5NSAzLjk1MjU4IDE4Ljc1MzkgNC4yMTM4NUMxOS4xMzY0IDYuMDcxNzcgMTkuMTcwOSA4Ljc3NzIyIDE4LjEzOSAxMS40NDA5QzE3LjAzMDMgMTQuMzAzMiAxNC42NjY4IDE3LjE4NDQgOS45OTk5OSAxOC45MzU0QzUuMzMzMTkgMTcuMTg0NCAyLjk2OTY4IDE0LjMwMzIgMS44NjA5NCAxMS40NDA5WiIvPgogICAgPHBhdGggY2xhc3M9ImpwLWljb24yIiBzdHJva2U9IiMzMzMzMzMiIHN0cm9rZS13aWR0aD0iMiIgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoOS4zMTU5MiA5LjMyMDMxKSIgZD0iTTcuMzY4NDIgMEwwIDcuMzY0NzkiLz4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiIgc3Ryb2tlPSIjMzMzMzMzIiBzdHJva2Utd2lkdGg9IjIiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDkuMzE1OTIgMTYuNjgzNikgc2NhbGUoMSAtMSkiIGQ9Ik03LjM2ODQyIDBMMCA3LjM2NDc5Ii8+Cjwvc3ZnPgo=);
  --jp-icon-notebook: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8ZyBjbGFzcz0ianAtbm90ZWJvb2staWNvbi1jb2xvciBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiNFRjZDMDAiPgogICAgPHBhdGggZD0iTTE4LjcgMy4zdjE1LjRIMy4zVjMuM2gxNS40bTEuNS0xLjVIMS44djE4LjNoMTguM2wuMS0xOC4zeiIvPgogICAgPHBhdGggZD0iTTE2LjUgMTYuNWwtNS40LTQuMy01LjYgNC4zdi0xMWgxMXoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-numbering: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjIiIGhlaWdodD0iMjIiIHZpZXdCb3g9IjAgMCAyOCAyOCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CgkJPHBhdGggZD0iTTQgMTlINlYxOS41SDVWMjAuNUg2VjIxSDRWMjJIN1YxOEg0VjE5Wk01IDEwSDZWNkg0VjdINVYxMFpNNCAxM0g1LjhMNCAxNS4xVjE2SDdWMTVINS4yTDcgMTIuOVYxMkg0VjEzWk05IDdWOUgyM1Y3SDlaTTkgMjFIMjNWMTlIOVYyMVpNOSAxNUgyM1YxM0g5VjE1WiIvPgoJPC9nPgo8L3N2Zz4K);
  --jp-icon-offline-bolt: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgd2lkdGg9IjE2Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTEyIDIuMDJjLTUuNTEgMC05Ljk4IDQuNDctOS45OCA5Ljk4czQuNDcgOS45OCA5Ljk4IDkuOTggOS45OC00LjQ3IDkuOTgtOS45OFMxNy41MSAyLjAyIDEyIDIuMDJ6TTExLjQ4IDIwdi02LjI2SDhMMTMgNHY2LjI2aDMuMzVMMTEuNDggMjB6Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-palette: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTE4IDEzVjIwSDRWNkg5LjAyQzkuMDcgNS4yOSA5LjI0IDQuNjIgOS41IDRINEMyLjkgNCAyIDQuOSAyIDZWMjBDMiAyMS4xIDIuOSAyMiA0IDIySDE4QzE5LjEgMjIgMjAgMjEuMSAyMCAyMFYxNUwxOCAxM1pNMTkuMyA4Ljg5QzE5Ljc0IDguMTkgMjAgNy4zOCAyMCA2LjVDMjAgNC4wMSAxNy45OSAyIDE1LjUgMkMxMy4wMSAyIDExIDQuMDEgMTEgNi41QzExIDguOTkgMTMuMDEgMTEgMTUuNDkgMTFDMTYuMzcgMTEgMTcuMTkgMTAuNzQgMTcuODggMTAuM0wyMSAxMy40MkwyMi40MiAxMkwxOS4zIDguODlaTTE1LjUgOUMxNC4xMiA5IDEzIDcuODggMTMgNi41QzEzIDUuMTIgMTQuMTIgNCAxNS41IDRDMTYuODggNCAxOCA1LjEyIDE4IDYuNUMxOCA3Ljg4IDE2Ljg4IDkgMTUuNSA5WiIvPgogICAgPHBhdGggZmlsbC1ydWxlPSJldmVub2RkIiBjbGlwLXJ1bGU9ImV2ZW5vZGQiIGQ9Ik00IDZIOS4wMTg5NEM5LjAwNjM5IDYuMTY1MDIgOSA2LjMzMTc2IDkgNi41QzkgOC44MTU3NyAxMC4yMTEgMTAuODQ4NyAxMi4wMzQzIDEySDlWMTRIMTZWMTIuOTgxMUMxNi41NzAzIDEyLjkzNzcgMTcuMTIgMTIuODIwNyAxNy42Mzk2IDEyLjYzOTZMMTggMTNWMjBINFY2Wk04IDhINlYxMEg4VjhaTTYgMTJIOFYxNEg2VjEyWk04IDE2SDZWMThIOFYxNlpNOSAxNkgxNlYxOEg5VjE2WiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-paste: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTE5IDJoLTQuMThDMTQuNC44NCAxMy4zIDAgMTIgMGMtMS4zIDAtMi40Ljg0LTIuODIgMkg1Yy0xLjEgMC0yIC45LTIgMnYxNmMwIDEuMS45IDIgMiAyaDE0YzEuMSAwIDItLjkgMi0yVjRjMC0xLjEtLjktMi0yLTJ6bS03IDBjLjU1IDAgMSAuNDUgMSAxcy0uNDUgMS0xIDEtMS0uNDUtMS0xIC40NS0xIDEtMXptNyAxOEg1VjRoMnYzaDEwVjRoMnYxNnoiLz4KICAgIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-pdf: url(data:image/svg+xml;base64,PHN2ZwogICB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyMiAyMiIgd2lkdGg9IjE2Ij4KICAgIDxwYXRoIHRyYW5zZm9ybT0icm90YXRlKDQ1KSIgY2xhc3M9ImpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iI0ZGMkEyQSIKICAgICAgIGQ9Im0gMjIuMzQ0MzY5LC0zLjAxNjM2NDIgaCA1LjYzODYwNCB2IDEuNTc5MjQzMyBoIC0zLjU0OTIyNyB2IDEuNTA4NjkyOTkgaCAzLjMzNzU3NiBWIDEuNjUwODE1NCBoIC0zLjMzNzU3NiB2IDMuNDM1MjYxMyBoIC0yLjA4OTM3NyB6IG0gLTcuMTM2NDQ0LDEuNTc5MjQzMyB2IDQuOTQzOTU0MyBoIDAuNzQ4OTIgcSAxLjI4MDc2MSwwIDEuOTUzNzAzLC0wLjYzNDk1MzUgMC42NzgzNjksLTAuNjM0OTUzNSAwLjY3ODM2OSwtMS44NDUxNjQxIDAsLTEuMjA0NzgzNTUgLTAuNjcyOTQyLC0xLjgzNDMxMDExIC0wLjY3Mjk0MiwtMC42Mjk1MjY1OSAtMS45NTkxMywtMC42Mjk1MjY1OSB6IG0gLTIuMDg5Mzc3LC0xLjU3OTI0MzMgaCAyLjIwMzM0MyBxIDEuODQ1MTY0LDAgMi43NDYwMzksMC4yNjU5MjA3IDAuOTA2MzAxLDAuMjYwNDkzNyAxLjU1MjEwOCwwLjg5MDAyMDMgMC41Njk4MywwLjU0ODEyMjMgMC44NDY2MDUsMS4yNjQ0ODAwNiAwLjI3Njc3NCwwLjcxNjM1NzgxIDAuMjc2Nzc0LDEuNjIyNjU4OTQgMCwwLjkxNzE1NTEgLTAuMjc2Nzc0LDEuNjM4OTM5OSAtMC4yNzY3NzUsMC43MTYzNTc4IC0wLjg0NjYwNSwxLjI2NDQ4IC0wLjY1MTIzNCwwLjYyOTUyNjYgLTEuNTYyOTYyLDAuODk1NDQ3MyAtMC45MTE3MjgsMC4yNjA0OTM3IC0yLjczNTE4NSwwLjI2MDQ5MzcgaCAtMi4yMDMzNDMgeiBtIC04LjE0NTg1NjUsMCBoIDMuNDY3ODIzIHEgMS41NDY2ODE2LDAgMi4zNzE1Nzg1LDAuNjg5MjIzIDAuODMwMzI0LDAuNjgzNzk2MSAwLjgzMDMyNCwxLjk1MzcwMzE0IDAsMS4yNzUzMzM5NyAtMC44MzAzMjQsMS45NjQ1NTcwNiBRIDkuOTg3MTk2MSwyLjI3NDkxNSA4LjQ0MDUxNDUsMi4yNzQ5MTUgSCA3LjA2MjA2ODQgViA1LjA4NjA3NjcgSCA0Ljk3MjY5MTUgWiBtIDIuMDg5Mzc2OSwxLjUxNDExOTkgdiAyLjI2MzAzOTQzIGggMS4xNTU5NDEgcSAwLjYwNzgxODgsMCAwLjkzODg2MjksLTAuMjkzMDU1NDcgMC4zMzEwNDQxLC0wLjI5ODQ4MjQxIDAuMzMxMDQ0MSwtMC44NDExNzc3MiAwLC0wLjU0MjY5NTMxIC0wLjMzMTA0NDEsLTAuODM1NzUwNzQgLTAuMzMxMDQ0MSwtMC4yOTMwNTU1IC0wLjkzODg2MjksLTAuMjkzMDU1NSB6IgovPgo8L3N2Zz4K);
  --jp-icon-python: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iLTEwIC0xMCAxMzEuMTYxMzYxNjk0MzM1OTQgMTMyLjM4ODk5OTkzODk2NDg0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjMzA2OTk4IiBkPSJNIDU0LjkxODc4NSw5LjE5Mjc0MjFlLTQgQyA1MC4zMzUxMzIsMC4wMjIyMTcyNyA0NS45NTc4NDYsMC40MTMxMzY5NyA0Mi4xMDYyODUsMS4wOTQ2NjkzIDMwLjc2MDA2OSwzLjA5OTE3MzEgMjguNzAwMDM2LDcuMjk0NzcxNCAyOC43MDAwMzUsMTUuMDMyMTY5IHYgMTAuMjE4NzUgaCAyNi44MTI1IHYgMy40MDYyNSBoIC0yNi44MTI1IC0xMC4wNjI1IGMgLTcuNzkyNDU5LDAgLTE0LjYxNTc1ODgsNC42ODM3MTcgLTE2Ljc0OTk5OTgsMTMuNTkzNzUgLTIuNDYxODE5OTgsMTAuMjEyOTY2IC0yLjU3MTAxNTA4LDE2LjU4NjAyMyAwLDI3LjI1IDEuOTA1OTI4Myw3LjkzNzg1MiA2LjQ1NzU0MzIsMTMuNTkzNzQ4IDE0LjI0OTk5OTgsMTMuNTkzNzUgaCA5LjIxODc1IHYgLTEyLjI1IGMgMCwtOC44NDk5MDIgNy42NTcxNDQsLTE2LjY1NjI0OCAxNi43NSwtMTYuNjU2MjUgaCAyNi43ODEyNSBjIDcuNDU0OTUxLDAgMTMuNDA2MjUzLC02LjEzODE2NCAxMy40MDYyNSwtMTMuNjI1IHYgLTI1LjUzMTI1IGMgMCwtNy4yNjYzMzg2IC02LjEyOTk4LC0xMi43MjQ3NzcxIC0xMy40MDYyNSwtMTMuOTM3NDk5NyBDIDY0LjI4MTU0OCwwLjMyNzk0Mzk3IDU5LjUwMjQzOCwtMC4wMjAzNzkwMyA1NC45MTg3ODUsOS4xOTI3NDIxZS00IFogbSAtMTQuNSw4LjIxODc1MDEyNTc5IGMgMi43Njk1NDcsMCA1LjAzMTI1LDIuMjk4NjQ1NiA1LjAzMTI1LDUuMTI0OTk5NiAtMmUtNiwyLjgxNjMzNiAtMi4yNjE3MDMsNS4wOTM3NSAtNS4wMzEyNSw1LjA5Mzc1IC0yLjc3OTQ3NiwtMWUtNiAtNS4wMzEyNSwtMi4yNzc0MTUgLTUuMDMxMjUsLTUuMDkzNzUgLTEwZS03LC0yLjgyNjM1MyAyLjI1MTc3NCwtNS4xMjQ5OTk2IDUuMDMxMjUsLTUuMTI0OTk5NiB6Ii8+CiAgPHBhdGggY2xhc3M9ImpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iI2ZmZDQzYiIgZD0ibSA4NS42Mzc1MzUsMjguNjU3MTY5IHYgMTEuOTA2MjUgYyAwLDkuMjMwNzU1IC03LjgyNTg5NSwxNi45OTk5OTkgLTE2Ljc1LDE3IGggLTI2Ljc4MTI1IGMgLTcuMzM1ODMzLDAgLTEzLjQwNjI0OSw2LjI3ODQ4MyAtMTMuNDA2MjUsMTMuNjI1IHYgMjUuNTMxMjQ3IGMgMCw3LjI2NjM0NCA2LjMxODU4OCwxMS41NDAzMjQgMTMuNDA2MjUsMTMuNjI1MDA0IDguNDg3MzMxLDIuNDk1NjEgMTYuNjI2MjM3LDIuOTQ2NjMgMjYuNzgxMjUsMCA2Ljc1MDE1NSwtMS45NTQzOSAxMy40MDYyNTMsLTUuODg3NjEgMTMuNDA2MjUsLTEzLjYyNTAwNCBWIDg2LjUwMDkxOSBoIC0yNi43ODEyNSB2IC0zLjQwNjI1IGggMjYuNzgxMjUgMTMuNDA2MjU0IGMgNy43OTI0NjEsMCAxMC42OTYyNTEsLTUuNDM1NDA4IDEzLjQwNjI0MSwtMTMuNTkzNzUgMi43OTkzMywtOC4zOTg4ODYgMi42ODAyMiwtMTYuNDc1Nzc2IDAsLTI3LjI1IC0xLjkyNTc4LC03Ljc1NzQ0MSAtNS42MDM4NywtMTMuNTkzNzUgLTEzLjQwNjI0MSwtMTMuNTkzNzUgeiBtIC0xNS4wNjI1LDY0LjY1NjI1IGMgMi43Nzk0NzgsM2UtNiA1LjAzMTI1LDIuMjc3NDE3IDUuMDMxMjUsNS4wOTM3NDcgLTJlLTYsMi44MjYzNTQgLTIuMjUxNzc1LDUuMTI1MDA0IC01LjAzMTI1LDUuMTI1MDA0IC0yLjc2OTU1LDAgLTUuMDMxMjUsLTIuMjk4NjUgLTUuMDMxMjUsLTUuMTI1MDA0IDJlLTYsLTIuODE2MzMgMi4yNjE2OTcsLTUuMDkzNzQ3IDUuMDMxMjUsLTUuMDkzNzQ3IHoiLz4KPC9zdmc+Cg==);
  --jp-icon-r-kernel: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1jb250cmFzdDMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjMjE5NkYzIiBkPSJNNC40IDIuNWMxLjItLjEgMi45LS4zIDQuOS0uMyAyLjUgMCA0LjEuNCA1LjIgMS4zIDEgLjcgMS41IDEuOSAxLjUgMy41IDAgMi0xLjQgMy41LTIuOSA0LjEgMS4yLjQgMS43IDEuNiAyLjIgMyAuNiAxLjkgMSAzLjkgMS4zIDQuNmgtMy44Yy0uMy0uNC0uOC0xLjctMS4yLTMuN3MtMS4yLTIuNi0yLjYtMi42aC0uOXY2LjRINC40VjIuNXptMy43IDYuOWgxLjRjMS45IDAgMi45LS45IDIuOS0yLjNzLTEtMi4zLTIuOC0yLjNjLS43IDAtMS4zIDAtMS42LjJ2NC41aC4xdi0uMXoiLz4KPC9zdmc+Cg==);
  --jp-icon-react: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMTUwIDE1MCA1NDEuOSAyOTUuMyI+CiAgPGcgY2xhc3M9ImpwLWljb24tYnJhbmQyIGpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iIzYxREFGQiI+CiAgICA8cGF0aCBkPSJNNjY2LjMgMjk2LjVjMC0zMi41LTQwLjctNjMuMy0xMDMuMS04Mi40IDE0LjQtNjMuNiA4LTExNC4yLTIwLjItMTMwLjQtNi41LTMuOC0xNC4xLTUuNi0yMi40LTUuNnYyMi4zYzQuNiAwIDguMy45IDExLjQgMi42IDEzLjYgNy44IDE5LjUgMzcuNSAxNC45IDc1LjctMS4xIDkuNC0yLjkgMTkuMy01LjEgMjkuNC0xOS42LTQuOC00MS04LjUtNjMuNS0xMC45LTEzLjUtMTguNS0yNy41LTM1LjMtNDEuNi01MCAzMi42LTMwLjMgNjMuMi00Ni45IDg0LTQ2LjlWNzhjLTI3LjUgMC02My41IDE5LjYtOTkuOSA1My42LTM2LjQtMzMuOC03Mi40LTUzLjItOTkuOS01My4ydjIyLjNjMjAuNyAwIDUxLjQgMTYuNSA4NCA0Ni42LTE0IDE0LjctMjggMzEuNC00MS4zIDQ5LjktMjIuNiAyLjQtNDQgNi4xLTYzLjYgMTEtMi4zLTEwLTQtMTkuNy01LjItMjktNC43LTM4LjIgMS4xLTY3LjkgMTQuNi03NS44IDMtMS44IDYuOS0yLjYgMTEuNS0yLjZWNzguNWMtOC40IDAtMTYgMS44LTIyLjYgNS42LTI4LjEgMTYuMi0zNC40IDY2LjctMTkuOSAxMzAuMS02Mi4yIDE5LjItMTAyLjcgNDkuOS0xMDIuNyA4Mi4zIDAgMzIuNSA0MC43IDYzLjMgMTAzLjEgODIuNC0xNC40IDYzLjYtOCAxMTQuMiAyMC4yIDEzMC40IDYuNSAzLjggMTQuMSA1LjYgMjIuNSA1LjYgMjcuNSAwIDYzLjUtMTkuNiA5OS45LTUzLjYgMzYuNCAzMy44IDcyLjQgNTMuMiA5OS45IDUzLjIgOC40IDAgMTYtMS44IDIyLjYtNS42IDI4LjEtMTYuMiAzNC40LTY2LjcgMTkuOS0xMzAuMSA2Mi0xOS4xIDEwMi41LTQ5LjkgMTAyLjUtODIuM3ptLTEzMC4yLTY2LjdjLTMuNyAxMi45LTguMyAyNi4yLTEzLjUgMzkuNS00LjEtOC04LjQtMTYtMTMuMS0yNC00LjYtOC05LjUtMTUuOC0xNC40LTIzLjQgMTQuMiAyLjEgMjcuOSA0LjcgNDEgNy45em0tNDUuOCAxMDYuNWMtNy44IDEzLjUtMTUuOCAyNi4zLTI0LjEgMzguMi0xNC45IDEuMy0zMCAyLTQ1LjIgMi0xNS4xIDAtMzAuMi0uNy00NS0xLjktOC4zLTExLjktMTYuNC0yNC42LTI0LjItMzgtNy42LTEzLjEtMTQuNS0yNi40LTIwLjgtMzkuOCA2LjItMTMuNCAxMy4yLTI2LjggMjAuNy0zOS45IDcuOC0xMy41IDE1LjgtMjYuMyAyNC4xLTM4LjIgMTQuOS0xLjMgMzAtMiA0NS4yLTIgMTUuMSAwIDMwLjIuNyA0NSAxLjkgOC4zIDExLjkgMTYuNCAyNC42IDI0LjIgMzggNy42IDEzLjEgMTQuNSAyNi40IDIwLjggMzkuOC02LjMgMTMuNC0xMy4yIDI2LjgtMjAuNyAzOS45em0zMi4zLTEzYzUuNCAxMy40IDEwIDI2LjggMTMuOCAzOS44LTEzLjEgMy4yLTI2LjkgNS45LTQxLjIgOCA0LjktNy43IDkuOC0xNS42IDE0LjQtMjMuNyA0LjYtOCA4LjktMTYuMSAxMy0yNC4xek00MjEuMiA0MzBjLTkuMy05LjYtMTguNi0yMC4zLTI3LjgtMzIgOSAuNCAxOC4yLjcgMjcuNS43IDkuNCAwIDE4LjctLjIgMjcuOC0uNy05IDExLjctMTguMyAyMi40LTI3LjUgMzJ6bS03NC40LTU4LjljLTE0LjItMi4xLTI3LjktNC43LTQxLTcuOSAzLjctMTIuOSA4LjMtMjYuMiAxMy41LTM5LjUgNC4xIDggOC40IDE2IDEzLjEgMjQgNC43IDggOS41IDE1LjggMTQuNCAyMy40ek00MjAuNyAxNjNjOS4zIDkuNiAxOC42IDIwLjMgMjcuOCAzMi05LS40LTE4LjItLjctMjcuNS0uNy05LjQgMC0xOC43LjItMjcuOC43IDktMTEuNyAxOC4zLTIyLjQgMjcuNS0zMnptLTc0IDU4LjljLTQuOSA3LjctOS44IDE1LjYtMTQuNCAyMy43LTQuNiA4LTguOSAxNi0xMyAyNC01LjQtMTMuNC0xMC0yNi44LTEzLjgtMzkuOCAxMy4xLTMuMSAyNi45LTUuOCA0MS4yLTcuOXptLTkwLjUgMTI1LjJjLTM1LjQtMTUuMS01OC4zLTM0LjktNTguMy01MC42IDAtMTUuNyAyMi45LTM1LjYgNTguMy01MC42IDguNi0zLjcgMTgtNyAyNy43LTEwLjEgNS43IDE5LjYgMTMuMiA0MCAyMi41IDYwLjktOS4yIDIwLjgtMTYuNiA0MS4xLTIyLjIgNjAuNi05LjktMy4xLTE5LjMtNi41LTI4LTEwLjJ6TTMxMCA0OTBjLTEzLjYtNy44LTE5LjUtMzcuNS0xNC45LTc1LjcgMS4xLTkuNCAyLjktMTkuMyA1LjEtMjkuNCAxOS42IDQuOCA0MSA4LjUgNjMuNSAxMC45IDEzLjUgMTguNSAyNy41IDM1LjMgNDEuNiA1MC0zMi42IDMwLjMtNjMuMiA0Ni45LTg0IDQ2LjktNC41LS4xLTguMy0xLTExLjMtMi43em0yMzcuMi03Ni4yYzQuNyAzOC4yLTEuMSA2Ny45LTE0LjYgNzUuOC0zIDEuOC02LjkgMi42LTExLjUgMi42LTIwLjcgMC01MS40LTE2LjUtODQtNDYuNiAxNC0xNC43IDI4LTMxLjQgNDEuMy00OS45IDIyLjYtMi40IDQ0LTYuMSA2My42LTExIDIuMyAxMC4xIDQuMSAxOS44IDUuMiAyOS4xem0zOC41LTY2LjdjLTguNiAzLjctMTggNy0yNy43IDEwLjEtNS43LTE5LjYtMTMuMi00MC0yMi41LTYwLjkgOS4yLTIwLjggMTYuNi00MS4xIDIyLjItNjAuNiA5LjkgMy4xIDE5LjMgNi41IDI4LjEgMTAuMiAzNS40IDE1LjEgNTguMyAzNC45IDU4LjMgNTAuNi0uMSAxNS43LTIzIDM1LjYtNTguNCA1MC42ek0zMjAuOCA3OC40eiIvPgogICAgPGNpcmNsZSBjeD0iNDIwLjkiIGN5PSIyOTYuNSIgcj0iNDUuNyIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-redo: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIGhlaWdodD0iMjQiIHZpZXdCb3g9IjAgMCAyNCAyNCIgd2lkdGg9IjE2Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgICA8cGF0aCBkPSJNMCAwaDI0djI0SDB6IiBmaWxsPSJub25lIi8+PHBhdGggZD0iTTE4LjQgMTAuNkMxNi41NSA4Ljk5IDE0LjE1IDggMTEuNSA4Yy00LjY1IDAtOC41OCAzLjAzLTkuOTYgNy4yMkwzLjkgMTZjMS4wNS0zLjE5IDQuMDUtNS41IDcuNi01LjUgMS45NSAwIDMuNzMuNzIgNS4xMiAxLjg4TDEzIDE2aDlWN2wtMy42IDMuNnoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-refresh: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTkgMTMuNWMtMi40OSAwLTQuNS0yLjAxLTQuNS00LjVTNi41MSA0LjUgOSA0LjVjMS4yNCAwIDIuMzYuNTIgMy4xNyAxLjMzTDEwIDhoNVYzbC0xLjc2IDEuNzZDMTIuMTUgMy42OCAxMC42NiAzIDkgMyA1LjY5IDMgMy4wMSA1LjY5IDMuMDEgOVM1LjY5IDE1IDkgMTVjMi45NyAwIDUuNDMtMi4xNiA1LjktNWgtMS41MmMtLjQ2IDItMi4yNCAzLjUtNC4zOCAzLjV6Ii8+CiAgICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-regex: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIwIDIwIj4KICA8ZyBjbGFzcz0ianAtaWNvbjIiIGZpbGw9IiM0MTQxNDEiPgogICAgPHJlY3QgeD0iMiIgeT0iMiIgd2lkdGg9IjE2IiBoZWlnaHQ9IjE2Ii8+CiAgPC9nPgoKICA8ZyBjbGFzcz0ianAtaWNvbi1hY2NlbnQyIiBmaWxsPSIjRkZGIj4KICAgIDxjaXJjbGUgY2xhc3M9InN0MiIgY3g9IjUuNSIgY3k9IjE0LjUiIHI9IjEuNSIvPgogICAgPHJlY3QgeD0iMTIiIHk9IjQiIGNsYXNzPSJzdDIiIHdpZHRoPSIxIiBoZWlnaHQ9IjgiLz4KICAgIDxyZWN0IHg9IjguNSIgeT0iNy41IiB0cmFuc2Zvcm09Im1hdHJpeCgwLjg2NiAtMC41IDAuNSAwLjg2NiAtMi4zMjU1IDcuMzIxOSkiIGNsYXNzPSJzdDIiIHdpZHRoPSI4IiBoZWlnaHQ9IjEiLz4KICAgIDxyZWN0IHg9IjEyIiB5PSI0IiB0cmFuc2Zvcm09Im1hdHJpeCgwLjUgLTAuODY2IDAuODY2IDAuNSAtMC42Nzc5IDE0LjgyNTIpIiBjbGFzcz0ic3QyIiB3aWR0aD0iMSIgaGVpZ2h0PSI4Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-run: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTggNXYxNGwxMS03eiIvPgogICAgPC9nPgo8L3N2Zz4K);
  --jp-icon-running: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDUxMiA1MTIiPgogIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICA8cGF0aCBkPSJNMjU2IDhDMTE5IDggOCAxMTkgOCAyNTZzMTExIDI0OCAyNDggMjQ4IDI0OC0xMTEgMjQ4LTI0OFMzOTMgOCAyNTYgOHptOTYgMzI4YzAgOC44LTcuMiAxNi0xNiAxNkgxNzZjLTguOCAwLTE2LTcuMi0xNi0xNlYxNzZjMC04LjggNy4yLTE2IDE2LTE2aDE2MGM4LjggMCAxNiA3LjIgMTYgMTZ2MTYweiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-save: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTE3IDNINWMtMS4xMSAwLTIgLjktMiAydjE0YzAgMS4xLjg5IDIgMiAyaDE0YzEuMSAwIDItLjkgMi0yVjdsLTQtNHptLTUgMTZjLTEuNjYgMC0zLTEuMzQtMy0zczEuMzQtMyAzLTMgMyAxLjM0IDMgMy0xLjM0IDMtMyAzem0zLTEwSDVWNWgxMHY0eiIvPgogICAgPC9nPgo8L3N2Zz4K);
  --jp-icon-search: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMTggMTgiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTEyLjEsMTAuOWgtMC43bC0wLjItMC4yYzAuOC0wLjksMS4zLTIuMiwxLjMtMy41YzAtMy0yLjQtNS40LTUuNC01LjRTMS44LDQuMiwxLjgsNy4xczIuNCw1LjQsNS40LDUuNCBjMS4zLDAsMi41LTAuNSwzLjUtMS4zbDAuMiwwLjJ2MC43bDQuMSw0LjFsMS4yLTEuMkwxMi4xLDEwLjl6IE03LjEsMTAuOWMtMi4xLDAtMy43LTEuNy0zLjctMy43czEuNy0zLjcsMy43LTMuN3MzLjcsMS43LDMuNywzLjcgUzkuMiwxMC45LDcuMSwxMC45eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-settings: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMTkuNDMgMTIuOThjLjA0LS4zMi4wNy0uNjQuMDctLjk4cy0uMDMtLjY2LS4wNy0uOThsMi4xMS0xLjY1Yy4xOS0uMTUuMjQtLjQyLjEyLS42NGwtMi0zLjQ2Yy0uMTItLjIyLS4zOS0uMy0uNjEtLjIybC0yLjQ5IDFjLS41Mi0uNC0xLjA4LS43My0xLjY5LS45OGwtLjM4LTIuNjVBLjQ4OC40ODggMCAwMDE0IDJoLTRjLS4yNSAwLS40Ni4xOC0uNDkuNDJsLS4zOCAyLjY1Yy0uNjEuMjUtMS4xNy41OS0xLjY5Ljk4bC0yLjQ5LTFjLS4yMy0uMDktLjQ5IDAtLjYxLjIybC0yIDMuNDZjLS4xMy4yMi0uMDcuNDkuMTIuNjRsMi4xMSAxLjY1Yy0uMDQuMzItLjA3LjY1LS4wNy45OHMuMDMuNjYuMDcuOThsLTIuMTEgMS42NWMtLjE5LjE1LS4yNC40Mi0uMTIuNjRsMiAzLjQ2Yy4xMi4yMi4zOS4zLjYxLjIybDIuNDktMWMuNTIuNCAxLjA4LjczIDEuNjkuOThsLjM4IDIuNjVjLjAzLjI0LjI0LjQyLjQ5LjQyaDRjLjI1IDAgLjQ2LS4xOC40OS0uNDJsLjM4LTIuNjVjLjYxLS4yNSAxLjE3LS41OSAxLjY5LS45OGwyLjQ5IDFjLjIzLjA5LjQ5IDAgLjYxLS4yMmwyLTMuNDZjLjEyLS4yMi4wNy0uNDktLjEyLS42NGwtMi4xMS0xLjY1ek0xMiAxNS41Yy0xLjkzIDAtMy41LTEuNTctMy41LTMuNXMxLjU3LTMuNSAzLjUtMy41IDMuNSAxLjU3IDMuNSAzLjUtMS41NyAzLjUtMy41IDMuNXoiLz4KPC9zdmc+Cg==);
  --jp-icon-share: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTYiIHZpZXdCb3g9IjAgMCAyNCAyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTSAxOCAyIEMgMTYuMzU0OTkgMiAxNSAzLjM1NDk5MDQgMTUgNSBDIDE1IDUuMTkwOTUyOSAxNS4wMjE3OTEgNS4zNzcxMjI0IDE1LjA1NjY0MSA1LjU1ODU5MzggTCA3LjkyMTg3NSA5LjcyMDcwMzEgQyA3LjM5ODUzOTkgOS4yNzc4NTM5IDYuNzMyMDc3MSA5IDYgOSBDIDQuMzU0OTkwNCA5IDMgMTAuMzU0OTkgMyAxMiBDIDMgMTMuNjQ1MDEgNC4zNTQ5OTA0IDE1IDYgMTUgQyA2LjczMjA3NzEgMTUgNy4zOTg1Mzk5IDE0LjcyMjE0NiA3LjkyMTg3NSAxNC4yNzkyOTcgTCAxNS4wNTY2NDEgMTguNDM5NDUzIEMgMTUuMDIxNTU1IDE4LjYyMTUxNCAxNSAxOC44MDgzODYgMTUgMTkgQyAxNSAyMC42NDUwMSAxNi4zNTQ5OSAyMiAxOCAyMiBDIDE5LjY0NTAxIDIyIDIxIDIwLjY0NTAxIDIxIDE5IEMgMjEgMTcuMzU0OTkgMTkuNjQ1MDEgMTYgMTggMTYgQyAxNy4yNjc0OCAxNiAxNi42MDE1OTMgMTYuMjc5MzI4IDE2LjA3ODEyNSAxNi43MjI2NTYgTCA4Ljk0MzM1OTQgMTIuNTU4NTk0IEMgOC45NzgyMDk1IDEyLjM3NzEyMiA5IDEyLjE5MDk1MyA5IDEyIEMgOSAxMS44MDkwNDcgOC45NzgyMDk1IDExLjYyMjg3OCA4Ljk0MzM1OTQgMTEuNDQxNDA2IEwgMTYuMDc4MTI1IDcuMjc5Mjk2OSBDIDE2LjYwMTQ2IDcuNzIyMTQ2MSAxNy4yNjc5MjMgOCAxOCA4IEMgMTkuNjQ1MDEgOCAyMSA2LjY0NTAwOTYgMjEgNSBDIDIxIDMuMzU0OTkwNCAxOS42NDUwMSAyIDE4IDIgeiBNIDE4IDQgQyAxOC41NjQxMjkgNCAxOSA0LjQzNTg3MDYgMTkgNSBDIDE5IDUuNTY0MTI5NCAxOC41NjQxMjkgNiAxOCA2IEMgMTcuNDM1ODcxIDYgMTcgNS41NjQxMjk0IDE3IDUgQyAxNyA0LjQzNTg3MDYgMTcuNDM1ODcxIDQgMTggNCB6IE0gNiAxMSBDIDYuNTY0MTI5NCAxMSA3IDExLjQzNTg3MSA3IDEyIEMgNyAxMi41NjQxMjkgNi41NjQxMjk0IDEzIDYgMTMgQyA1LjQzNTg3MDYgMTMgNSAxMi41NjQxMjkgNSAxMiBDIDUgMTEuNDM1ODcxIDUuNDM1ODcwNiAxMSA2IDExIHogTSAxOCAxOCBDIDE4LjU2NDEyOSAxOCAxOSAxOC40MzU4NzEgMTkgMTkgQyAxOSAxOS41NjQxMjkgMTguNTY0MTI5IDIwIDE4IDIwIEMgMTcuNDM1ODcxIDIwIDE3IDE5LjU2NDEyOSAxNyAxOSBDIDE3IDE4LjQzNTg3MSAxNy40MzU4NzEgMTggMTggMTggeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-spreadsheet: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1jb250cmFzdDEganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNENBRjUwIiBkPSJNMi4yIDIuMnYxNy42aDE3LjZWMi4ySDIuMnptMTUuNCA3LjdoLTUuNVY0LjRoNS41djUuNXpNOS45IDQuNHY1LjVINC40VjQuNGg1LjV6bS01LjUgNy43aDUuNXY1LjVINC40di01LjV6bTcuNyA1LjV2LTUuNWg1LjV2NS41aC01LjV6Ii8+Cjwvc3ZnPgo=);
  --jp-icon-stop: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTAgMGgyNHYyNEgweiIgZmlsbD0ibm9uZSIvPgogICAgICAgIDxwYXRoIGQ9Ik02IDZoMTJ2MTJINnoiLz4KICAgIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-tab: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTIxIDNIM2MtMS4xIDAtMiAuOS0yIDJ2MTRjMCAxLjEuOSAyIDIgMmgxOGMxLjEgMCAyLS45IDItMlY1YzAtMS4xLS45LTItMi0yem0wIDE2SDNWNWgxMHY0aDh2MTB6Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-table-rows: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTAgMGgyNHYyNEgweiIgZmlsbD0ibm9uZSIvPgogICAgICAgIDxwYXRoIGQ9Ik0yMSw4SDNWNGgxOFY4eiBNMjEsMTBIM3Y0aDE4VjEweiBNMjEsMTZIM3Y0aDE4VjE2eiIvPgogICAgPC9nPgo8L3N2Zz4K);
  --jp-icon-tag: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjgiIGhlaWdodD0iMjgiIHZpZXdCb3g9IjAgMCA0MyAyOCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CgkJPHBhdGggZD0iTTI4LjgzMzIgMTIuMzM0TDMyLjk5OTggMTYuNTAwN0wzNy4xNjY1IDEyLjMzNEgyOC44MzMyWiIvPgoJCTxwYXRoIGQ9Ik0xNi4yMDk1IDIxLjYxMDRDMTUuNjg3MyAyMi4xMjk5IDE0Ljg0NDMgMjIuMTI5OSAxNC4zMjQ4IDIxLjYxMDRMNi45ODI5IDE0LjcyNDVDNi41NzI0IDE0LjMzOTQgNi4wODMxMyAxMy42MDk4IDYuMDQ3ODYgMTMuMDQ4MkM1Ljk1MzQ3IDExLjUyODggNi4wMjAwMiA4LjYxOTQ0IDYuMDY2MjEgNy4wNzY5NUM2LjA4MjgxIDYuNTE0NzcgNi41NTU0OCA2LjA0MzQ3IDcuMTE4MDQgNi4wMzA1NUM5LjA4ODYzIDUuOTg0NzMgMTMuMjYzOCA1LjkzNTc5IDEzLjY1MTggNi4zMjQyNUwyMS43MzY5IDEzLjYzOUMyMi4yNTYgMTQuMTU4NSAyMS43ODUxIDE1LjQ3MjQgMjEuMjYyIDE1Ljk5NDZMMTYuMjA5NSAyMS42MTA0Wk05Ljc3NTg1IDguMjY1QzkuMzM1NTEgNy44MjU2NiA4LjYyMzUxIDcuODI1NjYgOC4xODI4IDguMjY1QzcuNzQzNDYgOC43MDU3MSA3Ljc0MzQ2IDkuNDE3MzMgOC4xODI4IDkuODU2NjdDOC42MjM4MiAxMC4yOTY0IDkuMzM1ODIgMTAuMjk2NCA5Ljc3NTg1IDkuODU2NjdDMTAuMjE1NiA5LjQxNzMzIDEwLjIxNTYgOC43MDUzMyA5Ljc3NTg1IDguMjY1WiIvPgoJPC9nPgo8L3N2Zz4K);
  --jp-icon-terminal: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0IiA+CiAgICA8cmVjdCBjbGFzcz0ianAtdGVybWluYWwtaWNvbi1iYWNrZ3JvdW5kLWNvbG9yIGpwLWljb24tc2VsZWN0YWJsZSIgd2lkdGg9IjIwIiBoZWlnaHQ9IjIwIiB0cmFuc2Zvcm09InRyYW5zbGF0ZSgyIDIpIiBmaWxsPSIjMzMzMzMzIi8+CiAgICA8cGF0aCBjbGFzcz0ianAtdGVybWluYWwtaWNvbi1jb2xvciBqcC1pY29uLXNlbGVjdGFibGUtaW52ZXJzZSIgZD0iTTUuMDU2NjQgOC43NjE3MkM1LjA1NjY0IDguNTk3NjYgNS4wMzEyNSA4LjQ1MzEyIDQuOTgwNDcgOC4zMjgxMkM0LjkzMzU5IDguMTk5MjIgNC44NTU0NyA4LjA4MjAzIDQuNzQ2MDkgNy45NzY1NkM0LjY0MDYyIDcuODcxMDkgNC41IDcuNzc1MzkgNC4zMjQyMiA3LjY4OTQ1QzQuMTUyMzQgNy41OTk2MSAzLjk0MzM2IDcuNTExNzIgMy42OTcyNyA3LjQyNTc4QzMuMzAyNzMgNy4yODUxNiAyLjk0MzM2IDcuMTM2NzIgMi42MTkxNCA2Ljk4MDQ3QzIuMjk0OTIgNi44MjQyMiAyLjAxNzU4IDYuNjQyNTggMS43ODcxMSA2LjQzNTU1QzEuNTYwNTUgNi4yMjg1MiAxLjM4NDc3IDUuOTg4MjggMS4yNTk3NyA1LjcxNDg0QzEuMTM0NzcgNS40Mzc1IDEuMDcyMjcgNS4xMDkzOCAxLjA3MjI3IDQuNzMwNDdDMS4wNzIyNyA0LjM5ODQ0IDEuMTI4OTEgNC4wOTU3IDEuMjQyMTkgMy44MjIyN0MxLjM1NTQ3IDMuNTQ0OTIgMS41MTU2MiAzLjMwNDY5IDEuNzIyNjYgMy4xMDE1NkMxLjkyOTY5IDIuODk4NDQgMi4xNzk2OSAyLjczNDM3IDIuNDcyNjYgMi42MDkzOEMyLjc2NTYyIDIuNDg0MzggMy4wOTE4IDIuNDA0MyAzLjQ1MTE3IDIuMzY5MTRWMS4xMDkzOEg0LjM4ODY3VjIuMzgwODZDNC43NDAyMyAyLjQyNzczIDUuMDU2NjQgMi41MjM0NCA1LjMzNzg5IDIuNjY3OTdDNS42MTkxNCAyLjgxMjUgNS44NTc0MiAzLjAwMTk1IDYuMDUyNzMgMy4yMzYzM0M2LjI1MTk1IDMuNDY2OCA2LjQwNDMgMy43NDAyMyA2LjUwOTc3IDQuMDU2NjRDNi42MTkxNCA0LjM2OTE0IDYuNjczODMgNC43MjA3IDYuNjczODMgNS4xMTEzM0g1LjA0NDkyQzUuMDQ0OTIgNC42Mzg2NyA0LjkzNzUgNC4yODEyNSA0LjcyMjY2IDQuMDM5MDZDNC41MDc4MSAzLjc5Mjk3IDQuMjE2OCAzLjY2OTkyIDMuODQ5NjEgMy42Njk5MkMzLjY1MDM5IDMuNjY5OTIgMy40NzY1NiAzLjY5NzI3IDMuMzI4MTIgMy43NTE5NUMzLjE4MzU5IDMuODAyNzMgMy4wNjQ0NSAzLjg3Njk1IDIuOTcwNyAzLjk3NDYxQzIuODc2OTUgNC4wNjgzNiAyLjgwNjY0IDQuMTc5NjkgMi43NTk3NyA0LjMwODU5QzIuNzE2OCA0LjQzNzUgMi42OTUzMSA0LjU3ODEyIDIuNjk1MzEgNC43MzA0N0MyLjY5NTMxIDQuODgyODEgMi43MTY4IDUuMDE5NTMgMi43NTk3NyA1LjE0MDYyQzIuODA2NjQgNS4yNTc4MSAyLjg4MjgxIDUuMzY3MTkgMi45ODgyOCA1LjQ2ODc1QzMuMDk3NjYgNS41NzAzMSAzLjI0MDIzIDUuNjY3OTcgMy40MTYwMiA1Ljc2MTcyQzMuNTkxOCA1Ljg1MTU2IDMuODEwNTUgNS45NDMzNiA0LjA3MjI3IDYuMDM3MTFDNC40NjY4IDYuMTg1NTUgNC44MjQyMiA2LjMzOTg0IDUuMTQ0NTMgNi41QzUuNDY0ODQgNi42NTYyNSA1LjczODI4IDYuODM5ODQgNS45NjQ4NCA3LjA1MDc4QzYuMTk1MzEgNy4yNTc4MSA2LjM3MTA5IDcuNSA2LjQ5MjE5IDcuNzc3MzRDNi42MTcxOSA4LjA1MDc4IDYuNjc5NjkgOC4zNzUgNi42Nzk2OSA4Ljc1QzYuNjc5NjkgOS4wOTM3NSA2LjYyMzA1IDkuNDA0MyA2LjUwOTc3IDkuNjgxNjRDNi4zOTY0OCA5Ljk1NTA4IDYuMjM0MzggMTAuMTkxNCA2LjAyMzQ0IDEwLjM5MDZDNS44MTI1IDEwLjU4OTggNS41NTg1OSAxMC43NSA1LjI2MTcyIDEwLjg3MTFDNC45NjQ4NCAxMC45ODgzIDQuNjMyODEgMTEuMDY0NSA0LjI2NTYyIDExLjA5OTZWMTIuMjQ4SDMuMzMzOThWMTEuMDk5NkMzLjAwMTk1IDExLjA2ODQgMi42Nzk2OSAxMC45OTYxIDIuMzY3MTkgMTAuODgyOEMyLjA1NDY5IDEwLjc2NTYgMS43NzczNCAxMC41OTc3IDEuNTM1MTYgMTAuMzc4OUMxLjI5Njg4IDEwLjE2MDIgMS4xMDU0NyA5Ljg4NDc3IDAuOTYwOTM4IDkuNTUyNzNDMC44MTY0MDYgOS4yMTY4IDAuNzQ0MTQxIDguODE0NDUgMC43NDQxNDEgOC4zNDU3SDIuMzc4OTFDMi4zNzg5MSA4LjYyNjk1IDIuNDE5OTIgOC44NjMyOCAyLjUwMTk1IDkuMDU0NjlDMi41ODM5OCA5LjI0MjE5IDIuNjg5NDUgOS4zOTI1OCAyLjgxODM2IDkuNTA1ODZDMi45NTExNyA5LjYxNTIzIDMuMTAxNTYgOS42OTMzNiAzLjI2OTUzIDkuNzQwMjNDMy40Mzc1IDkuNzg3MTEgMy42MDkzOCA5LjgxMDU1IDMuNzg1MTYgOS44MTA1NUM0LjIwMzEyIDkuODEwNTUgNC41MTk1MyA5LjcxMjg5IDQuNzM0MzggOS41MTc1OEM0Ljk0OTIyIDkuMzIyMjcgNS4wNTY2NCA5LjA3MDMxIDUuMDU2NjQgOC43NjE3MlpNMTMuNDE4IDEyLjI3MTVIOC4wNzQyMlYxMUgxMy40MThWMTIuMjcxNVoiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDMuOTUyNjQgNikiIGZpbGw9IndoaXRlIi8+Cjwvc3ZnPgo=);
  --jp-icon-text-editor: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtdGV4dC1lZGl0b3ItaWNvbi1jb2xvciBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiM2MTYxNjEiIGQ9Ik0xNSAxNUgzdjJoMTJ2LTJ6bTAtOEgzdjJoMTJWN3pNMyAxM2gxOHYtMkgzdjJ6bTAgOGgxOHYtMkgzdjJ6TTMgM3YyaDE4VjNIM3oiLz4KPC9zdmc+Cg==);
  --jp-icon-toc: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIj4KICAgIDxwYXRoIGQ9Ik03LDVIMjFWN0g3VjVNNywxM1YxMUgyMVYxM0g3TTQsNC41QTEuNSwxLjUgMCAwLDEgNS41LDZBMS41LDEuNSAwIDAsMSA0LDcuNUExLjUsMS41IDAgMCwxIDIuNSw2QTEuNSwxLjUgMCAwLDEgNCw0LjVNNCwxMC41QTEuNSwxLjUgMCAwLDEgNS41LDEyQTEuNSwxLjUgMCAwLDEgNCwxMy41QTEuNSwxLjUgMCAwLDEgMi41LDEyQTEuNSwxLjUgMCAwLDEgNCwxMC41TTcsMTlWMTdIMjFWMTlIN000LDE2LjVBMS41LDEuNSAwIDAsMSA1LjUsMThBMS41LDEuNSAwIDAsMSA0LDE5LjVBMS41LDEuNSAwIDAsMSAyLjUsMThBMS41LDEuNSAwIDAsMSA0LDE2LjVaIiAvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-tree-view: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTAgMGgyNHYyNEgweiIgZmlsbD0ibm9uZSIvPgogICAgICAgIDxwYXRoIGQ9Ik0yMiAxMVYzaC03djNIOVYzSDJ2OGg3VjhoMnYxMGg0djNoN3YtOGgtN3YzaC0yVjhoMnYzeiIvPgogICAgPC9nPgo8L3N2Zz4K);
  --jp-icon-trusted: url(data:image/svg+xml;base64,PHN2ZyBmaWxsPSJub25lIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI1Ij4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiIgc3Ryb2tlPSIjMzMzMzMzIiBzdHJva2Utd2lkdGg9IjIiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDIgMykiIGQ9Ik0xLjg2MDk0IDExLjQ0MDlDMC44MjY0NDggOC43NzAyNyAwLjg2Mzc3OSA2LjA1NzY0IDEuMjQ5MDcgNC4xOTkzMkMyLjQ4MjA2IDMuOTMzNDcgNC4wODA2OCAzLjQwMzQ3IDUuNjAxMDIgMi44NDQ5QzcuMjM1NDkgMi4yNDQ0IDguODU2NjYgMS41ODE1IDkuOTg3NiAxLjA5NTM5QzExLjA1OTcgMS41ODM0MSAxMi42MDk0IDIuMjQ0NCAxNC4yMTggMi44NDMzOUMxNS43NTAzIDMuNDEzOTQgMTcuMzk5NSAzLjk1MjU4IDE4Ljc1MzkgNC4yMTM4NUMxOS4xMzY0IDYuMDcxNzcgMTkuMTcwOSA4Ljc3NzIyIDE4LjEzOSAxMS40NDA5QzE3LjAzMDMgMTQuMzAzMiAxNC42NjY4IDE3LjE4NDQgOS45OTk5OSAxOC45MzU0QzUuMzMzMiAxNy4xODQ0IDIuOTY5NjggMTQuMzAzMiAxLjg2MDk0IDExLjQ0MDlaIi8+CiAgICA8cGF0aCBjbGFzcz0ianAtaWNvbjIiIGZpbGw9IiMzMzMzMzMiIHN0cm9rZT0iIzMzMzMzMyIgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoOCA5Ljg2NzE5KSIgZD0iTTIuODYwMTUgNC44NjUzNUwwLjcyNjU0OSAyLjk5OTU5TDAgMy42MzA0NUwyLjg2MDE1IDYuMTMxNTdMOCAwLjYzMDg3Mkw3LjI3ODU3IDBMMi44NjAxNSA0Ljg2NTM1WiIvPgo8L3N2Zz4K);
  --jp-icon-undo: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTEyLjUgOGMtMi42NSAwLTUuMDUuOTktNi45IDIuNkwyIDd2OWg5bC0zLjYyLTMuNjJjMS4zOS0xLjE2IDMuMTYtMS44OCA1LjEyLTEuODggMy41NCAwIDYuNTUgMi4zMSA3LjYgNS41bDIuMzctLjc4QzIxLjA4IDExLjAzIDE3LjE1IDggMTIuNSA4eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-user: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTYiIHZpZXdCb3g9IjAgMCAyNCAyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTE2IDdhNCA0IDAgMTEtOCAwIDQgNCAwIDAxOCAwek0xMiAxNGE3IDcgMCAwMC03IDdoMTRhNyA3IDAgMDAtNy03eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-users: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjQiIGhlaWdodD0iMjQiIHZlcnNpb249IjEuMSIgdmlld0JveD0iMCAwIDM2IDI0IiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciPgogPGcgY2xhc3M9ImpwLWljb24zIiB0cmFuc2Zvcm09Im1hdHJpeCgxLjczMjcgMCAwIDEuNzMyNyAtMy42MjgyIC4wOTk1NzcpIiBmaWxsPSIjNjE2MTYxIj4KICA8cGF0aCB0cmFuc2Zvcm09Im1hdHJpeCgxLjUsMCwwLDEuNSwwLC02KSIgZD0ibTEyLjE4NiA3LjUwOThjLTEuMDUzNSAwLTEuOTc1NyAwLjU2NjUtMi40Nzg1IDEuNDEwMiAwLjc1MDYxIDAuMzEyNzcgMS4zOTc0IDAuODI2NDggMS44NzMgMS40NzI3aDMuNDg2M2MwLTEuNTkyLTEuMjg4OS0yLjg4MjgtMi44ODA5LTIuODgyOHoiLz4KICA8cGF0aCBkPSJtMjAuNDY1IDIuMzg5NWEyLjE4ODUgMi4xODg1IDAgMCAxLTIuMTg4NCAyLjE4ODUgMi4xODg1IDIuMTg4NSAwIDAgMS0yLjE4ODUtMi4xODg1IDIuMTg4NSAyLjE4ODUgMCAwIDEgMi4xODg1LTIuMTg4NSAyLjE4ODUgMi4xODg1IDAgMCAxIDIuMTg4NCAyLjE4ODV6Ii8+CiAgPHBhdGggdHJhbnNmb3JtPSJtYXRyaXgoMS41LDAsMCwxLjUsMCwtNikiIGQ9Im0zLjU4OTggOC40MjE5Yy0xLjExMjYgMC0yLjAxMzcgMC45MDExMS0yLjAxMzcgMi4wMTM3aDIuODE0NWMwLjI2Nzk3LTAuMzczMDkgMC41OTA3LTAuNzA0MzUgMC45NTg5OC0wLjk3ODUyLTAuMzQ0MzMtMC42MTY4OC0xLjAwMzEtMS4wMzUyLTEuNzU5OC0xLjAzNTJ6Ii8+CiAgPHBhdGggZD0ibTYuOTE1NCA0LjYyM2ExLjUyOTQgMS41Mjk0IDAgMCAxLTEuNTI5NCAxLjUyOTQgMS41Mjk0IDEuNTI5NCAwIDAgMS0xLjUyOTQtMS41Mjk0IDEuNTI5NCAxLjUyOTQgMCAwIDEgMS41Mjk0LTEuNTI5NCAxLjUyOTQgMS41Mjk0IDAgMCAxIDEuNTI5NCAxLjUyOTR6Ii8+CiAgPHBhdGggZD0ibTYuMTM1IDEzLjUzNWMwLTMuMjM5MiAyLjYyNTktNS44NjUgNS44NjUtNS44NjUgMy4yMzkyIDAgNS44NjUgMi42MjU5IDUuODY1IDUuODY1eiIvPgogIDxjaXJjbGUgY3g9IjEyIiBjeT0iMy43Njg1IiByPSIyLjk2ODUiLz4KIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-vega: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8ZyBjbGFzcz0ianAtaWNvbjEganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjMjEyMTIxIj4KICAgIDxwYXRoIGQ9Ik0xMC42IDUuNGwyLjItMy4ySDIuMnY3LjNsNC02LjZ6Ii8+CiAgICA8cGF0aCBkPSJNMTUuOCAyLjJsLTQuNCA2LjZMNyA2LjNsLTQuOCA4djUuNWgxNy42VjIuMmgtNHptLTcgMTUuNEg1LjV2LTQuNGgzLjN2NC40em00LjQgMEg5LjhWOS44aDMuNHY3Ljh6bTQuNCAwaC0zLjRWNi41aDMuNHYxMS4xeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-word: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIwIDIwIj4KIDxnIGNsYXNzPSJqcC1pY29uMiIgZmlsbD0iIzQxNDE0MSI+CiAgPHJlY3QgeD0iMiIgeT0iMiIgd2lkdGg9IjE2IiBoZWlnaHQ9IjE2Ii8+CiA8L2c+CiA8ZyBjbGFzcz0ianAtaWNvbi1hY2NlbnQyIiB0cmFuc2Zvcm09InRyYW5zbGF0ZSguNDMgLjA0MDEpIiBmaWxsPSIjZmZmIj4KICA8cGF0aCBkPSJtNC4xNCA4Ljc2cTAuMDY4Mi0xLjg5IDIuNDItMS44OSAxLjE2IDAgMS42OCAwLjQyIDAuNTY3IDAuNDEgMC41NjcgMS4xNnYzLjQ3cTAgMC40NjIgMC41MTQgMC40NjIgMC4xMDMgMCAwLjItMC4wMjMxdjAuNzE0cS0wLjM5OSAwLjEwMy0wLjY1MSAwLjEwMy0wLjQ1MiAwLTAuNjkzLTAuMjItMC4yMzEtMC4yLTAuMjg0LTAuNjYyLTAuOTU2IDAuODcyLTIgMC44NzItMC45MDMgMC0xLjQ3LTAuNDcyLTAuNTI1LTAuNDcyLTAuNTI1LTEuMjYgMC0wLjI2MiAwLjA0NTItMC40NzIgMC4wNTY3LTAuMjIgMC4xMTYtMC4zNzggMC4wNjgyLTAuMTY4IDAuMjMxLTAuMzA0IDAuMTU4LTAuMTQ3IDAuMjYyLTAuMjQyIDAuMTE2LTAuMDkxNCAwLjM2OC0wLjE2OCAwLjI2Mi0wLjA5MTQgMC4zOTktMC4xMjYgMC4xMzYtMC4wNDUyIDAuNDcyLTAuMTAzIDAuMzM2LTAuMDU3OCAwLjUwNC0wLjA3OTggMC4xNTgtMC4wMjMxIDAuNTY3LTAuMDc5OCAwLjU1Ni0wLjA2ODIgMC43NzctMC4yMjEgMC4yMi0wLjE1MiAwLjIyLTAuNDQxdi0wLjI1MnEwLTAuNDMtMC4zNTctMC42NjItMC4zMzYtMC4yMzEtMC45NzYtMC4yMzEtMC42NjIgMC0wLjk5OCAwLjI2Mi0wLjMzNiAwLjI1Mi0wLjM5OSAwLjc5OHptMS44OSAzLjY4cTAuNzg4IDAgMS4yNi0wLjQxIDAuNTA0LTAuNDIgMC41MDQtMC45MDN2LTEuMDVxLTAuMjg0IDAuMTM2LTAuODYxIDAuMjMxLTAuNTY3IDAuMDkxNC0wLjk4NyAwLjE1OC0wLjQyIDAuMDY4Mi0wLjc2NiAwLjMyNi0wLjMzNiAwLjI1Mi0wLjMzNiAwLjcwNHQwLjMwNCAwLjcwNCAwLjg2MSAwLjI1MnoiIHN0cm9rZS13aWR0aD0iMS4wNSIvPgogIDxwYXRoIGQ9Im0xMCA0LjU2aDAuOTQ1djMuMTVxMC42NTEtMC45NzYgMS44OS0wLjk3NiAxLjE2IDAgMS44OSAwLjg0IDAuNjgyIDAuODQgMC42ODIgMi4zMSAwIDEuNDctMC43MDQgMi40Mi0wLjcwNCAwLjg4Mi0xLjg5IDAuODgyLTEuMjYgMC0xLjg5LTEuMDJ2MC43NjZoLTAuODV6bTIuNjIgMy4wNHEtMC43NDYgMC0xLjE2IDAuNjQtMC40NTIgMC42My0wLjQ1MiAxLjY4IDAgMS4wNSAwLjQ1MiAxLjY4dDEuMTYgMC42M3EwLjc3NyAwIDEuMjYtMC42MyAwLjQ5NC0wLjY0IDAuNDk0LTEuNjggMC0xLjA1LTAuNDcyLTEuNjgtMC40NjItMC42NC0xLjI2LTAuNjR6IiBzdHJva2Utd2lkdGg9IjEuMDUiLz4KICA8cGF0aCBkPSJtMi43MyAxNS44IDEzLjYgMC4wMDgxYzAuMDA2OSAwIDAtMi42IDAtMi42IDAtMC4wMDc4LTEuMTUgMC0xLjE1IDAtMC4wMDY5IDAtMC4wMDgzIDEuNS0wLjAwODMgMS41LTJlLTMgLTAuMDAxNC0xMS4zLTAuMDAxNC0xMS4zLTAuMDAxNGwtMC4wMDU5Mi0xLjVjMC0wLjAwNzgtMS4xNyAwLjAwMTMtMS4xNyAwLjAwMTN6IiBzdHJva2Utd2lkdGg9Ii45NzUiLz4KIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-yaml: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8ZyBjbGFzcz0ianAtaWNvbi1jb250cmFzdDIganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjRDgxQjYwIj4KICAgIDxwYXRoIGQ9Ik03LjIgMTguNnYtNS40TDMgNS42aDMuM2wxLjQgMy4xYy4zLjkuNiAxLjYgMSAyLjUuMy0uOC42LTEuNiAxLTIuNWwxLjQtMy4xaDMuNGwtNC40IDcuNnY1LjVsLTIuOS0uMXoiLz4KICAgIDxjaXJjbGUgY2xhc3M9InN0MCIgY3g9IjE3LjYiIGN5PSIxNi41IiByPSIyLjEiLz4KICAgIDxjaXJjbGUgY2xhc3M9InN0MCIgY3g9IjE3LjYiIGN5PSIxMSIgcj0iMi4xIi8+CiAgPC9nPgo8L3N2Zz4K);
}

/* Icon CSS class declarations */

.jp-AddAboveIcon {
  background-image: var(--jp-icon-add-above);
}

.jp-AddBelowIcon {
  background-image: var(--jp-icon-add-below);
}

.jp-AddIcon {
  background-image: var(--jp-icon-add);
}

.jp-BellIcon {
  background-image: var(--jp-icon-bell);
}

.jp-BugDotIcon {
  background-image: var(--jp-icon-bug-dot);
}

.jp-BugIcon {
  background-image: var(--jp-icon-bug);
}

.jp-BuildIcon {
  background-image: var(--jp-icon-build);
}

.jp-CaretDownEmptyIcon {
  background-image: var(--jp-icon-caret-down-empty);
}

.jp-CaretDownEmptyThinIcon {
  background-image: var(--jp-icon-caret-down-empty-thin);
}

.jp-CaretDownIcon {
  background-image: var(--jp-icon-caret-down);
}

.jp-CaretLeftIcon {
  background-image: var(--jp-icon-caret-left);
}

.jp-CaretRightIcon {
  background-image: var(--jp-icon-caret-right);
}

.jp-CaretUpEmptyThinIcon {
  background-image: var(--jp-icon-caret-up-empty-thin);
}

.jp-CaretUpIcon {
  background-image: var(--jp-icon-caret-up);
}

.jp-CaseSensitiveIcon {
  background-image: var(--jp-icon-case-sensitive);
}

.jp-CheckIcon {
  background-image: var(--jp-icon-check);
}

.jp-CircleEmptyIcon {
  background-image: var(--jp-icon-circle-empty);
}

.jp-CircleIcon {
  background-image: var(--jp-icon-circle);
}

.jp-ClearIcon {
  background-image: var(--jp-icon-clear);
}

.jp-CloseIcon {
  background-image: var(--jp-icon-close);
}

.jp-CodeCheckIcon {
  background-image: var(--jp-icon-code-check);
}

.jp-CodeIcon {
  background-image: var(--jp-icon-code);
}

.jp-CollapseAllIcon {
  background-image: var(--jp-icon-collapse-all);
}

.jp-ConsoleIcon {
  background-image: var(--jp-icon-console);
}

.jp-CopyIcon {
  background-image: var(--jp-icon-copy);
}

.jp-CopyrightIcon {
  background-image: var(--jp-icon-copyright);
}

.jp-CutIcon {
  background-image: var(--jp-icon-cut);
}

.jp-DeleteIcon {
  background-image: var(--jp-icon-delete);
}

.jp-DownloadIcon {
  background-image: var(--jp-icon-download);
}

.jp-DuplicateIcon {
  background-image: var(--jp-icon-duplicate);
}

.jp-EditIcon {
  background-image: var(--jp-icon-edit);
}

.jp-EllipsesIcon {
  background-image: var(--jp-icon-ellipses);
}

.jp-ErrorIcon {
  background-image: var(--jp-icon-error);
}

.jp-ExpandAllIcon {
  background-image: var(--jp-icon-expand-all);
}

.jp-ExtensionIcon {
  background-image: var(--jp-icon-extension);
}

.jp-FastForwardIcon {
  background-image: var(--jp-icon-fast-forward);
}

.jp-FileIcon {
  background-image: var(--jp-icon-file);
}

.jp-FileUploadIcon {
  background-image: var(--jp-icon-file-upload);
}

.jp-FilterDotIcon {
  background-image: var(--jp-icon-filter-dot);
}

.jp-FilterIcon {
  background-image: var(--jp-icon-filter);
}

.jp-FilterListIcon {
  background-image: var(--jp-icon-filter-list);
}

.jp-FolderFavoriteIcon {
  background-image: var(--jp-icon-folder-favorite);
}

.jp-FolderIcon {
  background-image: var(--jp-icon-folder);
}

.jp-HomeIcon {
  background-image: var(--jp-icon-home);
}

.jp-Html5Icon {
  background-image: var(--jp-icon-html5);
}

.jp-ImageIcon {
  background-image: var(--jp-icon-image);
}

.jp-InfoIcon {
  background-image: var(--jp-icon-info);
}

.jp-InspectorIcon {
  background-image: var(--jp-icon-inspector);
}

.jp-JsonIcon {
  background-image: var(--jp-icon-json);
}

.jp-JuliaIcon {
  background-image: var(--jp-icon-julia);
}

.jp-JupyterFaviconIcon {
  background-image: var(--jp-icon-jupyter-favicon);
}

.jp-JupyterIcon {
  background-image: var(--jp-icon-jupyter);
}

.jp-JupyterlabWordmarkIcon {
  background-image: var(--jp-icon-jupyterlab-wordmark);
}

.jp-KernelIcon {
  background-image: var(--jp-icon-kernel);
}

.jp-KeyboardIcon {
  background-image: var(--jp-icon-keyboard);
}

.jp-LaunchIcon {
  background-image: var(--jp-icon-launch);
}

.jp-LauncherIcon {
  background-image: var(--jp-icon-launcher);
}

.jp-LineFormIcon {
  background-image: var(--jp-icon-line-form);
}

.jp-LinkIcon {
  background-image: var(--jp-icon-link);
}

.jp-ListIcon {
  background-image: var(--jp-icon-list);
}

.jp-MarkdownIcon {
  background-image: var(--jp-icon-markdown);
}

.jp-MoveDownIcon {
  background-image: var(--jp-icon-move-down);
}

.jp-MoveUpIcon {
  background-image: var(--jp-icon-move-up);
}

.jp-NewFolderIcon {
  background-image: var(--jp-icon-new-folder);
}

.jp-NotTrustedIcon {
  background-image: var(--jp-icon-not-trusted);
}

.jp-NotebookIcon {
  background-image: var(--jp-icon-notebook);
}

.jp-NumberingIcon {
  background-image: var(--jp-icon-numbering);
}

.jp-OfflineBoltIcon {
  background-image: var(--jp-icon-offline-bolt);
}

.jp-PaletteIcon {
  background-image: var(--jp-icon-palette);
}

.jp-PasteIcon {
  background-image: var(--jp-icon-paste);
}

.jp-PdfIcon {
  background-image: var(--jp-icon-pdf);
}

.jp-PythonIcon {
  background-image: var(--jp-icon-python);
}

.jp-RKernelIcon {
  background-image: var(--jp-icon-r-kernel);
}

.jp-ReactIcon {
  background-image: var(--jp-icon-react);
}

.jp-RedoIcon {
  background-image: var(--jp-icon-redo);
}

.jp-RefreshIcon {
  background-image: var(--jp-icon-refresh);
}

.jp-RegexIcon {
  background-image: var(--jp-icon-regex);
}

.jp-RunIcon {
  background-image: var(--jp-icon-run);
}

.jp-RunningIcon {
  background-image: var(--jp-icon-running);
}

.jp-SaveIcon {
  background-image: var(--jp-icon-save);
}

.jp-SearchIcon {
  background-image: var(--jp-icon-search);
}

.jp-SettingsIcon {
  background-image: var(--jp-icon-settings);
}

.jp-ShareIcon {
  background-image: var(--jp-icon-share);
}

.jp-SpreadsheetIcon {
  background-image: var(--jp-icon-spreadsheet);
}

.jp-StopIcon {
  background-image: var(--jp-icon-stop);
}

.jp-TabIcon {
  background-image: var(--jp-icon-tab);
}

.jp-TableRowsIcon {
  background-image: var(--jp-icon-table-rows);
}

.jp-TagIcon {
  background-image: var(--jp-icon-tag);
}

.jp-TerminalIcon {
  background-image: var(--jp-icon-terminal);
}

.jp-TextEditorIcon {
  background-image: var(--jp-icon-text-editor);
}

.jp-TocIcon {
  background-image: var(--jp-icon-toc);
}

.jp-TreeViewIcon {
  background-image: var(--jp-icon-tree-view);
}

.jp-TrustedIcon {
  background-image: var(--jp-icon-trusted);
}

.jp-UndoIcon {
  background-image: var(--jp-icon-undo);
}

.jp-UserIcon {
  background-image: var(--jp-icon-user);
}

.jp-UsersIcon {
  background-image: var(--jp-icon-users);
}

.jp-VegaIcon {
  background-image: var(--jp-icon-vega);
}

.jp-WordIcon {
  background-image: var(--jp-icon-word);
}

.jp-YamlIcon {
  background-image: var(--jp-icon-yaml);
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/**
 * (DEPRECATED) Support for consuming icons as CSS background images
 */

.jp-Icon,
.jp-MaterialIcon {
  background-position: center;
  background-repeat: no-repeat;
  background-size: 16px;
  min-width: 16px;
  min-height: 16px;
}

.jp-Icon-cover {
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}

/**
 * (DEPRECATED) Support for specific CSS icon sizes
 */

.jp-Icon-16 {
  background-size: 16px;
  min-width: 16px;
  min-height: 16px;
}

.jp-Icon-18 {
  background-size: 18px;
  min-width: 18px;
  min-height: 18px;
}

.jp-Icon-20 {
  background-size: 20px;
  min-width: 20px;
  min-height: 20px;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.lm-TabBar .lm-TabBar-addButton {
  align-items: center;
  display: flex;
  padding: 4px;
  padding-bottom: 5px;
  margin-right: 1px;
  background-color: var(--jp-layout-color2);
}

.lm-TabBar .lm-TabBar-addButton:hover {
  background-color: var(--jp-layout-color1);
}

.lm-DockPanel-tabBar .lm-TabBar-tab {
  width: var(--jp-private-horizontal-tab-width);
}

.lm-DockPanel-tabBar .lm-TabBar-content {
  flex: unset;
}

.lm-DockPanel-tabBar[data-orientation='horizontal'] {
  flex: 1 1 auto;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/**
 * Support for icons as inline SVG HTMLElements
 */

/* recolor the primary elements of an icon */
.jp-icon0[fill] {
  fill: var(--jp-inverse-layout-color0);
}

.jp-icon1[fill] {
  fill: var(--jp-inverse-layout-color1);
}

.jp-icon2[fill] {
  fill: var(--jp-inverse-layout-color2);
}

.jp-icon3[fill] {
  fill: var(--jp-inverse-layout-color3);
}

.jp-icon4[fill] {
  fill: var(--jp-inverse-layout-color4);
}

.jp-icon0[stroke] {
  stroke: var(--jp-inverse-layout-color0);
}

.jp-icon1[stroke] {
  stroke: var(--jp-inverse-layout-color1);
}

.jp-icon2[stroke] {
  stroke: var(--jp-inverse-layout-color2);
}

.jp-icon3[stroke] {
  stroke: var(--jp-inverse-layout-color3);
}

.jp-icon4[stroke] {
  stroke: var(--jp-inverse-layout-color4);
}

/* recolor the accent elements of an icon */
.jp-icon-accent0[fill] {
  fill: var(--jp-layout-color0);
}

.jp-icon-accent1[fill] {
  fill: var(--jp-layout-color1);
}

.jp-icon-accent2[fill] {
  fill: var(--jp-layout-color2);
}

.jp-icon-accent3[fill] {
  fill: var(--jp-layout-color3);
}

.jp-icon-accent4[fill] {
  fill: var(--jp-layout-color4);
}

.jp-icon-accent0[stroke] {
  stroke: var(--jp-layout-color0);
}

.jp-icon-accent1[stroke] {
  stroke: var(--jp-layout-color1);
}

.jp-icon-accent2[stroke] {
  stroke: var(--jp-layout-color2);
}

.jp-icon-accent3[stroke] {
  stroke: var(--jp-layout-color3);
}

.jp-icon-accent4[stroke] {
  stroke: var(--jp-layout-color4);
}

/* set the color of an icon to transparent */
.jp-icon-none[fill] {
  fill: none;
}

.jp-icon-none[stroke] {
  stroke: none;
}

/* brand icon colors. Same for light and dark */
.jp-icon-brand0[fill] {
  fill: var(--jp-brand-color0);
}

.jp-icon-brand1[fill] {
  fill: var(--jp-brand-color1);
}

.jp-icon-brand2[fill] {
  fill: var(--jp-brand-color2);
}

.jp-icon-brand3[fill] {
  fill: var(--jp-brand-color3);
}

.jp-icon-brand4[fill] {
  fill: var(--jp-brand-color4);
}

.jp-icon-brand0[stroke] {
  stroke: var(--jp-brand-color0);
}

.jp-icon-brand1[stroke] {
  stroke: var(--jp-brand-color1);
}

.jp-icon-brand2[stroke] {
  stroke: var(--jp-brand-color2);
}

.jp-icon-brand3[stroke] {
  stroke: var(--jp-brand-color3);
}

.jp-icon-brand4[stroke] {
  stroke: var(--jp-brand-color4);
}

/* warn icon colors. Same for light and dark */
.jp-icon-warn0[fill] {
  fill: var(--jp-warn-color0);
}

.jp-icon-warn1[fill] {
  fill: var(--jp-warn-color1);
}

.jp-icon-warn2[fill] {
  fill: var(--jp-warn-color2);
}

.jp-icon-warn3[fill] {
  fill: var(--jp-warn-color3);
}

.jp-icon-warn0[stroke] {
  stroke: var(--jp-warn-color0);
}

.jp-icon-warn1[stroke] {
  stroke: var(--jp-warn-color1);
}

.jp-icon-warn2[stroke] {
  stroke: var(--jp-warn-color2);
}

.jp-icon-warn3[stroke] {
  stroke: var(--jp-warn-color3);
}

/* icon colors that contrast well with each other and most backgrounds */
.jp-icon-contrast0[fill] {
  fill: var(--jp-icon-contrast-color0);
}

.jp-icon-contrast1[fill] {
  fill: var(--jp-icon-contrast-color1);
}

.jp-icon-contrast2[fill] {
  fill: var(--jp-icon-contrast-color2);
}

.jp-icon-contrast3[fill] {
  fill: var(--jp-icon-contrast-color3);
}

.jp-icon-contrast0[stroke] {
  stroke: var(--jp-icon-contrast-color0);
}

.jp-icon-contrast1[stroke] {
  stroke: var(--jp-icon-contrast-color1);
}

.jp-icon-contrast2[stroke] {
  stroke: var(--jp-icon-contrast-color2);
}

.jp-icon-contrast3[stroke] {
  stroke: var(--jp-icon-contrast-color3);
}

.jp-icon-dot[fill] {
  fill: var(--jp-warn-color0);
}

.jp-jupyter-icon-color[fill] {
  fill: var(--jp-jupyter-icon-color, var(--jp-warn-color0));
}

.jp-notebook-icon-color[fill] {
  fill: var(--jp-notebook-icon-color, var(--jp-warn-color0));
}

.jp-json-icon-color[fill] {
  fill: var(--jp-json-icon-color, var(--jp-warn-color1));
}

.jp-console-icon-color[fill] {
  fill: var(--jp-console-icon-color, white);
}

.jp-console-icon-background-color[fill] {
  fill: var(--jp-console-icon-background-color, var(--jp-brand-color1));
}

.jp-terminal-icon-color[fill] {
  fill: var(--jp-terminal-icon-color, var(--jp-layout-color2));
}

.jp-terminal-icon-background-color[fill] {
  fill: var(
    --jp-terminal-icon-background-color,
    var(--jp-inverse-layout-color2)
  );
}

.jp-text-editor-icon-color[fill] {
  fill: var(--jp-text-editor-icon-color, var(--jp-inverse-layout-color3));
}

.jp-inspector-icon-color[fill] {
  fill: var(--jp-inspector-icon-color, var(--jp-inverse-layout-color3));
}

/* CSS for icons in selected filebrowser listing items */
.jp-DirListing-item.jp-mod-selected .jp-icon-selectable[fill] {
  fill: #fff;
}

.jp-DirListing-item.jp-mod-selected .jp-icon-selectable-inverse[fill] {
  fill: var(--jp-brand-color1);
}

/* stylelint-disable selector-max-class, selector-max-compound-selectors */

/**
* TODO: come up with non css-hack solution for showing the busy icon on top
*  of the close icon
* CSS for complex behavior of close icon of tabs in the main area tabbar
*/
.lm-DockPanel-tabBar
  .lm-TabBar-tab.lm-mod-closable.jp-mod-dirty
  > .lm-TabBar-tabCloseIcon
  > :not(:hover)
  > .jp-icon3[fill] {
  fill: none;
}

.lm-DockPanel-tabBar
  .lm-TabBar-tab.lm-mod-closable.jp-mod-dirty
  > .lm-TabBar-tabCloseIcon
  > :not(:hover)
  > .jp-icon-busy[fill] {
  fill: var(--jp-inverse-layout-color3);
}

/* stylelint-enable selector-max-class, selector-max-compound-selectors */

/* CSS for icons in status bar */
#jp-main-statusbar .jp-mod-selected .jp-icon-selectable[fill] {
  fill: #fff;
}

#jp-main-statusbar .jp-mod-selected .jp-icon-selectable-inverse[fill] {
  fill: var(--jp-brand-color1);
}

/* special handling for splash icon CSS. While the theme CSS reloads during
   splash, the splash icon can loose theming. To prevent that, we set a
   default for its color variable */
:root {
  --jp-warn-color0: var(--md-orange-700);
}

/* not sure what to do with this one, used in filebrowser listing */
.jp-DragIcon {
  margin-right: 4px;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/**
 * Support for alt colors for icons as inline SVG HTMLElements
 */

/* alt recolor the primary elements of an icon */
.jp-icon-alt .jp-icon0[fill] {
  fill: var(--jp-layout-color0);
}

.jp-icon-alt .jp-icon1[fill] {
  fill: var(--jp-layout-color1);
}

.jp-icon-alt .jp-icon2[fill] {
  fill: var(--jp-layout-color2);
}

.jp-icon-alt .jp-icon3[fill] {
  fill: var(--jp-layout-color3);
}

.jp-icon-alt .jp-icon4[fill] {
  fill: var(--jp-layout-color4);
}

.jp-icon-alt .jp-icon0[stroke] {
  stroke: var(--jp-layout-color0);
}

.jp-icon-alt .jp-icon1[stroke] {
  stroke: var(--jp-layout-color1);
}

.jp-icon-alt .jp-icon2[stroke] {
  stroke: var(--jp-layout-color2);
}

.jp-icon-alt .jp-icon3[stroke] {
  stroke: var(--jp-layout-color3);
}

.jp-icon-alt .jp-icon4[stroke] {
  stroke: var(--jp-layout-color4);
}

/* alt recolor the accent elements of an icon */
.jp-icon-alt .jp-icon-accent0[fill] {
  fill: var(--jp-inverse-layout-color0);
}

.jp-icon-alt .jp-icon-accent1[fill] {
  fill: var(--jp-inverse-layout-color1);
}

.jp-icon-alt .jp-icon-accent2[fill] {
  fill: var(--jp-inverse-layout-color2);
}

.jp-icon-alt .jp-icon-accent3[fill] {
  fill: var(--jp-inverse-layout-color3);
}

.jp-icon-alt .jp-icon-accent4[fill] {
  fill: var(--jp-inverse-layout-color4);
}

.jp-icon-alt .jp-icon-accent0[stroke] {
  stroke: var(--jp-inverse-layout-color0);
}

.jp-icon-alt .jp-icon-accent1[stroke] {
  stroke: var(--jp-inverse-layout-color1);
}

.jp-icon-alt .jp-icon-accent2[stroke] {
  stroke: var(--jp-inverse-layout-color2);
}

.jp-icon-alt .jp-icon-accent3[stroke] {
  stroke: var(--jp-inverse-layout-color3);
}

.jp-icon-alt .jp-icon-accent4[stroke] {
  stroke: var(--jp-inverse-layout-color4);
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-icon-hoverShow:not(:hover) .jp-icon-hoverShow-content {
  display: none !important;
}

/**
 * Support for hover colors for icons as inline SVG HTMLElements
 */

/**
 * regular colors
 */

/* recolor the primary elements of an icon */
.jp-icon-hover :hover .jp-icon0-hover[fill] {
  fill: var(--jp-inverse-layout-color0);
}

.jp-icon-hover :hover .jp-icon1-hover[fill] {
  fill: var(--jp-inverse-layout-color1);
}

.jp-icon-hover :hover .jp-icon2-hover[fill] {
  fill: var(--jp-inverse-layout-color2);
}

.jp-icon-hover :hover .jp-icon3-hover[fill] {
  fill: var(--jp-inverse-layout-color3);
}

.jp-icon-hover :hover .jp-icon4-hover[fill] {
  fill: var(--jp-inverse-layout-color4);
}

.jp-icon-hover :hover .jp-icon0-hover[stroke] {
  stroke: var(--jp-inverse-layout-color0);
}

.jp-icon-hover :hover .jp-icon1-hover[stroke] {
  stroke: var(--jp-inverse-layout-color1);
}

.jp-icon-hover :hover .jp-icon2-hover[stroke] {
  stroke: var(--jp-inverse-layout-color2);
}

.jp-icon-hover :hover .jp-icon3-hover[stroke] {
  stroke: var(--jp-inverse-layout-color3);
}

.jp-icon-hover :hover .jp-icon4-hover[stroke] {
  stroke: var(--jp-inverse-layout-color4);
}

/* recolor the accent elements of an icon */
.jp-icon-hover :hover .jp-icon-accent0-hover[fill] {
  fill: var(--jp-layout-color0);
}

.jp-icon-hover :hover .jp-icon-accent1-hover[fill] {
  fill: var(--jp-layout-color1);
}

.jp-icon-hover :hover .jp-icon-accent2-hover[fill] {
  fill: var(--jp-layout-color2);
}

.jp-icon-hover :hover .jp-icon-accent3-hover[fill] {
  fill: var(--jp-layout-color3);
}

.jp-icon-hover :hover .jp-icon-accent4-hover[fill] {
  fill: var(--jp-layout-color4);
}

.jp-icon-hover :hover .jp-icon-accent0-hover[stroke] {
  stroke: var(--jp-layout-color0);
}

.jp-icon-hover :hover .jp-icon-accent1-hover[stroke] {
  stroke: var(--jp-layout-color1);
}

.jp-icon-hover :hover .jp-icon-accent2-hover[stroke] {
  stroke: var(--jp-layout-color2);
}

.jp-icon-hover :hover .jp-icon-accent3-hover[stroke] {
  stroke: var(--jp-layout-color3);
}

.jp-icon-hover :hover .jp-icon-accent4-hover[stroke] {
  stroke: var(--jp-layout-color4);
}

/* set the color of an icon to transparent */
.jp-icon-hover :hover .jp-icon-none-hover[fill] {
  fill: none;
}

.jp-icon-hover :hover .jp-icon-none-hover[stroke] {
  stroke: none;
}

/**
 * inverse colors
 */

/* inverse recolor the primary elements of an icon */
.jp-icon-hover.jp-icon-alt :hover .jp-icon0-hover[fill] {
  fill: var(--jp-layout-color0);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon1-hover[fill] {
  fill: var(--jp-layout-color1);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon2-hover[fill] {
  fill: var(--jp-layout-color2);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon3-hover[fill] {
  fill: var(--jp-layout-color3);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon4-hover[fill] {
  fill: var(--jp-layout-color4);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon0-hover[stroke] {
  stroke: var(--jp-layout-color0);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon1-hover[stroke] {
  stroke: var(--jp-layout-color1);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon2-hover[stroke] {
  stroke: var(--jp-layout-color2);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon3-hover[stroke] {
  stroke: var(--jp-layout-color3);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon4-hover[stroke] {
  stroke: var(--jp-layout-color4);
}

/* inverse recolor the accent elements of an icon */
.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent0-hover[fill] {
  fill: var(--jp-inverse-layout-color0);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent1-hover[fill] {
  fill: var(--jp-inverse-layout-color1);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent2-hover[fill] {
  fill: var(--jp-inverse-layout-color2);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent3-hover[fill] {
  fill: var(--jp-inverse-layout-color3);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent4-hover[fill] {
  fill: var(--jp-inverse-layout-color4);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent0-hover[stroke] {
  stroke: var(--jp-inverse-layout-color0);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent1-hover[stroke] {
  stroke: var(--jp-inverse-layout-color1);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent2-hover[stroke] {
  stroke: var(--jp-inverse-layout-color2);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent3-hover[stroke] {
  stroke: var(--jp-inverse-layout-color3);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent4-hover[stroke] {
  stroke: var(--jp-inverse-layout-color4);
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-IFrame {
  width: 100%;
  height: 100%;
}

.jp-IFrame > iframe {
  border: none;
}

/*
When drag events occur, `lm-mod-override-cursor` is added to the body.
Because iframes steal all cursor events, the following two rules are necessary
to suppress pointer events while resize drags are occurring. There may be a
better solution to this problem.
*/
body.lm-mod-override-cursor .jp-IFrame {
  position: relative;
}

body.lm-mod-override-cursor .jp-IFrame::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: transparent;
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2014-2016, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-HoverBox {
  position: fixed;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-FormGroup-content fieldset {
  border: none;
  padding: 0;
  min-width: 0;
  width: 100%;
}

/* stylelint-disable selector-max-type */

.jp-FormGroup-content fieldset .jp-inputFieldWrapper input,
.jp-FormGroup-content fieldset .jp-inputFieldWrapper select,
.jp-FormGroup-content fieldset .jp-inputFieldWrapper textarea {
  font-size: var(--jp-content-font-size2);
  border-color: var(--jp-input-border-color);
  border-style: solid;
  border-radius: var(--jp-border-radius);
  border-width: 1px;
  padding: 6px 8px;
  background: none;
  color: var(--jp-ui-font-color0);
  height: inherit;
}

.jp-FormGroup-content fieldset input[type='checkbox'] {
  position: relative;
  top: 2px;
  margin-left: 0;
}

.jp-FormGroup-content button.jp-mod-styled {
  cursor: pointer;
}

.jp-FormGroup-content .checkbox label {
  cursor: pointer;
  font-size: var(--jp-content-font-size1);
}

.jp-FormGroup-content .jp-root > fieldset > legend {
  display: none;
}

.jp-FormGroup-content .jp-root > fieldset > p {
  display: none;
}

/** copy of `input.jp-mod-styled:focus` style */
.jp-FormGroup-content fieldset input:focus,
.jp-FormGroup-content fieldset select:focus {
  -moz-outline-radius: unset;
  outline: var(--jp-border-width) solid var(--md-blue-500);
  outline-offset: -1px;
  box-shadow: inset 0 0 4px var(--md-blue-300);
}

.jp-FormGroup-content fieldset input:hover:not(:focus),
.jp-FormGroup-content fieldset select:hover:not(:focus) {
  background-color: var(--jp-border-color2);
}

/* stylelint-enable selector-max-type */

.jp-FormGroup-content .checkbox .field-description {
  /* Disable default description field for checkbox:
   because other widgets do not have description fields,
   we add descriptions to each widget on the field level.
  */
  display: none;
}

.jp-FormGroup-content #root__description {
  display: none;
}

.jp-FormGroup-content .jp-modifiedIndicator {
  width: 5px;
  background-color: var(--jp-brand-color2);
  margin-top: 0;
  margin-left: calc(var(--jp-private-settingeditor-modifier-indent) * -1);
  flex-shrink: 0;
}

.jp-FormGroup-content .jp-modifiedIndicator.jp-errorIndicator {
  background-color: var(--jp-error-color0);
  margin-right: 0.5em;
}

/* RJSF ARRAY style */

.jp-arrayFieldWrapper legend {
  font-size: var(--jp-content-font-size2);
  color: var(--jp-ui-font-color0);
  flex-basis: 100%;
  padding: 4px 0;
  font-weight: var(--jp-content-heading-font-weight);
  border-bottom: 1px solid var(--jp-border-color2);
}

.jp-arrayFieldWrapper .field-description {
  padding: 4px 0;
  white-space: pre-wrap;
}

.jp-arrayFieldWrapper .array-item {
  width: 100%;
  border: 1px solid var(--jp-border-color2);
  border-radius: 4px;
  margin: 4px;
}

.jp-ArrayOperations {
  display: flex;
  margin-left: 8px;
}

.jp-ArrayOperationsButton {
  margin: 2px;
}

.jp-ArrayOperationsButton .jp-icon3[fill] {
  fill: var(--jp-ui-font-color0);
}

button.jp-ArrayOperationsButton.jp-mod-styled:disabled {
  cursor: not-allowed;
  opacity: 0.5;
}

/* RJSF form validation error */

.jp-FormGroup-content .validationErrors {
  color: var(--jp-error-color0);
}

/* Hide panel level error as duplicated the field level error */
.jp-FormGroup-content .panel.errors {
  display: none;
}

/* RJSF normal content (settings-editor) */

.jp-FormGroup-contentNormal {
  display: flex;
  align-items: center;
  flex-wrap: wrap;
}

.jp-FormGroup-contentNormal .jp-FormGroup-contentItem {
  margin-left: 7px;
  color: var(--jp-ui-font-color0);
}

.jp-FormGroup-contentNormal .jp-FormGroup-description {
  flex-basis: 100%;
  padding: 4px 7px;
}

.jp-FormGroup-contentNormal .jp-FormGroup-default {
  flex-basis: 100%;
  padding: 4px 7px;
}

.jp-FormGroup-contentNormal .jp-FormGroup-fieldLabel {
  font-size: var(--jp-content-font-size1);
  font-weight: normal;
  min-width: 120px;
}

.jp-FormGroup-contentNormal fieldset:not(:first-child) {
  margin-left: 7px;
}

.jp-FormGroup-contentNormal .field-array-of-string .array-item {
  /* Display `jp-ArrayOperations` buttons side-by-side with content except
    for small screens where flex-wrap will place them one below the other.
  */
  display: flex;
  align-items: center;
  flex-wrap: wrap;
}

.jp-FormGroup-contentNormal .jp-objectFieldWrapper .form-group {
  padding: 2px 8px 2px var(--jp-private-settingeditor-modifier-indent);
  margin-top: 2px;
}

/* RJSF compact content (metadata-form) */

.jp-FormGroup-content.jp-FormGroup-contentCompact {
  width: 100%;
}

.jp-FormGroup-contentCompact .form-group {
  display: flex;
  padding: 0.5em 0.2em 0.5em 0;
}

.jp-FormGroup-contentCompact
  .jp-FormGroup-compactTitle
  .jp-FormGroup-description {
  font-size: var(--jp-ui-font-size1);
  color: var(--jp-ui-font-color2);
}

.jp-FormGroup-contentCompact .jp-FormGroup-fieldLabel {
  padding-bottom: 0.3em;
}

.jp-FormGroup-contentCompact .jp-inputFieldWrapper .form-control {
  width: 100%;
  box-sizing: border-box;
}

.jp-FormGroup-contentCompact .jp-arrayFieldWrapper .jp-FormGroup-compactTitle {
  padding-bottom: 7px;
}

.jp-FormGroup-contentCompact
  .jp-objectFieldWrapper
  .jp-objectFieldWrapper
  .form-group {
  padding: 2px 8px 2px var(--jp-private-settingeditor-modifier-indent);
  margin-top: 2px;
}

.jp-FormGroup-contentCompact ul.error-detail {
  margin-block-start: 0.5em;
  margin-block-end: 0.5em;
  padding-inline-start: 1em;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

.jp-SidePanel {
  display: flex;
  flex-direction: column;
  min-width: var(--jp-sidebar-min-width);
  overflow-y: auto;
  color: var(--jp-ui-font-color1);
  background: var(--jp-layout-color1);
  font-size: var(--jp-ui-font-size1);
}

.jp-SidePanel-header {
  flex: 0 0 auto;
  display: flex;
  border-bottom: var(--jp-border-width) solid var(--jp-border-color2);
  font-size: var(--jp-ui-font-size0);
  font-weight: 600;
  letter-spacing: 1px;
  margin: 0;
  padding: 2px;
  text-transform: uppercase;
}

.jp-SidePanel-toolbar {
  flex: 0 0 auto;
}

.jp-SidePanel-content {
  flex: 1 1 auto;
}

.jp-SidePanel-toolbar,
.jp-AccordionPanel-toolbar {
  height: var(--jp-private-toolbar-height);
}

.jp-SidePanel-toolbar.jp-Toolbar-micro {
  display: none;
}

.lm-AccordionPanel .jp-AccordionPanel-title {
  box-sizing: border-box;
  line-height: 25px;
  margin: 0;
  display: flex;
  align-items: center;
  background: var(--jp-layout-color1);
  color: var(--jp-ui-font-color1);
  border-bottom: var(--jp-border-width) solid var(--jp-toolbar-border-color);
  box-shadow: var(--jp-toolbar-box-shadow);
  font-size: var(--jp-ui-font-size0);
}

.jp-AccordionPanel-title {
  cursor: pointer;
  user-select: none;
  -moz-user-select: none;
  -webkit-user-select: none;
  text-transform: uppercase;
}

.lm-AccordionPanel[data-orientation='horizontal'] > .jp-AccordionPanel-title {
  /* Title is rotated for horizontal accordion panel using CSS */
  display: block;
  transform-origin: top left;
  transform: rotate(-90deg) translate(-100%);
}

.jp-AccordionPanel-title .lm-AccordionPanel-titleLabel {
  user-select: none;
  text-overflow: ellipsis;
  white-space: nowrap;
  overflow: hidden;
}

.jp-AccordionPanel-title .lm-AccordionPanel-titleCollapser {
  transform: rotate(-90deg);
  margin: auto 0;
  height: 16px;
}

.jp-AccordionPanel-title.lm-mod-expanded .lm-AccordionPanel-titleCollapser {
  transform: rotate(0deg);
}

.lm-AccordionPanel .jp-AccordionPanel-toolbar {
  background: none;
  box-shadow: none;
  border: none;
  margin-left: auto;
}

.lm-AccordionPanel .lm-SplitPanel-handle:hover {
  background: var(--jp-layout-color3);
}

.jp-text-truncated {
  overflow: hidden;
  text-overflow: ellipsis;
  white-space: nowrap;
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2017, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-Spinner {
  position: absolute;
  display: flex;
  justify-content: center;
  align-items: center;
  z-index: 10;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  background: var(--jp-layout-color0);
  outline: none;
}

.jp-SpinnerContent {
  font-size: 10px;
  margin: 50px auto;
  text-indent: -9999em;
  width: 3em;
  height: 3em;
  border-radius: 50%;
  background: var(--jp-brand-color3);
  background: linear-gradient(
    to right,
    #f37626 10%,
    rgba(255, 255, 255, 0) 42%
  );
  position: relative;
  animation: load3 1s infinite linear, fadeIn 1s;
}

.jp-SpinnerContent::before {
  width: 50%;
  height: 50%;
  background: #f37626;
  border-radius: 100% 0 0;
  position: absolute;
  top: 0;
  left: 0;
  content: '';
}

.jp-SpinnerContent::after {
  background: var(--jp-layout-color0);
  width: 75%;
  height: 75%;
  border-radius: 50%;
  content: '';
  margin: auto;
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  right: 0;
}

@keyframes fadeIn {
  0% {
    opacity: 0;
  }

  100% {
    opacity: 1;
  }
}

@keyframes load3 {
  0% {
    transform: rotate(0deg);
  }

  100% {
    transform: rotate(360deg);
  }
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2014-2017, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

button.jp-mod-styled {
  font-size: var(--jp-ui-font-size1);
  color: var(--jp-ui-font-color0);
  border: none;
  box-sizing: border-box;
  text-align: center;
  line-height: 32px;
  height: 32px;
  padding: 0 12px;
  letter-spacing: 0.8px;
  outline: none;
  appearance: none;
  -webkit-appearance: none;
  -moz-appearance: none;
}

input.jp-mod-styled {
  background: var(--jp-input-background);
  height: 28px;
  box-sizing: border-box;
  border: var(--jp-border-width) solid var(--jp-border-color1);
  padding-left: 7px;
  padding-right: 7px;
  font-size: var(--jp-ui-font-size2);
  color: var(--jp-ui-font-color0);
  outline: none;
  appearance: none;
  -webkit-appearance: none;
  -moz-appearance: none;
}

input[type='checkbox'].jp-mod-styled {
  appearance: checkbox;
  -webkit-appearance: checkbox;
  -moz-appearance: checkbox;
  height: auto;
}

input.jp-mod-styled:focus {
  border: var(--jp-border-width) solid var(--md-blue-500);
  box-shadow: inset 0 0 4px var(--md-blue-300);
}

.jp-select-wrapper {
  display: flex;
  position: relative;
  flex-direction: column;
  padding: 1px;
  background-color: var(--jp-layout-color1);
  box-sizing: border-box;
  margin-bottom: 12px;
}

.jp-select-wrapper:not(.multiple) {
  height: 28px;
}

.jp-select-wrapper.jp-mod-focused select.jp-mod-styled {
  border: var(--jp-border-width) solid var(--jp-input-active-border-color);
  box-shadow: var(--jp-input-box-shadow);
  background-color: var(--jp-input-active-background);
}

select.jp-mod-styled:hover {
  cursor: pointer;
  color: var(--jp-ui-font-color0);
  background-color: var(--jp-input-hover-background);
  box-shadow: inset 0 0 1px rgba(0, 0, 0, 0.5);
}

select.jp-mod-styled {
  flex: 1 1 auto;
  width: 100%;
  font-size: var(--jp-ui-font-size2);
  background: var(--jp-input-background);
  color: var(--jp-ui-font-color0);
  padding: 0 25px 0 8px;
  border: var(--jp-border-width) solid var(--jp-input-border-color);
  border-radius: 0;
  outline: none;
  appearance: none;
  -webkit-appearance: none;
  -moz-appearance: none;
}

select.jp-mod-styled:not([multiple]) {
  height: 32px;
}

select.jp-mod-styled[multiple] {
  max-height: 200px;
  overflow-y: auto;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-switch {
  display: flex;
  align-items: center;
  padding-left: 4px;
  padding-right: 4px;
  font-size: var(--jp-ui-font-size1);
  background-color: transparent;
  color: var(--jp-ui-font-color1);
  border: none;
  height: 20px;
}

.jp-switch:hover {
  background-color: var(--jp-layout-color2);
}

.jp-switch-label {
  margin-right: 5px;
  font-family: var(--jp-ui-font-family);
}

.jp-switch-track {
  cursor: pointer;
  background-color: var(--jp-switch-color, var(--jp-border-color1));
  -webkit-transition: 0.4s;
  transition: 0.4s;
  border-radius: 34px;
  height: 16px;
  width: 35px;
  position: relative;
}

.jp-switch-track::before {
  content: '';
  position: absolute;
  height: 10px;
  width: 10px;
  margin: 3px;
  left: 0;
  background-color: var(--jp-ui-inverse-font-color1);
  -webkit-transition: 0.4s;
  transition: 0.4s;
  border-radius: 50%;
}

.jp-switch[aria-checked='true'] .jp-switch-track {
  background-color: var(--jp-switch-true-position-color, var(--jp-warn-color0));
}

.jp-switch[aria-checked='true'] .jp-switch-track::before {
  /* track width (35) - margins (3 + 3) - thumb width (10) */
  left: 19px;
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2014-2016, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

:root {
  --jp-private-toolbar-height: calc(
    28px + var(--jp-border-width)
  ); /* leave 28px for content */
}

.jp-Toolbar {
  color: var(--jp-ui-font-color1);
  flex: 0 0 auto;
  display: flex;
  flex-direction: row;
  border-bottom: var(--jp-border-width) solid var(--jp-toolbar-border-color);
  box-shadow: var(--jp-toolbar-box-shadow);
  background: var(--jp-toolbar-background);
  min-height: var(--jp-toolbar-micro-height);
  padding: 2px;
  z-index: 8;
  overflow-x: hidden;
}

/* Toolbar items */

.jp-Toolbar > .jp-Toolbar-item.jp-Toolbar-spacer {
  flex-grow: 1;
  flex-shrink: 1;
}

.jp-Toolbar-item.jp-Toolbar-kernelStatus {
  display: inline-block;
  width: 32px;
  background-repeat: no-repeat;
  background-position: center;
  background-size: 16px;
}

.jp-Toolbar > .jp-Toolbar-item {
  flex: 0 0 auto;
  display: flex;
  padding-left: 1px;
  padding-right: 1px;
  font-size: var(--jp-ui-font-size1);
  line-height: var(--jp-private-toolbar-height);
  height: 100%;
}

/* Toolbar buttons */

/* This is the div we use to wrap the react component into a Widget */
div.jp-ToolbarButton {
  color: transparent;
  border: none;
  box-sizing: border-box;
  outline: none;
  appearance: none;
  -webkit-appearance: none;
  -moz-appearance: none;
  padding: 0;
  margin: 0;
}

button.jp-ToolbarButtonComponent {
  background: var(--jp-layout-color1);
  border: none;
  box-sizing: border-box;
  outline: none;
  appearance: none;
  -webkit-appearance: none;
  -moz-appearance: none;
  padding: 0 6px;
  margin: 0;
  height: 24px;
  border-radius: var(--jp-border-radius);
  display: flex;
  align-items: center;
  text-align: center;
  font-size: 14px;
  min-width: unset;
  min-height: unset;
}

button.jp-ToolbarButtonComponent:disabled {
  opacity: 0.4;
}

button.jp-ToolbarButtonComponent > span {
  padding: 0;
  flex: 0 0 auto;
}

button.jp-ToolbarButtonComponent .jp-ToolbarButtonComponent-label {
  font-size: var(--jp-ui-font-size1);
  line-height: 100%;
  padding-left: 2px;
  color: var(--jp-ui-font-color1);
  font-family: var(--jp-ui-font-family);
}

#jp-main-dock-panel[data-mode='single-document']
  .jp-MainAreaWidget
  > .jp-Toolbar.jp-Toolbar-micro {
  padding: 0;
  min-height: 0;
}

#jp-main-dock-panel[data-mode='single-document']
  .jp-MainAreaWidget
  > .jp-Toolbar {
  border: none;
  box-shadow: none;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

.jp-WindowedPanel-outer {
  position: relative;
  overflow-y: auto;
}

.jp-WindowedPanel-inner {
  position: relative;
}

.jp-WindowedPanel-window {
  position: absolute;
  left: 0;
  right: 0;
  overflow: visible;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/* Sibling imports */

body {
  color: var(--jp-ui-font-color1);
  font-size: var(--jp-ui-font-size1);
}

/* Disable native link decoration styles everywhere outside of dialog boxes */
a {
  text-decoration: unset;
  color: unset;
}

a:hover {
  text-decoration: unset;
  color: unset;
}

/* Accessibility for links inside dialog box text */
.jp-Dialog-content a {
  text-decoration: revert;
  color: var(--jp-content-link-color);
}

.jp-Dialog-content a:hover {
  text-decoration: revert;
}

/* Styles for ui-components */
.jp-Button {
  color: var(--jp-ui-font-color2);
  border-radius: var(--jp-border-radius);
  padding: 0 12px;
  font-size: var(--jp-ui-font-size1);

  /* Copy from blueprint 3 */
  display: inline-flex;
  flex-direction: row;
  border: none;
  cursor: pointer;
  align-items: center;
  justify-content: center;
  text-align: left;
  vertical-align: middle;
  min-height: 30px;
  min-width: 30px;
}

.jp-Button:disabled {
  cursor: not-allowed;
}

.jp-Button:empty {
  padding: 0 !important;
}

.jp-Button.jp-mod-small {
  min-height: 24px;
  min-width: 24px;
  font-size: 12px;
  padding: 0 7px;
}

/* Use our own theme for hover styles */
.jp-Button.jp-mod-minimal:hover {
  background-color: var(--jp-layout-color2);
}

.jp-Button.jp-mod-minimal {
  background: none;
}

.jp-InputGroup {
  display: block;
  position: relative;
}

.jp-InputGroup input {
  box-sizing: border-box;
  border: none;
  border-radius: 0;
  background-color: transparent;
  color: var(--jp-ui-font-color0);
  box-shadow: inset 0 0 0 var(--jp-border-width) var(--jp-input-border-color);
  padding-bottom: 0;
  padding-top: 0;
  padding-left: 10px;
  padding-right: 28px;
  position: relative;
  width: 100%;
  -webkit-appearance: none;
  -moz-appearance: none;
  appearance: none;
  font-size: 14px;
  font-weight: 400;
  height: 30px;
  line-height: 30px;
  outline: none;
  vertical-align: middle;
}

.jp-InputGroup input:focus {
  box-shadow: inset 0 0 0 var(--jp-border-width)
      var(--jp-input-active-box-shadow-color),
    inset 0 0 0 3px var(--jp-input-active-box-shadow-color);
}

.jp-InputGroup input:disabled {
  cursor: not-allowed;
  resize: block;
  background-color: var(--jp-layout-color2);
  color: var(--jp-ui-font-color2);
}

.jp-InputGroup input:disabled ~ span {
  cursor: not-allowed;
  color: var(--jp-ui-font-color2);
}

.jp-InputGroup input::placeholder,
input::placeholder {
  color: var(--jp-ui-font-color2);
}

.jp-InputGroupAction {
  position: absolute;
  bottom: 1px;
  right: 0;
  padding: 6px;
}

.jp-HTMLSelect.jp-DefaultStyle select {
  background-color: initial;
  border: none;
  border-radius: 0;
  box-shadow: none;
  color: var(--jp-ui-font-color0);
  display: block;
  font-size: var(--jp-ui-font-size1);
  font-family: var(--jp-ui-font-family);
  height: 24px;
  line-height: 14px;
  padding: 0 25px 0 10px;
  text-align: left;
  -moz-appearance: none;
  -webkit-appearance: none;
}

.jp-HTMLSelect.jp-DefaultStyle select:disabled {
  background-color: var(--jp-layout-color2);
  color: var(--jp-ui-font-color2);
  cursor: not-allowed;
  resize: block;
}

.jp-HTMLSelect.jp-DefaultStyle select:disabled ~ span {
  cursor: not-allowed;
}

/* Use our own theme for hover and option styles */
/* stylelint-disable-next-line selector-max-type */
.jp-HTMLSelect.jp-DefaultStyle select:hover,
.jp-HTMLSelect.jp-DefaultStyle select > option {
  background-color: var(--jp-layout-color2);
  color: var(--jp-ui-font-color0);
}

select {
  box-sizing: border-box;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Styles
|----------------------------------------------------------------------------*/

.jp-StatusBar-Widget {
  display: flex;
  align-items: center;
  background: var(--jp-layout-color2);
  min-height: var(--jp-statusbar-height);
  justify-content: space-between;
  padding: 0 10px;
}

.jp-StatusBar-Left {
  display: flex;
  align-items: center;
  flex-direction: row;
}

.jp-StatusBar-Middle {
  display: flex;
  align-items: center;
}

.jp-StatusBar-Right {
  display: flex;
  align-items: center;
  flex-direction: row-reverse;
}

.jp-StatusBar-Item {
  max-height: var(--jp-statusbar-height);
  margin: 0 2px;
  height: var(--jp-statusbar-height);
  white-space: nowrap;
  text-overflow: ellipsis;
  color: var(--jp-ui-font-color1);
  padding: 0 6px;
}

.jp-mod-highlighted:hover {
  background-color: var(--jp-layout-color3);
}

.jp-mod-clicked {
  background-color: var(--jp-brand-color1);
}

.jp-mod-clicked:hover {
  background-color: var(--jp-brand-color0);
}

.jp-mod-clicked .jp-StatusBar-TextItem {
  color: var(--jp-ui-inverse-font-color1);
}

.jp-StatusBar-HoverItem {
  box-shadow: '0px 4px 4px rgba(0, 0, 0, 0.25)';
}

.jp-StatusBar-TextItem {
  font-size: var(--jp-ui-font-size1);
  font-family: var(--jp-ui-font-family);
  line-height: 24px;
  color: var(--jp-ui-font-color1);
}

.jp-StatusBar-GroupItem {
  display: flex;
  align-items: center;
  flex-direction: row;
}

.jp-Statusbar-ProgressCircle svg {
  display: block;
  margin: 0 auto;
  width: 16px;
  height: 24px;
  align-self: normal;
}

.jp-Statusbar-ProgressCircle path {
  fill: var(--jp-inverse-layout-color3);
}

.jp-Statusbar-ProgressBar-progress-bar {
  height: 10px;
  width: 100px;
  border: solid 0.25px var(--jp-brand-color2);
  border-radius: 3px;
  overflow: hidden;
  align-self: center;
}

.jp-Statusbar-ProgressBar-progress-bar > div {
  background-color: var(--jp-brand-color2);
  background-image: linear-gradient(
    -45deg,
    rgba(255, 255, 255, 0.2) 25%,
    transparent 25%,
    transparent 50%,
    rgba(255, 255, 255, 0.2) 50%,
    rgba(255, 255, 255, 0.2) 75%,
    transparent 75%,
    transparent
  );
  background-size: 40px 40px;
  float: left;
  width: 0%;
  height: 100%;
  font-size: 12px;
  line-height: 14px;
  color: #fff;
  text-align: center;
  animation: jp-Statusbar-ExecutionTime-progress-bar 2s linear infinite;
}

.jp-Statusbar-ProgressBar-progress-bar p {
  color: var(--jp-ui-font-color1);
  font-family: var(--jp-ui-font-family);
  font-size: var(--jp-ui-font-size1);
  line-height: 10px;
  width: 100px;
}

@keyframes jp-Statusbar-ExecutionTime-progress-bar {
  0% {
    background-position: 0 0;
  }

  100% {
    background-position: 40px 40px;
  }
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Variables
|----------------------------------------------------------------------------*/

:root {
  --jp-private-commandpalette-search-height: 28px;
}

/*-----------------------------------------------------------------------------
| Overall styles
|----------------------------------------------------------------------------*/

.lm-CommandPalette {
  padding-bottom: 0;
  color: var(--jp-ui-font-color1);
  background: var(--jp-layout-color1);

  /* This is needed so that all font sizing of children done in ems is
   * relative to this base size */
  font-size: var(--jp-ui-font-size1);
}

/*-----------------------------------------------------------------------------
| Modal variant
|----------------------------------------------------------------------------*/

.jp-ModalCommandPalette {
  position: absolute;
  z-index: 10000;
  top: 38px;
  left: 30%;
  margin: 0;
  padding: 4px;
  width: 40%;
  box-shadow: var(--jp-elevation-z4);
  border-radius: 4px;
  background: var(--jp-layout-color0);
}

.jp-ModalCommandPalette .lm-CommandPalette {
  max-height: 40vh;
}

.jp-ModalCommandPalette .lm-CommandPalette .lm-close-icon::after {
  display: none;
}

.jp-ModalCommandPalette .lm-CommandPalette .lm-CommandPalette-header {
  display: none;
}

.jp-ModalCommandPalette .lm-CommandPalette .lm-CommandPalette-item {
  margin-left: 4px;
  margin-right: 4px;
}

.jp-ModalCommandPalette
  .lm-CommandPalette
  .lm-CommandPalette-item.lm-mod-disabled {
  display: none;
}

/*-----------------------------------------------------------------------------
| Search
|----------------------------------------------------------------------------*/

.lm-CommandPalette-search {
  padding: 4px;
  background-color: var(--jp-layout-color1);
  z-index: 2;
}

.lm-CommandPalette-wrapper {
  overflow: overlay;
  padding: 0 9px;
  background-color: var(--jp-input-active-background);
  height: 30px;
  box-shadow: inset 0 0 0 var(--jp-border-width) var(--jp-input-border-color);
}

.lm-CommandPalette.lm-mod-focused .lm-CommandPalette-wrapper {
  box-shadow: inset 0 0 0 1px var(--jp-input-active-box-shadow-color),
    inset 0 0 0 3px var(--jp-input-active-box-shadow-color);
}

.jp-SearchIconGroup {
  color: white;
  background-color: var(--jp-brand-color1);
  position: absolute;
  top: 4px;
  right: 4px;
  padding: 5px 5px 1px;
}

.jp-SearchIconGroup svg {
  height: 20px;
  width: 20px;
}

.jp-SearchIconGroup .jp-icon3[fill] {
  fill: var(--jp-layout-color0);
}

.lm-CommandPalette-input {
  background: transparent;
  width: calc(100% - 18px);
  float: left;
  border: none;
  outline: none;
  font-size: var(--jp-ui-font-size1);
  color: var(--jp-ui-font-color0);
  line-height: var(--jp-private-commandpalette-search-height);
}

.lm-CommandPalette-input::-webkit-input-placeholder,
.lm-CommandPalette-input::-moz-placeholder,
.lm-CommandPalette-input:-ms-input-placeholder {
  color: var(--jp-ui-font-color2);
  font-size: var(--jp-ui-font-size1);
}

/*-----------------------------------------------------------------------------
| Results
|----------------------------------------------------------------------------*/

.lm-CommandPalette-header:first-child {
  margin-top: 0;
}

.lm-CommandPalette-header {
  border-bottom: solid var(--jp-border-width) var(--jp-border-color2);
  color: var(--jp-ui-font-color1);
  cursor: pointer;
  display: flex;
  font-size: var(--jp-ui-font-size0);
  font-weight: 600;
  letter-spacing: 1px;
  margin-top: 8px;
  padding: 8px 0 8px 12px;
  text-transform: uppercase;
}

.lm-CommandPalette-header.lm-mod-active {
  background: var(--jp-layout-color2);
}

.lm-CommandPalette-header > mark {
  background-color: transparent;
  font-weight: bold;
  color: var(--jp-ui-font-color1);
}

.lm-CommandPalette-item {
  padding: 4px 12px 4px 4px;
  color: var(--jp-ui-font-color1);
  font-size: var(--jp-ui-font-size1);
  font-weight: 400;
  display: flex;
}

.lm-CommandPalette-item.lm-mod-disabled {
  color: var(--jp-ui-font-color2);
}

.lm-CommandPalette-item.lm-mod-active {
  color: var(--jp-ui-inverse-font-color1);
  background: var(--jp-brand-color1);
}

.lm-CommandPalette-item.lm-mod-active .lm-CommandPalette-itemLabel > mark {
  color: var(--jp-ui-inverse-font-color0);
}

.lm-CommandPalette-item.lm-mod-active .jp-icon-selectable[fill] {
  fill: var(--jp-layout-color0);
}

.lm-CommandPalette-item.lm-mod-active:hover:not(.lm-mod-disabled) {
  color: var(--jp-ui-inverse-font-color1);
  background: var(--jp-brand-color1);
}

.lm-CommandPalette-item:hover:not(.lm-mod-active):not(.lm-mod-disabled) {
  background: var(--jp-layout-color2);
}

.lm-CommandPalette-itemContent {
  overflow: hidden;
}

.lm-CommandPalette-itemLabel > mark {
  color: var(--jp-ui-font-color0);
  background-color: transparent;
  font-weight: bold;
}

.lm-CommandPalette-item.lm-mod-disabled mark {
  color: var(--jp-ui-font-color2);
}

.lm-CommandPalette-item .lm-CommandPalette-itemIcon {
  margin: 0 4px 0 0;
  position: relative;
  width: 16px;
  top: 2px;
  flex: 0 0 auto;
}

.lm-CommandPalette-item.lm-mod-disabled .lm-CommandPalette-itemIcon {
  opacity: 0.6;
}

.lm-CommandPalette-item .lm-CommandPalette-itemShortcut {
  flex: 0 0 auto;
}

.lm-CommandPalette-itemCaption {
  display: none;
}

.lm-CommandPalette-content {
  background-color: var(--jp-layout-color1);
}

.lm-CommandPalette-content:empty::after {
  content: 'No results';
  margin: auto;
  margin-top: 20px;
  width: 100px;
  display: block;
  font-size: var(--jp-ui-font-size2);
  font-family: var(--jp-ui-font-family);
  font-weight: lighter;
}

.lm-CommandPalette-emptyMessage {
  text-align: center;
  margin-top: 24px;
  line-height: 1.32;
  padding: 0 8px;
  color: var(--jp-content-font-color3);
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2014-2017, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-Dialog {
  position: absolute;
  z-index: 10000;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  top: 0;
  left: 0;
  margin: 0;
  padding: 0;
  width: 100%;
  height: 100%;
  background: var(--jp-dialog-background);
}

.jp-Dialog-content {
  display: flex;
  flex-direction: column;
  margin-left: auto;
  margin-right: auto;
  background: var(--jp-layout-color1);
  padding: 24px 24px 12px;
  min-width: 300px;
  min-height: 150px;
  max-width: 1000px;
  max-height: 500px;
  box-sizing: border-box;
  box-shadow: var(--jp-elevation-z20);
  word-wrap: break-word;
  border-radius: var(--jp-border-radius);

  /* This is needed so that all font sizing of children done in ems is
   * relative to this base size */
  font-size: var(--jp-ui-font-size1);
  color: var(--jp-ui-font-color1);
  resize: both;
}

.jp-Dialog-content.jp-Dialog-content-small {
  max-width: 500px;
}

.jp-Dialog-button {
  overflow: visible;
}

button.jp-Dialog-button:focus {
  outline: 1px solid var(--jp-brand-color1);
  outline-offset: 4px;
  -moz-outline-radius: 0;
}

button.jp-Dialog-button:focus::-moz-focus-inner {
  border: 0;
}

button.jp-Dialog-button.jp-mod-styled.jp-mod-accept:focus,
button.jp-Dialog-button.jp-mod-styled.jp-mod-warn:focus,
button.jp-Dialog-button.jp-mod-styled.jp-mod-reject:focus {
  outline-offset: 4px;
  -moz-outline-radius: 0;
}

button.jp-Dialog-button.jp-mod-styled.jp-mod-accept:focus {
  outline: 1px solid var(--jp-accept-color-normal, var(--jp-brand-color1));
}

button.jp-Dialog-button.jp-mod-styled.jp-mod-warn:focus {
  outline: 1px solid var(--jp-warn-color-normal, var(--jp-error-color1));
}

button.jp-Dialog-button.jp-mod-styled.jp-mod-reject:focus {
  outline: 1px solid var(--jp-reject-color-normal, var(--md-grey-600));
}

button.jp-Dialog-close-button {
  padding: 0;
  height: 100%;
  min-width: unset;
  min-height: unset;
}

.jp-Dialog-header {
  display: flex;
  justify-content: space-between;
  flex: 0 0 auto;
  padding-bottom: 12px;
  font-size: var(--jp-ui-font-size3);
  font-weight: 400;
  color: var(--jp-ui-font-color1);
}

.jp-Dialog-body {
  display: flex;
  flex-direction: column;
  flex: 1 1 auto;
  font-size: var(--jp-ui-font-size1);
  background: var(--jp-layout-color1);
  color: var(--jp-ui-font-color1);
  overflow: auto;
}

.jp-Dialog-footer {
  display: flex;
  flex-direction: row;
  justify-content: flex-end;
  align-items: center;
  flex: 0 0 auto;
  margin-left: -12px;
  margin-right: -12px;
  padding: 12px;
}

.jp-Dialog-checkbox {
  padding-right: 5px;
}

.jp-Dialog-checkbox > input:focus-visible {
  outline: 1px solid var(--jp-input-active-border-color);
  outline-offset: 1px;
}

.jp-Dialog-spacer {
  flex: 1 1 auto;
}

.jp-Dialog-title {
  overflow: hidden;
  white-space: nowrap;
  text-overflow: ellipsis;
}

.jp-Dialog-body > .jp-select-wrapper {
  width: 100%;
}

.jp-Dialog-body > button {
  padding: 0 16px;
}

.jp-Dialog-body > label {
  line-height: 1.4;
  color: var(--jp-ui-font-color0);
}

.jp-Dialog-button.jp-mod-styled:not(:last-child) {
  margin-right: 12px;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

.jp-Input-Boolean-Dialog {
  flex-direction: row-reverse;
  align-items: end;
  width: 100%;
}

.jp-Input-Boolean-Dialog > label {
  flex: 1 1 auto;
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2014-2016, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-MainAreaWidget > :focus {
  outline: none;
}

.jp-MainAreaWidget .jp-MainAreaWidget-error {
  padding: 6px;
}

.jp-MainAreaWidget .jp-MainAreaWidget-error > pre {
  width: auto;
  padding: 10px;
  background: var(--jp-error-color3);
  border: var(--jp-border-width) solid var(--jp-error-color1);
  border-radius: var(--jp-border-radius);
  color: var(--jp-ui-font-color1);
  font-size: var(--jp-ui-font-size1);
  white-space: pre-wrap;
  word-wrap: break-word;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/**
 * google-material-color v1.2.6
 * https://github.com/danlevan/google-material-color
 */
:root {
  --md-red-50: #ffebee;
  --md-red-100: #ffcdd2;
  --md-red-200: #ef9a9a;
  --md-red-300: #e57373;
  --md-red-400: #ef5350;
  --md-red-500: #f44336;
  --md-red-600: #e53935;
  --md-red-700: #d32f2f;
  --md-red-800: #c62828;
  --md-red-900: #b71c1c;
  --md-red-A100: #ff8a80;
  --md-red-A200: #ff5252;
  --md-red-A400: #ff1744;
  --md-red-A700: #d50000;
  --md-pink-50: #fce4ec;
  --md-pink-100: #f8bbd0;
  --md-pink-200: #f48fb1;
  --md-pink-300: #f06292;
  --md-pink-400: #ec407a;
  --md-pink-500: #e91e63;
  --md-pink-600: #d81b60;
  --md-pink-700: #c2185b;
  --md-pink-800: #ad1457;
  --md-pink-900: #880e4f;
  --md-pink-A100: #ff80ab;
  --md-pink-A200: #ff4081;
  --md-pink-A400: #f50057;
  --md-pink-A700: #c51162;
  --md-purple-50: #f3e5f5;
  --md-purple-100: #e1bee7;
  --md-purple-200: #ce93d8;
  --md-purple-300: #ba68c8;
  --md-purple-400: #ab47bc;
  --md-purple-500: #9c27b0;
  --md-purple-600: #8e24aa;
  --md-purple-700: #7b1fa2;
  --md-purple-800: #6a1b9a;
  --md-purple-900: #4a148c;
  --md-purple-A100: #ea80fc;
  --md-purple-A200: #e040fb;
  --md-purple-A400: #d500f9;
  --md-purple-A700: #a0f;
  --md-deep-purple-50: #ede7f6;
  --md-deep-purple-100: #d1c4e9;
  --md-deep-purple-200: #b39ddb;
  --md-deep-purple-300: #9575cd;
  --md-deep-purple-400: #7e57c2;
  --md-deep-purple-500: #673ab7;
  --md-deep-purple-600: #5e35b1;
  --md-deep-purple-700: #512da8;
  --md-deep-purple-800: #4527a0;
  --md-deep-purple-900: #311b92;
  --md-deep-purple-A100: #b388ff;
  --md-deep-purple-A200: #7c4dff;
  --md-deep-purple-A400: #651fff;
  --md-deep-purple-A700: #6200ea;
  --md-indigo-50: #e8eaf6;
  --md-indigo-100: #c5cae9;
  --md-indigo-200: #9fa8da;
  --md-indigo-300: #7986cb;
  --md-indigo-400: #5c6bc0;
  --md-indigo-500: #3f51b5;
  --md-indigo-600: #3949ab;
  --md-indigo-700: #303f9f;
  --md-indigo-800: #283593;
  --md-indigo-900: #1a237e;
  --md-indigo-A100: #8c9eff;
  --md-indigo-A200: #536dfe;
  --md-indigo-A400: #3d5afe;
  --md-indigo-A700: #304ffe;
  --md-blue-50: #e3f2fd;
  --md-blue-100: #bbdefb;
  --md-blue-200: #90caf9;
  --md-blue-300: #64b5f6;
  --md-blue-400: #42a5f5;
  --md-blue-500: #2196f3;
  --md-blue-600: #1e88e5;
  --md-blue-700: #1976d2;
  --md-blue-800: #1565c0;
  --md-blue-900: #0d47a1;
  --md-blue-A100: #82b1ff;
  --md-blue-A200: #448aff;
  --md-blue-A400: #2979ff;
  --md-blue-A700: #2962ff;
  --md-light-blue-50: #e1f5fe;
  --md-light-blue-100: #b3e5fc;
  --md-light-blue-200: #81d4fa;
  --md-light-blue-300: #4fc3f7;
  --md-light-blue-400: #29b6f6;
  --md-light-blue-500: #03a9f4;
  --md-light-blue-600: #039be5;
  --md-light-blue-700: #0288d1;
  --md-light-blue-800: #0277bd;
  --md-light-blue-900: #01579b;
  --md-light-blue-A100: #80d8ff;
  --md-light-blue-A200: #40c4ff;
  --md-light-blue-A400: #00b0ff;
  --md-light-blue-A700: #0091ea;
  --md-cyan-50: #e0f7fa;
  --md-cyan-100: #b2ebf2;
  --md-cyan-200: #80deea;
  --md-cyan-300: #4dd0e1;
  --md-cyan-400: #26c6da;
  --md-cyan-500: #00bcd4;
  --md-cyan-600: #00acc1;
  --md-cyan-700: #0097a7;
  --md-cyan-800: #00838f;
  --md-cyan-900: #006064;
  --md-cyan-A100: #84ffff;
  --md-cyan-A200: #18ffff;
  --md-cyan-A400: #00e5ff;
  --md-cyan-A700: #00b8d4;
  --md-teal-50: #e0f2f1;
  --md-teal-100: #b2dfdb;
  --md-teal-200: #80cbc4;
  --md-teal-300: #4db6ac;
  --md-teal-400: #26a69a;
  --md-teal-500: #009688;
  --md-teal-600: #00897b;
  --md-teal-700: #00796b;
  --md-teal-800: #00695c;
  --md-teal-900: #004d40;
  --md-teal-A100: #a7ffeb;
  --md-teal-A200: #64ffda;
  --md-teal-A400: #1de9b6;
  --md-teal-A700: #00bfa5;
  --md-green-50: #e8f5e9;
  --md-green-100: #c8e6c9;
  --md-green-200: #a5d6a7;
  --md-green-300: #81c784;
  --md-green-400: #66bb6a;
  --md-green-500: #4caf50;
  --md-green-600: #43a047;
  --md-green-700: #388e3c;
  --md-green-800: #2e7d32;
  --md-green-900: #1b5e20;
  --md-green-A100: #b9f6ca;
  --md-green-A200: #69f0ae;
  --md-green-A400: #00e676;
  --md-green-A700: #00c853;
  --md-light-green-50: #f1f8e9;
  --md-light-green-100: #dcedc8;
  --md-light-green-200: #c5e1a5;
  --md-light-green-300: #aed581;
  --md-light-green-400: #9ccc65;
  --md-light-green-500: #8bc34a;
  --md-light-green-600: #7cb342;
  --md-light-green-700: #689f38;
  --md-light-green-800: #558b2f;
  --md-light-green-900: #33691e;
  --md-light-green-A100: #ccff90;
  --md-light-green-A200: #b2ff59;
  --md-light-green-A400: #76ff03;
  --md-light-green-A700: #64dd17;
  --md-lime-50: #f9fbe7;
  --md-lime-100: #f0f4c3;
  --md-lime-200: #e6ee9c;
  --md-lime-300: #dce775;
  --md-lime-400: #d4e157;
  --md-lime-500: #cddc39;
  --md-lime-600: #c0ca33;
  --md-lime-700: #afb42b;
  --md-lime-800: #9e9d24;
  --md-lime-900: #827717;
  --md-lime-A100: #f4ff81;
  --md-lime-A200: #eeff41;
  --md-lime-A400: #c6ff00;
  --md-lime-A700: #aeea00;
  --md-yellow-50: #fffde7;
  --md-yellow-100: #fff9c4;
  --md-yellow-200: #fff59d;
  --md-yellow-300: #fff176;
  --md-yellow-400: #ffee58;
  --md-yellow-500: #ffeb3b;
  --md-yellow-600: #fdd835;
  --md-yellow-700: #fbc02d;
  --md-yellow-800: #f9a825;
  --md-yellow-900: #f57f17;
  --md-yellow-A100: #ffff8d;
  --md-yellow-A200: #ff0;
  --md-yellow-A400: #ffea00;
  --md-yellow-A700: #ffd600;
  --md-amber-50: #fff8e1;
  --md-amber-100: #ffecb3;
  --md-amber-200: #ffe082;
  --md-amber-300: #ffd54f;
  --md-amber-400: #ffca28;
  --md-amber-500: #ffc107;
  --md-amber-600: #ffb300;
  --md-amber-700: #ffa000;
  --md-amber-800: #ff8f00;
  --md-amber-900: #ff6f00;
  --md-amber-A100: #ffe57f;
  --md-amber-A200: #ffd740;
  --md-amber-A400: #ffc400;
  --md-amber-A700: #ffab00;
  --md-orange-50: #fff3e0;
  --md-orange-100: #ffe0b2;
  --md-orange-200: #ffcc80;
  --md-orange-300: #ffb74d;
  --md-orange-400: #ffa726;
  --md-orange-500: #ff9800;
  --md-orange-600: #fb8c00;
  --md-orange-700: #f57c00;
  --md-orange-800: #ef6c00;
  --md-orange-900: #e65100;
  --md-orange-A100: #ffd180;
  --md-orange-A200: #ffab40;
  --md-orange-A400: #ff9100;
  --md-orange-A700: #ff6d00;
  --md-deep-orange-50: #fbe9e7;
  --md-deep-orange-100: #ffccbc;
  --md-deep-orange-200: #ffab91;
  --md-deep-orange-300: #ff8a65;
  --md-deep-orange-400: #ff7043;
  --md-deep-orange-500: #ff5722;
  --md-deep-orange-600: #f4511e;
  --md-deep-orange-700: #e64a19;
  --md-deep-orange-800: #d84315;
  --md-deep-orange-900: #bf360c;
  --md-deep-orange-A100: #ff9e80;
  --md-deep-orange-A200: #ff6e40;
  --md-deep-orange-A400: #ff3d00;
  --md-deep-orange-A700: #dd2c00;
  --md-brown-50: #efebe9;
  --md-brown-100: #d7ccc8;
  --md-brown-200: #bcaaa4;
  --md-brown-300: #a1887f;
  --md-brown-400: #8d6e63;
  --md-brown-500: #795548;
  --md-brown-600: #6d4c41;
  --md-brown-700: #5d4037;
  --md-brown-800: #4e342e;
  --md-brown-900: #3e2723;
  --md-grey-50: #fafafa;
  --md-grey-100: #f5f5f5;
  --md-grey-200: #eee;
  --md-grey-300: #e0e0e0;
  --md-grey-400: #bdbdbd;
  --md-grey-500: #9e9e9e;
  --md-grey-600: #757575;
  --md-grey-700: #616161;
  --md-grey-800: #424242;
  --md-grey-900: #212121;
  --md-blue-grey-50: #eceff1;
  --md-blue-grey-100: #cfd8dc;
  --md-blue-grey-200: #b0bec5;
  --md-blue-grey-300: #90a4ae;
  --md-blue-grey-400: #78909c;
  --md-blue-grey-500: #607d8b;
  --md-blue-grey-600: #546e7a;
  --md-blue-grey-700: #455a64;
  --md-blue-grey-800: #37474f;
  --md-blue-grey-900: #263238;
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2014-2017, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| RenderedText
|----------------------------------------------------------------------------*/

:root {
  /* This is the padding value to fill the gaps between lines containing spans with background color. */
  --jp-private-code-span-padding: calc(
    (var(--jp-code-line-height) - 1) * var(--jp-code-font-size) / 2
  );
}

.jp-RenderedText {
  text-align: left;
  padding-left: var(--jp-code-padding);
  line-height: var(--jp-code-line-height);
  font-family: var(--jp-code-font-family);
}

.jp-RenderedText pre,
.jp-RenderedJavaScript pre,
.jp-RenderedHTMLCommon pre {
  color: var(--jp-content-font-color1);
  font-size: var(--jp-code-font-size);
  border: none;
  margin: 0;
  padding: 0;
}

.jp-RenderedText pre a:link {
  text-decoration: none;
  color: var(--jp-content-link-color);
}

.jp-RenderedText pre a:hover {
  text-decoration: underline;
  color: var(--jp-content-link-color);
}

.jp-RenderedText pre a:visited {
  text-decoration: none;
  color: var(--jp-content-link-color);
}

/* console foregrounds and backgrounds */
.jp-RenderedText pre .ansi-black-fg {
  color: #3e424d;
}

.jp-RenderedText pre .ansi-red-fg {
  color: #e75c58;
}

.jp-RenderedText pre .ansi-green-fg {
  color: #00a250;
}

.jp-RenderedText pre .ansi-yellow-fg {
  color: #ddb62b;
}

.jp-RenderedText pre .ansi-blue-fg {
  color: #208ffb;
}

.jp-RenderedText pre .ansi-magenta-fg {
  color: #d160c4;
}

.jp-RenderedText pre .ansi-cyan-fg {
  color: #60c6c8;
}

.jp-RenderedText pre .ansi-white-fg {
  color: #c5c1b4;
}

.jp-RenderedText pre .ansi-black-bg {
  background-color: #3e424d;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-red-bg {
  background-color: #e75c58;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-green-bg {
  background-color: #00a250;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-yellow-bg {
  background-color: #ddb62b;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-blue-bg {
  background-color: #208ffb;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-magenta-bg {
  background-color: #d160c4;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-cyan-bg {
  background-color: #60c6c8;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-white-bg {
  background-color: #c5c1b4;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-black-intense-fg {
  color: #282c36;
}

.jp-RenderedText pre .ansi-red-intense-fg {
  color: #b22b31;
}

.jp-RenderedText pre .ansi-green-intense-fg {
  color: #007427;
}

.jp-RenderedText pre .ansi-yellow-intense-fg {
  color: #b27d12;
}

.jp-RenderedText pre .ansi-blue-intense-fg {
  color: #0065ca;
}

.jp-RenderedText pre .ansi-magenta-intense-fg {
  color: #a03196;
}

.jp-RenderedText pre .ansi-cyan-intense-fg {
  color: #258f8f;
}

.jp-RenderedText pre .ansi-white-intense-fg {
  color: #a1a6b2;
}

.jp-RenderedText pre .ansi-black-intense-bg {
  background-color: #282c36;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-red-intense-bg {
  background-color: #b22b31;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-green-intense-bg {
  background-color: #007427;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-yellow-intense-bg {
  background-color: #b27d12;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-blue-intense-bg {
  background-color: #0065ca;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-magenta-intense-bg {
  background-color: #a03196;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-cyan-intense-bg {
  background-color: #258f8f;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-white-intense-bg {
  background-color: #a1a6b2;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-default-inverse-fg {
  color: var(--jp-ui-inverse-font-color0);
}

.jp-RenderedText pre .ansi-default-inverse-bg {
  background-color: var(--jp-inverse-layout-color0);
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-bold {
  font-weight: bold;
}

.jp-RenderedText pre .ansi-underline {
  text-decoration: underline;
}

.jp-RenderedText[data-mime-type='application/vnd.jupyter.stderr'] {
  background: var(--jp-rendermime-error-background);
  padding-top: var(--jp-code-padding);
}

/*-----------------------------------------------------------------------------
| RenderedLatex
|----------------------------------------------------------------------------*/

.jp-RenderedLatex {
  color: var(--jp-content-font-color1);
  font-size: var(--jp-content-font-size1);
  line-height: var(--jp-content-line-height);
}

/* Left-justify outputs.*/
.jp-OutputArea-output.jp-RenderedLatex {
  padding: var(--jp-code-padding);
  text-align: left;
}

/*-----------------------------------------------------------------------------
| RenderedHTML
|----------------------------------------------------------------------------*/

.jp-RenderedHTMLCommon {
  color: var(--jp-content-font-color1);
  font-family: var(--jp-content-font-family);
  font-size: var(--jp-content-font-size1);
  line-height: var(--jp-content-line-height);

  /* Give a bit more R padding on Markdown text to keep line lengths reasonable */
  padding-right: 20px;
}

.jp-RenderedHTMLCommon em {
  font-style: italic;
}

.jp-RenderedHTMLCommon strong {
  font-weight: bold;
}

.jp-RenderedHTMLCommon u {
  text-decoration: underline;
}

.jp-RenderedHTMLCommon a:link {
  text-decoration: none;
  color: var(--jp-content-link-color);
}

.jp-RenderedHTMLCommon a:hover {
  text-decoration: underline;
  color: var(--jp-content-link-color);
}

.jp-RenderedHTMLCommon a:visited {
  text-decoration: none;
  color: var(--jp-content-link-color);
}

/* Headings */

.jp-RenderedHTMLCommon h1,
.jp-RenderedHTMLCommon h2,
.jp-RenderedHTMLCommon h3,
.jp-RenderedHTMLCommon h4,
.jp-RenderedHTMLCommon h5,
.jp-RenderedHTMLCommon h6 {
  line-height: var(--jp-content-heading-line-height);
  font-weight: var(--jp-content-heading-font-weight);
  font-style: normal;
  margin: var(--jp-content-heading-margin-top) 0
    var(--jp-content-heading-margin-bottom) 0;
}

.jp-RenderedHTMLCommon h1:first-child,
.jp-RenderedHTMLCommon h2:first-child,
.jp-RenderedHTMLCommon h3:first-child,
.jp-RenderedHTMLCommon h4:first-child,
.jp-RenderedHTMLCommon h5:first-child,
.jp-RenderedHTMLCommon h6:first-child {
  margin-top: calc(0.5 * var(--jp-content-heading-margin-top));
}

.jp-RenderedHTMLCommon h1:last-child,
.jp-RenderedHTMLCommon h2:last-child,
.jp-RenderedHTMLCommon h3:last-child,
.jp-RenderedHTMLCommon h4:last-child,
.jp-RenderedHTMLCommon h5:last-child,
.jp-RenderedHTMLCommon h6:last-child {
  margin-bottom: calc(0.5 * var(--jp-content-heading-margin-bottom));
}

.jp-RenderedHTMLCommon h1 {
  font-size: var(--jp-content-font-size5);
}

.jp-RenderedHTMLCommon h2 {
  font-size: var(--jp-content-font-size4);
}

.jp-RenderedHTMLCommon h3 {
  font-size: var(--jp-content-font-size3);
}

.jp-RenderedHTMLCommon h4 {
  font-size: var(--jp-content-font-size2);
}

.jp-RenderedHTMLCommon h5 {
  font-size: var(--jp-content-font-size1);
}

.jp-RenderedHTMLCommon h6 {
  font-size: var(--jp-content-font-size0);
}

/* Lists */

/* stylelint-disable selector-max-type, selector-max-compound-selectors */

.jp-RenderedHTMLCommon ul:not(.list-inline),
.jp-RenderedHTMLCommon ol:not(.list-inline) {
  padding-left: 2em;
}

.jp-RenderedHTMLCommon ul {
  list-style: disc;
}

.jp-RenderedHTMLCommon ul ul {
  list-style: square;
}

.jp-RenderedHTMLCommon ul ul ul {
  list-style: circle;
}

.jp-RenderedHTMLCommon ol {
  list-style: decimal;
}

.jp-RenderedHTMLCommon ol ol {
  list-style: upper-alpha;
}

.jp-RenderedHTMLCommon ol ol ol {
  list-style: lower-alpha;
}

.jp-RenderedHTMLCommon ol ol ol ol {
  list-style: lower-roman;
}

.jp-RenderedHTMLCommon ol ol ol ol ol {
  list-style: decimal;
}

.jp-RenderedHTMLCommon ol,
.jp-RenderedHTMLCommon ul {
  margin-bottom: 1em;
}

.jp-RenderedHTMLCommon ul ul,
.jp-RenderedHTMLCommon ul ol,
.jp-RenderedHTMLCommon ol ul,
.jp-RenderedHTMLCommon ol ol {
  margin-bottom: 0;
}

/* stylelint-enable selector-max-type, selector-max-compound-selectors */

.jp-RenderedHTMLCommon hr {
  color: var(--jp-border-color2);
  background-color: var(--jp-border-color1);
  margin-top: 1em;
  margin-bottom: 1em;
}

.jp-RenderedHTMLCommon > pre {
  margin: 1.5em 2em;
}

.jp-RenderedHTMLCommon pre,
.jp-RenderedHTMLCommon code {
  border: 0;
  background-color: var(--jp-layout-color0);
  color: var(--jp-content-font-color1);
  font-family: var(--jp-code-font-family);
  font-size: inherit;
  line-height: var(--jp-code-line-height);
  padding: 0;
  white-space: pre-wrap;
}

.jp-RenderedHTMLCommon :not(pre) > code {
  background-color: var(--jp-layout-color2);
  padding: 1px 5px;
}

/* Tables */

.jp-RenderedHTMLCommon table {
  border-collapse: collapse;
  border-spacing: 0;
  border: none;
  color: var(--jp-ui-font-color1);
  font-size: var(--jp-ui-font-size1);
  table-layout: fixed;
  margin-left: auto;
  margin-bottom: 1em;
  margin-right: auto;
}

.jp-RenderedHTMLCommon thead {
  border-bottom: var(--jp-border-width) solid var(--jp-border-color1);
  vertical-align: bottom;
}

.jp-RenderedHTMLCommon td,
.jp-RenderedHTMLCommon th,
.jp-RenderedHTMLCommon tr {
  vertical-align: middle;
  padding: 0.5em;
  line-height: normal;
  white-space: normal;
  max-width: none;
  border: none;
}

.jp-RenderedMarkdown.jp-RenderedHTMLCommon td,
.jp-RenderedMarkdown.jp-RenderedHTMLCommon th {
  max-width: none;
}

:not(.jp-RenderedMarkdown).jp-RenderedHTMLCommon td,
:not(.jp-RenderedMarkdown).jp-RenderedHTMLCommon th,
:not(.jp-RenderedMarkdown).jp-RenderedHTMLCommon tr {
  text-align: right;
}

.jp-RenderedHTMLCommon th {
  font-weight: bold;
}

.jp-RenderedHTMLCommon tbody tr:nth-child(odd) {
  background: var(--jp-layout-color0);
}

.jp-RenderedHTMLCommon tbody tr:nth-child(even) {
  background: var(--jp-rendermime-table-row-background);
}

.jp-RenderedHTMLCommon tbody tr:hover {
  background: var(--jp-rendermime-table-row-hover-background);
}

.jp-RenderedHTMLCommon p {
  text-align: left;
  margin: 0;
  margin-bottom: 1em;
}

.jp-RenderedHTMLCommon img {
  -moz-force-broken-image-icon: 1;
}

/* Restrict to direct children as other images could be nested in other content. */
.jp-RenderedHTMLCommon > img {
  display: block;
  margin-left: 0;
  margin-right: 0;
  margin-bottom: 1em;
}

/* Change color behind transparent images if they need it... */
[data-jp-theme-light='false'] .jp-RenderedImage img.jp-needs-light-background {
  background-color: var(--jp-inverse-layout-color1);
}

[data-jp-theme-light='true'] .jp-RenderedImage img.jp-needs-dark-background {
  background-color: var(--jp-inverse-layout-color1);
}

.jp-RenderedHTMLCommon img,
.jp-RenderedImage img,
.jp-RenderedHTMLCommon svg,
.jp-RenderedSVG svg {
  max-width: 100%;
  height: auto;
}

.jp-RenderedHTMLCommon img.jp-mod-unconfined,
.jp-RenderedImage img.jp-mod-unconfined,
.jp-RenderedHTMLCommon svg.jp-mod-unconfined,
.jp-RenderedSVG svg.jp-mod-unconfined {
  max-width: none;
}

.jp-RenderedHTMLCommon .alert {
  padding: var(--jp-notebook-padding);
  border: var(--jp-border-width) solid transparent;
  border-radius: var(--jp-border-radius);
  margin-bottom: 1em;
}

.jp-RenderedHTMLCommon .alert-info {
  color: var(--jp-info-color0);
  background-color: var(--jp-info-color3);
  border-color: var(--jp-info-color2);
}

.jp-RenderedHTMLCommon .alert-info hr {
  border-color: var(--jp-info-color3);
}

.jp-RenderedHTMLCommon .alert-info > p:last-child,
.jp-RenderedHTMLCommon .alert-info > ul:last-child {
  margin-bottom: 0;
}

.jp-RenderedHTMLCommon .alert-warning {
  color: var(--jp-warn-color0);
  background-color: var(--jp-warn-color3);
  border-color: var(--jp-warn-color2);
}

.jp-RenderedHTMLCommon .alert-warning hr {
  border-color: var(--jp-warn-color3);
}

.jp-RenderedHTMLCommon .alert-warning > p:last-child,
.jp-RenderedHTMLCommon .alert-warning > ul:last-child {
  margin-bottom: 0;
}

.jp-RenderedHTMLCommon .alert-success {
  color: var(--jp-success-color0);
  background-color: var(--jp-success-color3);
  border-color: var(--jp-success-color2);
}

.jp-RenderedHTMLCommon .alert-success hr {
  border-color: var(--jp-success-color3);
}

.jp-RenderedHTMLCommon .alert-success > p:last-child,
.jp-RenderedHTMLCommon .alert-success > ul:last-child {
  margin-bottom: 0;
}

.jp-RenderedHTMLCommon .alert-danger {
  color: var(--jp-error-color0);
  background-color: var(--jp-error-color3);
  border-color: var(--jp-error-color2);
}

.jp-RenderedHTMLCommon .alert-danger hr {
  border-color: var(--jp-error-color3);
}

.jp-RenderedHTMLCommon .alert-danger > p:last-child,
.jp-RenderedHTMLCommon .alert-danger > ul:last-child {
  margin-bottom: 0;
}

.jp-RenderedHTMLCommon blockquote {
  margin: 1em 2em;
  padding: 0 1em;
  border-left: 5px solid var(--jp-border-color2);
}

a.jp-InternalAnchorLink {
  visibility: hidden;
  margin-left: 8px;
  color: var(--md-blue-800);
}

h1:hover .jp-InternalAnchorLink,
h2:hover .jp-InternalAnchorLink,
h3:hover .jp-InternalAnchorLink,
h4:hover .jp-InternalAnchorLink,
h5:hover .jp-InternalAnchorLink,
h6:hover .jp-InternalAnchorLink {
  visibility: visible;
}

.jp-RenderedHTMLCommon kbd {
  background-color: var(--jp-rendermime-table-row-background);
  border: 1px solid var(--jp-border-color0);
  border-bottom-color: var(--jp-border-color2);
  border-radius: 3px;
  box-shadow: inset 0 -1px 0 rgba(0, 0, 0, 0.25);
  display: inline-block;
  font-size: var(--jp-ui-font-size0);
  line-height: 1em;
  padding: 0.2em 0.5em;
}

/* Most direct children of .jp-RenderedHTMLCommon have a margin-bottom of 1.0.
 * At the bottom of cells this is a bit too much as there is also spacing
 * between cells. Going all the way to 0 gets too tight between markdown and
 * code cells.
 */
.jp-RenderedHTMLCommon > *:last-child {
  margin-bottom: 0.5em;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-cursor-backdrop {
  position: fixed;
  width: 200px;
  height: 200px;
  margin-top: -100px;
  margin-left: -100px;
  will-change: transform;
  z-index: 100;
}

.lm-mod-drag-image {
  will-change: transform;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

.jp-lineFormSearch {
  padding: 4px 12px;
  background-color: var(--jp-layout-color2);
  box-shadow: var(--jp-toolbar-box-shadow);
  z-index: 2;
  font-size: var(--jp-ui-font-size1);
}

.jp-lineFormCaption {
  font-size: var(--jp-ui-font-size0);
  line-height: var(--jp-ui-font-size1);
  margin-top: 4px;
  color: var(--jp-ui-font-color0);
}

.jp-baseLineForm {
  border: none;
  border-radius: 0;
  position: absolute;
  background-size: 16px;
  background-repeat: no-repeat;
  background-position: center;
  outline: none;
}

.jp-lineFormButtonContainer {
  top: 4px;
  right: 8px;
  height: 24px;
  padding: 0 12px;
  width: 12px;
}

.jp-lineFormButtonIcon {
  top: 0;
  right: 0;
  background-color: var(--jp-brand-color1);
  height: 100%;
  width: 100%;
  box-sizing: border-box;
  padding: 4px 6px;
}

.jp-lineFormButton {
  top: 0;
  right: 0;
  background-color: transparent;
  height: 100%;
  width: 100%;
  box-sizing: border-box;
}

.jp-lineFormWrapper {
  overflow: hidden;
  padding: 0 8px;
  border: 1px solid var(--jp-border-color0);
  background-color: var(--jp-input-active-background);
  height: 22px;
}

.jp-lineFormWrapperFocusWithin {
  border: var(--jp-border-width) solid var(--md-blue-500);
  box-shadow: inset 0 0 4px var(--md-blue-300);
}

.jp-lineFormInput {
  background: transparent;
  width: 200px;
  height: 100%;
  border: none;
  outline: none;
  color: var(--jp-ui-font-color0);
  line-height: 28px;
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2014-2016, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-JSONEditor {
  display: flex;
  flex-direction: column;
  width: 100%;
}

.jp-JSONEditor-host {
  flex: 1 1 auto;
  border: var(--jp-border-width) solid var(--jp-input-border-color);
  border-radius: 0;
  background: var(--jp-layout-color0);
  min-height: 50px;
  padding: 1px;
}

.jp-JSONEditor.jp-mod-error .jp-JSONEditor-host {
  border-color: red;
  outline-color: red;
}

.jp-JSONEditor-header {
  display: flex;
  flex: 1 0 auto;
  padding: 0 0 0 12px;
}

.jp-JSONEditor-header label {
  flex: 0 0 auto;
}

.jp-JSONEditor-commitButton {
  height: 16px;
  width: 16px;
  background-size: 18px;
  background-repeat: no-repeat;
  background-position: center;
}

.jp-JSONEditor-host.jp-mod-focused {
  background-color: var(--jp-input-active-background);
  border: 1px solid var(--jp-input-active-border-color);
  box-shadow: var(--jp-input-box-shadow);
}

.jp-Editor.jp-mod-dropTarget {
  border: var(--jp-border-width) solid var(--jp-input-active-border-color);
  box-shadow: var(--jp-input-box-shadow);
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/
.jp-DocumentSearch-input {
  border: none;
  outline: none;
  color: var(--jp-ui-font-color0);
  font-size: var(--jp-ui-font-size1);
  background-color: var(--jp-layout-color0);
  font-family: var(--jp-ui-font-family);
  padding: 2px 1px;
  resize: none;
}

.jp-DocumentSearch-overlay {
  position: absolute;
  background-color: var(--jp-toolbar-background);
  border-bottom: var(--jp-border-width) solid var(--jp-toolbar-border-color);
  border-left: var(--jp-border-width) solid var(--jp-toolbar-border-color);
  top: 0;
  right: 0;
  z-index: 7;
  min-width: 405px;
  padding: 2px;
  font-size: var(--jp-ui-font-size1);

  --jp-private-document-search-button-height: 20px;
}

.jp-DocumentSearch-overlay button {
  background-color: var(--jp-toolbar-background);
  outline: 0;
}

.jp-DocumentSearch-overlay button:hover {
  background-color: var(--jp-layout-color2);
}

.jp-DocumentSearch-overlay button:active {
  background-color: var(--jp-layout-color3);
}

.jp-DocumentSearch-overlay-row {
  display: flex;
  align-items: center;
  margin-bottom: 2px;
}

.jp-DocumentSearch-button-content {
  display: inline-block;
  cursor: pointer;
  box-sizing: border-box;
  width: 100%;
  height: 100%;
}

.jp-DocumentSearch-button-content svg {
  width: 100%;
  height: 100%;
}

.jp-DocumentSearch-input-wrapper {
  border: var(--jp-border-width) solid var(--jp-border-color0);
  display: flex;
  background-color: var(--jp-layout-color0);
  margin: 2px;
}

.jp-DocumentSearch-input-wrapper:focus-within {
  border-color: var(--jp-cell-editor-active-border-color);
}

.jp-DocumentSearch-toggle-wrapper,
.jp-DocumentSearch-button-wrapper {
  all: initial;
  overflow: hidden;
  display: inline-block;
  border: none;
  box-sizing: border-box;
}

.jp-DocumentSearch-toggle-wrapper {
  width: 14px;
  height: 14px;
}

.jp-DocumentSearch-button-wrapper {
  width: var(--jp-private-document-search-button-height);
  height: var(--jp-private-document-search-button-height);
}

.jp-DocumentSearch-toggle-wrapper:focus,
.jp-DocumentSearch-button-wrapper:focus {
  outline: var(--jp-border-width) solid
    var(--jp-cell-editor-active-border-color);
  outline-offset: -1px;
}

.jp-DocumentSearch-toggle-wrapper,
.jp-DocumentSearch-button-wrapper,
.jp-DocumentSearch-button-content:focus {
  outline: none;
}

.jp-DocumentSearch-toggle-placeholder {
  width: 5px;
}

.jp-DocumentSearch-input-button::before {
  display: block;
  padding-top: 100%;
}

.jp-DocumentSearch-input-button-off {
  opacity: var(--jp-search-toggle-off-opacity);
}

.jp-DocumentSearch-input-button-off:hover {
  opacity: var(--jp-search-toggle-hover-opacity);
}

.jp-DocumentSearch-input-button-on {
  opacity: var(--jp-search-toggle-on-opacity);
}

.jp-DocumentSearch-index-counter {
  padding-left: 10px;
  padding-right: 10px;
  user-select: none;
  min-width: 35px;
  display: inline-block;
}

.jp-DocumentSearch-up-down-wrapper {
  display: inline-block;
  padding-right: 2px;
  margin-left: auto;
  white-space: nowrap;
}

.jp-DocumentSearch-spacer {
  margin-left: auto;
}

.jp-DocumentSearch-up-down-wrapper button {
  outline: 0;
  border: none;
  width: var(--jp-private-document-search-button-height);
  height: var(--jp-private-document-search-button-height);
  vertical-align: middle;
  margin: 1px 5px 2px;
}

.jp-DocumentSearch-up-down-button:hover {
  background-color: var(--jp-layout-color2);
}

.jp-DocumentSearch-up-down-button:active {
  background-color: var(--jp-layout-color3);
}

.jp-DocumentSearch-filter-button {
  border-radius: var(--jp-border-radius);
}

.jp-DocumentSearch-filter-button:hover {
  background-color: var(--jp-layout-color2);
}

.jp-DocumentSearch-filter-button-enabled {
  background-color: var(--jp-layout-color2);
}

.jp-DocumentSearch-filter-button-enabled:hover {
  background-color: var(--jp-layout-color3);
}

.jp-DocumentSearch-search-options {
  padding: 0 8px;
  margin-left: 3px;
  width: 100%;
  display: grid;
  justify-content: start;
  grid-template-columns: 1fr 1fr;
  align-items: center;
  justify-items: stretch;
}

.jp-DocumentSearch-search-filter-disabled {
  color: var(--jp-ui-font-color2);
}

.jp-DocumentSearch-search-filter {
  display: flex;
  align-items: center;
  user-select: none;
}

.jp-DocumentSearch-regex-error {
  color: var(--jp-error-color0);
}

.jp-DocumentSearch-replace-button-wrapper {
  overflow: hidden;
  display: inline-block;
  box-sizing: border-box;
  border: var(--jp-border-width) solid var(--jp-border-color0);
  margin: auto 2px;
  padding: 1px 4px;
  height: calc(var(--jp-private-document-search-button-height) + 2px);
}

.jp-DocumentSearch-replace-button-wrapper:focus {
  border: var(--jp-border-width) solid var(--jp-cell-editor-active-border-color);
}

.jp-DocumentSearch-replace-button {
  display: inline-block;
  text-align: center;
  cursor: pointer;
  box-sizing: border-box;
  color: var(--jp-ui-font-color1);

  /* height - 2 * (padding of wrapper) */
  line-height: calc(var(--jp-private-document-search-button-height) - 2px);
  width: 100%;
  height: 100%;
}

.jp-DocumentSearch-replace-button:focus {
  outline: none;
}

.jp-DocumentSearch-replace-wrapper-class {
  margin-left: 14px;
  display: flex;
}

.jp-DocumentSearch-replace-toggle {
  border: none;
  background-color: var(--jp-toolbar-background);
  border-radius: var(--jp-border-radius);
}

.jp-DocumentSearch-replace-toggle:hover {
  background-color: var(--jp-layout-color2);
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.cm-editor {
  line-height: var(--jp-code-line-height);
  font-size: var(--jp-code-font-size);
  font-family: var(--jp-code-font-family);
  border: 0;
  border-radius: 0;
  height: auto;

  /* Changed to auto to autogrow */
}

.cm-editor pre {
  padding: 0 var(--jp-code-padding);
}

.jp-CodeMirrorEditor[data-type='inline'] .cm-dialog {
  background-color: var(--jp-layout-color0);
  color: var(--jp-content-font-color1);
}

.jp-CodeMirrorEditor {
  cursor: text;
}

/* When zoomed out 67% and 33% on a screen of 1440 width x 900 height */
@media screen and (min-width: 2138px) and (max-width: 4319px) {
  .jp-CodeMirrorEditor[data-type='inline'] .cm-cursor {
    border-left: var(--jp-code-cursor-width1) solid
      var(--jp-editor-cursor-color);
  }
}

/* When zoomed out less than 33% */
@media screen and (min-width: 4320px) {
  .jp-CodeMirrorEditor[data-type='inline'] .cm-cursor {
    border-left: var(--jp-code-cursor-width2) solid
      var(--jp-editor-cursor-color);
  }
}

.cm-editor.jp-mod-readOnly .cm-cursor {
  display: none;
}

.jp-CollaboratorCursor {
  border-left: 5px solid transparent;
  border-right: 5px solid transparent;
  border-top: none;
  border-bottom: 3px solid;
  background-clip: content-box;
  margin-left: -5px;
  margin-right: -5px;
}

.cm-searching,
.cm-searching span {
  /* `.cm-searching span`: we need to override syntax highlighting */
  background-color: var(--jp-search-unselected-match-background-color);
  color: var(--jp-search-unselected-match-color);
}

.cm-searching::selection,
.cm-searching span::selection {
  background-color: var(--jp-search-unselected-match-background-color);
  color: var(--jp-search-unselected-match-color);
}

.jp-current-match > .cm-searching,
.jp-current-match > .cm-searching span,
.cm-searching > .jp-current-match,
.cm-searching > .jp-current-match span {
  background-color: var(--jp-search-selected-match-background-color);
  color: var(--jp-search-selected-match-color);
}

.jp-current-match > .cm-searching::selection,
.cm-searching > .jp-current-match::selection,
.jp-current-match > .cm-searching span::selection {
  background-color: var(--jp-search-selected-match-background-color);
  color: var(--jp-search-selected-match-color);
}

.cm-trailingspace {
  background-image: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAgAAAAFCAYAAAB4ka1VAAAAsElEQVQIHQGlAFr/AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA7+r3zKmT0/+pk9P/7+r3zAAAAAAAAAAABAAAAAAAAAAA6OPzM+/q9wAAAAAA6OPzMwAAAAAAAAAAAgAAAAAAAAAAGR8NiRQaCgAZIA0AGR8NiQAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAQyoYJ/SY80UAAAAASUVORK5CYII=);
  background-position: center left;
  background-repeat: repeat-x;
}

.jp-CollaboratorCursor-hover {
  position: absolute;
  z-index: 1;
  transform: translateX(-50%);
  color: white;
  border-radius: 3px;
  padding-left: 4px;
  padding-right: 4px;
  padding-top: 1px;
  padding-bottom: 1px;
  text-align: center;
  font-size: var(--jp-ui-font-size1);
  white-space: nowrap;
}

.jp-CodeMirror-ruler {
  border-left: 1px dashed var(--jp-border-color2);
}

/* Styles for shared cursors (remote cursor locations and selected ranges) */
.jp-CodeMirrorEditor .cm-ySelectionCaret {
  position: relative;
  border-left: 1px solid black;
  margin-left: -1px;
  margin-right: -1px;
  box-sizing: border-box;
}

.jp-CodeMirrorEditor .cm-ySelectionCaret > .cm-ySelectionInfo {
  white-space: nowrap;
  position: absolute;
  top: -1.15em;
  padding-bottom: 0.05em;
  left: -1px;
  font-size: 0.95em;
  font-family: var(--jp-ui-font-family);
  font-weight: bold;
  line-height: normal;
  user-select: none;
  color: white;
  padding-left: 2px;
  padding-right: 2px;
  z-index: 101;
  transition: opacity 0.3s ease-in-out;
}

.jp-CodeMirrorEditor .cm-ySelectionInfo {
  transition-delay: 0.7s;
  opacity: 0;
}

.jp-CodeMirrorEditor .cm-ySelectionCaret:hover > .cm-ySelectionInfo {
  opacity: 1;
  transition-delay: 0s;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-MimeDocument {
  outline: none;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Variables
|----------------------------------------------------------------------------*/

:root {
  --jp-private-filebrowser-button-height: 28px;
  --jp-private-filebrowser-button-width: 48px;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-FileBrowser .jp-SidePanel-content {
  display: flex;
  flex-direction: column;
}

.jp-FileBrowser-toolbar.jp-Toolbar {
  flex-wrap: wrap;
  row-gap: 12px;
  border-bottom: none;
  height: auto;
  margin: 8px 12px 0;
  box-shadow: none;
  padding: 0;
  justify-content: flex-start;
}

.jp-FileBrowser-Panel {
  flex: 1 1 auto;
  display: flex;
  flex-direction: column;
}

.jp-BreadCrumbs {
  flex: 0 0 auto;
  margin: 8px 12px;
}

.jp-BreadCrumbs-item {
  margin: 0 2px;
  padding: 0 2px;
  border-radius: var(--jp-border-radius);
  cursor: pointer;
}

.jp-BreadCrumbs-item:hover {
  background-color: var(--jp-layout-color2);
}

.jp-BreadCrumbs-item:first-child {
  margin-left: 0;
}

.jp-BreadCrumbs-item.jp-mod-dropTarget {
  background-color: var(--jp-brand-color2);
  opacity: 0.7;
}

/*-----------------------------------------------------------------------------
| Buttons
|----------------------------------------------------------------------------*/

.jp-FileBrowser-toolbar > .jp-Toolbar-item {
  flex: 0 0 auto;
  padding-left: 0;
  padding-right: 2px;
  align-items: center;
  height: unset;
}

.jp-FileBrowser-toolbar > .jp-Toolbar-item .jp-ToolbarButtonComponent {
  width: 40px;
}

/*-----------------------------------------------------------------------------
| Other styles
|----------------------------------------------------------------------------*/

.jp-FileDialog.jp-mod-conflict input {
  color: var(--jp-error-color1);
}

.jp-FileDialog .jp-new-name-title {
  margin-top: 12px;
}

.jp-LastModified-hidden {
  display: none;
}

.jp-FileSize-hidden {
  display: none;
}

.jp-FileBrowser .lm-AccordionPanel > h3:first-child {
  display: none;
}

/*-----------------------------------------------------------------------------
| DirListing
|----------------------------------------------------------------------------*/

.jp-DirListing {
  flex: 1 1 auto;
  display: flex;
  flex-direction: column;
  outline: 0;
}

.jp-DirListing-header {
  flex: 0 0 auto;
  display: flex;
  flex-direction: row;
  align-items: center;
  overflow: hidden;
  border-top: var(--jp-border-width) solid var(--jp-border-color2);
  border-bottom: var(--jp-border-width) solid var(--jp-border-color1);
  box-shadow: var(--jp-toolbar-box-shadow);
  z-index: 2;
}

.jp-DirListing-headerItem {
  padding: 4px 12px 2px;
  font-weight: 500;
}

.jp-DirListing-headerItem:hover {
  background: var(--jp-layout-color2);
}

.jp-DirListing-headerItem.jp-id-name {
  flex: 1 0 84px;
}

.jp-DirListing-headerItem.jp-id-modified {
  flex: 0 0 112px;
  border-left: var(--jp-border-width) solid var(--jp-border-color2);
  text-align: right;
}

.jp-DirListing-headerItem.jp-id-filesize {
  flex: 0 0 75px;
  border-left: var(--jp-border-width) solid var(--jp-border-color2);
  text-align: right;
}

.jp-id-narrow {
  display: none;
  flex: 0 0 5px;
  padding: 4px;
  border-left: var(--jp-border-width) solid var(--jp-border-color2);
  text-align: right;
  color: var(--jp-border-color2);
}

.jp-DirListing-narrow .jp-id-narrow {
  display: block;
}

.jp-DirListing-narrow .jp-id-modified,
.jp-DirListing-narrow .jp-DirListing-itemModified {
  display: none;
}

.jp-DirListing-headerItem.jp-mod-selected {
  font-weight: 600;
}

/* increase specificity to override bundled default */
.jp-DirListing-content {
  flex: 1 1 auto;
  margin: 0;
  padding: 0;
  list-style-type: none;
  overflow: auto;
  background-color: var(--jp-layout-color1);
}

.jp-DirListing-content mark {
  color: var(--jp-ui-font-color0);
  background-color: transparent;
  font-weight: bold;
}

.jp-DirListing-content .jp-DirListing-item.jp-mod-selected mark {
  color: var(--jp-ui-inverse-font-color0);
}

/* Style the directory listing content when a user drops a file to upload */
.jp-DirListing.jp-mod-native-drop .jp-DirListing-content {
  outline: 5px dashed rgba(128, 128, 128, 0.5);
  outline-offset: -10px;
  cursor: copy;
}

.jp-DirListing-item {
  display: flex;
  flex-direction: row;
  align-items: center;
  padding: 4px 12px;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

.jp-DirListing-checkboxWrapper {
  /* Increases hit area of checkbox. */
  padding: 4px;
}

.jp-DirListing-header
  .jp-DirListing-checkboxWrapper
  + .jp-DirListing-headerItem {
  padding-left: 4px;
}

.jp-DirListing-content .jp-DirListing-checkboxWrapper {
  position: relative;
  left: -4px;
  margin: -4px 0 -4px -8px;
}

.jp-DirListing-checkboxWrapper.jp-mod-visible {
  visibility: visible;
}

/* For devices that support hovering, hide checkboxes until hovered, selected...
*/
@media (hover: hover) {
  .jp-DirListing-checkboxWrapper {
    visibility: hidden;
  }

  .jp-DirListing-item:hover .jp-DirListing-checkboxWrapper,
  .jp-DirListing-item.jp-mod-selected .jp-DirListing-checkboxWrapper {
    visibility: visible;
  }
}

.jp-DirListing-item[data-is-dot] {
  opacity: 75%;
}

.jp-DirListing-item.jp-mod-selected {
  color: var(--jp-ui-inverse-font-color1);
  background: var(--jp-brand-color1);
}

.jp-DirListing-item.jp-mod-dropTarget {
  background: var(--jp-brand-color3);
}

.jp-DirListing-item:hover:not(.jp-mod-selected) {
  background: var(--jp-layout-color2);
}

.jp-DirListing-itemIcon {
  flex: 0 0 20px;
  margin-right: 4px;
}

.jp-DirListing-itemText {
  flex: 1 0 64px;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
  user-select: none;
}

.jp-DirListing-itemText:focus {
  outline-width: 2px;
  outline-color: var(--jp-inverse-layout-color1);
  outline-style: solid;
  outline-offset: 1px;
}

.jp-DirListing-item.jp-mod-selected .jp-DirListing-itemText:focus {
  outline-color: var(--jp-layout-color1);
}

.jp-DirListing-itemModified {
  flex: 0 0 125px;
  text-align: right;
}

.jp-DirListing-itemFileSize {
  flex: 0 0 90px;
  text-align: right;
}

.jp-DirListing-editor {
  flex: 1 0 64px;
  outline: none;
  border: none;
  color: var(--jp-ui-font-color1);
  background-color: var(--jp-layout-color1);
}

.jp-DirListing-item.jp-mod-running .jp-DirListing-itemIcon::before {
  color: var(--jp-success-color1);
  content: '\25CF';
  font-size: 8px;
  position: absolute;
  left: -8px;
}

.jp-DirListing-item.jp-mod-running.jp-mod-selected
  .jp-DirListing-itemIcon::before {
  color: var(--jp-ui-inverse-font-color1);
}

.jp-DirListing-item.lm-mod-drag-image,
.jp-DirListing-item.jp-mod-selected.lm-mod-drag-image {
  font-size: var(--jp-ui-font-size1);
  padding-left: 4px;
  margin-left: 4px;
  width: 160px;
  background-color: var(--jp-ui-inverse-font-color2);
  box-shadow: var(--jp-elevation-z2);
  border-radius: 0;
  color: var(--jp-ui-font-color1);
  transform: translateX(-40%) translateY(-58%);
}

.jp-Document {
  min-width: 120px;
  min-height: 120px;
  outline: none;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Main OutputArea
| OutputArea has a list of Outputs
|----------------------------------------------------------------------------*/

.jp-OutputArea {
  overflow-y: auto;
}

.jp-OutputArea-child {
  display: table;
  table-layout: fixed;
  width: 100%;
  overflow: hidden;
}

.jp-OutputPrompt {
  width: var(--jp-cell-prompt-width);
  color: var(--jp-cell-outprompt-font-color);
  font-family: var(--jp-cell-prompt-font-family);
  padding: var(--jp-code-padding);
  letter-spacing: var(--jp-cell-prompt-letter-spacing);
  line-height: var(--jp-code-line-height);
  font-size: var(--jp-code-font-size);
  border: var(--jp-border-width) solid transparent;
  opacity: var(--jp-cell-prompt-opacity);

  /* Right align prompt text, don't wrap to handle large prompt numbers */
  text-align: right;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;

  /* Disable text selection */
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

.jp-OutputArea-prompt {
  display: table-cell;
  vertical-align: top;
}

.jp-OutputArea-output {
  display: table-cell;
  width: 100%;
  height: auto;
  overflow: auto;
  user-select: text;
  -moz-user-select: text;
  -webkit-user-select: text;
  -ms-user-select: text;
}

.jp-OutputArea .jp-RenderedText {
  padding-left: 1ch;
}

/**
 * Prompt overlay.
 */

.jp-OutputArea-promptOverlay {
  position: absolute;
  top: 0;
  width: var(--jp-cell-prompt-width);
  height: 100%;
  opacity: 0.5;
}

.jp-OutputArea-promptOverlay:hover {
  background: var(--jp-layout-color2);
  box-shadow: inset 0 0 1px var(--jp-inverse-layout-color0);
  cursor: zoom-out;
}

.jp-mod-outputsScrolled .jp-OutputArea-promptOverlay:hover {
  cursor: zoom-in;
}

/**
 * Isolated output.
 */
.jp-OutputArea-output.jp-mod-isolated {
  width: 100%;
  display: block;
}

/*
When drag events occur, `lm-mod-override-cursor` is added to the body.
Because iframes steal all cursor events, the following two rules are necessary
to suppress pointer events while resize drags are occurring. There may be a
better solution to this problem.
*/
body.lm-mod-override-cursor .jp-OutputArea-output.jp-mod-isolated {
  position: relative;
}

body.lm-mod-override-cursor .jp-OutputArea-output.jp-mod-isolated::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: transparent;
}

/* pre */

.jp-OutputArea-output pre {
  border: none;
  margin: 0;
  padding: 0;
  overflow-x: auto;
  overflow-y: auto;
  word-break: break-all;
  word-wrap: break-word;
  white-space: pre-wrap;
}

/* tables */

.jp-OutputArea-output.jp-RenderedHTMLCommon table {
  margin-left: 0;
  margin-right: 0;
}

/* description lists */

.jp-OutputArea-output dl,
.jp-OutputArea-output dt,
.jp-OutputArea-output dd {
  display: block;
}

.jp-OutputArea-output dl {
  width: 100%;
  overflow: hidden;
  padding: 0;
  margin: 0;
}

.jp-OutputArea-output dt {
  font-weight: bold;
  float: left;
  width: 20%;
  padding: 0;
  margin: 0;
}

.jp-OutputArea-output dd {
  float: left;
  width: 80%;
  padding: 0;
  margin: 0;
}

.jp-TrimmedOutputs pre {
  background: var(--jp-layout-color3);
  font-size: calc(var(--jp-code-font-size) * 1.4);
  text-align: center;
  text-transform: uppercase;
}

/* Hide the gutter in case of
 *  - nested output areas (e.g. in the case of output widgets)
 *  - mirrored output areas
 */
.jp-OutputArea .jp-OutputArea .jp-OutputArea-prompt {
  display: none;
}

/* Hide empty lines in the output area, for instance due to cleared widgets */
.jp-OutputArea-prompt:empty {
  padding: 0;
  border: 0;
}

/*-----------------------------------------------------------------------------
| executeResult is added to any Output-result for the display of the object
| returned by a cell
|----------------------------------------------------------------------------*/

.jp-OutputArea-output.jp-OutputArea-executeResult {
  margin-left: 0;
  width: 100%;
}

/* Text output with the Out[] prompt needs a top padding to match the
 * alignment of the Out[] prompt itself.
 */
.jp-OutputArea-executeResult .jp-RenderedText.jp-OutputArea-output {
  padding-top: var(--jp-code-padding);
  border-top: var(--jp-border-width) solid transparent;
}

/*-----------------------------------------------------------------------------
| The Stdin output
|----------------------------------------------------------------------------*/

.jp-Stdin-prompt {
  color: var(--jp-content-font-color0);
  padding-right: var(--jp-code-padding);
  vertical-align: baseline;
  flex: 0 0 auto;
}

.jp-Stdin-input {
  font-family: var(--jp-code-font-family);
  font-size: inherit;
  color: inherit;
  background-color: inherit;
  width: 42%;
  min-width: 200px;

  /* make sure input baseline aligns with prompt */
  vertical-align: baseline;

  /* padding + margin = 0.5em between prompt and cursor */
  padding: 0 0.25em;
  margin: 0 0.25em;
  flex: 0 0 70%;
}

.jp-Stdin-input::placeholder {
  opacity: 0;
}

.jp-Stdin-input:focus {
  box-shadow: none;
}

.jp-Stdin-input:focus::placeholder {
  opacity: 1;
}

/*-----------------------------------------------------------------------------
| Output Area View
|----------------------------------------------------------------------------*/

.jp-LinkedOutputView .jp-OutputArea {
  height: 100%;
  display: block;
}

.jp-LinkedOutputView .jp-OutputArea-output:only-child {
  height: 100%;
}

/*-----------------------------------------------------------------------------
| Printing
|----------------------------------------------------------------------------*/

@media print {
  .jp-OutputArea-child {
    break-inside: avoid-page;
  }
}

/*-----------------------------------------------------------------------------
| Mobile
|----------------------------------------------------------------------------*/
@media only screen and (max-width: 760px) {
  .jp-OutputPrompt {
    display: table-row;
    text-align: left;
  }

  .jp-OutputArea-child .jp-OutputArea-output {
    display: table-row;
    margin-left: var(--jp-notebook-padding);
  }
}

/* Trimmed outputs warning */
.jp-TrimmedOutputs > a {
  margin: 10px;
  text-decoration: none;
  cursor: pointer;
}

.jp-TrimmedOutputs > a:hover {
  text-decoration: none;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Table of Contents
|----------------------------------------------------------------------------*/

:root {
  --jp-private-toc-active-width: 4px;
}

.jp-TableOfContents {
  display: flex;
  flex-direction: column;
  background: var(--jp-layout-color1);
  color: var(--jp-ui-font-color1);
  font-size: var(--jp-ui-font-size1);
  height: 100%;
}

.jp-TableOfContents-placeholder {
  text-align: center;
}

.jp-TableOfContents-placeholderContent {
  color: var(--jp-content-font-color2);
  padding: 8px;
}

.jp-TableOfContents-placeholderContent > h3 {
  margin-bottom: var(--jp-content-heading-margin-bottom);
}

.jp-TableOfContents .jp-SidePanel-content {
  overflow-y: auto;
}

.jp-TableOfContents-tree {
  margin: 4px;
}

.jp-TableOfContents ol {
  list-style-type: none;
}

/* stylelint-disable-next-line selector-max-type */
.jp-TableOfContents li > ol {
  /* Align left border with triangle icon center */
  padding-left: 11px;
}

.jp-TableOfContents-content {
  /* left margin for the active heading indicator */
  margin: 0 0 0 var(--jp-private-toc-active-width);
  padding: 0;
  background-color: var(--jp-layout-color1);
}

.jp-tocItem {
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

.jp-tocItem-heading {
  display: flex;
  cursor: pointer;
}

.jp-tocItem-heading:hover {
  background-color: var(--jp-layout-color2);
}

.jp-tocItem-content {
  display: block;
  padding: 4px 0;
  white-space: nowrap;
  text-overflow: ellipsis;
  overflow-x: hidden;
}

.jp-tocItem-collapser {
  height: 20px;
  margin: 2px 2px 0;
  padding: 0;
  background: none;
  border: none;
  cursor: pointer;
}

.jp-tocItem-collapser:hover {
  background-color: var(--jp-layout-color3);
}

/* Active heading indicator */

.jp-tocItem-heading::before {
  content: ' ';
  background: transparent;
  width: var(--jp-private-toc-active-width);
  height: 24px;
  position: absolute;
  left: 0;
  border-radius: var(--jp-border-radius);
}

.jp-tocItem-heading.jp-tocItem-active::before {
  background-color: var(--jp-brand-color1);
}

.jp-tocItem-heading:hover.jp-tocItem-active::before {
  background: var(--jp-brand-color0);
  opacity: 1;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-Collapser {
  flex: 0 0 var(--jp-cell-collapser-width);
  padding: 0;
  margin: 0;
  border: none;
  outline: none;
  background: transparent;
  border-radius: var(--jp-border-radius);
  opacity: 1;
}

.jp-Collapser-child {
  display: block;
  width: 100%;
  box-sizing: border-box;

  /* height: 100% doesn't work because the height of its parent is computed from content */
  position: absolute;
  top: 0;
  bottom: 0;
}

/*-----------------------------------------------------------------------------
| Printing
|----------------------------------------------------------------------------*/

/*
Hiding collapsers in print mode.

Note: input and output wrappers have "display: block" propery in print mode.
*/

@media print {
  .jp-Collapser {
    display: none;
  }
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Header/Footer
|----------------------------------------------------------------------------*/

/* Hidden by zero height by default */
.jp-CellHeader,
.jp-CellFooter {
  height: 0;
  width: 100%;
  padding: 0;
  margin: 0;
  border: none;
  outline: none;
  background: transparent;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Input
|----------------------------------------------------------------------------*/

/* All input areas */
.jp-InputArea {
  display: table;
  table-layout: fixed;
  width: 100%;
  overflow: hidden;
}

.jp-InputArea-editor {
  display: table-cell;
  overflow: hidden;
  vertical-align: top;

  /* This is the non-active, default styling */
  border: var(--jp-border-width) solid var(--jp-cell-editor-border-color);
  border-radius: 0;
  background: var(--jp-cell-editor-background);
}

.jp-InputPrompt {
  display: table-cell;
  vertical-align: top;
  width: var(--jp-cell-prompt-width);
  color: var(--jp-cell-inprompt-font-color);
  font-family: var(--jp-cell-prompt-font-family);
  padding: var(--jp-code-padding);
  letter-spacing: var(--jp-cell-prompt-letter-spacing);
  opacity: var(--jp-cell-prompt-opacity);
  line-height: var(--jp-code-line-height);
  font-size: var(--jp-code-font-size);
  border: var(--jp-border-width) solid transparent;

  /* Right align prompt text, don't wrap to handle large prompt numbers */
  text-align: right;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;

  /* Disable text selection */
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

/*-----------------------------------------------------------------------------
| Mobile
|----------------------------------------------------------------------------*/
@media only screen and (max-width: 760px) {
  .jp-InputArea-editor {
    display: table-row;
    margin-left: var(--jp-notebook-padding);
  }

  .jp-InputPrompt {
    display: table-row;
    text-align: left;
  }
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Placeholder
|----------------------------------------------------------------------------*/

.jp-Placeholder {
  display: table;
  table-layout: fixed;
  width: 100%;
}

.jp-Placeholder-prompt {
  display: table-cell;
  box-sizing: border-box;
}

.jp-Placeholder-content {
  display: table-cell;
  padding: 4px 6px;
  border: 1px solid transparent;
  border-radius: 0;
  background: none;
  box-sizing: border-box;
  cursor: pointer;
}

.jp-Placeholder-contentContainer {
  display: flex;
}

.jp-Placeholder-content:hover,
.jp-InputPlaceholder > .jp-Placeholder-content:hover {
  border-color: var(--jp-layout-color3);
}

.jp-Placeholder-content .jp-MoreHorizIcon {
  width: 32px;
  height: 16px;
  border: 1px solid transparent;
  border-radius: var(--jp-border-radius);
}

.jp-Placeholder-content .jp-MoreHorizIcon:hover {
  border: 1px solid var(--jp-border-color1);
  box-shadow: 0 0 2px 0 rgba(0, 0, 0, 0.25);
  background-color: var(--jp-layout-color0);
}

.jp-PlaceholderText {
  white-space: nowrap;
  overflow-x: hidden;
  color: var(--jp-inverse-layout-color3);
  font-family: var(--jp-code-font-family);
}

.jp-InputPlaceholder > .jp-Placeholder-content {
  border-color: var(--jp-cell-editor-border-color);
  background: var(--jp-cell-editor-background);
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Private CSS variables
|----------------------------------------------------------------------------*/

:root {
  --jp-private-cell-scrolling-output-offset: 5px;
}

/*-----------------------------------------------------------------------------
| Cell
|----------------------------------------------------------------------------*/

.jp-Cell {
  padding: var(--jp-cell-padding);
  margin: 0;
  border: none;
  outline: none;
  background: transparent;
}

/*-----------------------------------------------------------------------------
| Common input/output
|----------------------------------------------------------------------------*/

.jp-Cell-inputWrapper,
.jp-Cell-outputWrapper {
  display: flex;
  flex-direction: row;
  padding: 0;
  margin: 0;

  /* Added to reveal the box-shadow on the input and output collapsers. */
  overflow: visible;
}

/* Only input/output areas inside cells */
.jp-Cell-inputArea,
.jp-Cell-outputArea {
  flex: 1 1 auto;
}

/*-----------------------------------------------------------------------------
| Collapser
|----------------------------------------------------------------------------*/

/* Make the output collapser disappear when there is not output, but do so
 * in a manner that leaves it in the layout and preserves its width.
 */
.jp-Cell.jp-mod-noOutputs .jp-Cell-outputCollapser {
  border: none !important;
  background: transparent !important;
}

.jp-Cell:not(.jp-mod-noOutputs) .jp-Cell-outputCollapser {
  min-height: var(--jp-cell-collapser-min-height);
}

/*-----------------------------------------------------------------------------
| Output
|----------------------------------------------------------------------------*/

/* Put a space between input and output when there IS output */
.jp-Cell:not(.jp-mod-noOutputs) .jp-Cell-outputWrapper {
  margin-top: 5px;
}

.jp-CodeCell.jp-mod-outputsScrolled .jp-Cell-outputArea {
  overflow-y: auto;
  max-height: 24em;
  margin-left: var(--jp-private-cell-scrolling-output-offset);
  resize: vertical;
}

.jp-CodeCell.jp-mod-outputsScrolled .jp-Cell-outputArea[style*='height'] {
  max-height: unset;
}

.jp-CodeCell.jp-mod-outputsScrolled .jp-Cell-outputArea::after {
  content: ' ';
  box-shadow: inset 0 0 6px 2px rgb(0 0 0 / 30%);
  width: 100%;
  height: 100%;
  position: sticky;
  bottom: 0;
  top: 0;
  margin-top: -50%;
  float: left;
  display: block;
  pointer-events: none;
}

.jp-CodeCell.jp-mod-outputsScrolled .jp-OutputArea-child {
  padding-top: 6px;
}

.jp-CodeCell.jp-mod-outputsScrolled .jp-OutputArea-prompt {
  width: calc(
    var(--jp-cell-prompt-width) - var(--jp-private-cell-scrolling-output-offset)
  );
}

.jp-CodeCell.jp-mod-outputsScrolled .jp-OutputArea-promptOverlay {
  left: calc(-1 * var(--jp-private-cell-scrolling-output-offset));
}

/*-----------------------------------------------------------------------------
| CodeCell
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| MarkdownCell
|----------------------------------------------------------------------------*/

.jp-MarkdownOutput {
  display: table-cell;
  width: 100%;
  margin-top: 0;
  margin-bottom: 0;
  padding-left: var(--jp-code-padding);
}

.jp-MarkdownOutput.jp-RenderedHTMLCommon {
  overflow: auto;
}

/* collapseHeadingButton (show always if hiddenCellsButton is _not_ shown) */
.jp-collapseHeadingButton {
  display: flex;
  min-height: var(--jp-cell-collapser-min-height);
  font-size: var(--jp-code-font-size);
  position: absolute;
  background-color: transparent;
  background-size: 25px;
  background-repeat: no-repeat;
  background-position-x: center;
  background-position-y: top;
  background-image: var(--jp-icon-caret-down);
  right: 0;
  top: 0;
  bottom: 0;
}

.jp-collapseHeadingButton.jp-mod-collapsed {
  background-image: var(--jp-icon-caret-right);
}

/*
 set the container font size to match that of content
 so that the nested collapse buttons have the right size
*/
.jp-MarkdownCell .jp-InputPrompt {
  font-size: var(--jp-content-font-size1);
}

/*
  Align collapseHeadingButton with cell top header
  The font sizes are identical to the ones in packages/rendermime/style/base.css
*/
.jp-mod-rendered .jp-collapseHeadingButton[data-heading-level='1'] {
  font-size: var(--jp-content-font-size5);
  background-position-y: calc(0.3 * var(--jp-content-font-size5));
}

.jp-mod-rendered .jp-collapseHeadingButton[data-heading-level='2'] {
  font-size: var(--jp-content-font-size4);
  background-position-y: calc(0.3 * var(--jp-content-font-size4));
}

.jp-mod-rendered .jp-collapseHeadingButton[data-heading-level='3'] {
  font-size: var(--jp-content-font-size3);
  background-position-y: calc(0.3 * var(--jp-content-font-size3));
}

.jp-mod-rendered .jp-collapseHeadingButton[data-heading-level='4'] {
  font-size: var(--jp-content-font-size2);
  background-position-y: calc(0.3 * var(--jp-content-font-size2));
}

.jp-mod-rendered .jp-collapseHeadingButton[data-heading-level='5'] {
  font-size: var(--jp-content-font-size1);
  background-position-y: top;
}

.jp-mod-rendered .jp-collapseHeadingButton[data-heading-level='6'] {
  font-size: var(--jp-content-font-size0);
  background-position-y: top;
}

/* collapseHeadingButton (show only on (hover,active) if hiddenCellsButton is shown) */
.jp-Notebook.jp-mod-showHiddenCellsButton .jp-collapseHeadingButton {
  display: none;
}

.jp-Notebook.jp-mod-showHiddenCellsButton
  :is(.jp-MarkdownCell:hover, .jp-mod-active)
  .jp-collapseHeadingButton {
  display: flex;
}

/* showHiddenCellsButton (only show if jp-mod-showHiddenCellsButton is set, which
is a consequence of the showHiddenCellsButton option in Notebook Settings)*/
.jp-Notebook.jp-mod-showHiddenCellsButton .jp-showHiddenCellsButton {
  margin-left: calc(var(--jp-cell-prompt-width) + 2 * var(--jp-code-padding));
  margin-top: var(--jp-code-padding);
  border: 1px solid var(--jp-border-color2);
  background-color: var(--jp-border-color3) !important;
  color: var(--jp-content-font-color0) !important;
  display: flex;
}

.jp-Notebook.jp-mod-showHiddenCellsButton .jp-showHiddenCellsButton:hover {
  background-color: var(--jp-border-color2) !important;
}

.jp-showHiddenCellsButton {
  display: none;
}

/*-----------------------------------------------------------------------------
| Printing
|----------------------------------------------------------------------------*/

/*
Using block instead of flex to allow the use of the break-inside CSS property for
cell outputs.
*/

@media print {
  .jp-Cell-inputWrapper,
  .jp-Cell-outputWrapper {
    display: block;
  }
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Variables
|----------------------------------------------------------------------------*/

:root {
  --jp-notebook-toolbar-padding: 2px 5px 2px 2px;
}

/*-----------------------------------------------------------------------------

/*-----------------------------------------------------------------------------
| Styles
|----------------------------------------------------------------------------*/

.jp-NotebookPanel-toolbar {
  padding: var(--jp-notebook-toolbar-padding);

  /* disable paint containment from lumino 2.0 default strict CSS containment */
  contain: style size !important;
}

.jp-Toolbar-item.jp-Notebook-toolbarCellType .jp-select-wrapper.jp-mod-focused {
  border: none;
  box-shadow: none;
}

.jp-Notebook-toolbarCellTypeDropdown select {
  height: 24px;
  font-size: var(--jp-ui-font-size1);
  line-height: 14px;
  border-radius: 0;
  display: block;
}

.jp-Notebook-toolbarCellTypeDropdown span {
  top: 5px !important;
}

.jp-Toolbar-responsive-popup {
  position: absolute;
  height: fit-content;
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: flex-end;
  border-bottom: var(--jp-border-width) solid var(--jp-toolbar-border-color);
  box-shadow: var(--jp-toolbar-box-shadow);
  background: var(--jp-toolbar-background);
  min-height: var(--jp-toolbar-micro-height);
  padding: var(--jp-notebook-toolbar-padding);
  z-index: 1;
  right: 0;
  top: 0;
}

.jp-Toolbar > .jp-Toolbar-responsive-opener {
  margin-left: auto;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Variables
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------

/*-----------------------------------------------------------------------------
| Styles
|----------------------------------------------------------------------------*/

.jp-Notebook-ExecutionIndicator {
  position: relative;
  display: inline-block;
  height: 100%;
  z-index: 9997;
}

.jp-Notebook-ExecutionIndicator-tooltip {
  visibility: hidden;
  height: auto;
  width: max-content;
  width: -moz-max-content;
  background-color: var(--jp-layout-color2);
  color: var(--jp-ui-font-color1);
  text-align: justify;
  border-radius: 6px;
  padding: 0 5px;
  position: fixed;
  display: table;
}

.jp-Notebook-ExecutionIndicator-tooltip.up {
  transform: translateX(-50%) translateY(-100%) translateY(-32px);
}

.jp-Notebook-ExecutionIndicator-tooltip.down {
  transform: translateX(calc(-100% + 16px)) translateY(5px);
}

.jp-Notebook-ExecutionIndicator-tooltip.hidden {
  display: none;
}

.jp-Notebook-ExecutionIndicator:hover .jp-Notebook-ExecutionIndicator-tooltip {
  visibility: visible;
}

.jp-Notebook-ExecutionIndicator span {
  font-size: var(--jp-ui-font-size1);
  font-family: var(--jp-ui-font-family);
  color: var(--jp-ui-font-color1);
  line-height: 24px;
  display: block;
}

.jp-Notebook-ExecutionIndicator-progress-bar {
  display: flex;
  justify-content: center;
  height: 100%;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*
 * Execution indicator
 */
.jp-tocItem-content::after {
  content: '';

  /* Must be identical to form a circle */
  width: 12px;
  height: 12px;
  background: none;
  border: none;
  position: absolute;
  right: 0;
}

.jp-tocItem-content[data-running='0']::after {
  border-radius: 50%;
  border: var(--jp-border-width) solid var(--jp-inverse-layout-color3);
  background: none;
}

.jp-tocItem-content[data-running='1']::after {
  border-radius: 50%;
  border: var(--jp-border-width) solid var(--jp-inverse-layout-color3);
  background-color: var(--jp-inverse-layout-color3);
}

.jp-tocItem-content[data-running='0'],
.jp-tocItem-content[data-running='1'] {
  margin-right: 12px;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

.jp-Notebook-footer {
  height: 27px;
  margin-left: calc(
    var(--jp-cell-prompt-width) + var(--jp-cell-collapser-width) +
      var(--jp-cell-padding)
  );
  width: calc(
    100% -
      (
        var(--jp-cell-prompt-width) + var(--jp-cell-collapser-width) +
          var(--jp-cell-padding) + var(--jp-cell-padding)
      )
  );
  border: var(--jp-border-width) solid var(--jp-cell-editor-border-color);
  color: var(--jp-ui-font-color3);
  margin-top: 6px;
  background: none;
  cursor: pointer;
}

.jp-Notebook-footer:focus {
  border-color: var(--jp-cell-editor-active-border-color);
}

/* For devices that support hovering, hide footer until hover */
@media (hover: hover) {
  .jp-Notebook-footer {
    opacity: 0;
  }

  .jp-Notebook-footer:focus,
  .jp-Notebook-footer:hover {
    opacity: 1;
  }
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Imports
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| CSS variables
|----------------------------------------------------------------------------*/

:root {
  --jp-side-by-side-output-size: 1fr;
  --jp-side-by-side-resized-cell: var(--jp-side-by-side-output-size);
  --jp-private-notebook-dragImage-width: 304px;
  --jp-private-notebook-dragImage-height: 36px;
  --jp-private-notebook-selected-color: var(--md-blue-400);
  --jp-private-notebook-active-color: var(--md-green-400);
}

/*-----------------------------------------------------------------------------
| Notebook
|----------------------------------------------------------------------------*/

/* stylelint-disable selector-max-class */

.jp-NotebookPanel {
  display: block;
  height: 100%;
}

.jp-NotebookPanel.jp-Document {
  min-width: 240px;
  min-height: 120px;
}

.jp-Notebook {
  padding: var(--jp-notebook-padding);
  outline: none;
  overflow: auto;
  background: var(--jp-layout-color0);
}

.jp-Notebook.jp-mod-scrollPastEnd::after {
  display: block;
  content: '';
  min-height: var(--jp-notebook-scroll-padding);
}

.jp-MainAreaWidget-ContainStrict .jp-Notebook * {
  contain: strict;
}

.jp-Notebook .jp-Cell {
  overflow: visible;
}

.jp-Notebook .jp-Cell .jp-InputPrompt {
  cursor: move;
}

/*-----------------------------------------------------------------------------
| Notebook state related styling
|
| The notebook and cells each have states, here are the possibilities:
|
| - Notebook
|   - Command
|   - Edit
| - Cell
|   - None
|   - Active (only one can be active)
|   - Selected (the cells actions are applied to)
|   - Multiselected (when multiple selected, the cursor)
|   - No outputs
|----------------------------------------------------------------------------*/

/* Command or edit modes */

.jp-Notebook .jp-Cell:not(.jp-mod-active) .jp-InputPrompt {
  opacity: var(--jp-cell-prompt-not-active-opacity);
  color: var(--jp-cell-prompt-not-active-font-color);
}

.jp-Notebook .jp-Cell:not(.jp-mod-active) .jp-OutputPrompt {
  opacity: var(--jp-cell-prompt-not-active-opacity);
  color: var(--jp-cell-prompt-not-active-font-color);
}

/* cell is active */
.jp-Notebook .jp-Cell.jp-mod-active .jp-Collapser {
  background: var(--jp-brand-color1);
}

/* cell is dirty */
.jp-Notebook .jp-Cell.jp-mod-dirty .jp-InputPrompt {
  color: var(--jp-warn-color1);
}

.jp-Notebook .jp-Cell.jp-mod-dirty .jp-InputPrompt::before {
  color: var(--jp-warn-color1);
  content: '•';
}

.jp-Notebook .jp-Cell.jp-mod-active.jp-mod-dirty .jp-Collapser {
  background: var(--jp-warn-color1);
}

/* collapser is hovered */
.jp-Notebook .jp-Cell .jp-Collapser:hover {
  box-shadow: var(--jp-elevation-z2);
  background: var(--jp-brand-color1);
  opacity: var(--jp-cell-collapser-not-active-hover-opacity);
}

/* cell is active and collapser is hovered */
.jp-Notebook .jp-Cell.jp-mod-active .jp-Collapser:hover {
  background: var(--jp-brand-color0);
  opacity: 1;
}

/* Command mode */

.jp-Notebook.jp-mod-commandMode .jp-Cell.jp-mod-selected {
  background: var(--jp-notebook-multiselected-color);
}

.jp-Notebook.jp-mod-commandMode
  .jp-Cell.jp-mod-active.jp-mod-selected:not(.jp-mod-multiSelected) {
  background: transparent;
}

/* Edit mode */

.jp-Notebook.jp-mod-editMode .jp-Cell.jp-mod-active .jp-InputArea-editor {
  border: var(--jp-border-width) solid var(--jp-cell-editor-active-border-color);
  box-shadow: var(--jp-input-box-shadow);
  background-color: var(--jp-cell-editor-active-background);
}

/*-----------------------------------------------------------------------------
| Notebook drag and drop
|----------------------------------------------------------------------------*/

.jp-Notebook-cell.jp-mod-dropSource {
  opacity: 0.5;
}

.jp-Notebook-cell.jp-mod-dropTarget,
.jp-Notebook.jp-mod-commandMode
  .jp-Notebook-cell.jp-mod-active.jp-mod-selected.jp-mod-dropTarget {
  border-top-color: var(--jp-private-notebook-selected-color);
  border-top-style: solid;
  border-top-width: 2px;
}

.jp-dragImage {
  display: block;
  flex-direction: row;
  width: var(--jp-private-notebook-dragImage-width);
  height: var(--jp-private-notebook-dragImage-height);
  border: var(--jp-border-width) solid var(--jp-cell-editor-border-color);
  background: var(--jp-cell-editor-background);
  overflow: visible;
}

.jp-dragImage-singlePrompt {
  box-shadow: 2px 2px 4px 0 rgba(0, 0, 0, 0.12);
}

.jp-dragImage .jp-dragImage-content {
  flex: 1 1 auto;
  z-index: 2;
  font-size: var(--jp-code-font-size);
  font-family: var(--jp-code-font-family);
  line-height: var(--jp-code-line-height);
  padding: var(--jp-code-padding);
  border: var(--jp-border-width) solid var(--jp-cell-editor-border-color);
  background: var(--jp-cell-editor-background-color);
  color: var(--jp-content-font-color3);
  text-align: left;
  margin: 4px 4px 4px 0;
}

.jp-dragImage .jp-dragImage-prompt {
  flex: 0 0 auto;
  min-width: 36px;
  color: var(--jp-cell-inprompt-font-color);
  padding: var(--jp-code-padding);
  padding-left: 12px;
  font-family: var(--jp-cell-prompt-font-family);
  letter-spacing: var(--jp-cell-prompt-letter-spacing);
  line-height: 1.9;
  font-size: var(--jp-code-font-size);
  border: var(--jp-border-width) solid transparent;
}

.jp-dragImage-multipleBack {
  z-index: -1;
  position: absolute;
  height: 32px;
  width: 300px;
  top: 8px;
  left: 8px;
  background: var(--jp-layout-color2);
  border: var(--jp-border-width) solid var(--jp-input-border-color);
  box-shadow: 2px 2px 4px 0 rgba(0, 0, 0, 0.12);
}

/*-----------------------------------------------------------------------------
| Cell toolbar
|----------------------------------------------------------------------------*/

.jp-NotebookTools {
  display: block;
  min-width: var(--jp-sidebar-min-width);
  color: var(--jp-ui-font-color1);
  background: var(--jp-layout-color1);

  /* This is needed so that all font sizing of children done in ems is
    * relative to this base size */
  font-size: var(--jp-ui-font-size1);
  overflow: auto;
}

.jp-ActiveCellTool {
  padding: 12px 0;
  display: flex;
}

.jp-ActiveCellTool-Content {
  flex: 1 1 auto;
}

.jp-ActiveCellTool .jp-ActiveCellTool-CellContent {
  background: var(--jp-cell-editor-background);
  border: var(--jp-border-width) solid var(--jp-cell-editor-border-color);
  border-radius: 0;
  min-height: 29px;
}

.jp-ActiveCellTool .jp-InputPrompt {
  min-width: calc(var(--jp-cell-prompt-width) * 0.75);
}

.jp-ActiveCellTool-CellContent > pre {
  padding: 5px 4px;
  margin: 0;
  white-space: normal;
}

.jp-MetadataEditorTool {
  flex-direction: column;
  padding: 12px 0;
}

.jp-RankedPanel > :not(:first-child) {
  margin-top: 12px;
}

.jp-KeySelector select.jp-mod-styled {
  font-size: var(--jp-ui-font-size1);
  color: var(--jp-ui-font-color0);
  border: var(--jp-border-width) solid var(--jp-border-color1);
}

.jp-KeySelector label,
.jp-MetadataEditorTool label,
.jp-NumberSetter label {
  line-height: 1.4;
}

.jp-NotebookTools .jp-select-wrapper {
  margin-top: 4px;
  margin-bottom: 0;
}

.jp-NumberSetter input {
  width: 100%;
  margin-top: 4px;
}

.jp-NotebookTools .jp-Collapse {
  margin-top: 16px;
}

/*-----------------------------------------------------------------------------
| Presentation Mode (.jp-mod-presentationMode)
|----------------------------------------------------------------------------*/

.jp-mod-presentationMode .jp-Notebook {
  --jp-content-font-size1: var(--jp-content-presentation-font-size1);
  --jp-code-font-size: var(--jp-code-presentation-font-size);
}

.jp-mod-presentationMode .jp-Notebook .jp-Cell .jp-InputPrompt,
.jp-mod-presentationMode .jp-Notebook .jp-Cell .jp-OutputPrompt {
  flex: 0 0 110px;
}

/*-----------------------------------------------------------------------------
| Side-by-side Mode (.jp-mod-sideBySide)
|----------------------------------------------------------------------------*/
.jp-mod-sideBySide.jp-Notebook .jp-Notebook-cell {
  margin-top: 3em;
  margin-bottom: 3em;
  margin-left: 5%;
  margin-right: 5%;
}

.jp-mod-sideBySide.jp-Notebook .jp-CodeCell {
  display: grid;
  grid-template-columns: minmax(0, 1fr) min-content minmax(
      0,
      var(--jp-side-by-side-output-size)
    );
  grid-template-rows: auto minmax(0, 1fr) auto;
  grid-template-areas:
    'header header header'
    'input handle output'
    'footer footer footer';
}

.jp-mod-sideBySide.jp-Notebook .jp-CodeCell.jp-mod-resizedCell {
  grid-template-columns: minmax(0, 1fr) min-content minmax(
      0,
      var(--jp-side-by-side-resized-cell)
    );
}

.jp-mod-sideBySide.jp-Notebook .jp-CodeCell .jp-CellHeader {
  grid-area: header;
}

.jp-mod-sideBySide.jp-Notebook .jp-CodeCell .jp-Cell-inputWrapper {
  grid-area: input;
}

.jp-mod-sideBySide.jp-Notebook .jp-CodeCell .jp-Cell-outputWrapper {
  /* overwrite the default margin (no vertical separation needed in side by side move */
  margin-top: 0;
  grid-area: output;
}

.jp-mod-sideBySide.jp-Notebook .jp-CodeCell .jp-CellFooter {
  grid-area: footer;
}

.jp-mod-sideBySide.jp-Notebook .jp-CodeCell .jp-CellResizeHandle {
  grid-area: handle;
  user-select: none;
  display: block;
  height: 100%;
  cursor: ew-resize;
  padding: 0 var(--jp-cell-padding);
}

.jp-mod-sideBySide.jp-Notebook .jp-CodeCell .jp-CellResizeHandle::after {
  content: '';
  display: block;
  background: var(--jp-border-color2);
  height: 100%;
  width: 5px;
}

.jp-mod-sideBySide.jp-Notebook
  .jp-CodeCell.jp-mod-resizedCell
  .jp-CellResizeHandle::after {
  background: var(--jp-border-color0);
}

.jp-CellResizeHandle {
  display: none;
}

/*-----------------------------------------------------------------------------
| Placeholder
|----------------------------------------------------------------------------*/

.jp-Cell-Placeholder {
  padding-left: 55px;
}

.jp-Cell-Placeholder-wrapper {
  background: #fff;
  border: 1px solid;
  border-color: #e5e6e9 #dfe0e4 #d0d1d5;
  border-radius: 4px;
  -webkit-border-radius: 4px;
  margin: 10px 15px;
}

.jp-Cell-Placeholder-wrapper-inner {
  padding: 15px;
  position: relative;
}

.jp-Cell-Placeholder-wrapper-body {
  background-repeat: repeat;
  background-size: 50% auto;
}

.jp-Cell-Placeholder-wrapper-body div {
  background: #f6f7f8;
  background-image: -webkit-linear-gradient(
    left,
    #f6f7f8 0%,
    #edeef1 20%,
    #f6f7f8 40%,
    #f6f7f8 100%
  );
  background-repeat: no-repeat;
  background-size: 800px 104px;
  height: 104px;
  position: absolute;
  right: 15px;
  left: 15px;
  top: 15px;
}

div.jp-Cell-Placeholder-h1 {
  top: 20px;
  height: 20px;
  left: 15px;
  width: 150px;
}

div.jp-Cell-Placeholder-h2 {
  left: 15px;
  top: 50px;
  height: 10px;
  width: 100px;
}

div.jp-Cell-Placeholder-content-1,
div.jp-Cell-Placeholder-content-2,
div.jp-Cell-Placeholder-content-3 {
  left: 15px;
  right: 15px;
  height: 10px;
}

div.jp-Cell-Placeholder-content-1 {
  top: 100px;
}

div.jp-Cell-Placeholder-content-2 {
  top: 120px;
}

div.jp-Cell-Placeholder-content-3 {
  top: 140px;
}

</style>
<style type="text/css">
/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*
The following CSS variables define the main, public API for styling JupyterLab.
These variables should be used by all plugins wherever possible. In other
words, plugins should not define custom colors, sizes, etc unless absolutely
necessary. This enables users to change the visual theme of JupyterLab
by changing these variables.

Many variables appear in an ordered sequence (0,1,2,3). These sequences
are designed to work well together, so for example, `--jp-border-color1` should
be used with `--jp-layout-color1`. The numbers have the following meanings:

* 0: super-primary, reserved for special emphasis
* 1: primary, most important under normal situations
* 2: secondary, next most important under normal situations
* 3: tertiary, next most important under normal situations

Throughout JupyterLab, we are mostly following principles from Google's
Material Design when selecting colors. We are not, however, following
all of MD as it is not optimized for dense, information rich UIs.
*/

:root {
  /* Elevation
   *
   * We style box-shadows using Material Design's idea of elevation. These particular numbers are taken from here:
   *
   * https://github.com/material-components/material-components-web
   * https://material-components-web.appspot.com/elevation.html
   */

  --jp-shadow-base-lightness: 0;
  --jp-shadow-umbra-color: rgba(
    var(--jp-shadow-base-lightness),
    var(--jp-shadow-base-lightness),
    var(--jp-shadow-base-lightness),
    0.2
  );
  --jp-shadow-penumbra-color: rgba(
    var(--jp-shadow-base-lightness),
    var(--jp-shadow-base-lightness),
    var(--jp-shadow-base-lightness),
    0.14
  );
  --jp-shadow-ambient-color: rgba(
    var(--jp-shadow-base-lightness),
    var(--jp-shadow-base-lightness),
    var(--jp-shadow-base-lightness),
    0.12
  );
  --jp-elevation-z0: none;
  --jp-elevation-z1: 0 2px 1px -1px var(--jp-shadow-umbra-color),
    0 1px 1px 0 var(--jp-shadow-penumbra-color),
    0 1px 3px 0 var(--jp-shadow-ambient-color);
  --jp-elevation-z2: 0 3px 1px -2px var(--jp-shadow-umbra-color),
    0 2px 2px 0 var(--jp-shadow-penumbra-color),
    0 1px 5px 0 var(--jp-shadow-ambient-color);
  --jp-elevation-z4: 0 2px 4px -1px var(--jp-shadow-umbra-color),
    0 4px 5px 0 var(--jp-shadow-penumbra-color),
    0 1px 10px 0 var(--jp-shadow-ambient-color);
  --jp-elevation-z6: 0 3px 5px -1px var(--jp-shadow-umbra-color),
    0 6px 10px 0 var(--jp-shadow-penumbra-color),
    0 1px 18px 0 var(--jp-shadow-ambient-color);
  --jp-elevation-z8: 0 5px 5px -3px var(--jp-shadow-umbra-color),
    0 8px 10px 1px var(--jp-shadow-penumbra-color),
    0 3px 14px 2px var(--jp-shadow-ambient-color);
  --jp-elevation-z12: 0 7px 8px -4px var(--jp-shadow-umbra-color),
    0 12px 17px 2px var(--jp-shadow-penumbra-color),
    0 5px 22px 4px var(--jp-shadow-ambient-color);
  --jp-elevation-z16: 0 8px 10px -5px var(--jp-shadow-umbra-color),
    0 16px 24px 2px var(--jp-shadow-penumbra-color),
    0 6px 30px 5px var(--jp-shadow-ambient-color);
  --jp-elevation-z20: 0 10px 13px -6px var(--jp-shadow-umbra-color),
    0 20px 31px 3px var(--jp-shadow-penumbra-color),
    0 8px 38px 7px var(--jp-shadow-ambient-color);
  --jp-elevation-z24: 0 11px 15px -7px var(--jp-shadow-umbra-color),
    0 24px 38px 3px var(--jp-shadow-penumbra-color),
    0 9px 46px 8px var(--jp-shadow-ambient-color);

  /* Borders
   *
   * The following variables, specify the visual styling of borders in JupyterLab.
   */

  --jp-border-width: 1px;
  --jp-border-color0: var(--md-grey-400);
  --jp-border-color1: var(--md-grey-400);
  --jp-border-color2: var(--md-grey-300);
  --jp-border-color3: var(--md-grey-200);
  --jp-inverse-border-color: var(--md-grey-600);
  --jp-border-radius: 2px;

  /* UI Fonts
   *
   * The UI font CSS variables are used for the typography all of the JupyterLab
   * user interface elements that are not directly user generated content.
   *
   * The font sizing here is done assuming that the body font size of --jp-ui-font-size1
   * is applied to a parent element. When children elements, such as headings, are sized
   * in em all things will be computed relative to that body size.
   */

  --jp-ui-font-scale-factor: 1.2;
  --jp-ui-font-size0: 0.83333em;
  --jp-ui-font-size1: 13px; /* Base font size */
  --jp-ui-font-size2: 1.2em;
  --jp-ui-font-size3: 1.44em;
  --jp-ui-font-family: system-ui, -apple-system, blinkmacsystemfont, 'Segoe UI',
    helvetica, arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji',
    'Segoe UI Symbol';

  /*
   * Use these font colors against the corresponding main layout colors.
   * In a light theme, these go from dark to light.
   */

  /* Defaults use Material Design specification */
  --jp-ui-font-color0: rgba(0, 0, 0, 1);
  --jp-ui-font-color1: rgba(0, 0, 0, 0.87);
  --jp-ui-font-color2: rgba(0, 0, 0, 0.54);
  --jp-ui-font-color3: rgba(0, 0, 0, 0.38);

  /*
   * Use these against the brand/accent/warn/error colors.
   * These will typically go from light to darker, in both a dark and light theme.
   */

  --jp-ui-inverse-font-color0: rgba(255, 255, 255, 1);
  --jp-ui-inverse-font-color1: rgba(255, 255, 255, 1);
  --jp-ui-inverse-font-color2: rgba(255, 255, 255, 0.7);
  --jp-ui-inverse-font-color3: rgba(255, 255, 255, 0.5);

  /* Content Fonts
   *
   * Content font variables are used for typography of user generated content.
   *
   * The font sizing here is done assuming that the body font size of --jp-content-font-size1
   * is applied to a parent element. When children elements, such as headings, are sized
   * in em all things will be computed relative to that body size.
   */

  --jp-content-line-height: 1.6;
  --jp-content-font-scale-factor: 1.2;
  --jp-content-font-size0: 0.83333em;
  --jp-content-font-size1: 14px; /* Base font size */
  --jp-content-font-size2: 1.2em;
  --jp-content-font-size3: 1.44em;
  --jp-content-font-size4: 1.728em;
  --jp-content-font-size5: 2.0736em;

  /* This gives a magnification of about 125% in presentation mode over normal. */
  --jp-content-presentation-font-size1: 17px;
  --jp-content-heading-line-height: 1;
  --jp-content-heading-margin-top: 1.2em;
  --jp-content-heading-margin-bottom: 0.8em;
  --jp-content-heading-font-weight: 500;

  /* Defaults use Material Design specification */
  --jp-content-font-color0: rgba(0, 0, 0, 1);
  --jp-content-font-color1: rgba(0, 0, 0, 0.87);
  --jp-content-font-color2: rgba(0, 0, 0, 0.54);
  --jp-content-font-color3: rgba(0, 0, 0, 0.38);
  --jp-content-link-color: var(--md-blue-900);
  --jp-content-font-family: system-ui, -apple-system, blinkmacsystemfont,
    'Segoe UI', helvetica, arial, sans-serif, 'Apple Color Emoji',
    'Segoe UI Emoji', 'Segoe UI Symbol';

  /*
   * Code Fonts
   *
   * Code font variables are used for typography of code and other monospaces content.
   */

  --jp-code-font-size: 13px;
  --jp-code-line-height: 1.3077; /* 17px for 13px base */
  --jp-code-padding: 5px; /* 5px for 13px base, codemirror highlighting needs integer px value */
  --jp-code-font-family-default: menlo, consolas, 'DejaVu Sans Mono', monospace;
  --jp-code-font-family: var(--jp-code-font-family-default);

  /* This gives a magnification of about 125% in presentation mode over normal. */
  --jp-code-presentation-font-size: 16px;

  /* may need to tweak cursor width if you change font size */
  --jp-code-cursor-width0: 1.4px;
  --jp-code-cursor-width1: 2px;
  --jp-code-cursor-width2: 4px;

  /* Layout
   *
   * The following are the main layout colors use in JupyterLab. In a light
   * theme these would go from light to dark.
   */

  --jp-layout-color0: white;
  --jp-layout-color1: white;
  --jp-layout-color2: var(--md-grey-200);
  --jp-layout-color3: var(--md-grey-400);
  --jp-layout-color4: var(--md-grey-600);

  /* Inverse Layout
   *
   * The following are the inverse layout colors use in JupyterLab. In a light
   * theme these would go from dark to light.
   */

  --jp-inverse-layout-color0: #111;
  --jp-inverse-layout-color1: var(--md-grey-900);
  --jp-inverse-layout-color2: var(--md-grey-800);
  --jp-inverse-layout-color3: var(--md-grey-700);
  --jp-inverse-layout-color4: var(--md-grey-600);

  /* Brand/accent */

  --jp-brand-color0: var(--md-blue-900);
  --jp-brand-color1: var(--md-blue-700);
  --jp-brand-color2: var(--md-blue-300);
  --jp-brand-color3: var(--md-blue-100);
  --jp-brand-color4: var(--md-blue-50);
  --jp-accent-color0: var(--md-green-900);
  --jp-accent-color1: var(--md-green-700);
  --jp-accent-color2: var(--md-green-300);
  --jp-accent-color3: var(--md-green-100);

  /* State colors (warn, error, success, info) */

  --jp-warn-color0: var(--md-orange-900);
  --jp-warn-color1: var(--md-orange-700);
  --jp-warn-color2: var(--md-orange-300);
  --jp-warn-color3: var(--md-orange-100);
  --jp-error-color0: var(--md-red-900);
  --jp-error-color1: var(--md-red-700);
  --jp-error-color2: var(--md-red-300);
  --jp-error-color3: var(--md-red-100);
  --jp-success-color0: var(--md-green-900);
  --jp-success-color1: var(--md-green-700);
  --jp-success-color2: var(--md-green-300);
  --jp-success-color3: var(--md-green-100);
  --jp-info-color0: var(--md-cyan-900);
  --jp-info-color1: var(--md-cyan-700);
  --jp-info-color2: var(--md-cyan-300);
  --jp-info-color3: var(--md-cyan-100);

  /* Cell specific styles */

  --jp-cell-padding: 5px;
  --jp-cell-collapser-width: 8px;
  --jp-cell-collapser-min-height: 20px;
  --jp-cell-collapser-not-active-hover-opacity: 0.6;
  --jp-cell-editor-background: var(--md-grey-100);
  --jp-cell-editor-border-color: var(--md-grey-300);
  --jp-cell-editor-box-shadow: inset 0 0 2px var(--md-blue-300);
  --jp-cell-editor-active-background: var(--jp-layout-color0);
  --jp-cell-editor-active-border-color: var(--jp-brand-color1);
  --jp-cell-prompt-width: 64px;
  --jp-cell-prompt-font-family: var(--jp-code-font-family-default);
  --jp-cell-prompt-letter-spacing: 0;
  --jp-cell-prompt-opacity: 1;
  --jp-cell-prompt-not-active-opacity: 0.5;
  --jp-cell-prompt-not-active-font-color: var(--md-grey-700);

  /* A custom blend of MD grey and blue 600
   * See https://meyerweb.com/eric/tools/color-blend/#546E7A:1E88E5:5:hex */
  --jp-cell-inprompt-font-color: #307fc1;

  /* A custom blend of MD grey and orange 600
   * https://meyerweb.com/eric/tools/color-blend/#546E7A:F4511E:5:hex */
  --jp-cell-outprompt-font-color: #bf5b3d;

  /* Notebook specific styles */

  --jp-notebook-padding: 10px;
  --jp-notebook-select-background: var(--jp-layout-color1);
  --jp-notebook-multiselected-color: var(--md-blue-50);

  /* The scroll padding is calculated to fill enough space at the bottom of the
  notebook to show one single-line cell (with appropriate padding) at the top
  when the notebook is scrolled all the way to the bottom. We also subtract one
  pixel so that no scrollbar appears if we have just one single-line cell in the
  notebook. This padding is to enable a 'scroll past end' feature in a notebook.
  */
  --jp-notebook-scroll-padding: calc(
    100% - var(--jp-code-font-size) * var(--jp-code-line-height) -
      var(--jp-code-padding) - var(--jp-cell-padding) - 1px
  );

  /* Rendermime styles */

  --jp-rendermime-error-background: #fdd;
  --jp-rendermime-table-row-background: var(--md-grey-100);
  --jp-rendermime-table-row-hover-background: var(--md-light-blue-50);

  /* Dialog specific styles */

  --jp-dialog-background: rgba(0, 0, 0, 0.25);

  /* Console specific styles */

  --jp-console-padding: 10px;

  /* Toolbar specific styles */

  --jp-toolbar-border-color: var(--jp-border-color1);
  --jp-toolbar-micro-height: 8px;
  --jp-toolbar-background: var(--jp-layout-color1);
  --jp-toolbar-box-shadow: 0 0 2px 0 rgba(0, 0, 0, 0.24);
  --jp-toolbar-header-margin: 4px 4px 0 4px;
  --jp-toolbar-active-background: var(--md-grey-300);

  /* Statusbar specific styles */

  --jp-statusbar-height: 24px;

  /* Input field styles */

  --jp-input-box-shadow: inset 0 0 2px var(--md-blue-300);
  --jp-input-active-background: var(--jp-layout-color1);
  --jp-input-hover-background: var(--jp-layout-color1);
  --jp-input-background: var(--md-grey-100);
  --jp-input-border-color: var(--jp-inverse-border-color);
  --jp-input-active-border-color: var(--jp-brand-color1);
  --jp-input-active-box-shadow-color: rgba(19, 124, 189, 0.3);

  /* General editor styles */

  --jp-editor-selected-background: #d9d9d9;
  --jp-editor-selected-focused-background: #d7d4f0;
  --jp-editor-cursor-color: var(--jp-ui-font-color0);

  /* Code mirror specific styles */

  --jp-mirror-editor-keyword-color: #008000;
  --jp-mirror-editor-atom-color: #88f;
  --jp-mirror-editor-number-color: #080;
  --jp-mirror-editor-def-color: #00f;
  --jp-mirror-editor-variable-color: var(--md-grey-900);
  --jp-mirror-editor-variable-2-color: rgb(0, 54, 109);
  --jp-mirror-editor-variable-3-color: #085;
  --jp-mirror-editor-punctuation-color: #05a;
  --jp-mirror-editor-property-color: #05a;
  --jp-mirror-editor-operator-color: #a2f;
  --jp-mirror-editor-comment-color: #408080;
  --jp-mirror-editor-string-color: #ba2121;
  --jp-mirror-editor-string-2-color: #708;
  --jp-mirror-editor-meta-color: #a2f;
  --jp-mirror-editor-qualifier-color: #555;
  --jp-mirror-editor-builtin-color: #008000;
  --jp-mirror-editor-bracket-color: #997;
  --jp-mirror-editor-tag-color: #170;
  --jp-mirror-editor-attribute-color: #00c;
  --jp-mirror-editor-header-color: blue;
  --jp-mirror-editor-quote-color: #090;
  --jp-mirror-editor-link-color: #00c;
  --jp-mirror-editor-error-color: #f00;
  --jp-mirror-editor-hr-color: #999;

  /*
    RTC user specific colors.
    These colors are used for the cursor, username in the editor,
    and the icon of the user.
  */

  --jp-collaborator-color1: #ffad8e;
  --jp-collaborator-color2: #dac83d;
  --jp-collaborator-color3: #72dd76;
  --jp-collaborator-color4: #00e4d0;
  --jp-collaborator-color5: #45d4ff;
  --jp-collaborator-color6: #e2b1ff;
  --jp-collaborator-color7: #ff9de6;

  /* Vega extension styles */

  --jp-vega-background: white;

  /* Sidebar-related styles */

  --jp-sidebar-min-width: 250px;

  /* Search-related styles */

  --jp-search-toggle-off-opacity: 0.5;
  --jp-search-toggle-hover-opacity: 0.8;
  --jp-search-toggle-on-opacity: 1;
  --jp-search-selected-match-background-color: rgb(245, 200, 0);
  --jp-search-selected-match-color: black;
  --jp-search-unselected-match-background-color: var(
    --jp-inverse-layout-color0
  );
  --jp-search-unselected-match-color: var(--jp-ui-inverse-font-color0);

  /* Icon colors that work well with light or dark backgrounds */
  --jp-icon-contrast-color0: var(--md-purple-600);
  --jp-icon-contrast-color1: var(--md-green-600);
  --jp-icon-contrast-color2: var(--md-pink-600);
  --jp-icon-contrast-color3: var(--md-blue-600);

  /* Button colors */
  --jp-accept-color-normal: var(--md-blue-700);
  --jp-accept-color-hover: var(--md-blue-800);
  --jp-accept-color-active: var(--md-blue-900);
  --jp-warn-color-normal: var(--md-red-700);
  --jp-warn-color-hover: var(--md-red-800);
  --jp-warn-color-active: var(--md-red-900);
  --jp-reject-color-normal: var(--md-grey-600);
  --jp-reject-color-hover: var(--md-grey-700);
  --jp-reject-color-active: var(--md-grey-800);

  /* File or activity icons and switch semantic variables */
  --jp-jupyter-icon-color: #f37626;
  --jp-notebook-icon-color: #f37626;
  --jp-json-icon-color: var(--md-orange-700);
  --jp-console-icon-background-color: var(--md-blue-700);
  --jp-console-icon-color: white;
  --jp-terminal-icon-background-color: var(--md-grey-800);
  --jp-terminal-icon-color: var(--md-grey-200);
  --jp-text-editor-icon-color: var(--md-grey-700);
  --jp-inspector-icon-color: var(--md-grey-700);
  --jp-switch-color: var(--md-grey-400);
  --jp-switch-true-position-color: var(--md-orange-900);
}
</style>
<style type="text/css">
a.anchor-link {
   display: none;
}
.highlight  {
    margin: 0.4em;
}
.jp-Notebook {
    padding: 0;
}
:root {
    --jp-ui-font-size1: 20px;       /* instead of 14px */
    --jp-content-font-size1: 20px;  /* instead of 14px */
    --jp-code-font-size: 19px;      /* instead of 13px */
    --jp-cell-prompt-width: 110px;  /* instead of 64px */
}
@media print {
  body {
    margin: 0;
  }
}
</style>
<style type="text/css">
/* Overrides of notebook CSS for static HTML export */
.reveal {
  font-size: 160%;
}
.reveal table {
  font-size: var(--jp-ui-font-size1);
}
.reveal pre {
  width: inherit;
  padding: 0.4em;
  margin: 0px;
  font-family: monospace, sans-serif;
  font-size: 80%;
  box-shadow: 0px 0px 0px rgba(0, 0, 0, 0);
}
.reveal pre code {
  padding: 0px;
}
.reveal section img {
  border: 0px solid black;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0);
}
.reveal .slides {
  text-align: left;
}
.reveal.fade {
  opacity: 1;
}
.reveal .progress {
  position: static;
}

div.jp-InputArea-editor {
  padding: 0.06em;
}

div.code_cell {
  background-color: transparent;
}

div.output_area pre {
  font-family: monospace, sans-serif;
  font-size: 80%;
}

div.jp-OutputPrompt {
  /* 5px right shift to account for margin in parent container */
  margin: 5px 5px 0 0;
}

.reveal div.highlight {
  margin: 0;
}

.reveal div.highlight > pre {
  margin: 0;
  width: 100%;
  font-size: var(--jp-code-font-size);
}

.reveal div.jp-OutputArea-output > pre {
  margin: 0;
  width: 90%;
  font-size: var(--jp-code-font-size);
  box-shadow: none;
}

main {
  height: 100%;
}

/* Reveal navigation controls */

.reveal .controls .navigate-left,
.reveal .controls .navigate-left.enabled {
  border-right-color: #727272;
}
.reveal .controls .navigate-left.enabled:hover,
.reveal .controls .navigate-left.enabled.enabled:hover {
  border-right-color: #dfdfdf;
}
.reveal .controls .navigate-right,
.reveal .controls .navigate-right.enabled {
  border-left-color: #727272;
}
.reveal .controls .navigate-right.enabled:hover,
.reveal .controls .navigate-right.enabled.enabled:hover {
  border-left-color: #dfdfdf;
}
.reveal .controls .navigate-up,
.reveal .controls .navigate-up.enabled {
  border-bottom-color: #727272;
}
.reveal .controls .navigate-up.enabled:hover,
.reveal .controls .navigate-up.enabled.enabled:hover {
  border-bottom-color: #dfdfdf;
}
.reveal .controls .navigate-down,
.reveal .controls .navigate-down.enabled {
  border-top-color: #727272;
}
.reveal .controls .navigate-down.enabled:hover,
.reveal .controls .navigate-down.enabled.enabled:hover {
  border-top-color: #dfdfdf;
}
.reveal .progress span {
  background: #727272;
}

/* Scrollbars */

::-webkit-scrollbar {
  width: 6px;
  height: 6px;
}
::-webkit-scrollbar * {
  background: transparent;
}
::-webkit-scrollbar-thumb {
  background: #727272 !important;
}
</style>
<!-- Load mathjax -->
<script src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/latest.js?config=TeX-AMS_CHTML-full,Safe"> </script>
<!-- MathJax configuration -->
<script type="text/x-mathjax-config">
    init_mathjax = function() {
        if (window.MathJax) {
        // MathJax loaded
            MathJax.Hub.Config({
                TeX: {
                    equationNumbers: {
                    autoNumber: "AMS",
                    useLabelIds: true
                    }
                },
                tex2jax: {
                    inlineMath: [ ['$','$'], ["\\(","\\)"] ],
                    displayMath: [ ['$$','$$'], ["\\[","\\]"] ],
                    processEscapes: true,
                    processEnvironments: true
                },
                displayAlign: 'center',
                messageStyle: 'none',
                CommonHTML: {
                    linebreaks: {
                    automatic: true
                    }
                }
            });

            MathJax.Hub.Queue(["Typeset", MathJax.Hub]);
        }
    }
    init_mathjax();
    </script>
<!-- End of mathjax configuration --><!-- Reveal Theme -->
<link href="https://unpkg.com/reveal.js@4.0.2/dist/theme/simple.css" id="theme" rel="stylesheet"/>
</head>
<body class="jp-Notebook" data-jp-theme-light="true" data-jp-theme-name="JupyterLab Light">
<main>
<div class="reveal">
<div class="slides"><section><section>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p style="text-align:center">
<a href="https://skills.network/?utm_medium=Exinfluencer&amp;utm_source=Exinfluencer&amp;utm_content=000026UJ&amp;utm_term=10006555&amp;utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMDeveloperSkillsNetworkML0101ENSkillsNetwork20718538-2022-01-01" target="_blank">
<img alt="Skills Network Logo" src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/assets/logos/SN_web_lightmode.png" width="300"/>
</a>
</p>
<h1 id="Final-Project:-Building-a-Rainfall-Prediction-Classifier">Final Project: Building a Rainfall Prediction Classifier<a class="anchor-link" href="#Final-Project:-Building-a-Rainfall-Prediction-Classifier">¶</a></h1><p>Estimated time needed: <strong>60</strong> minutes</p>
<h2 id="Objectives">Objectives<a class="anchor-link" href="#Objectives">¶</a></h2><p>After completing this lab you will be able to:</p>
<ul>
<li>Explore and perform feature engineering on a real-world data set</li>
<li>Build a classifier pipeline and optimize it using grid search cross validation</li>
<li>Evaluate your model by interpreting various performance metrics and visualizations</li>
<li>Implement a different classifier by updating your pipeline</li>
<li>Use an appropriate set of parameters to search over in each case</li>
</ul>
<h2 id="Instruction(s)">Instruction(s)<a class="anchor-link" href="#Instruction(s)">¶</a></h2><p>After completing the Notebook:</p>
<ul>
<li>Download the notebook using <strong>File</strong> &gt; <strong>Download</strong>.</li>
<li>This notebook will be then graded using <strong>AI grader</strong> in the subsequent section.</li>
<li>Copy/Paste your markdown responses in the subsequent <strong>AI Mark assignment</strong>.</li>
</ul>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h1 id="About-The-Dataset">About The Dataset<a class="anchor-link" href="#About-The-Dataset">¶</a></h1><p>The original source of the data is Australian Government's Bureau of Meteorology and the latest data can be gathered from <a href="http://www.bom.gov.au/climate/dwo/?utm_medium=Exinfluencer&amp;utm_source=Exinfluencer&amp;utm_content=000026UJ&amp;utm_term=10006555&amp;utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMDeveloperSkillsNetworkML0101ENSkillsNetwork20718538-2022-01-01">http://www.bom.gov.au/climate/dwo/</a>.</p>
<p>The dataset you'll use in this project was downloaded from Kaggle at <a href="https://www.kaggle.com/datasets/jsphyg/weather-dataset-rattle-package?resource=download&amp;select=weatherAUS.csv">https://www.kaggle.com/datasets/jsphyg/weather-dataset-rattle-package/</a><br/>
Column definitions were gathered from <a href="http://www.bom.gov.au/climate/dwo/IDCJDW0000.shtml?utm_medium=Exinfluencer&amp;utm_source=Exinfluencer&amp;utm_content=000026UJ&amp;utm_term=10006555&amp;utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMDeveloperSkillsNetworkML0101ENSkillsNetwork20718538-2022-01-01">http://www.bom.gov.au/climate/dwo/IDCJDW0000.shtml</a></p>
<p>The dataset contains observations of weather metrics for each day from 2008 to 2017, and includes the following fields:</p>
<table>
<thead>
<tr>
<th style="text-align:left">Field</th>
<th style="text-align:left">Description</th>
<th style="text-align:left">Unit</th>
<th style="text-align:left">Type</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:left">Date</td>
<td style="text-align:left">Date of the Observation in YYYY-MM-DD</td>
<td style="text-align:left">Date</td>
<td style="text-align:left">object</td>
</tr>
<tr>
<td style="text-align:left">Location</td>
<td style="text-align:left">Location of the Observation</td>
<td style="text-align:left">Location</td>
<td style="text-align:left">object</td>
</tr>
<tr>
<td style="text-align:left">MinTemp</td>
<td style="text-align:left">Minimum temperature</td>
<td style="text-align:left">Celsius</td>
<td style="text-align:left">float</td>
</tr>
<tr>
<td style="text-align:left">MaxTemp</td>
<td style="text-align:left">Maximum temperature</td>
<td style="text-align:left">Celsius</td>
<td style="text-align:left">float</td>
</tr>
<tr>
<td style="text-align:left">Rainfall</td>
<td style="text-align:left">Amount of rainfall</td>
<td style="text-align:left">Millimeters</td>
<td style="text-align:left">float</td>
</tr>
<tr>
<td style="text-align:left">Evaporation</td>
<td style="text-align:left">Amount of evaporation</td>
<td style="text-align:left">Millimeters</td>
<td style="text-align:left">float</td>
</tr>
<tr>
<td style="text-align:left">Sunshine</td>
<td style="text-align:left">Amount of bright sunshine</td>
<td style="text-align:left">hours</td>
<td style="text-align:left">float</td>
</tr>
<tr>
<td style="text-align:left">WindGustDir</td>
<td style="text-align:left">Direction of the strongest gust</td>
<td style="text-align:left">Compass Points</td>
<td style="text-align:left">object</td>
</tr>
<tr>
<td style="text-align:left">WindGustSpeed</td>
<td style="text-align:left">Speed of the strongest gust</td>
<td style="text-align:left">Kilometers/Hour</td>
<td style="text-align:left">object</td>
</tr>
<tr>
<td style="text-align:left">WindDir9am</td>
<td style="text-align:left">Wind direction averaged over 10 minutes prior to 9am</td>
<td style="text-align:left">Compass Points</td>
<td style="text-align:left">object</td>
</tr>
<tr>
<td style="text-align:left">WindDir3pm</td>
<td style="text-align:left">Wind direction averaged over 10 minutes prior to 3pm</td>
<td style="text-align:left">Compass Points</td>
<td style="text-align:left">object</td>
</tr>
<tr>
<td style="text-align:left">WindSpeed9am</td>
<td style="text-align:left">Wind speed averaged over 10 minutes prior to 9am</td>
<td style="text-align:left">Kilometers/Hour</td>
<td style="text-align:left">float</td>
</tr>
<tr>
<td style="text-align:left">WindSpeed3pm</td>
<td style="text-align:left">Wind speed averaged over 10 minutes prior to 3pm</td>
<td style="text-align:left">Kilometers/Hour</td>
<td style="text-align:left">float</td>
</tr>
<tr>
<td style="text-align:left">Humidity9am</td>
<td style="text-align:left">Humidity at 9am</td>
<td style="text-align:left">Percent</td>
<td style="text-align:left">float</td>
</tr>
<tr>
<td style="text-align:left">Humidity3pm</td>
<td style="text-align:left">Humidity at 3pm</td>
<td style="text-align:left">Percent</td>
<td style="text-align:left">float</td>
</tr>
<tr>
<td style="text-align:left">Pressure9am</td>
<td style="text-align:left">Atmospheric pressure reduced to mean sea level at 9am</td>
<td style="text-align:left">Hectopascal</td>
<td style="text-align:left">float</td>
</tr>
<tr>
<td style="text-align:left">Pressure3pm</td>
<td style="text-align:left">Atmospheric pressure reduced to mean sea level at 3pm</td>
<td style="text-align:left">Hectopascal</td>
<td style="text-align:left">float</td>
</tr>
<tr>
<td style="text-align:left">Cloud9am</td>
<td style="text-align:left">Fraction of the sky obscured by cloud at 9am</td>
<td style="text-align:left">Eights</td>
<td style="text-align:left">float</td>
</tr>
<tr>
<td style="text-align:left">Cloud3pm</td>
<td style="text-align:left">Fraction of the sky obscured by cloud at 3pm</td>
<td style="text-align:left">Eights</td>
<td style="text-align:left">float</td>
</tr>
<tr>
<td style="text-align:left">Temp9am</td>
<td style="text-align:left">Temperature at 9am</td>
<td style="text-align:left">Celsius</td>
<td style="text-align:left">float</td>
</tr>
<tr>
<td style="text-align:left">Temp3pm</td>
<td style="text-align:left">Temperature at 3pm</td>
<td style="text-align:left">Celsius</td>
<td style="text-align:left">float</td>
</tr>
<tr>
<td style="text-align:left">RainToday</td>
<td style="text-align:left">If there was at least 1mm of rain today</td>
<td style="text-align:left">Yes/No</td>
<td style="text-align:left">object</td>
</tr>
<tr>
<td style="text-align:left">RainTomorrow</td>
<td style="text-align:left">If there is at least 1mm of rain tomorrow</td>
<td style="text-align:left">Yes/No</td>
<td style="text-align:left">object</td>
</tr>
</tbody>
</table>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h2 id="Install-and-import-the-required-libraries">Install and import the required libraries<a class="anchor-link" href="#Install-and-import-the-required-libraries">¶</a></h2>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Exectue the following cells to install and import the necessary libraries.</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [1]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="o">!</span>pip<span class="w"> </span>install<span class="w"> </span>numpy
<span class="o">!</span>pip<span class="w"> </span>install<span class="w"> </span>pandas
<span class="o">!</span>pip<span class="w"> </span>install<span class="w"> </span>matplotlib
<span class="o">!</span>pip<span class="w"> </span>install<span class="w"> </span>scikit-learn
<span class="o">!</span>pip<span class="w"> </span>install<span class="w"> </span>seaborn
</pre></div>
</div>
</div>
</div>
</div>
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
<div class="jp-OutputPrompt jp-OutputArea-prompt"></div>
<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="text/plain" tabindex="0">
<pre>Collecting numpy
  Downloading numpy-2.3.2-cp312-cp312-manylinux_2_27_x86_64.manylinux_2_28_x86_64.whl.metadata (62 kB)
Downloading numpy-2.3.2-cp312-cp312-manylinux_2_27_x86_64.manylinux_2_28_x86_64.whl (16.6 MB)
   <span class="ansi-black-intense-fg">━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━</span> <span class="ansi-green-fg">16.6/16.6 MB</span> <span class="ansi-red-fg">161.0 MB/s</span> eta <span class="ansi-cyan-fg">0:00:00</span>
Installing collected packages: numpy
Successfully installed numpy-2.3.2
Collecting pandas
  Downloading pandas-2.3.1-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.metadata (91 kB)
Requirement already satisfied: numpy&gt;=1.26.0 in /opt/conda/lib/python3.12/site-packages (from pandas) (2.3.2)
Requirement already satisfied: python-dateutil&gt;=2.8.2 in /opt/conda/lib/python3.12/site-packages (from pandas) (2.9.0.post0)
Requirement already satisfied: pytz&gt;=2020.1 in /opt/conda/lib/python3.12/site-packages (from pandas) (2024.2)
Collecting tzdata&gt;=2022.7 (from pandas)
  Downloading tzdata-2025.2-py2.py3-none-any.whl.metadata (1.4 kB)
Requirement already satisfied: six&gt;=1.5 in /opt/conda/lib/python3.12/site-packages (from python-dateutil&gt;=2.8.2-&gt;pandas) (1.17.0)
Downloading pandas-2.3.1-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (12.0 MB)
   <span class="ansi-black-intense-fg">━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━</span> <span class="ansi-green-fg">12.0/12.0 MB</span> <span class="ansi-red-fg">152.6 MB/s</span> eta <span class="ansi-cyan-fg">0:00:00</span>
Downloading tzdata-2025.2-py2.py3-none-any.whl (347 kB)
Installing collected packages: tzdata, pandas
Successfully installed pandas-2.3.1 tzdata-2025.2
Collecting matplotlib
  Downloading matplotlib-3.10.5-cp312-cp312-manylinux2014_x86_64.manylinux_2_17_x86_64.whl.metadata (11 kB)
Collecting contourpy&gt;=1.0.1 (from matplotlib)
  Downloading contourpy-1.3.3-cp312-cp312-manylinux_2_27_x86_64.manylinux_2_28_x86_64.whl.metadata (5.5 kB)
Collecting cycler&gt;=0.10 (from matplotlib)
  Downloading cycler-0.12.1-py3-none-any.whl.metadata (3.8 kB)
Collecting fonttools&gt;=4.22.0 (from matplotlib)
  Downloading fonttools-4.59.1-cp312-cp312-manylinux1_x86_64.manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_5_x86_64.whl.metadata (108 kB)
Collecting kiwisolver&gt;=1.3.1 (from matplotlib)
  Downloading kiwisolver-1.4.9-cp312-cp312-manylinux2014_x86_64.manylinux_2_17_x86_64.whl.metadata (6.3 kB)
Requirement already satisfied: numpy&gt;=1.23 in /opt/conda/lib/python3.12/site-packages (from matplotlib) (2.3.2)
Requirement already satisfied: packaging&gt;=20.0 in /opt/conda/lib/python3.12/site-packages (from matplotlib) (24.2)
Collecting pillow&gt;=8 (from matplotlib)
  Downloading pillow-11.3.0-cp312-cp312-manylinux_2_27_x86_64.manylinux_2_28_x86_64.whl.metadata (9.0 kB)
Collecting pyparsing&gt;=2.3.1 (from matplotlib)
  Downloading pyparsing-3.2.3-py3-none-any.whl.metadata (5.0 kB)
Requirement already satisfied: python-dateutil&gt;=2.7 in /opt/conda/lib/python3.12/site-packages (from matplotlib) (2.9.0.post0)
Requirement already satisfied: six&gt;=1.5 in /opt/conda/lib/python3.12/site-packages (from python-dateutil&gt;=2.7-&gt;matplotlib) (1.17.0)
Downloading matplotlib-3.10.5-cp312-cp312-manylinux2014_x86_64.manylinux_2_17_x86_64.whl (8.7 MB)
   <span class="ansi-black-intense-fg">━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━</span> <span class="ansi-green-fg">8.7/8.7 MB</span> <span class="ansi-red-fg">133.0 MB/s</span> eta <span class="ansi-cyan-fg">0:00:00</span>
Downloading contourpy-1.3.3-cp312-cp312-manylinux_2_27_x86_64.manylinux_2_28_x86_64.whl (362 kB)
Downloading cycler-0.12.1-py3-none-any.whl (8.3 kB)
Downloading fonttools-4.59.1-cp312-cp312-manylinux1_x86_64.manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_5_x86_64.whl (4.9 MB)
   <span class="ansi-black-intense-fg">━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━</span> <span class="ansi-green-fg">4.9/4.9 MB</span> <span class="ansi-red-fg">130.0 MB/s</span> eta <span class="ansi-cyan-fg">0:00:00</span>
Downloading kiwisolver-1.4.9-cp312-cp312-manylinux2014_x86_64.manylinux_2_17_x86_64.whl (1.5 MB)
   <span class="ansi-black-intense-fg">━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━</span> <span class="ansi-green-fg">1.5/1.5 MB</span> <span class="ansi-red-fg">46.4 MB/s</span> eta <span class="ansi-cyan-fg">0:00:00</span>
Downloading pillow-11.3.0-cp312-cp312-manylinux_2_27_x86_64.manylinux_2_28_x86_64.whl (6.6 MB)
   <span class="ansi-black-intense-fg">━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━</span> <span class="ansi-green-fg">6.6/6.6 MB</span> <span class="ansi-red-fg">150.8 MB/s</span> eta <span class="ansi-cyan-fg">0:00:00</span>
Downloading pyparsing-3.2.3-py3-none-any.whl (111 kB)
Installing collected packages: pyparsing, pillow, kiwisolver, fonttools, cycler, contourpy, matplotlib
Successfully installed contourpy-1.3.3 cycler-0.12.1 fonttools-4.59.1 kiwisolver-1.4.9 matplotlib-3.10.5 pillow-11.3.0 pyparsing-3.2.3
Collecting scikit-learn
  Downloading scikit_learn-1.7.1-cp312-cp312-manylinux2014_x86_64.manylinux_2_17_x86_64.whl.metadata (11 kB)
Requirement already satisfied: numpy&gt;=1.22.0 in /opt/conda/lib/python3.12/site-packages (from scikit-learn) (2.3.2)
Collecting scipy&gt;=1.8.0 (from scikit-learn)
  Downloading scipy-1.16.1-cp312-cp312-manylinux2014_x86_64.manylinux_2_17_x86_64.whl.metadata (61 kB)
Collecting joblib&gt;=1.2.0 (from scikit-learn)
  Downloading joblib-1.5.1-py3-none-any.whl.metadata (5.6 kB)
Collecting threadpoolctl&gt;=3.1.0 (from scikit-learn)
  Downloading threadpoolctl-3.6.0-py3-none-any.whl.metadata (13 kB)
Downloading scikit_learn-1.7.1-cp312-cp312-manylinux2014_x86_64.manylinux_2_17_x86_64.whl (9.5 MB)
   <span class="ansi-black-intense-fg">━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━</span> <span class="ansi-green-fg">9.5/9.5 MB</span> <span class="ansi-red-fg">100.8 MB/s</span> eta <span class="ansi-cyan-fg">0:00:00</span>
Downloading joblib-1.5.1-py3-none-any.whl (307 kB)
Downloading scipy-1.16.1-cp312-cp312-manylinux2014_x86_64.manylinux_2_17_x86_64.whl (35.2 MB)
   <span class="ansi-black-intense-fg">━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━</span> <span class="ansi-green-fg">35.2/35.2 MB</span> <span class="ansi-red-fg">173.4 MB/s</span> eta <span class="ansi-cyan-fg">0:00:00</span>00:01
Downloading threadpoolctl-3.6.0-py3-none-any.whl (18 kB)
Installing collected packages: threadpoolctl, scipy, joblib, scikit-learn
Successfully installed joblib-1.5.1 scikit-learn-1.7.1 scipy-1.16.1 threadpoolctl-3.6.0
Collecting seaborn
  Downloading seaborn-0.13.2-py3-none-any.whl.metadata (5.4 kB)
Requirement already satisfied: numpy!=1.24.0,&gt;=1.20 in /opt/conda/lib/python3.12/site-packages (from seaborn) (2.3.2)
Requirement already satisfied: pandas&gt;=1.2 in /opt/conda/lib/python3.12/site-packages (from seaborn) (2.3.1)
Requirement already satisfied: matplotlib!=3.6.1,&gt;=3.4 in /opt/conda/lib/python3.12/site-packages (from seaborn) (3.10.5)
Requirement already satisfied: contourpy&gt;=1.0.1 in /opt/conda/lib/python3.12/site-packages (from matplotlib!=3.6.1,&gt;=3.4-&gt;seaborn) (1.3.3)
Requirement already satisfied: cycler&gt;=0.10 in /opt/conda/lib/python3.12/site-packages (from matplotlib!=3.6.1,&gt;=3.4-&gt;seaborn) (0.12.1)
Requirement already satisfied: fonttools&gt;=4.22.0 in /opt/conda/lib/python3.12/site-packages (from matplotlib!=3.6.1,&gt;=3.4-&gt;seaborn) (4.59.1)
Requirement already satisfied: kiwisolver&gt;=1.3.1 in /opt/conda/lib/python3.12/site-packages (from matplotlib!=3.6.1,&gt;=3.4-&gt;seaborn) (1.4.9)
Requirement already satisfied: packaging&gt;=20.0 in /opt/conda/lib/python3.12/site-packages (from matplotlib!=3.6.1,&gt;=3.4-&gt;seaborn) (24.2)
Requirement already satisfied: pillow&gt;=8 in /opt/conda/lib/python3.12/site-packages (from matplotlib!=3.6.1,&gt;=3.4-&gt;seaborn) (11.3.0)
Requirement already satisfied: pyparsing&gt;=2.3.1 in /opt/conda/lib/python3.12/site-packages (from matplotlib!=3.6.1,&gt;=3.4-&gt;seaborn) (3.2.3)
Requirement already satisfied: python-dateutil&gt;=2.7 in /opt/conda/lib/python3.12/site-packages (from matplotlib!=3.6.1,&gt;=3.4-&gt;seaborn) (2.9.0.post0)
Requirement already satisfied: pytz&gt;=2020.1 in /opt/conda/lib/python3.12/site-packages (from pandas&gt;=1.2-&gt;seaborn) (2024.2)
Requirement already satisfied: tzdata&gt;=2022.7 in /opt/conda/lib/python3.12/site-packages (from pandas&gt;=1.2-&gt;seaborn) (2025.2)
Requirement already satisfied: six&gt;=1.5 in /opt/conda/lib/python3.12/site-packages (from python-dateutil&gt;=2.7-&gt;matplotlib!=3.6.1,&gt;=3.4-&gt;seaborn) (1.17.0)
Downloading seaborn-0.13.2-py3-none-any.whl (294 kB)
Installing collected packages: seaborn
Successfully installed seaborn-0.13.2
</pre>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [2]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="kn">import</span><span class="w"> </span><span class="nn">pandas</span><span class="w"> </span><span class="k">as</span><span class="w"> </span><span class="nn">pd</span>
<span class="kn">import</span><span class="w"> </span><span class="nn">matplotlib.pyplot</span><span class="w"> </span><span class="k">as</span><span class="w"> </span><span class="nn">plt</span>
<span class="kn">from</span><span class="w"> </span><span class="nn">sklearn.compose</span><span class="w"> </span><span class="kn">import</span> <span class="n">ColumnTransformer</span>
<span class="kn">from</span><span class="w"> </span><span class="nn">sklearn.pipeline</span><span class="w"> </span><span class="kn">import</span> <span class="n">Pipeline</span>
<span class="kn">from</span><span class="w"> </span><span class="nn">sklearn.preprocessing</span><span class="w"> </span><span class="kn">import</span> <span class="n">StandardScaler</span><span class="p">,</span> <span class="n">OneHotEncoder</span>
<span class="kn">from</span><span class="w"> </span><span class="nn">sklearn.model_selection</span><span class="w"> </span><span class="kn">import</span> <span class="n">train_test_split</span><span class="p">,</span> <span class="n">GridSearchCV</span><span class="p">,</span> <span class="n">StratifiedKFold</span>
<span class="kn">from</span><span class="w"> </span><span class="nn">sklearn.ensemble</span><span class="w"> </span><span class="kn">import</span> <span class="n">RandomForestClassifier</span>
<span class="kn">from</span><span class="w"> </span><span class="nn">sklearn.linear_model</span><span class="w"> </span><span class="kn">import</span> <span class="n">LogisticRegression</span>
<span class="kn">from</span><span class="w"> </span><span class="nn">sklearn.metrics</span><span class="w"> </span><span class="kn">import</span> <span class="n">classification_report</span><span class="p">,</span> <span class="n">confusion_matrix</span><span class="p">,</span> <span class="n">ConfusionMatrixDisplay</span>
<span class="kn">import</span><span class="w"> </span><span class="nn">seaborn</span><span class="w"> </span><span class="k">as</span><span class="w"> </span><span class="nn">sns</span>
</pre></div>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h2 id="Load-the-data">Load the data<a class="anchor-link" href="#Load-the-data">¶</a></h2>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Execute the following cells to load the dataset as a pandas dataframe.</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [3]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">url</span><span class="o">=</span><span class="s2">"https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/_0eYOqji3unP1tDNKWZMjg/weatherAUS-2.csv"</span>
<span class="n">df</span> <span class="o">=</span> <span class="n">pd</span><span class="o">.</span><span class="n">read_csv</span><span class="p">(</span><span class="n">url</span><span class="p">)</span>
<span class="n">df</span><span class="o">.</span><span class="n">head</span><span class="p">()</span>
</pre></div>
</div>
</div>
</div>
</div>
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child jp-OutputArea-executeResult">
<div class="jp-OutputPrompt jp-OutputArea-prompt">Out[3]:</div>
<div class="jp-RenderedHTMLCommon jp-RenderedHTML jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/html" tabindex="0">
<div>
<style scoped="">
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
<thead>
<tr style="text-align: right;">
<th></th>
<th>Date</th>
<th>Location</th>
<th>MinTemp</th>
<th>MaxTemp</th>
<th>Rainfall</th>
<th>Evaporation</th>
<th>Sunshine</th>
<th>WindGustDir</th>
<th>WindGustSpeed</th>
<th>WindDir9am</th>
<th>...</th>
<th>Humidity9am</th>
<th>Humidity3pm</th>
<th>Pressure9am</th>
<th>Pressure3pm</th>
<th>Cloud9am</th>
<th>Cloud3pm</th>
<th>Temp9am</th>
<th>Temp3pm</th>
<th>RainToday</th>
<th>RainTomorrow</th>
</tr>
</thead>
<tbody>
<tr>
<th>0</th>
<td>2008-12-01</td>
<td>Albury</td>
<td>13.4</td>
<td>22.9</td>
<td>0.6</td>
<td>NaN</td>
<td>NaN</td>
<td>W</td>
<td>44.0</td>
<td>W</td>
<td>...</td>
<td>71.0</td>
<td>22.0</td>
<td>1007.7</td>
<td>1007.1</td>
<td>8.0</td>
<td>NaN</td>
<td>16.9</td>
<td>21.8</td>
<td>No</td>
<td>No</td>
</tr>
<tr>
<th>1</th>
<td>2008-12-02</td>
<td>Albury</td>
<td>7.4</td>
<td>25.1</td>
<td>0.0</td>
<td>NaN</td>
<td>NaN</td>
<td>WNW</td>
<td>44.0</td>
<td>NNW</td>
<td>...</td>
<td>44.0</td>
<td>25.0</td>
<td>1010.6</td>
<td>1007.8</td>
<td>NaN</td>
<td>NaN</td>
<td>17.2</td>
<td>24.3</td>
<td>No</td>
<td>No</td>
</tr>
<tr>
<th>2</th>
<td>2008-12-03</td>
<td>Albury</td>
<td>12.9</td>
<td>25.7</td>
<td>0.0</td>
<td>NaN</td>
<td>NaN</td>
<td>WSW</td>
<td>46.0</td>
<td>W</td>
<td>...</td>
<td>38.0</td>
<td>30.0</td>
<td>1007.6</td>
<td>1008.7</td>
<td>NaN</td>
<td>2.0</td>
<td>21.0</td>
<td>23.2</td>
<td>No</td>
<td>No</td>
</tr>
<tr>
<th>3</th>
<td>2008-12-04</td>
<td>Albury</td>
<td>9.2</td>
<td>28.0</td>
<td>0.0</td>
<td>NaN</td>
<td>NaN</td>
<td>NE</td>
<td>24.0</td>
<td>SE</td>
<td>...</td>
<td>45.0</td>
<td>16.0</td>
<td>1017.6</td>
<td>1012.8</td>
<td>NaN</td>
<td>NaN</td>
<td>18.1</td>
<td>26.5</td>
<td>No</td>
<td>No</td>
</tr>
<tr>
<th>4</th>
<td>2008-12-05</td>
<td>Albury</td>
<td>17.5</td>
<td>32.3</td>
<td>1.0</td>
<td>NaN</td>
<td>NaN</td>
<td>W</td>
<td>41.0</td>
<td>ENE</td>
<td>...</td>
<td>82.0</td>
<td>33.0</td>
<td>1010.8</td>
<td>1006.0</td>
<td>7.0</td>
<td>8.0</td>
<td>17.8</td>
<td>29.7</td>
<td>No</td>
<td>No</td>
</tr>
</tbody>
</table>
<p>5 rows × 23 columns</p>
</div>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [4]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">df</span><span class="o">.</span><span class="n">count</span><span class="p">()</span>
</pre></div>
</div>
</div>
</div>
</div>
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child jp-OutputArea-executeResult">
<div class="jp-OutputPrompt jp-OutputArea-prompt">Out[4]:</div>
<div class="jp-RenderedText jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/plain" tabindex="0">
<pre>Date             145460
Location         145460
MinTemp          143975
MaxTemp          144199
Rainfall         142199
Evaporation       82670
Sunshine          75625
WindGustDir      135134
WindGustSpeed    135197
WindDir9am       134894
WindDir3pm       141232
WindSpeed9am     143693
WindSpeed3pm     142398
Humidity9am      142806
Humidity3pm      140953
Pressure9am      130395
Pressure3pm      130432
Cloud9am          89572
Cloud3pm          86102
Temp9am          143693
Temp3pm          141851
RainToday        142199
RainTomorrow     142193
dtype: int64</pre>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Sunshine and cloud cover seem like important features, but they have a lot of missing values, far too many to impute their missing values.</p>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h3 id="Drop-all-rows-with-missing-values">Drop all rows with missing values<a class="anchor-link" href="#Drop-all-rows-with-missing-values">¶</a></h3><p>To try to keep things simple we'll drop rows with missing values and see what's left</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [5]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">df</span> <span class="o">=</span> <span class="n">df</span><span class="o">.</span><span class="n">dropna</span><span class="p">()</span>
<span class="n">df</span><span class="o">.</span><span class="n">info</span><span class="p">()</span>
</pre></div>
</div>
</div>
</div>
</div>
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
<div class="jp-OutputPrompt jp-OutputArea-prompt"></div>
<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="text/plain" tabindex="0">
<pre>&lt;class 'pandas.core.frame.DataFrame'&gt;
Index: 56420 entries, 6049 to 142302
Data columns (total 23 columns):
 #   Column         Non-Null Count  Dtype  
---  ------         --------------  -----  
 0   Date           56420 non-null  object 
 1   Location       56420 non-null  object 
 2   MinTemp        56420 non-null  float64
 3   MaxTemp        56420 non-null  float64
 4   Rainfall       56420 non-null  float64
 5   Evaporation    56420 non-null  float64
 6   Sunshine       56420 non-null  float64
 7   WindGustDir    56420 non-null  object 
 8   WindGustSpeed  56420 non-null  float64
 9   WindDir9am     56420 non-null  object 
 10  WindDir3pm     56420 non-null  object 
 11  WindSpeed9am   56420 non-null  float64
 12  WindSpeed3pm   56420 non-null  float64
 13  Humidity9am    56420 non-null  float64
 14  Humidity3pm    56420 non-null  float64
 15  Pressure9am    56420 non-null  float64
 16  Pressure3pm    56420 non-null  float64
 17  Cloud9am       56420 non-null  float64
 18  Cloud3pm       56420 non-null  float64
 19  Temp9am        56420 non-null  float64
 20  Temp3pm        56420 non-null  float64
 21  RainToday      56420 non-null  object 
 22  RainTomorrow   56420 non-null  object 
dtypes: float64(16), object(7)
memory usage: 10.3+ MB
</pre>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Since we still have 56k observations left after dropping missing values, we may not need to impute any missing values.<br/>
Let's see how we do.</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [6]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">df</span><span class="o">.</span><span class="n">columns</span>
</pre></div>
</div>
</div>
</div>
</div>
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child jp-OutputArea-executeResult">
<div class="jp-OutputPrompt jp-OutputArea-prompt">Out[6]:</div>
<div class="jp-RenderedText jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/plain" tabindex="0">
<pre>Index(['Date', 'Location', 'MinTemp', 'MaxTemp', 'Rainfall', 'Evaporation',
       'Sunshine', 'WindGustDir', 'WindGustSpeed', 'WindDir9am', 'WindDir3pm',
       'WindSpeed9am', 'WindSpeed3pm', 'Humidity9am', 'Humidity3pm',
       'Pressure9am', 'Pressure3pm', 'Cloud9am', 'Cloud3pm', 'Temp9am',
       'Temp3pm', 'RainToday', 'RainTomorrow'],
      dtype='object')</pre>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h2 id="Data-leakage-considerations">Data leakage considerations<a class="anchor-link" href="#Data-leakage-considerations">¶</a></h2><p>Consider the descriptions above for the columns in the data set. Are there any practical limitations to being able to predict whether it will rain tomorrow given the available data?</p>
<h2 id="Points-to-note---1">Points to note - 1<a class="anchor-link" href="#Points-to-note---1">¶</a></h2><p>List some of the features that would be inefficient in predicting tomorrow's rainfall. There will be a question in the quiz that follows based on this observation.</p>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<details><summary>Click here for Hint</summary>
<pre><code>    </code></pre>
<p>Consider features that rely on the entire duration of today for their evaluation.</p>
</details>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>If we adjust our approach and aim to predict today’s rainfall using historical weather data up to and including yesterday, then we can legitimately utilize all of the available features. This shift would be particularly useful for practical applications, such as deciding whether you will bike to work today.</p>
<p>With this new target, we should update the names of the rain columns accordingly to avoid confusion.</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [7]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">df</span> <span class="o">=</span> <span class="n">df</span><span class="o">.</span><span class="n">rename</span><span class="p">(</span><span class="n">columns</span><span class="o">=</span><span class="p">{</span><span class="s1">'RainToday'</span><span class="p">:</span> <span class="s1">'RainYesterday'</span><span class="p">,</span>
                        <span class="s1">'RainTomorrow'</span><span class="p">:</span> <span class="s1">'RainToday'</span>
                        <span class="p">})</span>
</pre></div>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h2 id="Data-Granularity">Data Granularity<a class="anchor-link" href="#Data-Granularity">¶</a></h2>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Would the weather patterns have the same predictability in vastly different locations in Australia? I would think not.<br/>
The chance of rain in one location can be much higher than in another.
Using all of the locations requires a more complex model as it needs to adapt to local weather patterns.<br/>
Let's see how many observations we have for each location, and see if we can reduce our attention to a smaller region.</p>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h2 id="Location-selection">Location selection<a class="anchor-link" href="#Location-selection">¶</a></h2><p>You could do some research to group cities in the <code>Location</code> column by distance, which I've done for you behind the scenes.<br/>
I found that Watsonia is only 15 km from Melbourne, and the Melbourne Airport is only 18 km from Melbourne.<br/>
Let's group these three locations together and use only their weather data to build our localized prediction model.<br/>
Because there might still be some slight variations in the weather patterns we'll keep <code>Location</code> as a categorical variable.</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [8]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">df</span> <span class="o">=</span> <span class="n">df</span><span class="p">[</span><span class="n">df</span><span class="o">.</span><span class="n">Location</span><span class="o">.</span><span class="n">isin</span><span class="p">([</span><span class="s1">'Melbourne'</span><span class="p">,</span><span class="s1">'MelbourneAirport'</span><span class="p">,</span><span class="s1">'Watsonia'</span><span class="p">,])]</span>
<span class="n">df</span><span class="o">.</span> <span class="n">info</span><span class="p">()</span>
</pre></div>
</div>
</div>
</div>
</div>
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
<div class="jp-OutputPrompt jp-OutputArea-prompt"></div>
<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="text/plain" tabindex="0">
<pre>&lt;class 'pandas.core.frame.DataFrame'&gt;
Index: 7557 entries, 64191 to 80997
Data columns (total 23 columns):
 #   Column         Non-Null Count  Dtype  
---  ------         --------------  -----  
 0   Date           7557 non-null   object 
 1   Location       7557 non-null   object 
 2   MinTemp        7557 non-null   float64
 3   MaxTemp        7557 non-null   float64
 4   Rainfall       7557 non-null   float64
 5   Evaporation    7557 non-null   float64
 6   Sunshine       7557 non-null   float64
 7   WindGustDir    7557 non-null   object 
 8   WindGustSpeed  7557 non-null   float64
 9   WindDir9am     7557 non-null   object 
 10  WindDir3pm     7557 non-null   object 
 11  WindSpeed9am   7557 non-null   float64
 12  WindSpeed3pm   7557 non-null   float64
 13  Humidity9am    7557 non-null   float64
 14  Humidity3pm    7557 non-null   float64
 15  Pressure9am    7557 non-null   float64
 16  Pressure3pm    7557 non-null   float64
 17  Cloud9am       7557 non-null   float64
 18  Cloud3pm       7557 non-null   float64
 19  Temp9am        7557 non-null   float64
 20  Temp3pm        7557 non-null   float64
 21  RainYesterday  7557 non-null   object 
 22  RainToday      7557 non-null   object 
dtypes: float64(16), object(7)
memory usage: 1.4+ MB
</pre>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>We still have 7557 records, which should be enough to build a reasonably good model.<br/>
You could always gather more data if needed by partioning the data into similar locations or simplyby updating it from the source to include a larger time frame.</p>
<h2 id="Extracting-a-seasonality-feature">Extracting a seasonality feature<a class="anchor-link" href="#Extracting-a-seasonality-feature">¶</a></h2><p>Now consider the <code>Date</code> column. We expect the weather patterns to be seasonal, having different predictablitiy levels in winter and summer for example.<br/>
There may be some variation with <code>Year</code> as well, but we'll leave that out for now.
Let's engineer a <code>Season</code> feature from <code>Date</code> and drop <code>Date</code> afterward, since it is most likely less informative than season.
An easy way to do this is to define a function that assigns seasons to given months, then use that function to transform the <code>Date</code> column.</p>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h3 id="Create-a-function-to-map-dates-to-seasons">Create a function to map dates to seasons<a class="anchor-link" href="#Create-a-function-to-map-dates-to-seasons">¶</a></h3>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [9]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="k">def</span><span class="w"> </span><span class="nf">date_to_season</span><span class="p">(</span><span class="n">date</span><span class="p">):</span>
    <span class="n">month</span> <span class="o">=</span> <span class="n">date</span><span class="o">.</span><span class="n">month</span>
    <span class="k">if</span> <span class="p">(</span><span class="n">month</span> <span class="o">==</span> <span class="mi">12</span><span class="p">)</span> <span class="ow">or</span> <span class="p">(</span><span class="n">month</span> <span class="o">==</span> <span class="mi">1</span><span class="p">)</span> <span class="ow">or</span> <span class="p">(</span><span class="n">month</span> <span class="o">==</span> <span class="mi">2</span><span class="p">):</span>
        <span class="k">return</span> <span class="s1">'Summer'</span>
    <span class="k">elif</span> <span class="p">(</span><span class="n">month</span> <span class="o">==</span> <span class="mi">3</span><span class="p">)</span> <span class="ow">or</span> <span class="p">(</span><span class="n">month</span> <span class="o">==</span> <span class="mi">4</span><span class="p">)</span> <span class="ow">or</span> <span class="p">(</span><span class="n">month</span> <span class="o">==</span> <span class="mi">5</span><span class="p">):</span>
        <span class="k">return</span> <span class="s1">'Autumn'</span>
    <span class="k">elif</span> <span class="p">(</span><span class="n">month</span> <span class="o">==</span> <span class="mi">6</span><span class="p">)</span> <span class="ow">or</span> <span class="p">(</span><span class="n">month</span> <span class="o">==</span> <span class="mi">7</span><span class="p">)</span> <span class="ow">or</span> <span class="p">(</span><span class="n">month</span> <span class="o">==</span> <span class="mi">8</span><span class="p">):</span>
        <span class="k">return</span> <span class="s1">'Winter'</span>
    <span class="k">elif</span> <span class="p">(</span><span class="n">month</span> <span class="o">==</span> <span class="mi">9</span><span class="p">)</span> <span class="ow">or</span> <span class="p">(</span><span class="n">month</span> <span class="o">==</span> <span class="mi">10</span><span class="p">)</span> <span class="ow">or</span> <span class="p">(</span><span class="n">month</span> <span class="o">==</span> <span class="mi">11</span><span class="p">):</span>
        <span class="k">return</span> <span class="s1">'Spring'</span>
</pre></div>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h2 id="Exercise-1:-Map-the-dates-to-seasons-and-drop-the-Date-column">Exercise 1: Map the dates to seasons and drop the Date column<a class="anchor-link" href="#Exercise-1:-Map-the-dates-to-seasons-and-drop-the-Date-column">¶</a></h2><p>Complete the code:</p>
<div class="highlight"><pre><span></span><span class="c1"># Convert the 'Date' column to datetime format</span>
<span class="n">df</span><span class="p">[</span><span class="s1">'Date'</span><span class="p">]</span> <span class="o">=</span> <span class="n">pd</span><span class="o">.</span><span class="n">to_datetime</span><span class="p">(</span><span class="o">...</span><span class="p">)</span>

<span class="c1"># Apply the function to the 'Date' column</span>
<span class="n">df</span><span class="p">[</span><span class="s1">'Season'</span><span class="p">]</span> <span class="o">=</span> <span class="n">df</span><span class="p">[</span><span class="s1">'Date'</span><span class="p">]</span><span class="o">.</span><span class="n">apply</span><span class="p">(</span><span class="n">date_to_season</span><span class="p">)</span>

<span class="n">df</span><span class="o">=</span><span class="n">df</span><span class="o">.</span><span class="n">drop</span><span class="p">(</span><span class="n">columns</span><span class="o">=...</span><span class="p">)</span>
<span class="n">df</span>
</pre></div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [10]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="c1"># Write your response.</span>
<span class="n">df</span><span class="p">[</span><span class="s1">'Date'</span><span class="p">]</span> <span class="o">=</span> <span class="n">pd</span><span class="o">.</span><span class="n">to_datetime</span><span class="p">(</span><span class="n">df</span><span class="p">[</span><span class="s1">'Date'</span><span class="p">],</span> <span class="nb">format</span><span class="o">=</span><span class="s2">"%Y-%m-</span><span class="si">%d</span><span class="s2">"</span><span class="p">)</span> 
<span class="n">df</span><span class="p">[</span><span class="s1">'Season'</span><span class="p">]</span> <span class="o">=</span> <span class="n">df</span><span class="p">[</span><span class="s1">'Date'</span><span class="p">]</span><span class="o">.</span><span class="n">apply</span><span class="p">(</span><span class="n">date_to_season</span><span class="p">)</span> 
<span class="n">df</span><span class="o">=</span><span class="n">df</span><span class="o">.</span><span class="n">drop</span><span class="p">(</span><span class="n">columns</span><span class="o">=</span><span class="s1">'Date'</span><span class="p">)</span> 
<span class="n">df</span>
</pre></div>
</div>
</div>
</div>
</div>
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child jp-OutputArea-executeResult">
<div class="jp-OutputPrompt jp-OutputArea-prompt">Out[10]:</div>
<div class="jp-RenderedHTMLCommon jp-RenderedHTML jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/html" tabindex="0">
<div>
<style scoped="">
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
<thead>
<tr style="text-align: right;">
<th></th>
<th>Location</th>
<th>MinTemp</th>
<th>MaxTemp</th>
<th>Rainfall</th>
<th>Evaporation</th>
<th>Sunshine</th>
<th>WindGustDir</th>
<th>WindGustSpeed</th>
<th>WindDir9am</th>
<th>WindDir3pm</th>
<th>...</th>
<th>Humidity3pm</th>
<th>Pressure9am</th>
<th>Pressure3pm</th>
<th>Cloud9am</th>
<th>Cloud3pm</th>
<th>Temp9am</th>
<th>Temp3pm</th>
<th>RainYesterday</th>
<th>RainToday</th>
<th>Season</th>
</tr>
</thead>
<tbody>
<tr>
<th>64191</th>
<td>MelbourneAirport</td>
<td>11.2</td>
<td>19.9</td>
<td>0.0</td>
<td>5.6</td>
<td>8.8</td>
<td>SW</td>
<td>69.0</td>
<td>W</td>
<td>SW</td>
<td>...</td>
<td>37.0</td>
<td>1005.1</td>
<td>1006.4</td>
<td>7.0</td>
<td>7.0</td>
<td>15.9</td>
<td>18.1</td>
<td>No</td>
<td>Yes</td>
<td>Summer</td>
</tr>
<tr>
<th>64192</th>
<td>MelbourneAirport</td>
<td>7.8</td>
<td>17.8</td>
<td>1.2</td>
<td>7.2</td>
<td>12.9</td>
<td>SSE</td>
<td>56.0</td>
<td>SW</td>
<td>SSE</td>
<td>...</td>
<td>43.0</td>
<td>1018.0</td>
<td>1019.3</td>
<td>6.0</td>
<td>7.0</td>
<td>12.5</td>
<td>15.8</td>
<td>Yes</td>
<td>No</td>
<td>Summer</td>
</tr>
<tr>
<th>64193</th>
<td>MelbourneAirport</td>
<td>6.3</td>
<td>21.1</td>
<td>0.0</td>
<td>6.2</td>
<td>10.5</td>
<td>SSE</td>
<td>31.0</td>
<td>E</td>
<td>S</td>
<td>...</td>
<td>35.0</td>
<td>1020.8</td>
<td>1017.6</td>
<td>1.0</td>
<td>7.0</td>
<td>13.4</td>
<td>19.6</td>
<td>No</td>
<td>No</td>
<td>Summer</td>
</tr>
<tr>
<th>64194</th>
<td>MelbourneAirport</td>
<td>8.1</td>
<td>29.2</td>
<td>0.0</td>
<td>6.4</td>
<td>12.5</td>
<td>SSE</td>
<td>35.0</td>
<td>NE</td>
<td>SSE</td>
<td>...</td>
<td>23.0</td>
<td>1016.2</td>
<td>1012.8</td>
<td>5.0</td>
<td>4.0</td>
<td>16.0</td>
<td>28.2</td>
<td>No</td>
<td>No</td>
<td>Summer</td>
</tr>
<tr>
<th>64195</th>
<td>MelbourneAirport</td>
<td>9.7</td>
<td>29.0</td>
<td>0.0</td>
<td>7.4</td>
<td>12.3</td>
<td>SE</td>
<td>33.0</td>
<td>SW</td>
<td>SSE</td>
<td>...</td>
<td>31.0</td>
<td>1011.9</td>
<td>1010.3</td>
<td>6.0</td>
<td>2.0</td>
<td>19.4</td>
<td>27.1</td>
<td>No</td>
<td>No</td>
<td>Summer</td>
</tr>
<tr>
<th>...</th>
<td>...</td>
<td>...</td>
<td>...</td>
<td>...</td>
<td>...</td>
<td>...</td>
<td>...</td>
<td>...</td>
<td>...</td>
<td>...</td>
<td>...</td>
<td>...</td>
<td>...</td>
<td>...</td>
<td>...</td>
<td>...</td>
<td>...</td>
<td>...</td>
<td>...</td>
<td>...</td>
<td>...</td>
</tr>
<tr>
<th>80992</th>
<td>Watsonia</td>
<td>3.6</td>
<td>14.5</td>
<td>0.0</td>
<td>2.4</td>
<td>8.8</td>
<td>NNE</td>
<td>41.0</td>
<td>ENE</td>
<td>NNE</td>
<td>...</td>
<td>66.0</td>
<td>1028.4</td>
<td>1025.0</td>
<td>1.0</td>
<td>7.0</td>
<td>5.2</td>
<td>13.8</td>
<td>No</td>
<td>No</td>
<td>Winter</td>
</tr>
<tr>
<th>80994</th>
<td>Watsonia</td>
<td>4.8</td>
<td>13.3</td>
<td>0.4</td>
<td>0.6</td>
<td>0.0</td>
<td>NNW</td>
<td>24.0</td>
<td>NE</td>
<td>NNE</td>
<td>...</td>
<td>63.0</td>
<td>1028.5</td>
<td>1025.1</td>
<td>7.0</td>
<td>7.0</td>
<td>5.6</td>
<td>12.4</td>
<td>No</td>
<td>No</td>
<td>Winter</td>
</tr>
<tr>
<th>80995</th>
<td>Watsonia</td>
<td>5.6</td>
<td>13.1</td>
<td>0.0</td>
<td>1.6</td>
<td>6.0</td>
<td>NNW</td>
<td>52.0</td>
<td>NE</td>
<td>N</td>
<td>...</td>
<td>67.0</td>
<td>1019.0</td>
<td>1014.0</td>
<td>1.0</td>
<td>7.0</td>
<td>8.8</td>
<td>11.6</td>
<td>No</td>
<td>Yes</td>
<td>Winter</td>
</tr>
<tr>
<th>80996</th>
<td>Watsonia</td>
<td>6.9</td>
<td>12.1</td>
<td>3.2</td>
<td>1.8</td>
<td>5.6</td>
<td>SSW</td>
<td>24.0</td>
<td>WNW</td>
<td>SW</td>
<td>...</td>
<td>61.0</td>
<td>1018.7</td>
<td>1017.3</td>
<td>2.0</td>
<td>7.0</td>
<td>7.9</td>
<td>11.0</td>
<td>Yes</td>
<td>No</td>
<td>Winter</td>
</tr>
<tr>
<th>80997</th>
<td>Watsonia</td>
<td>7.9</td>
<td>13.0</td>
<td>0.0</td>
<td>2.8</td>
<td>3.8</td>
<td>NNW</td>
<td>39.0</td>
<td>N</td>
<td>N</td>
<td>...</td>
<td>69.0</td>
<td>1017.6</td>
<td>1015.3</td>
<td>7.0</td>
<td>7.0</td>
<td>9.0</td>
<td>11.7</td>
<td>No</td>
<td>No</td>
<td>Winter</td>
</tr>
</tbody>
</table>
<p>7557 rows × 23 columns</p>
</div>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Looks like we have a good set of features to work with.</p>
<p>Let's go ahead and build our model.</p>
<p>But wait, let's take a look at how well balanced our target is.</p>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h2 id="Exercise-2.-Define-the-feature-and-target-dataframes">Exercise 2. Define the feature and target dataframes<a class="anchor-link" href="#Exercise-2.-Define-the-feature-and-target-dataframes">¶</a></h2><p>Complete the followng code:</p>
<div class="highlight"><pre><span></span><span class="n">X</span> <span class="o">=</span> <span class="n">df</span><span class="o">.</span><span class="n">drop</span><span class="p">(</span><span class="n">columns</span><span class="o">=</span><span class="s1">'...'</span><span class="p">,</span> <span class="n">axis</span><span class="o">=</span><span class="mi">1</span><span class="p">)</span>
<span class="n">y</span> <span class="o">=</span> <span class="n">df</span><span class="p">[</span><span class="s1">'...'</span><span class="p">]</span>
</pre></div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [26]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="c1"># Write your response.</span>
<span class="n">X</span> <span class="o">=</span> <span class="n">df</span><span class="o">.</span><span class="n">drop</span><span class="p">(</span><span class="n">columns</span><span class="o">=</span><span class="s1">'RainYesterday'</span><span class="p">,</span> <span class="n">axis</span><span class="o">=</span><span class="mi">1</span><span class="p">)</span>
<span class="n">y</span> <span class="o">=</span> <span class="n">df</span><span class="p">[</span><span class="s1">'RainToday'</span><span class="p">]</span>  
</pre></div>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h2 id="Exercise-3.-How-balanced-are-the-classes?">Exercise 3. How balanced are the classes?<a class="anchor-link" href="#Exercise-3.-How-balanced-are-the-classes?">¶</a></h2><p>Display the counts of each class.</p>
<p>Complete the following code:</p>
<div class="highlight"><pre><span></span><span class="o">...</span> <span class="o">.</span><span class="n">value_counts</span><span class="p">()</span>
</pre></div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [27]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="c1"># Write your response.</span>
<span class="n">df</span><span class="o">.</span><span class="n">value_counts</span><span class="p">()</span>  
</pre></div>
</div>
</div>
</div>
</div>
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child jp-OutputArea-executeResult">
<div class="jp-OutputPrompt jp-OutputArea-prompt">Out[27]:</div>
<div class="jp-RenderedText jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/plain" tabindex="0">
<pre>Location   MinTemp  MaxTemp  Rainfall  Evaporation  Sunshine  WindGustDir  WindGustSpeed  WindDir9am  WindDir3pm  WindSpeed9am  WindSpeed3pm  Humidity9am  Humidity3pm  Pressure9am  Pressure3pm  Cloud9am  Cloud3pm  Temp9am  Temp3pm  RainYesterday  RainToday  Season
Melbourne  2.3      15.2     0.0       1.0          8.6       NNE          31.0           N           N           15.0          15.0          87.0         43.0         1026.1       1022.1       1.0       3.0       3.9      13.9     No             No         Winter    1
           2.9      18.0     0.0       1.2          10.1      N            46.0           N           NNE         11.0          24.0          75.0         29.0         1023.8       1020.2       1.0       3.0       5.9      17.2     No             No         Autumn    1
           3.0      11.1     0.2       0.4          5.3       N            39.0           NNE         N           11.0          19.0          88.0         55.0         1021.1       1017.4       1.0       7.0       4.8      10.0     No             No         Winter    1
           3.1      12.5     0.0       1.2          2.5       N            54.0           N           N           19.0          30.0          81.0         58.0         1021.7       1017.6       7.0       7.0       6.5      12.0     No             No         Winter    1
                    14.5     0.0       2.6          8.2       N            24.0           N           ENE         17.0          11.0          87.0         62.0         1037.3       1033.1       1.0       3.0       4.2      12.6     No             No         Winter    1
                                                                                                                                                                                                                                                                           ..
Watsonia   24.9     44.7     0.0       20.4         10.3      SSW          57.0           N           NW          24.0          19.0          18.0         12.0         1011.4       1009.2       1.0       4.0       36.4     43.1     No             No         Summer    1
           25.2     27.1     0.0       16.4         9.0       NNE          50.0           N           SW          22.0          19.0          39.0         43.0         1007.0       1009.8       6.0       6.0       27.1     23.8     No             No         Autumn    1
           26.4     33.8     0.0       15.4         3.4       WNW          61.0           NE          N           11.0          22.0          57.0         55.0         1002.9       999.9        7.0       8.0       29.3     31.1     No             Yes        Summer    1
           28.0     42.8     0.0       22.8         8.6       W            50.0           SSW         WSW         19.0          13.0          31.0         16.0         1014.9       1013.1       7.0       6.0       32.3     40.1     No             No         Summer    1
           28.1     34.5     0.0       16.4         10.7      NNE          50.0           N           SW          19.0          19.0          31.0         44.0         1005.7       1006.6       7.0       6.0       29.6     27.8     No             No         Summer    1
Name: count, Length: 7557, dtype: int64</pre>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h2 id="Exercise-4.-What-can-you-conclude-from-these-counts?">Exercise 4. What can you conclude from these counts?<a class="anchor-link" href="#Exercise-4.-What-can-you-conclude-from-these-counts?">¶</a></h2><ul>
<li>How often does it rain annualy in the Melbourne area?</li>
<li>How accurate would you be if you just assumed it won't rain every day?</li>
<li>Is this a balanced dataset?</li>
<li>Next steps?</li>
</ul>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h2 id="Write-your-response-here-and-convert-the-cell-to-a-markdown.">Write your response here and convert the cell to a markdown.<a class="anchor-link" href="#Write-your-response-here-and-convert-the-cell-to-a-markdown.">¶</a></h2>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h2 id="Exercise-5.-Split-data-into-training-and-test-sets,-ensuring-target-stratification">Exercise 5. Split data into training and test sets, ensuring target stratification<a class="anchor-link" href="#Exercise-5.-Split-data-into-training-and-test-sets,-ensuring-target-stratification">¶</a></h2><p>Complete the followng code:</p>
<div class="highlight"><pre><span></span><span class="n">X_train</span><span class="p">,</span> <span class="n">X_test</span><span class="p">,</span> <span class="n">y_train</span><span class="p">,</span> <span class="n">y_test</span> <span class="o">=</span> <span class="n">train_test_split</span><span class="p">(</span><span class="o">...</span><span class="p">,</span> <span class="o">...</span><span class="p">,</span> <span class="n">test_size</span><span class="o">=</span><span class="mf">0.2</span><span class="p">,</span> <span class="n">stratify</span><span class="o">=...</span><span class="p">,</span> <span class="n">random_state</span><span class="o">=</span><span class="mi">42</span><span class="p">)</span>
</pre></div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [28]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="c1"># Write your response.</span>
<span class="n">X_train</span><span class="p">,</span> <span class="n">X_test</span><span class="p">,</span> <span class="n">y_train</span><span class="p">,</span> <span class="n">y_test</span> <span class="o">=</span> <span class="n">train_test_split</span><span class="p">(</span><span class="n">X</span><span class="p">,</span> <span class="n">y</span><span class="p">,</span> <span class="n">test_size</span><span class="o">=</span><span class="mf">0.2</span><span class="p">,</span> <span class="n">stratify</span><span class="o">=</span><span class="n">y</span><span class="p">,</span> <span class="n">random_state</span><span class="o">=</span><span class="mi">42</span><span class="p">)</span> 
</pre></div>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h2 id="Define-preprocessing-transformers-for-numerical-and-categorical-features">Define preprocessing transformers for numerical and categorical features<a class="anchor-link" href="#Define-preprocessing-transformers-for-numerical-and-categorical-features">¶</a></h2><h2 id="Exercise-6.-Automatically-detect-numerical-and-categorical-columns-and-assign-them-to-separate-numeric-and-categorical-features">Exercise 6. Automatically detect numerical and categorical columns and assign them to separate numeric and categorical features<a class="anchor-link" href="#Exercise-6.-Automatically-detect-numerical-and-categorical-columns-and-assign-them-to-separate-numeric-and-categorical-features">¶</a></h2><p>Complete the followng code:</p>
<div class="highlight"><pre><span></span><span class="n">numeric_features</span> <span class="o">=</span> <span class="n">X_train</span><span class="o">.</span><span class="n">select_dtypes</span><span class="p">(</span><span class="n">include</span><span class="o">=</span><span class="p">[</span><span class="s1">'...'</span><span class="p">])</span><span class="o">.</span><span class="n">columns</span><span class="o">.</span><span class="n">tolist</span><span class="p">()</span>  
<span class="n">categorical_features</span> <span class="o">=</span> <span class="n">X_train</span><span class="o">.</span><span class="n">select_dtypes</span><span class="p">(</span><span class="n">include</span><span class="o">=</span><span class="p">[</span><span class="s1">'...'</span><span class="p">,</span> <span class="s1">'category'</span><span class="p">])</span><span class="o">.</span><span class="n">columns</span><span class="o">.</span><span class="n">tolist</span><span class="p">()</span>
</pre></div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [31]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="c1"># Write your response.</span>
<span class="n">numeric_features</span> <span class="o">=</span> <span class="n">X_train</span><span class="o">.</span><span class="n">select_dtypes</span><span class="p">(</span><span class="n">include</span><span class="o">=</span><span class="p">[</span><span class="s1">'float64'</span><span class="p">])</span><span class="o">.</span><span class="n">columns</span><span class="o">.</span><span class="n">tolist</span><span class="p">()</span>  
<span class="n">categorical_features</span> <span class="o">=</span> <span class="n">X_train</span><span class="o">.</span><span class="n">select_dtypes</span><span class="p">(</span><span class="n">include</span><span class="o">=</span><span class="p">[</span><span class="s1">'object'</span><span class="p">,</span> <span class="s1">'category'</span><span class="p">])</span><span class="o">.</span><span class="n">columns</span><span class="o">.</span><span class="n">tolist</span><span class="p">()</span>
</pre></div>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h3 id="Define-separate-transformers-for-both-feature-types-and-combine-them-into-a-single-preprocessing-transformer">Define separate transformers for both feature types and combine them into a single preprocessing transformer<a class="anchor-link" href="#Define-separate-transformers-for-both-feature-types-and-combine-them-into-a-single-preprocessing-transformer">¶</a></h3>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [32]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="c1"># Scale the numeric features</span>
<span class="n">numeric_transformer</span> <span class="o">=</span> <span class="n">Pipeline</span><span class="p">(</span><span class="n">steps</span><span class="o">=</span><span class="p">[(</span><span class="s1">'scaler'</span><span class="p">,</span> <span class="n">StandardScaler</span><span class="p">())])</span>

<span class="c1"># One-hot encode the categoricals </span>
<span class="n">categorical_transformer</span> <span class="o">=</span> <span class="n">Pipeline</span><span class="p">(</span><span class="n">steps</span><span class="o">=</span><span class="p">[(</span><span class="s1">'onehot'</span><span class="p">,</span> <span class="n">OneHotEncoder</span><span class="p">(</span><span class="n">handle_unknown</span><span class="o">=</span><span class="s1">'ignore'</span><span class="p">))])</span>
</pre></div>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h2 id="Exercise-7.-Combine-the-transformers-into-a-single-preprocessing-column-transformer">Exercise 7. Combine the transformers into a single preprocessing column transformer<a class="anchor-link" href="#Exercise-7.-Combine-the-transformers-into-a-single-preprocessing-column-transformer">¶</a></h2><p>Complete the followng code:</p>
<div class="highlight"><pre><span></span><span class="n">preprocessor</span> <span class="o">=</span> <span class="n">ColumnTransformer</span><span class="p">(</span>
    <span class="n">transformers</span><span class="o">=</span><span class="p">[</span>
        <span class="p">(</span><span class="s1">'num'</span><span class="p">,</span> <span class="n">numeric_transformer</span><span class="p">,</span> <span class="o">...</span><span class="p">),</span>
        <span class="p">(</span><span class="s1">'cat'</span><span class="p">,</span> <span class="n">categorical_transformer</span><span class="p">,</span> <span class="o">...</span><span class="p">)</span>
    <span class="p">]</span>
<span class="p">)</span>
</pre></div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [35]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="c1"># Write your response.</span>
<span class="n">preprocessor</span> <span class="o">=</span> <span class="n">ColumnTransformer</span><span class="p">(</span>
    <span class="n">transformers</span><span class="o">=</span><span class="p">[</span>
        <span class="p">(</span><span class="s1">'num'</span><span class="p">,</span> <span class="n">numeric_transformer</span><span class="p">,</span> <span class="n">numeric_features</span><span class="p">),</span>
        <span class="p">(</span><span class="s1">'cat'</span><span class="p">,</span> <span class="n">categorical_transformer</span><span class="p">,</span> <span class="n">categorical_features</span><span class="p">)</span>
    <span class="p">]</span> 
<span class="p">)</span>
</pre></div>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h2 id="Exercise-8.-Create-a-pipeline-by-combining-the-preprocessing-with-a-Random-Forest-classifier">Exercise 8. Create a pipeline by combining the preprocessing with a Random Forest classifier<a class="anchor-link" href="#Exercise-8.-Create-a-pipeline-by-combining-the-preprocessing-with-a-Random-Forest-classifier">¶</a></h2><p>Complete the following code:</p>
<div class="highlight"><pre><span></span><span class="n">pipeline</span> <span class="o">=</span> <span class="n">Pipeline</span><span class="p">(</span><span class="n">steps</span><span class="o">=</span><span class="p">[</span>
    <span class="p">(</span><span class="s1">'preprocessor'</span><span class="p">,</span> <span class="o">...</span><span class="p">),</span>
    <span class="p">(</span><span class="s1">'...'</span><span class="p">,</span> <span class="n">RandomForestClassifier</span><span class="p">(</span><span class="n">random_state</span><span class="o">=</span><span class="mi">42</span><span class="p">))</span>
<span class="p">])</span>
</pre></div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [37]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="c1"># Write your response.</span>
<span class="n">pipeline</span> <span class="o">=</span> <span class="n">Pipeline</span><span class="p">(</span><span class="n">steps</span><span class="o">=</span><span class="p">[</span>
    <span class="p">(</span><span class="s1">'preprocessor'</span><span class="p">,</span> <span class="n">preprocessor</span><span class="p">),</span>
    <span class="p">(</span><span class="s1">'classifier'</span><span class="p">,</span> <span class="n">RandomForestClassifier</span><span class="p">(</span><span class="n">random_state</span><span class="o">=</span><span class="mi">42</span><span class="p">))</span>
<span class="p">])</span> 
</pre></div>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h3 id="Define-a-parameter-grid-to-use-in-a-cross-validation-grid-search-model-optimizer">Define a parameter grid to use in a cross validation grid search model optimizer<a class="anchor-link" href="#Define-a-parameter-grid-to-use-in-a-cross-validation-grid-search-model-optimizer">¶</a></h3>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [38]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">param_grid</span> <span class="o">=</span> <span class="p">{</span>
    <span class="s1">'classifier__n_estimators'</span><span class="p">:</span> <span class="p">[</span><span class="mi">50</span><span class="p">,</span> <span class="mi">100</span><span class="p">],</span>
    <span class="s1">'classifier__max_depth'</span><span class="p">:</span> <span class="p">[</span><span class="kc">None</span><span class="p">,</span> <span class="mi">10</span><span class="p">,</span> <span class="mi">20</span><span class="p">],</span>
    <span class="s1">'classifier__min_samples_split'</span><span class="p">:</span> <span class="p">[</span><span class="mi">2</span><span class="p">,</span> <span class="mi">5</span><span class="p">]</span>
<span class="p">}</span>
</pre></div>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h3 id="Pipeline-usage-in-crossvalidation">Pipeline usage in crossvalidation<a class="anchor-link" href="#Pipeline-usage-in-crossvalidation">¶</a></h3><p>Recall that the pipeline is repeatedly used within the crossvalidation by fitting on each internal training fold and predicting on its corresponding validation fold</p>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h2 id="Perform-grid-search-cross-validation-and-fit-the-best-model-to-the-training-data">Perform grid search cross-validation and fit the best model to the training data<a class="anchor-link" href="#Perform-grid-search-cross-validation-and-fit-the-best-model-to-the-training-data">¶</a></h2><h3 id="Select-a-cross-validation-method,-ensuring-target-stratification-during-validation">Select a cross-validation method, ensuring target stratification during validation<a class="anchor-link" href="#Select-a-cross-validation-method,-ensuring-target-stratification-during-validation">¶</a></h3>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [40]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">cv</span> <span class="o">=</span> <span class="n">StratifiedKFold</span><span class="p">(</span><span class="n">n_splits</span><span class="o">=</span><span class="mi">5</span><span class="p">,</span> <span class="n">shuffle</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
</pre></div>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h2 id="Exercise-9.-Instantiate-and-fit-GridSearchCV-to-the-pipeline">Exercise 9. Instantiate and fit GridSearchCV to the pipeline<a class="anchor-link" href="#Exercise-9.-Instantiate-and-fit-GridSearchCV-to-the-pipeline">¶</a></h2><p>Complete the followng code:</p>
<div class="highlight"><pre><span></span><span class="n">grid_search</span> <span class="o">=</span> <span class="n">GridSearchCV</span><span class="p">(</span><span class="o">...</span><span class="p">,</span> <span class="n">param_grid</span><span class="p">,</span> <span class="n">cv</span><span class="o">=...</span><span class="p">,</span> <span class="n">scoring</span><span class="o">=</span><span class="s1">'accuracy'</span><span class="p">,</span> <span class="n">verbose</span><span class="o">=</span><span class="mi">2</span><span class="p">)</span>  
<span class="n">grid_search</span><span class="o">.</span><span class="n">fit</span><span class="p">(</span><span class="o">...</span><span class="p">,</span> <span class="o">...</span><span class="p">)</span>
</pre></div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [41]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="c1">### Write your response.</span>
<span class="n">grid_search</span> <span class="o">=</span> <span class="n">GridSearchCV</span><span class="p">(</span><span class="n">pipeline</span><span class="p">,</span> <span class="n">param_grid</span><span class="p">,</span> <span class="n">cv</span><span class="o">=</span><span class="mi">5</span><span class="p">,</span> <span class="n">scoring</span><span class="o">=</span><span class="s1">'accuracy'</span><span class="p">,</span> <span class="n">verbose</span><span class="o">=</span><span class="mi">2</span><span class="p">)</span> 
<span class="n">grid_search</span><span class="o">.</span><span class="n">fit</span><span class="p">(</span><span class="n">X_train</span><span class="p">,</span> <span class="n">y_train</span><span class="p">)</span> 
</pre></div>
</div>
</div>
</div>
</div>
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
<div class="jp-OutputPrompt jp-OutputArea-prompt"></div>
<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="text/plain" tabindex="0">
<pre>Fitting 5 folds for each of 12 candidates, totalling 60 fits
[CV] END classifier__max_depth=None, classifier__min_samples_split=2, classifier__n_estimators=50; total time=   0.6s
[CV] END classifier__max_depth=None, classifier__min_samples_split=2, classifier__n_estimators=50; total time=   0.7s
[CV] END classifier__max_depth=None, classifier__min_samples_split=2, classifier__n_estimators=50; total time=   0.3s
[CV] END classifier__max_depth=None, classifier__min_samples_split=2, classifier__n_estimators=50; total time=   0.5s
[CV] END classifier__max_depth=None, classifier__min_samples_split=2, classifier__n_estimators=50; total time=   0.5s
[CV] END classifier__max_depth=None, classifier__min_samples_split=2, classifier__n_estimators=100; total time=   0.6s
[CV] END classifier__max_depth=None, classifier__min_samples_split=2, classifier__n_estimators=100; total time=   0.9s
[CV] END classifier__max_depth=None, classifier__min_samples_split=2, classifier__n_estimators=100; total time=   0.9s
[CV] END classifier__max_depth=None, classifier__min_samples_split=2, classifier__n_estimators=100; total time=   0.8s
[CV] END classifier__max_depth=None, classifier__min_samples_split=2, classifier__n_estimators=100; total time=   1.0s
[CV] END classifier__max_depth=None, classifier__min_samples_split=5, classifier__n_estimators=50; total time=   0.3s
[CV] END classifier__max_depth=None, classifier__min_samples_split=5, classifier__n_estimators=50; total time=   0.4s
[CV] END classifier__max_depth=None, classifier__min_samples_split=5, classifier__n_estimators=50; total time=   0.6s
[CV] END classifier__max_depth=None, classifier__min_samples_split=5, classifier__n_estimators=50; total time=   0.3s
[CV] END classifier__max_depth=None, classifier__min_samples_split=5, classifier__n_estimators=50; total time=   0.2s
[CV] END classifier__max_depth=None, classifier__min_samples_split=5, classifier__n_estimators=100; total time=   0.4s
[CV] END classifier__max_depth=None, classifier__min_samples_split=5, classifier__n_estimators=100; total time=   0.5s
[CV] END classifier__max_depth=None, classifier__min_samples_split=5, classifier__n_estimators=100; total time=   0.3s
[CV] END classifier__max_depth=None, classifier__min_samples_split=5, classifier__n_estimators=100; total time=   0.4s
[CV] END classifier__max_depth=None, classifier__min_samples_split=5, classifier__n_estimators=100; total time=   0.4s
[CV] END classifier__max_depth=10, classifier__min_samples_split=2, classifier__n_estimators=50; total time=   0.2s
[CV] END classifier__max_depth=10, classifier__min_samples_split=2, classifier__n_estimators=50; total time=   0.2s
[CV] END classifier__max_depth=10, classifier__min_samples_split=2, classifier__n_estimators=50; total time=   0.2s
[CV] END classifier__max_depth=10, classifier__min_samples_split=2, classifier__n_estimators=50; total time=   0.2s
[CV] END classifier__max_depth=10, classifier__min_samples_split=2, classifier__n_estimators=50; total time=   0.2s
[CV] END classifier__max_depth=10, classifier__min_samples_split=2, classifier__n_estimators=100; total time=   0.3s
[CV] END classifier__max_depth=10, classifier__min_samples_split=2, classifier__n_estimators=100; total time=   0.4s
[CV] END classifier__max_depth=10, classifier__min_samples_split=2, classifier__n_estimators=100; total time=   0.3s
[CV] END classifier__max_depth=10, classifier__min_samples_split=2, classifier__n_estimators=100; total time=   0.3s
[CV] END classifier__max_depth=10, classifier__min_samples_split=2, classifier__n_estimators=100; total time=   0.3s
[CV] END classifier__max_depth=10, classifier__min_samples_split=5, classifier__n_estimators=50; total time=   0.2s
[CV] END classifier__max_depth=10, classifier__min_samples_split=5, classifier__n_estimators=50; total time=   0.2s
[CV] END classifier__max_depth=10, classifier__min_samples_split=5, classifier__n_estimators=50; total time=   0.2s
[CV] END classifier__max_depth=10, classifier__min_samples_split=5, classifier__n_estimators=50; total time=   0.2s
[CV] END classifier__max_depth=10, classifier__min_samples_split=5, classifier__n_estimators=50; total time=   0.2s
[CV] END classifier__max_depth=10, classifier__min_samples_split=5, classifier__n_estimators=100; total time=   0.3s
[CV] END classifier__max_depth=10, classifier__min_samples_split=5, classifier__n_estimators=100; total time=   0.4s
[CV] END classifier__max_depth=10, classifier__min_samples_split=5, classifier__n_estimators=100; total time=   0.3s
[CV] END classifier__max_depth=10, classifier__min_samples_split=5, classifier__n_estimators=100; total time=   0.3s
[CV] END classifier__max_depth=10, classifier__min_samples_split=5, classifier__n_estimators=100; total time=   0.3s
[CV] END classifier__max_depth=20, classifier__min_samples_split=2, classifier__n_estimators=50; total time=   0.2s
[CV] END classifier__max_depth=20, classifier__min_samples_split=2, classifier__n_estimators=50; total time=   0.2s
[CV] END classifier__max_depth=20, classifier__min_samples_split=2, classifier__n_estimators=50; total time=   0.2s
[CV] END classifier__max_depth=20, classifier__min_samples_split=2, classifier__n_estimators=50; total time=   0.2s
[CV] END classifier__max_depth=20, classifier__min_samples_split=2, classifier__n_estimators=50; total time=   0.2s
[CV] END classifier__max_depth=20, classifier__min_samples_split=2, classifier__n_estimators=100; total time=   0.4s
[CV] END classifier__max_depth=20, classifier__min_samples_split=2, classifier__n_estimators=100; total time=   0.3s
[CV] END classifier__max_depth=20, classifier__min_samples_split=2, classifier__n_estimators=100; total time=   0.3s
[CV] END classifier__max_depth=20, classifier__min_samples_split=2, classifier__n_estimators=100; total time=   0.4s
[CV] END classifier__max_depth=20, classifier__min_samples_split=2, classifier__n_estimators=100; total time=   0.3s
[CV] END classifier__max_depth=20, classifier__min_samples_split=5, classifier__n_estimators=50; total time=   0.2s
[CV] END classifier__max_depth=20, classifier__min_samples_split=5, classifier__n_estimators=50; total time=   0.2s
[CV] END classifier__max_depth=20, classifier__min_samples_split=5, classifier__n_estimators=50; total time=   0.2s
[CV] END classifier__max_depth=20, classifier__min_samples_split=5, classifier__n_estimators=50; total time=   0.2s
[CV] END classifier__max_depth=20, classifier__min_samples_split=5, classifier__n_estimators=50; total time=   0.2s
[CV] END classifier__max_depth=20, classifier__min_samples_split=5, classifier__n_estimators=100; total time=   0.4s
[CV] END classifier__max_depth=20, classifier__min_samples_split=5, classifier__n_estimators=100; total time=   0.3s
[CV] END classifier__max_depth=20, classifier__min_samples_split=5, classifier__n_estimators=100; total time=   0.4s
[CV] END classifier__max_depth=20, classifier__min_samples_split=5, classifier__n_estimators=100; total time=   0.4s
[CV] END classifier__max_depth=20, classifier__min_samples_split=5, classifier__n_estimators=100; total time=   0.3s
</pre>
</div>
</div>
<div class="jp-OutputArea-child jp-OutputArea-executeResult">
<div class="jp-OutputPrompt jp-OutputArea-prompt">Out[41]:</div>
<div class="jp-RenderedHTMLCommon jp-RenderedHTML jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/html" tabindex="0">
<style>#sk-container-id-1 {
  /* Definition of color scheme common for light and dark mode */
  --sklearn-color-text: #000;
  --sklearn-color-text-muted: #666;
  --sklearn-color-line: gray;
  /* Definition of color scheme for unfitted estimators */
  --sklearn-color-unfitted-level-0: #fff5e6;
  --sklearn-color-unfitted-level-1: #f6e4d2;
  --sklearn-color-unfitted-level-2: #ffe0b3;
  --sklearn-color-unfitted-level-3: chocolate;
  /* Definition of color scheme for fitted estimators */
  --sklearn-color-fitted-level-0: #f0f8ff;
  --sklearn-color-fitted-level-1: #d4ebff;
  --sklearn-color-fitted-level-2: #b3dbfd;
  --sklearn-color-fitted-level-3: cornflowerblue;

  /* Specific color for light theme */
  --sklearn-color-text-on-default-background: var(--sg-text-color, var(--theme-code-foreground, var(--jp-content-font-color1, black)));
  --sklearn-color-background: var(--sg-background-color, var(--theme-background, var(--jp-layout-color0, white)));
  --sklearn-color-border-box: var(--sg-text-color, var(--theme-code-foreground, var(--jp-content-font-color1, black)));
  --sklearn-color-icon: #696969;

  @media (prefers-color-scheme: dark) {
    /* Redefinition of color scheme for dark theme */
    --sklearn-color-text-on-default-background: var(--sg-text-color, var(--theme-code-foreground, var(--jp-content-font-color1, white)));
    --sklearn-color-background: var(--sg-background-color, var(--theme-background, var(--jp-layout-color0, #111)));
    --sklearn-color-border-box: var(--sg-text-color, var(--theme-code-foreground, var(--jp-content-font-color1, white)));
    --sklearn-color-icon: #878787;
  }
}

#sk-container-id-1 {
  color: var(--sklearn-color-text);
}

#sk-container-id-1 pre {
  padding: 0;
}

#sk-container-id-1 input.sk-hidden--visually {
  border: 0;
  clip: rect(1px 1px 1px 1px);
  clip: rect(1px, 1px, 1px, 1px);
  height: 1px;
  margin: -1px;
  overflow: hidden;
  padding: 0;
  position: absolute;
  width: 1px;
}

#sk-container-id-1 div.sk-dashed-wrapped {
  border: 1px dashed var(--sklearn-color-line);
  margin: 0 0.4em 0.5em 0.4em;
  box-sizing: border-box;
  padding-bottom: 0.4em;
  background-color: var(--sklearn-color-background);
}

#sk-container-id-1 div.sk-container {
  /* jupyter's `normalize.less` sets `[hidden] { display: none; }`
     but bootstrap.min.css set `[hidden] { display: none !important; }`
     so we also need the `!important` here to be able to override the
     default hidden behavior on the sphinx rendered scikit-learn.org.
     See: https://github.com/scikit-learn/scikit-learn/issues/21755 */
  display: inline-block !important;
  position: relative;
}

#sk-container-id-1 div.sk-text-repr-fallback {
  display: none;
}

div.sk-parallel-item,
div.sk-serial,
div.sk-item {
  /* draw centered vertical line to link estimators */
  background-image: linear-gradient(var(--sklearn-color-text-on-default-background), var(--sklearn-color-text-on-default-background));
  background-size: 2px 100%;
  background-repeat: no-repeat;
  background-position: center center;
}

/* Parallel-specific style estimator block */

#sk-container-id-1 div.sk-parallel-item::after {
  content: "";
  width: 100%;
  border-bottom: 2px solid var(--sklearn-color-text-on-default-background);
  flex-grow: 1;
}

#sk-container-id-1 div.sk-parallel {
  display: flex;
  align-items: stretch;
  justify-content: center;
  background-color: var(--sklearn-color-background);
  position: relative;
}

#sk-container-id-1 div.sk-parallel-item {
  display: flex;
  flex-direction: column;
}

#sk-container-id-1 div.sk-parallel-item:first-child::after {
  align-self: flex-end;
  width: 50%;
}

#sk-container-id-1 div.sk-parallel-item:last-child::after {
  align-self: flex-start;
  width: 50%;
}

#sk-container-id-1 div.sk-parallel-item:only-child::after {
  width: 0;
}

/* Serial-specific style estimator block */

#sk-container-id-1 div.sk-serial {
  display: flex;
  flex-direction: column;
  align-items: center;
  background-color: var(--sklearn-color-background);
  padding-right: 1em;
  padding-left: 1em;
}


/* Toggleable style: style used for estimator/Pipeline/ColumnTransformer box that is
clickable and can be expanded/collapsed.
- Pipeline and ColumnTransformer use this feature and define the default style
- Estimators will overwrite some part of the style using the `sk-estimator` class
*/

/* Pipeline and ColumnTransformer style (default) */

#sk-container-id-1 div.sk-toggleable {
  /* Default theme specific background. It is overwritten whether we have a
  specific estimator or a Pipeline/ColumnTransformer */
  background-color: var(--sklearn-color-background);
}

/* Toggleable label */
#sk-container-id-1 label.sk-toggleable__label {
  cursor: pointer;
  display: flex;
  width: 100%;
  margin-bottom: 0;
  padding: 0.5em;
  box-sizing: border-box;
  text-align: center;
  align-items: start;
  justify-content: space-between;
  gap: 0.5em;
}

#sk-container-id-1 label.sk-toggleable__label .caption {
  font-size: 0.6rem;
  font-weight: lighter;
  color: var(--sklearn-color-text-muted);
}

#sk-container-id-1 label.sk-toggleable__label-arrow:before {
  /* Arrow on the left of the label */
  content: "▸";
  float: left;
  margin-right: 0.25em;
  color: var(--sklearn-color-icon);
}

#sk-container-id-1 label.sk-toggleable__label-arrow:hover:before {
  color: var(--sklearn-color-text);
}

/* Toggleable content - dropdown */

#sk-container-id-1 div.sk-toggleable__content {
  display: none;
  text-align: left;
  /* unfitted */
  background-color: var(--sklearn-color-unfitted-level-0);
}

#sk-container-id-1 div.sk-toggleable__content.fitted {
  /* fitted */
  background-color: var(--sklearn-color-fitted-level-0);
}

#sk-container-id-1 div.sk-toggleable__content pre {
  margin: 0.2em;
  border-radius: 0.25em;
  color: var(--sklearn-color-text);
  /* unfitted */
  background-color: var(--sklearn-color-unfitted-level-0);
}

#sk-container-id-1 div.sk-toggleable__content.fitted pre {
  /* unfitted */
  background-color: var(--sklearn-color-fitted-level-0);
}

#sk-container-id-1 input.sk-toggleable__control:checked~div.sk-toggleable__content {
  /* Expand drop-down */
  display: block;
  width: 100%;
  overflow: visible;
}

#sk-container-id-1 input.sk-toggleable__control:checked~label.sk-toggleable__label-arrow:before {
  content: "▾";
}

/* Pipeline/ColumnTransformer-specific style */

#sk-container-id-1 div.sk-label input.sk-toggleable__control:checked~label.sk-toggleable__label {
  color: var(--sklearn-color-text);
  background-color: var(--sklearn-color-unfitted-level-2);
}

#sk-container-id-1 div.sk-label.fitted input.sk-toggleable__control:checked~label.sk-toggleable__label {
  background-color: var(--sklearn-color-fitted-level-2);
}

/* Estimator-specific style */

/* Colorize estimator box */
#sk-container-id-1 div.sk-estimator input.sk-toggleable__control:checked~label.sk-toggleable__label {
  /* unfitted */
  background-color: var(--sklearn-color-unfitted-level-2);
}

#sk-container-id-1 div.sk-estimator.fitted input.sk-toggleable__control:checked~label.sk-toggleable__label {
  /* fitted */
  background-color: var(--sklearn-color-fitted-level-2);
}

#sk-container-id-1 div.sk-label label.sk-toggleable__label,
#sk-container-id-1 div.sk-label label {
  /* The background is the default theme color */
  color: var(--sklearn-color-text-on-default-background);
}

/* On hover, darken the color of the background */
#sk-container-id-1 div.sk-label:hover label.sk-toggleable__label {
  color: var(--sklearn-color-text);
  background-color: var(--sklearn-color-unfitted-level-2);
}

/* Label box, darken color on hover, fitted */
#sk-container-id-1 div.sk-label.fitted:hover label.sk-toggleable__label.fitted {
  color: var(--sklearn-color-text);
  background-color: var(--sklearn-color-fitted-level-2);
}

/* Estimator label */

#sk-container-id-1 div.sk-label label {
  font-family: monospace;
  font-weight: bold;
  display: inline-block;
  line-height: 1.2em;
}

#sk-container-id-1 div.sk-label-container {
  text-align: center;
}

/* Estimator-specific */
#sk-container-id-1 div.sk-estimator {
  font-family: monospace;
  border: 1px dotted var(--sklearn-color-border-box);
  border-radius: 0.25em;
  box-sizing: border-box;
  margin-bottom: 0.5em;
  /* unfitted */
  background-color: var(--sklearn-color-unfitted-level-0);
}

#sk-container-id-1 div.sk-estimator.fitted {
  /* fitted */
  background-color: var(--sklearn-color-fitted-level-0);
}

/* on hover */
#sk-container-id-1 div.sk-estimator:hover {
  /* unfitted */
  background-color: var(--sklearn-color-unfitted-level-2);
}

#sk-container-id-1 div.sk-estimator.fitted:hover {
  /* fitted */
  background-color: var(--sklearn-color-fitted-level-2);
}

/* Specification for estimator info (e.g. "i" and "?") */

/* Common style for "i" and "?" */

.sk-estimator-doc-link,
a:link.sk-estimator-doc-link,
a:visited.sk-estimator-doc-link {
  float: right;
  font-size: smaller;
  line-height: 1em;
  font-family: monospace;
  background-color: var(--sklearn-color-background);
  border-radius: 1em;
  height: 1em;
  width: 1em;
  text-decoration: none !important;
  margin-left: 0.5em;
  text-align: center;
  /* unfitted */
  border: var(--sklearn-color-unfitted-level-1) 1pt solid;
  color: var(--sklearn-color-unfitted-level-1);
}

.sk-estimator-doc-link.fitted,
a:link.sk-estimator-doc-link.fitted,
a:visited.sk-estimator-doc-link.fitted {
  /* fitted */
  border: var(--sklearn-color-fitted-level-1) 1pt solid;
  color: var(--sklearn-color-fitted-level-1);
}

/* On hover */
div.sk-estimator:hover .sk-estimator-doc-link:hover,
.sk-estimator-doc-link:hover,
div.sk-label-container:hover .sk-estimator-doc-link:hover,
.sk-estimator-doc-link:hover {
  /* unfitted */
  background-color: var(--sklearn-color-unfitted-level-3);
  color: var(--sklearn-color-background);
  text-decoration: none;
}

div.sk-estimator.fitted:hover .sk-estimator-doc-link.fitted:hover,
.sk-estimator-doc-link.fitted:hover,
div.sk-label-container:hover .sk-estimator-doc-link.fitted:hover,
.sk-estimator-doc-link.fitted:hover {
  /* fitted */
  background-color: var(--sklearn-color-fitted-level-3);
  color: var(--sklearn-color-background);
  text-decoration: none;
}

/* Span, style for the box shown on hovering the info icon */
.sk-estimator-doc-link span {
  display: none;
  z-index: 9999;
  position: relative;
  font-weight: normal;
  right: .2ex;
  padding: .5ex;
  margin: .5ex;
  width: min-content;
  min-width: 20ex;
  max-width: 50ex;
  color: var(--sklearn-color-text);
  box-shadow: 2pt 2pt 4pt #999;
  /* unfitted */
  background: var(--sklearn-color-unfitted-level-0);
  border: .5pt solid var(--sklearn-color-unfitted-level-3);
}

.sk-estimator-doc-link.fitted span {
  /* fitted */
  background: var(--sklearn-color-fitted-level-0);
  border: var(--sklearn-color-fitted-level-3);
}

.sk-estimator-doc-link:hover span {
  display: block;
}

/* "?"-specific style due to the `<a>` HTML tag */

#sk-container-id-1 a.estimator_doc_link {
  float: right;
  font-size: 1rem;
  line-height: 1em;
  font-family: monospace;
  background-color: var(--sklearn-color-background);
  border-radius: 1rem;
  height: 1rem;
  width: 1rem;
  text-decoration: none;
  /* unfitted */
  color: var(--sklearn-color-unfitted-level-1);
  border: var(--sklearn-color-unfitted-level-1) 1pt solid;
}

#sk-container-id-1 a.estimator_doc_link.fitted {
  /* fitted */
  border: var(--sklearn-color-fitted-level-1) 1pt solid;
  color: var(--sklearn-color-fitted-level-1);
}

/* On hover */
#sk-container-id-1 a.estimator_doc_link:hover {
  /* unfitted */
  background-color: var(--sklearn-color-unfitted-level-3);
  color: var(--sklearn-color-background);
  text-decoration: none;
}

#sk-container-id-1 a.estimator_doc_link.fitted:hover {
  /* fitted */
  background-color: var(--sklearn-color-fitted-level-3);
}

.estimator-table summary {
    padding: .5rem;
    font-family: monospace;
    cursor: pointer;
}

.estimator-table details[open] {
    padding-left: 0.1rem;
    padding-right: 0.1rem;
    padding-bottom: 0.3rem;
}

.estimator-table .parameters-table {
    margin-left: auto !important;
    margin-right: auto !important;
}

.estimator-table .parameters-table tr:nth-child(odd) {
    background-color: #fff;
}

.estimator-table .parameters-table tr:nth-child(even) {
    background-color: #f6f6f6;
}

.estimator-table .parameters-table tr:hover {
    background-color: #e0e0e0;
}

.estimator-table table td {
    border: 1px solid rgba(106, 105, 104, 0.232);
}

.user-set td {
    color:rgb(255, 94, 0);
    text-align: left;
}

.user-set td.value pre {
    color:rgb(255, 94, 0) !important;
    background-color: transparent !important;
}

.default td {
    color: black;
    text-align: left;
}

.user-set td i,
.default td i {
    color: black;
}

.copy-paste-icon {
    background-image: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCA0NDggNTEyIj48IS0tIUZvbnQgQXdlc29tZSBGcmVlIDYuNy4yIGJ5IEBmb250YXdlc29tZSAtIGh0dHBzOi8vZm9udGF3ZXNvbWUuY29tIExpY2Vuc2UgLSBodHRwczovL2ZvbnRhd2Vzb21lLmNvbS9saWNlbnNlL2ZyZWUgQ29weXJpZ2h0IDIwMjUgRm9udGljb25zLCBJbmMuLS0+PHBhdGggZD0iTTIwOCAwTDMzMi4xIDBjMTIuNyAwIDI0LjkgNS4xIDMzLjkgMTQuMWw2Ny45IDY3LjljOSA5IDE0LjEgMjEuMiAxNC4xIDMzLjlMNDQ4IDMzNmMwIDI2LjUtMjEuNSA0OC00OCA0OGwtMTkyIDBjLTI2LjUgMC00OC0yMS41LTQ4LTQ4bDAtMjg4YzAtMjYuNSAyMS41LTQ4IDQ4LTQ4ek00OCAxMjhsODAgMCAwIDY0LTY0IDAgMCAyNTYgMTkyIDAgMC0zMiA2NCAwIDAgNDhjMCAyNi41LTIxLjUgNDgtNDggNDhMNDggNTEyYy0yNi41IDAtNDgtMjEuNS00OC00OEwwIDE3NmMwLTI2LjUgMjEuNS00OCA0OC00OHoiLz48L3N2Zz4=);
    background-repeat: no-repeat;
    background-size: 14px 14px;
    background-position: 0;
    display: inline-block;
    width: 14px;
    height: 14px;
    cursor: pointer;
}
</style><body><div class="sk-top-container" id="sk-container-id-1"><div class="sk-text-repr-fallback"><pre>GridSearchCV(cv=5,
             estimator=Pipeline(steps=[('preprocessor',
                                        ColumnTransformer(transformers=[('num',
                                                                         Pipeline(steps=[('scaler',
                                                                                          StandardScaler())]),
                                                                         ['MinTemp',
                                                                          'MaxTemp',
                                                                          'Rainfall',
                                                                          'Evaporation',
                                                                          'Sunshine',
                                                                          'WindGustSpeed',
                                                                          'WindSpeed9am',
                                                                          'WindSpeed3pm',
                                                                          'Humidity9am',
                                                                          'Humidity3pm',
                                                                          'Pressure9am',
                                                                          'Pressure3pm',
                                                                          'Cloud9am',
                                                                          'Cloud3pm',
                                                                          'Temp9am',
                                                                          'Temp3pm']),
                                                                        ('...
                                                                         Pipeline(steps=[('onehot',
                                                                                          OneHotEncoder(handle_unknown='ignore'))]),
                                                                         ['Location',
                                                                          'WindGustDir',
                                                                          'WindDir9am',
                                                                          'WindDir3pm',
                                                                          'RainToday',
                                                                          'Season'])])),
                                       ('classifier',
                                        RandomForestClassifier(random_state=42))]),
             param_grid={'classifier__max_depth': [None, 10, 20],
                         'classifier__min_samples_split': [2, 5],
                         'classifier__n_estimators': [50, 100]},
             scoring='accuracy', verbose=2)</pre><b>In a Jupyter environment, please rerun this cell to show the HTML representation or trust the notebook. <br/>On GitHub, the HTML representation is unable to render, please try loading this page with nbviewer.org.</b></div><div class="sk-container" hidden=""><div class="sk-item sk-dashed-wrapped"><div class="sk-label-container"><div class="sk-label fitted sk-toggleable"><input class="sk-toggleable__control sk-hidden--visually" id="sk-estimator-id-1" type="checkbox"/><label class="sk-toggleable__label fitted sk-toggleable__label-arrow" for="sk-estimator-id-1"><div><div>GridSearchCV</div></div><div><a class="sk-estimator-doc-link fitted" href="https://scikit-learn.org/1.7/modules/generated/sklearn.model_selection.GridSearchCV.html" rel="noreferrer" target="_blank">?<span>Documentation for GridSearchCV</span></a><span class="sk-estimator-doc-link fitted">i<span>Fitted</span></span></div></label><div class="sk-toggleable__content fitted" data-param-prefix="">
<div class="estimator-table">
<details>
<summary>Parameters</summary>
<table class="parameters-table">
<tbody>
<tr class="user-set">
<td><i class="copy-paste-icon" onclick="copyToClipboard('estimator',
                          this.parentElement.nextElementSibling)"></i></td>
<td class="param">estimator </td>
<td class="value">Pipeline(step...m_state=42))])</td>
</tr>
<tr class="user-set">
<td><i class="copy-paste-icon" onclick="copyToClipboard('param_grid',
                          this.parentElement.nextElementSibling)"></i></td>
<td class="param">param_grid </td>
<td class="value">{'classifier__max_depth': [None, 10, ...], 'classifier__min_samples_split': [2, 5], 'classifier__n_estimators': [50, 100]}</td>
</tr>
<tr class="user-set">
<td><i class="copy-paste-icon" onclick="copyToClipboard('scoring',
                          this.parentElement.nextElementSibling)"></i></td>
<td class="param">scoring </td>
<td class="value">'accuracy'</td>
</tr>
<tr class="default">
<td><i class="copy-paste-icon" onclick="copyToClipboard('n_jobs',
                          this.parentElement.nextElementSibling)"></i></td>
<td class="param">n_jobs </td>
<td class="value">None</td>
</tr>
<tr class="default">
<td><i class="copy-paste-icon" onclick="copyToClipboard('refit',
                          this.parentElement.nextElementSibling)"></i></td>
<td class="param">refit </td>
<td class="value">True</td>
</tr>
<tr class="user-set">
<td><i class="copy-paste-icon" onclick="copyToClipboard('cv',
                          this.parentElement.nextElementSibling)"></i></td>
<td class="param">cv </td>
<td class="value">5</td>
</tr>
<tr class="user-set">
<td><i class="copy-paste-icon" onclick="copyToClipboard('verbose',
                          this.parentElement.nextElementSibling)"></i></td>
<td class="param">verbose </td>
<td class="value">2</td>
</tr>
<tr class="default">
<td><i class="copy-paste-icon" onclick="copyToClipboard('pre_dispatch',
                          this.parentElement.nextElementSibling)"></i></td>
<td class="param">pre_dispatch </td>
<td class="value">'2*n_jobs'</td>
</tr>
<tr class="default">
<td><i class="copy-paste-icon" onclick="copyToClipboard('error_score',
                          this.parentElement.nextElementSibling)"></i></td>
<td class="param">error_score </td>
<td class="value">nan</td>
</tr>
<tr class="default">
<td><i class="copy-paste-icon" onclick="copyToClipboard('return_train_score',
                          this.parentElement.nextElementSibling)"></i></td>
<td class="param">return_train_score </td>
<td class="value">False</td>
</tr>
</tbody>
</table>
</details>
</div>
</div></div></div><div class="sk-parallel"><div class="sk-parallel-item"><div class="sk-item"><div class="sk-label-container"><div class="sk-label fitted sk-toggleable"><input class="sk-toggleable__control sk-hidden--visually" id="sk-estimator-id-2" type="checkbox"/><label class="sk-toggleable__label fitted sk-toggleable__label-arrow" for="sk-estimator-id-2"><div><div>best_estimator_: Pipeline</div></div></label><div class="sk-toggleable__content fitted" data-param-prefix="best_estimator___"></div></div><div class="sk-serial"><div class="sk-item"><div class="sk-serial"><div class="sk-item sk-dashed-wrapped"><div class="sk-label-container"><div class="sk-label fitted sk-toggleable"><input class="sk-toggleable__control sk-hidden--visually" id="sk-estimator-id-3" type="checkbox"/><label class="sk-toggleable__label fitted sk-toggleable__label-arrow" for="sk-estimator-id-3"><div><div>preprocessor: ColumnTransformer</div></div><div><a class="sk-estimator-doc-link fitted" href="https://scikit-learn.org/1.7/modules/generated/sklearn.compose.ColumnTransformer.html" rel="noreferrer" target="_blank">?<span>Documentation for preprocessor: ColumnTransformer</span></a></div></label><div class="sk-toggleable__content fitted" data-param-prefix="best_estimator___preprocessor__">
<div class="estimator-table">
<details>
<summary>Parameters</summary>
<table class="parameters-table">
<tbody>
<tr class="user-set">
<td><i class="copy-paste-icon" onclick="copyToClipboard('transformers',
                          this.parentElement.nextElementSibling)"></i></td>
<td class="param">transformers </td>
<td class="value">[('num', ...), ('cat', ...)]</td>
</tr>
<tr class="default">
<td><i class="copy-paste-icon" onclick="copyToClipboard('remainder',
                          this.parentElement.nextElementSibling)"></i></td>
<td class="param">remainder </td>
<td class="value">'drop'</td>
</tr>
<tr class="default">
<td><i class="copy-paste-icon" onclick="copyToClipboard('sparse_threshold',
                          this.parentElement.nextElementSibling)"></i></td>
<td class="param">sparse_threshold </td>
<td class="value">0.3</td>
</tr>
<tr class="default">
<td><i class="copy-paste-icon" onclick="copyToClipboard('n_jobs',
                          this.parentElement.nextElementSibling)"></i></td>
<td class="param">n_jobs </td>
<td class="value">None</td>
</tr>
<tr class="default">
<td><i class="copy-paste-icon" onclick="copyToClipboard('transformer_weights',
                          this.parentElement.nextElementSibling)"></i></td>
<td class="param">transformer_weights </td>
<td class="value">None</td>
</tr>
<tr class="default">
<td><i class="copy-paste-icon" onclick="copyToClipboard('verbose',
                          this.parentElement.nextElementSibling)"></i></td>
<td class="param">verbose </td>
<td class="value">False</td>
</tr>
<tr class="default">
<td><i class="copy-paste-icon" onclick="copyToClipboard('verbose_feature_names_out',
                          this.parentElement.nextElementSibling)"></i></td>
<td class="param">verbose_feature_names_out </td>
<td class="value">True</td>
</tr>
<tr class="default">
<td><i class="copy-paste-icon" onclick="copyToClipboard('force_int_remainder_cols',
                          this.parentElement.nextElementSibling)"></i></td>
<td class="param">force_int_remainder_cols </td>
<td class="value">'deprecated'</td>
</tr>
</tbody>
</table>
</details>
</div>
</div></div></div><div class="sk-parallel"><div class="sk-parallel-item"><div class="sk-item"><div class="sk-label-container"><div class="sk-label fitted sk-toggleable"><input class="sk-toggleable__control sk-hidden--visually" id="sk-estimator-id-4" type="checkbox"/><label class="sk-toggleable__label fitted sk-toggleable__label-arrow" for="sk-estimator-id-4"><div><div>num</div></div></label><div class="sk-toggleable__content fitted" data-param-prefix="best_estimator___preprocessor__num__"><pre>['MinTemp', 'MaxTemp', 'Rainfall', 'Evaporation', 'Sunshine', 'WindGustSpeed', 'WindSpeed9am', 'WindSpeed3pm', 'Humidity9am', 'Humidity3pm', 'Pressure9am', 'Pressure3pm', 'Cloud9am', 'Cloud3pm', 'Temp9am', 'Temp3pm']</pre></div></div></div><div class="sk-serial"><div class="sk-item"><div class="sk-serial"><div class="sk-item"><div class="sk-estimator fitted sk-toggleable"><input class="sk-toggleable__control sk-hidden--visually" id="sk-estimator-id-5" type="checkbox"/><label class="sk-toggleable__label fitted sk-toggleable__label-arrow" for="sk-estimator-id-5"><div><div>StandardScaler</div></div><div><a class="sk-estimator-doc-link fitted" href="https://scikit-learn.org/1.7/modules/generated/sklearn.preprocessing.StandardScaler.html" rel="noreferrer" target="_blank">?<span>Documentation for StandardScaler</span></a></div></label><div class="sk-toggleable__content fitted" data-param-prefix="best_estimator___preprocessor__num__scaler__">
<div class="estimator-table">
<details>
<summary>Parameters</summary>
<table class="parameters-table">
<tbody>
<tr class="default">
<td><i class="copy-paste-icon" onclick="copyToClipboard('copy',
                          this.parentElement.nextElementSibling)"></i></td>
<td class="param">copy </td>
<td class="value">True</td>
</tr>
<tr class="default">
<td><i class="copy-paste-icon" onclick="copyToClipboard('with_mean',
                          this.parentElement.nextElementSibling)"></i></td>
<td class="param">with_mean </td>
<td class="value">True</td>
</tr>
<tr class="default">
<td><i class="copy-paste-icon" onclick="copyToClipboard('with_std',
                          this.parentElement.nextElementSibling)"></i></td>
<td class="param">with_std </td>
<td class="value">True</td>
</tr>
</tbody>
</table>
</details>
</div>
</div></div></div></div></div></div></div></div><div class="sk-parallel-item"><div class="sk-item"><div class="sk-label-container"><div class="sk-label fitted sk-toggleable"><input class="sk-toggleable__control sk-hidden--visually" id="sk-estimator-id-6" type="checkbox"/><label class="sk-toggleable__label fitted sk-toggleable__label-arrow" for="sk-estimator-id-6"><div><div>cat</div></div></label><div class="sk-toggleable__content fitted" data-param-prefix="best_estimator___preprocessor__cat__"><pre>['Location', 'WindGustDir', 'WindDir9am', 'WindDir3pm', 'RainToday', 'Season']</pre></div></div></div><div class="sk-serial"><div class="sk-item"><div class="sk-serial"><div class="sk-item"><div class="sk-estimator fitted sk-toggleable"><input class="sk-toggleable__control sk-hidden--visually" id="sk-estimator-id-7" type="checkbox"/><label class="sk-toggleable__label fitted sk-toggleable__label-arrow" for="sk-estimator-id-7"><div><div>OneHotEncoder</div></div><div><a class="sk-estimator-doc-link fitted" href="https://scikit-learn.org/1.7/modules/generated/sklearn.preprocessing.OneHotEncoder.html" rel="noreferrer" target="_blank">?<span>Documentation for OneHotEncoder</span></a></div></label><div class="sk-toggleable__content fitted" data-param-prefix="best_estimator___preprocessor__cat__onehot__">
<div class="estimator-table">
<details>
<summary>Parameters</summary>
<table class="parameters-table">
<tbody>
<tr class="default">
<td><i class="copy-paste-icon" onclick="copyToClipboard('categories',
                          this.parentElement.nextElementSibling)"></i></td>
<td class="param">categories </td>
<td class="value">'auto'</td>
</tr>
<tr class="default">
<td><i class="copy-paste-icon" onclick="copyToClipboard('drop',
                          this.parentElement.nextElementSibling)"></i></td>
<td class="param">drop </td>
<td class="value">None</td>
</tr>
<tr class="default">
<td><i class="copy-paste-icon" onclick="copyToClipboard('sparse_output',
                          this.parentElement.nextElementSibling)"></i></td>
<td class="param">sparse_output </td>
<td class="value">True</td>
</tr>
<tr class="default">
<td><i class="copy-paste-icon" onclick="copyToClipboard('dtype',
                          this.parentElement.nextElementSibling)"></i></td>
<td class="param">dtype </td>
<td class="value">&lt;class 'numpy.float64'&gt;</td>
</tr>
<tr class="user-set">
<td><i class="copy-paste-icon" onclick="copyToClipboard('handle_unknown',
                          this.parentElement.nextElementSibling)"></i></td>
<td class="param">handle_unknown </td>
<td class="value">'ignore'</td>
</tr>
<tr class="default">
<td><i class="copy-paste-icon" onclick="copyToClipboard('min_frequency',
                          this.parentElement.nextElementSibling)"></i></td>
<td class="param">min_frequency </td>
<td class="value">None</td>
</tr>
<tr class="default">
<td><i class="copy-paste-icon" onclick="copyToClipboard('max_categories',
                          this.parentElement.nextElementSibling)"></i></td>
<td class="param">max_categories </td>
<td class="value">None</td>
</tr>
<tr class="default">
<td><i class="copy-paste-icon" onclick="copyToClipboard('feature_name_combiner',
                          this.parentElement.nextElementSibling)"></i></td>
<td class="param">feature_name_combiner </td>
<td class="value">'concat'</td>
</tr>
</tbody>
</table>
</details>
</div>
</div></div></div></div></div></div></div></div></div></div><div class="sk-item"><div class="sk-estimator fitted sk-toggleable"><input class="sk-toggleable__control sk-hidden--visually" id="sk-estimator-id-8" type="checkbox"/><label class="sk-toggleable__label fitted sk-toggleable__label-arrow" for="sk-estimator-id-8"><div><div>RandomForestClassifier</div></div><div><a class="sk-estimator-doc-link fitted" href="https://scikit-learn.org/1.7/modules/generated/sklearn.ensemble.RandomForestClassifier.html" rel="noreferrer" target="_blank">?<span>Documentation for RandomForestClassifier</span></a></div></label><div class="sk-toggleable__content fitted" data-param-prefix="best_estimator___classifier__">
<div class="estimator-table">
<details>
<summary>Parameters</summary>
<table class="parameters-table">
<tbody>
<tr class="user-set">
<td><i class="copy-paste-icon" onclick="copyToClipboard('n_estimators',
                          this.parentElement.nextElementSibling)"></i></td>
<td class="param">n_estimators </td>
<td class="value">50</td>
</tr>
<tr class="default">
<td><i class="copy-paste-icon" onclick="copyToClipboard('criterion',
                          this.parentElement.nextElementSibling)"></i></td>
<td class="param">criterion </td>
<td class="value">'gini'</td>
</tr>
<tr class="default">
<td><i class="copy-paste-icon" onclick="copyToClipboard('max_depth',
                          this.parentElement.nextElementSibling)"></i></td>
<td class="param">max_depth </td>
<td class="value">None</td>
</tr>
<tr class="default">
<td><i class="copy-paste-icon" onclick="copyToClipboard('min_samples_split',
                          this.parentElement.nextElementSibling)"></i></td>
<td class="param">min_samples_split </td>
<td class="value">2</td>
</tr>
<tr class="default">
<td><i class="copy-paste-icon" onclick="copyToClipboard('min_samples_leaf',
                          this.parentElement.nextElementSibling)"></i></td>
<td class="param">min_samples_leaf </td>
<td class="value">1</td>
</tr>
<tr class="default">
<td><i class="copy-paste-icon" onclick="copyToClipboard('min_weight_fraction_leaf',
                          this.parentElement.nextElementSibling)"></i></td>
<td class="param">min_weight_fraction_leaf </td>
<td class="value">0.0</td>
</tr>
<tr class="default">
<td><i class="copy-paste-icon" onclick="copyToClipboard('max_features',
                          this.parentElement.nextElementSibling)"></i></td>
<td class="param">max_features </td>
<td class="value">'sqrt'</td>
</tr>
<tr class="default">
<td><i class="copy-paste-icon" onclick="copyToClipboard('max_leaf_nodes',
                          this.parentElement.nextElementSibling)"></i></td>
<td class="param">max_leaf_nodes </td>
<td class="value">None</td>
</tr>
<tr class="default">
<td><i class="copy-paste-icon" onclick="copyToClipboard('min_impurity_decrease',
                          this.parentElement.nextElementSibling)"></i></td>
<td class="param">min_impurity_decrease </td>
<td class="value">0.0</td>
</tr>
<tr class="default">
<td><i class="copy-paste-icon" onclick="copyToClipboard('bootstrap',
                          this.parentElement.nextElementSibling)"></i></td>
<td class="param">bootstrap </td>
<td class="value">True</td>
</tr>
<tr class="default">
<td><i class="copy-paste-icon" onclick="copyToClipboard('oob_score',
                          this.parentElement.nextElementSibling)"></i></td>
<td class="param">oob_score </td>
<td class="value">False</td>
</tr>
<tr class="default">
<td><i class="copy-paste-icon" onclick="copyToClipboard('n_jobs',
                          this.parentElement.nextElementSibling)"></i></td>
<td class="param">n_jobs </td>
<td class="value">None</td>
</tr>
<tr class="user-set">
<td><i class="copy-paste-icon" onclick="copyToClipboard('random_state',
                          this.parentElement.nextElementSibling)"></i></td>
<td class="param">random_state </td>
<td class="value">42</td>
</tr>
<tr class="default">
<td><i class="copy-paste-icon" onclick="copyToClipboard('verbose',
                          this.parentElement.nextElementSibling)"></i></td>
<td class="param">verbose </td>
<td class="value">0</td>
</tr>
<tr class="default">
<td><i class="copy-paste-icon" onclick="copyToClipboard('warm_start',
                          this.parentElement.nextElementSibling)"></i></td>
<td class="param">warm_start </td>
<td class="value">False</td>
</tr>
<tr class="default">
<td><i class="copy-paste-icon" onclick="copyToClipboard('class_weight',
                          this.parentElement.nextElementSibling)"></i></td>
<td class="param">class_weight </td>
<td class="value">None</td>
</tr>
<tr class="default">
<td><i class="copy-paste-icon" onclick="copyToClipboard('ccp_alpha',
                          this.parentElement.nextElementSibling)"></i></td>
<td class="param">ccp_alpha </td>
<td class="value">0.0</td>
</tr>
<tr class="default">
<td><i class="copy-paste-icon" onclick="copyToClipboard('max_samples',
                          this.parentElement.nextElementSibling)"></i></td>
<td class="param">max_samples </td>
<td class="value">None</td>
</tr>
<tr class="default">
<td><i class="copy-paste-icon" onclick="copyToClipboard('monotonic_cst',
                          this.parentElement.nextElementSibling)"></i></td>
<td class="param">monotonic_cst </td>
<td class="value">None</td>
</tr>
</tbody>
</table>
</details>
</div>
</div></div></div></div></div></div></div></div></div></div></div></div><script>function copyToClipboard(text, element) {
    // Get the parameter prefix from the closest toggleable content
    const toggleableContent = element.closest('.sk-toggleable__content');
    const paramPrefix = toggleableContent ? toggleableContent.dataset.paramPrefix : '';
    const fullParamName = paramPrefix ? `${paramPrefix}${text}` : text;

    const originalStyle = element.style;
    const computedStyle = window.getComputedStyle(element);
    const originalWidth = computedStyle.width;
    const originalHTML = element.innerHTML.replace('Copied!', '');

    navigator.clipboard.writeText(fullParamName)
        .then(() => {
            element.style.width = originalWidth;
            element.style.color = 'green';
            element.innerHTML = "Copied!";

            setTimeout(() => {
                element.innerHTML = originalHTML;
                element.style = originalStyle;
            }, 2000);
        })
        .catch(err => {
            console.error('Failed to copy:', err);
            element.style.color = 'red';
            element.innerHTML = "Failed!";
            setTimeout(() => {
                element.innerHTML = originalHTML;
                element.style = originalStyle;
            }, 2000);
        });
    return false;
}

document.querySelectorAll('.fa-regular.fa-copy').forEach(function(element) {
    const toggleableContent = element.closest('.sk-toggleable__content');
    const paramPrefix = toggleableContent ? toggleableContent.dataset.paramPrefix : '';
    const paramName = element.parentElement.nextElementSibling.textContent.trim();
    const fullParamName = paramPrefix ? `${paramPrefix}${paramName}` : paramName;

    element.setAttribute('title', fullParamName);
});
</script></div></body>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h3 id="Print-the-best-parameters-and-best-crossvalidation-score">Print the best parameters and best crossvalidation score<a class="anchor-link" href="#Print-the-best-parameters-and-best-crossvalidation-score">¶</a></h3>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [42]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="nb">print</span><span class="p">(</span><span class="s2">"</span><span class="se">\n</span><span class="s2">Best parameters found: "</span><span class="p">,</span> <span class="n">grid_search</span><span class="o">.</span><span class="n">best_params_</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">"Best cross-validation score: </span><span class="si">{:.2f}</span><span class="s2">"</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">grid_search</span><span class="o">.</span><span class="n">best_score_</span><span class="p">))</span>
</pre></div>
</div>
</div>
</div>
</div>
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
<div class="jp-OutputPrompt jp-OutputArea-prompt"></div>
<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="text/plain" tabindex="0">
<pre>
Best parameters found:  {'classifier__max_depth': None, 'classifier__min_samples_split': 2, 'classifier__n_estimators': 50}
Best cross-validation score: 1.00
</pre>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h2 id="Exercise-10.-Display-your-model's-estimated-score">Exercise 10. Display your model's estimated score<a class="anchor-link" href="#Exercise-10.-Display-your-model's-estimated-score">¶</a></h2><p>Complete the followng code:</p>
<div class="highlight"><pre><span></span><span class="n">test_score</span> <span class="o">=</span> <span class="n">grid_search</span><span class="o">.</span><span class="n">score</span><span class="p">(</span><span class="o">...</span><span class="p">,</span> <span class="o">...</span><span class="p">)</span>  
<span class="nb">print</span><span class="p">(</span><span class="s2">"Test set score: </span><span class="si">{:.2f}</span><span class="s2">"</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">test_score</span><span class="p">))</span>
</pre></div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [43]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="c1">## Write your response.</span>
<span class="n">test_score</span> <span class="o">=</span> <span class="n">grid_search</span><span class="o">.</span><span class="n">score</span><span class="p">(</span><span class="n">X_test</span><span class="p">,</span> <span class="n">y_test</span><span class="p">)</span>  
<span class="nb">print</span><span class="p">(</span><span class="s2">"Test set score: </span><span class="si">{:.2f}</span><span class="s2">"</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">test_score</span><span class="p">))</span>
</pre></div>
</div>
</div>
</div>
</div>
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
<div class="jp-OutputPrompt jp-OutputArea-prompt"></div>
<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="text/plain" tabindex="0">
<pre>Test set score: 1.00
</pre>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>So we have a reasonably accurate classifer, which is expected to correctly predict about 84% of the time whether it will rain today in the Melbourne area.<br/>
But careful here. Let's take a deeper look at the results.</p>
<p>The best model is stored within the gridsearch object.</p>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h2 id="Exercise-11.-Get-the-model-predictions-from-the-grid-search-estimator-on-the-unseen-data">Exercise 11. Get the model predictions from the grid search estimator on the unseen data<a class="anchor-link" href="#Exercise-11.-Get-the-model-predictions-from-the-grid-search-estimator-on-the-unseen-data">¶</a></h2><p>Complete the followng code:</p>
<div class="highlight"><pre><span></span><span class="n">y_pred</span> <span class="o">=</span> <span class="n">grid_search</span><span class="o">.</span><span class="n">predict</span><span class="p">(</span><span class="o">...</span><span class="p">)</span>
</pre></div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [44]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="c1">### Write your response.</span>
<span class="n">y_pred</span> <span class="o">=</span> <span class="n">grid_search</span><span class="o">.</span><span class="n">predict</span><span class="p">(</span><span class="n">X_test</span><span class="p">)</span>
</pre></div>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h2 id="Exercise-12.-Print-the-classification-report">Exercise 12. Print the classification report<a class="anchor-link" href="#Exercise-12.-Print-the-classification-report">¶</a></h2><p>Complete the followng code:</p>
<div class="highlight"><pre><span></span><span class="nb">print</span><span class="p">(</span><span class="s2">"</span><span class="se">\n</span><span class="s2">Classification Report:"</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="o">...</span><span class="p">(</span><span class="n">y_test</span><span class="p">,</span> <span class="n">y_pred</span><span class="p">))</span>
</pre></div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [46]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="c1">## Write your response.</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">"</span><span class="se">\n</span><span class="s2">Classification Report:"</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="n">classification_report</span><span class="p">(</span><span class="n">y_test</span><span class="p">,</span> <span class="n">y_pred</span><span class="p">))</span> 
</pre></div>
</div>
</div>
</div>
</div>
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
<div class="jp-OutputPrompt jp-OutputArea-prompt"></div>
<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="text/plain" tabindex="0">
<pre>
Classification Report:
              precision    recall  f1-score   support

          No       1.00      1.00      1.00      1154
         Yes       1.00      1.00      1.00       358

    accuracy                           1.00      1512
   macro avg       1.00      1.00      1.00      1512
weighted avg       1.00      1.00      1.00      1512

</pre>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h2 id="Exercise-13.-Plot-the-confusion-matrix">Exercise 13. Plot the confusion matrix<a class="anchor-link" href="#Exercise-13.-Plot-the-confusion-matrix">¶</a></h2><p>Complete the followng code:</p>
<div class="highlight"><pre><span></span><span class="n">conf_matrix</span> <span class="o">=</span> <span class="o">...</span><span class="p">(</span><span class="n">y_test</span><span class="p">,</span> <span class="n">y_pred</span><span class="p">)</span>
<span class="n">disp</span> <span class="o">=</span> <span class="n">ConfusionMatrixDisplay</span><span class="p">(</span><span class="n">confusion_matrix</span><span class="o">=...</span><span class="p">)</span>
<span class="n">disp</span><span class="o">.</span><span class="n">plot</span><span class="p">(</span><span class="n">cmap</span><span class="o">=</span><span class="s1">'Blues'</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s1">'Confusion Matrix'</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">show</span><span class="p">()</span>
</pre></div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [47]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="c1">## Write your response.</span>
<span class="n">conf_matrix</span> <span class="o">=</span> <span class="n">confusion_matrix</span><span class="p">(</span><span class="n">y_test</span><span class="p">,</span> <span class="n">y_pred</span><span class="p">)</span> 
<span class="n">disp</span> <span class="o">=</span> <span class="n">ConfusionMatrixDisplay</span><span class="p">(</span><span class="n">confusion_matrix</span><span class="o">=</span><span class="n">conf_matrix</span><span class="p">)</span> 
<span class="n">disp</span><span class="o">.</span><span class="n">plot</span><span class="p">(</span><span class="n">cmap</span><span class="o">=</span><span class="s1">'Blues'</span><span class="p">)</span> 
<span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s1">'Confusion Matrix'</span><span class="p">)</span> 
<span class="n">plt</span><span class="o">.</span><span class="n">show</span><span class="p">()</span> 
</pre></div>
</div>
</div>
</div>
</div>
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
<div class="jp-OutputPrompt jp-OutputArea-prompt"></div>
<div class="jp-RenderedImage jp-OutputArea-output" tabindex="0">
<img alt="No description has been provided for this image" class="" src="data:image/png;base64,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XDFCQkIkSWfPni1S/59//llWq1V16tRxao+MjFRYWJh+/vlnp/YaNWoUOkeFChX022+/XWbEhd13331q2bKl+vfvr4iICPXs2VPLly//y8SgIM569eoV2tegQQP9+uuvyszMdGr/871UqFBBkty6lzvuuEPBwcF65513tHTpUt14442FvssC+fn5mjlzpurWrSubzaZKlSqpcuXK+uGHH5Senl7ka1arVs2tyYLTp09XeHi4kpKSNHv2bFWpUqXIxwIoOpIBXDFCQkIUFRWlH3/80a3j/jyBzxU/P7+LthuGcdnXKBjPLhAYGKjNmzfr888/1wMPPKAffvhB9913n2677bZCfT3hyb0UsNls6tatmxYvXqwVK1a4rApI0uTJkzVs2DC1bt1ab775pj777DOtW7dO1113XZErINKF78cd3333nU6dOiVJ2rlzp1vHAig6kgFcUe68804dPHhQiYmJl+wbExOj/Px87d+/36k9JSVFaWlpjpUB3lChQgWnmfcF/lx9kCSr1ar27dtrxowZ2r17t5555hlt2LBB//3vfy967oI49+3bV2jf3r17ValSJQUFBXl2Ay706tVL3333nc6ePXvRSZcF3nvvPbVr106vvfaaevbsqQ4dOig+Pr7Qd1LUxKwoMjMz1bdvX8XGxmrgwIGaOnWqtm/f7rXzA/h/JAO4ojz55JMKCgpS//79lZKSUmj/wYMH9cILL0i6UOaWVGjG/4wZMyRJnTt39lpc11xzjdLT0/XDDz842k6ePKkVK1Y49UtNTS10bMHDd/683LFA1apV1aRJEy1evNjpl+uPP/6otWvXOu6zOLRr106TJk3Siy++qMjISJf9/Pz8ClUd3n33XR0/ftyprSBpuVji5K6RI0fq6NGjWrx4sWbMmKGaNWsqISHB5fcI4PLx0CFcUa655hotW7ZM9913nxo0aOD0BMItW7bo3XffVZ8+fSRJjRs3VkJCghYsWKC0tDS1adNG27Zt0+LFi9W1a1eXy9YuR8+ePTVy5Ej9/e9/12OPPaZz585p3rx5uvbaa50m0E2cOFGbN29W586dFRMTo1OnTumll15S9erVdeutt7o8/7Rp09SpUyfFxcWpX79++v333zVnzhyFhoZq/PjxXruPP7NarRo9evQl+915552aOHGi+vbtq1tuuUU7d+7U0qVLVbt2bad+11xz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x44dFRoaqrffflvPP/+827G+8sorhZITPz8/r8UKoHiRDKDUCgoKUp06dYrcv2nTpnrnnXdUpUqVQv86LlC1alVt3bpVrVu3lnThX8A7duxQ06ZNL9q/UaNGys/P16ZNmxQfH19of0FlIi8vz9EWGxsrm82mo0ePuqwoNGjQwDEZssDXX3996Zv8gy1btigmJkb/+c9/HG0///xzoX5Hjx7ViRMnFBUV5biO1WpVvXr1FBERoaioKB06dEi9e/d26/oArhxMIAT+p3fv3qpUqZK6dOmiL774QocPH9bGjRv12GOP6ZdffpEkDRkyRM8++6xWrlypvXv36pFHHvnLZwTUrFlTCQkJeuihh7Ry5UrHOZcvXy5JiomJkcVi0erVq3X69GllZGQoODhYw4cP19ChQ7V48WIdPHhQ3377rebMmeOYlPevf/1L+/fv14gRI7Rv3z4tW7ZMixYtcut+69atq6NHj+rtt9/WwYMHNXv27ItOhgwICFBCQoK+//57ffHFF3rsscfUo0cPRUZGSpImTJigKVOmaPbs2frpp5+0c+dOLVy4UDNmzHArHgC+QzIA/E+5cuW0efNm1ahRQ926dVODBg3Ur18/ZWVlOSoFTzzxhB544AElJCQoLi5OwcHB+vvf//6X5503b57uuecePfLII6pfv74GDBigzMxMSVK1atU0YcIEPfXUU4qIiNDgwYMlSZMmTdKYMWM0ZcoUNWjQQLfffrs+/vhj1apVS9KFcfz3339fK1euVOPGjTV//nxNnjzZrfu9++67NXToUA0ePFhNmjTRli1bNGbMmEL96tSpo27duumOO+5Qhw4ddP311zstHezfv79effVVLVy4UI0aNVKbNm20aNEiR6wArnwWw9XMJwAAYApUBgAAMDmSAQAATI5kAAAAkyMZAADA5EgGAAAwOZIBAABMjmQAAACTIxkAAMDkSAYAADA5kgEAAEyOZAAAAJMjGQAAwOT+D6WytssPXWTvAAAAAElFTkSuQmCC"/>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Let's consider wether the results indicate a good predictor of rainfall.</p>
<h2 id="Points-to-note---2">Points to note - 2<a class="anchor-link" href="#Points-to-note---2">¶</a></h2><p>What is the true positive rate? There will be a question on this in the assignment that follows.</p>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<details><summary>Click here for Hints</summary>
<p>Consider the confusion matrix or the classification report and claculate the true positve rate given the information.</p>
</details>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h2 id="Feature-importances">Feature importances<a class="anchor-link" href="#Feature-importances">¶</a></h2><p>Recall that to obtain the categorical feature importances, we have to work our way backward through the modelling pipeline to associate the feature importances with their original input variables, not the one-hot encoded ones. We don't need to do this for the numeric variables because we didn't modify their names in any way.<br/>
Remember we went from categorical features to one-hot encoded features, using the 'cat' column transformer.</p>
<p>Let's get all of the feature importances and associate them with their transformed features</p>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h2 id="Exercise-14.-Extract-the-feature-importances">Exercise 14. Extract the feature importances<a class="anchor-link" href="#Exercise-14.-Extract-the-feature-importances">¶</a></h2><p>Complete the followng code:</p>
<div class="highlight"><pre><span></span><span class="n">feature_importances</span> <span class="o">=</span> <span class="n">grid_search</span><span class="o">.</span><span class="n">best_estimator_</span><span class="p">[</span><span class="s1">'classifier'</span><span class="p">]</span><span class="o">.</span> <span class="o">...</span>
</pre></div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [50]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="c1">## Write your response.</span>
<span class="n">feature_importances</span> <span class="o">=</span> <span class="n">grid_search</span><span class="o">.</span><span class="n">best_estimator_</span><span class="p">[</span><span class="s1">'classifier'</span><span class="p">]</span><span class="o">.</span><span class="n">feature_importances_</span>  
</pre></div>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Now let's extract the feature importances and plot them as a bar graph.</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [51]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="c1"># Combine numeric and categorical feature names</span>
<span class="n">feature_names</span> <span class="o">=</span> <span class="n">numeric_features</span> <span class="o">+</span> <span class="nb">list</span><span class="p">(</span><span class="n">grid_search</span><span class="o">.</span><span class="n">best_estimator_</span><span class="p">[</span><span class="s1">'preprocessor'</span><span class="p">]</span>
                                        <span class="o">.</span><span class="n">named_transformers_</span><span class="p">[</span><span class="s1">'cat'</span><span class="p">]</span>
                                        <span class="o">.</span><span class="n">named_steps</span><span class="p">[</span><span class="s1">'onehot'</span><span class="p">]</span>
                                        <span class="o">.</span><span class="n">get_feature_names_out</span><span class="p">(</span><span class="n">categorical_features</span><span class="p">))</span>

<span class="n">feature_importances</span> <span class="o">=</span> <span class="n">grid_search</span><span class="o">.</span><span class="n">best_estimator_</span><span class="p">[</span><span class="s1">'classifier'</span><span class="p">]</span><span class="o">.</span><span class="n">feature_importances_</span>

<span class="n">importance_df</span> <span class="o">=</span> <span class="n">pd</span><span class="o">.</span><span class="n">DataFrame</span><span class="p">({</span><span class="s1">'Feature'</span><span class="p">:</span> <span class="n">feature_names</span><span class="p">,</span>
                              <span class="s1">'Importance'</span><span class="p">:</span> <span class="n">feature_importances</span>
                             <span class="p">})</span><span class="o">.</span><span class="n">sort_values</span><span class="p">(</span><span class="n">by</span><span class="o">=</span><span class="s1">'Importance'</span><span class="p">,</span> <span class="n">ascending</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>

<span class="n">N</span> <span class="o">=</span> <span class="mi">20</span>  <span class="c1"># Change this number to display more or fewer features</span>
<span class="n">top_features</span> <span class="o">=</span> <span class="n">importance_df</span><span class="o">.</span><span class="n">head</span><span class="p">(</span><span class="n">N</span><span class="p">)</span>

<span class="c1"># Plotting</span>
<span class="n">plt</span><span class="o">.</span><span class="n">figure</span><span class="p">(</span><span class="n">figsize</span><span class="o">=</span><span class="p">(</span><span class="mi">10</span><span class="p">,</span> <span class="mi">6</span><span class="p">))</span>
<span class="n">plt</span><span class="o">.</span><span class="n">barh</span><span class="p">(</span><span class="n">top_features</span><span class="p">[</span><span class="s1">'Feature'</span><span class="p">],</span> <span class="n">top_features</span><span class="p">[</span><span class="s1">'Importance'</span><span class="p">],</span> <span class="n">color</span><span class="o">=</span><span class="s1">'skyblue'</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">gca</span><span class="p">()</span><span class="o">.</span><span class="n">invert_yaxis</span><span class="p">()</span>  <span class="c1"># Invert y-axis to show the most important feature on top</span>
<span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="sa">f</span><span class="s1">'Top </span><span class="si">{</span><span class="n">N</span><span class="si">}</span><span class="s1"> Most Important Features in predicting whether it will rain today'</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s1">'Importance Score'</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">show</span><span class="p">()</span>
</pre></div>
</div>
</div>
</div>
</div>
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
<div class="jp-OutputPrompt jp-OutputArea-prompt"></div>
<div class="jp-RenderedImage jp-OutputArea-output" tabindex="0">
<img alt="No description has been provided for this image" class="" src="data:image/png;base64,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3fH48WNcuXKlqrtCH7nIyEh4eHhg79696Nu3b1V351/l4MGD6NWrF06dOoW2bdtWdXeI/pV++eUXeHt74+TJk1Uyukxvj89gEhEREb2lN9/xW1BQgHXr1kFHRwfNmzevol4R/ft99913MDMze++vjiHF4zOYRERERG9p3LhxePHiBZydnZGbm4v9+/cjJiYGixYt+qCv4iD6r9i1axf+/PNPHD58GGvWrKk2K7xTxTHAJCIiInpL7du3x4oVK3Do0CHk5OTA3Nwc69atk1tAjIgqbsCAAZBKpRg+fDhGjx5d1d2ht8BnMImIiIiIiEgh+AwmERERERERKQQDTCIiIiIiIlIIPoNJpSosLMT9+/ehra3NB6yJiIiIiD5igiDg+fPnqFu3LpSUSh+nZIBJpbp//z6MjY2ruhtERERERFRN3Lt3D/Xr1y/1OANMKpW2tjaAVzeRjo5OFfeGiIiIiIiqSkZGBoyNjcUYoTQMMKlURdNidXR0GGASEREREVG5j85xkR8iIiIiIiJSCAaYREREREREpBAMMImIiIiIiEghGGASERERERGRQjDAJCIiIiIiIoVggElEREREREQKwQCTiIiIiIiIFIIBJhERERERESkEA0wiIiIiIiJSCAaYREREREREpBAMMImIiIiIiEghGGASERERERGRQjDAJCIiIiIiIoVggElEREREREQKwQCTiIiIiIiIFIIBJhERERERESkEA0wiIiIiIiJSCAaYREREREREpBAqVd0Bqv5WxqdBXZpX1d0gIiIiIvpozGimX9VdeCscwSQiIiIiIiKFYIBJRERERERECvGvDjDd3d0xceLEKms/KCgIDg4OVdY+ERERERFRdVJlAaafnx8kEgkkEglq1KgBU1NTTJs2DTk5ORWuY//+/Zg/f36F8oaEhIjtlbYlJSW95dl8GEXXbMmSJXLpBw8ehEQiqaJeERERERERvVKlI5idO3dGSkoKbt++jVWrVmHz5s0IDAyscPlatWpBW1u7Qnn79++PlJQUcXN2dsbnn38ul2ZsbPy2p/LBqKurY+nSpXj69GlVd4WIiIiIiEhOlQaYampqMDIygrGxMby9veHp6Ynw8HAAQFpaGgYMGIB69epBU1MTdnZ2+Omnn+TKvzlF1sTEBIsWLcKwYcOgra2NBg0a4NtvvwUAaGhowMjISNxUVVWhqakp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h6enJ5YsWYLExES5spqammjUqJFc+aKyFWnvzTLx8fHIzMyEnp6eOEorlUpx586dYm0XCQgIQHp6urjdu3evgmdORERERETERX5E6urq6NixIzp27IjZs2fD398fgYGBiIqKAgAIgiDmzc/PL7GO16e8SiQSAEBhYSEAICgoCAMHDsThw4cRGhqKwMBA7Nq1C7169SpWtqj8622W115RmaL2MjMzUadOHfE50deV9koUNTU1qKmpldkmERERERFRaTiCWQpbW1tkZWXBwMAAAOQW3Hl9wZ/KsLS0xJdffonff/8dvXv3RnBwsCK6WqLmzZvjwYMHUFFRgbm5udymr6//3tolIiIiIqKP10cfYKalpaF9+/bYvn07/vzzT9y5cwd79+7FsmXL0LNnT2hoaKB169ZYsmQJEhIScOLECcyaNatSbbx48QJjx45FZGQk7t69i+joaJw7dw42Njbv6awAT09PODs7w9vbG7///juSkpIQExODr776qtjqtURERERERIrw0U+RlUqlaNWqFVatWoXExETk5+fD2NgYn3/+OWbOnAkA2LJlC4YPHw5HR0dYWVlh2bJl6NSpU4XbUFZWRlpaGoYMGYKHDx9CX18fvXv3xty5c9/XaUEikeDIkSP46quvMHToUDx69AhGRkZwdXWFoaHhe2uXiIiIiIg+XhKhvAf96KOVkZEBXV1dBJ68DXWp9gdte0YzTuMlIiIiIqouimKD9PR06OjolJrvo58iS0RERERERIrBAJOIiIiIiIgU4qN/BpPKN8ler8xhcCIiIiIiIoAjmERERERERKQgDDCJiIiIiIhIIRhgEhERERERkULwGUwq18r4NKhL8965Hr56hIiIiIjov40jmERERERERKQQDDCJiIiIiIhIIRhgEhERERERkUJUSYAZGRkJiUSCZ8+evVM9fn5+8Pb2VkifPgYSiQQHDx6s6m4QEREREdF/1DsHmJs2bYK2tjZevnwppmVmZqJGjRpwd3eXy1sUWNapUwcpKSnQ1dV91+aLefDgASZMmABzc3Ooq6vD0NAQbdu2xcaNG5Gdna2QNpKSkiCRSBAXFyeXnp2djYCAADRq1Ajq6uowMDCAm5sbfvnlF4W0S0REREREVJ298yqyHh4eyMzMxPnz59G6dWsAQFRUFIyMjBAbG4ucnByoq6sDACIiItCgQQNYWVm9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wcPDA4MHD0ZQUBDOnDmDFStWwNXVFePGjYOrq2u14w0dOhQTJkxAx44dER8fDx8fH3z44Ye1xrNo0SKYmJhIG5fuEhERERFRQ+g0dwBPGktLSwwcOBBJSUkQQmDgwIGwsLB4aL8uXbpIv2UyGaytrZGfn19nn6ysLBQVFcHc3Fyt/u7du8jJyZHKjo6Oas98WllZQVtbG1paWmp1fz2en59ftXJmZmat8cTExGD69OlSubCwkEkmERERERHVGxPMGkRERCA6OhoAsGrVqnr10dXVVSvLZDJUVlbW2aeoqAg2NjZQKpXV9pmamtY5dmOO9zB6enrQ09N7pDGIiIiIiKjlYoJZg/79+6O0tBQymQzBwcGP7Tje3t64evUqdHR04OjoqPHxDx48iDFjxqiVH3xZERERERERkSYxwayBtra29DIcbW3tx3acvn37ws/PD6GhoUhMTETHjh1x5coVfP/99xgyZAh8fHweafyqZzuff/55JCcnIyMjA5999pmGoiciIiIiIlLHBLMWxsbGj/0YMpkMO3fuxHvvvYdx48bh+vXrsLa2RkBAAKysrB55/Hnz5mHLli2IioqCjY0NNm/eDA8PDw1ETkREREREVJ1MCCGaOwjSPJlMhq+++gqhoaGNHqOwsBAmJiaI3XsecoVRtf3vdHv4y4+IiIiIiOjpV5UbqFSqOifj+JkSIiIiIiIi0ggmmERERERERKQRfAbzb0qTK5+ne5k3yTOpRERERET0dOMMJhEREREREWkEE0wiIiIiIiLSCCaYREREREREpBF8BpMeallWAeSKUrU6fqKEiIiIiIj+ijOYREREREREpBFMMImIiIiIiEgjmGASERERERGRRrSYBFMmk9W5xcXFNUtct2/fxrRp0+Dg4AB9fX34+/vj8OHDzRILERERERHRo2gxL/nJy8uTfm/duhVz587FmTNnpDqFQtEcYWHChAk4deoUNm7cCFtbW3z++efo27cvTp8+jbZt2zZLTERERERERI3RYmYwra2tpc3ExAQymUytbsuWLXB3d4dcLoebmxs+/vhjqW9ubi5kMhn+85//oGfPntDX10f37t1x9uxZHD58GD4+PlAoFHjxxRdx/fp1qV94eDhCQ0Mxb948WFpawtjYGJGRkSgtvf9G1rt37+LLL79EYmIiAgIC4OzsjLi4ODg7O2P16tXSOBs3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+xEeHo4hQ4YAuJ8g5ebmqgelo4O+ffuib9++iI2NhampKX7++WcEBwejVatW2L9/PxwcHADcT+wOHz6MadOmaeJUaj0/ACguLgYAWFpaIi8vT9pfWFiICxcuPLbj16U+15yIiIiIiKgpNCjBLCgowNChQxEREYEuXbrAyMgIR44cQWJiIkJCQtC3b1/4+fkhNDQUiYmJ6NixI65cuYLvv/8eQ4YMgY+PD1xcXLB9+3YMHjwYMpkMc+bMUZvB++6773D+/HkEBATAzMwMO3fuRGVlJVxdXWFoaIhJkyZh1qxZaN26Nezt7ZGYmIg7d+5g/PjxGrkgr7zyCnr06AF/f39YW1vjwoULiImJQceOHeHm5gYA6N27N5KSkjB48GCYmppi7ty50NbW1sjxG6o+15yIiIiIiKgpNCjBVCgU8PX1xfLly6XnIe3s7DBx4kS8++67kMlk2LlzJ9577z2MGzcO169fh7W1NQICAqRnEJctW4aIiAj4+/vDwsICb7/9ttoziKampti+fTvi4uJw7949uLi4YPPmzejUqRMAICEhAZWVlRg9ejRu374NHx8f7N69G2ZmZhq5IMHBwdi8eTMWLVoElUoFa2tr9O7dG3FxcdDRuX+5YmJicOHCBQwaNAgmJiaIj49vthnM+lxzIiIiIiKipiATf32YkOj/FRYWwsTEBLF7zyOuZ/vmDoeIiIiIiJpJVW6gUqlgbGxca7sGv0WWiIiIiIiIqCYtLsHs1KmT2uc8HtySk5ObOzwiIiIiIqKnlkbeIvs02blzZ42fFAHAZxZrMd3LvLlDICIiIiKip0CLSzCrPm9CREREREREmtXilsgSERERERHR48EEk4iIiIiIiDSCCSYRERERERFpBBNMIiIiIiIi0ggmmERERERERKQRTDCJiIiIiIhII5hgEhERERERkUYwwSQiIiIiIiKNYIJJREREREREGsEEk4iIiIiIiDSCCSYRERERERFpBBNMIiIiIiIi0ggmmERERERERKQRTDCJiIiIiIhII5hgEhERERERkUYwwSQiIiIiIiKNYIJJREREREREGsEEk4iIiIiIiDRCp7kDoCeXEAIAUFhY2MyREBERERFRc6rKCapyhNowwaRaFRQUAADs7OyaORIiIiIiInoS3L59GyYmJrXuZ4JJtWrdujUA4OLFi3XeRETNobCwEHZ2drh0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"/>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h2 id="Point-to-note---3">Point to note - 3<a class="anchor-link" href="#Point-to-note---3">¶</a></h2><p>Identify the most important feature for predicting whether it will rain based on the feature importance bar graph. There will be a question on this in the assignment that follows.</p>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h2 id="Try-another-model">Try another model<a class="anchor-link" href="#Try-another-model">¶</a></h2><h4 id="Some-thoughts.">Some thoughts.<a class="anchor-link" href="#Some-thoughts.">¶</a></h4><p>In practice you would want to try out different models and even revisit the data analysis to improve
your model's performance. Maybe you can engineer better features, drop irrelevant or redundant ones, project your data onto a dimensional feature space, or impute missing values to be able to use more data. You can also try a larger set of parameters to define you search grid, or even engineer new features using cluster analysis. You can even include the clustering algorithm's hyperparameters in your search grid!</p>
<p>With Scikit-learn's powerful pipeline and GridSearchCV classes, this is easy to do in a few steps.</p>
<h2 id="Exercise-15.-Update-the-pipeline-and-the-parameter-grid">Exercise 15. Update the pipeline and the parameter grid<a class="anchor-link" href="#Exercise-15.-Update-the-pipeline-and-the-parameter-grid">¶</a></h2><p>Let's update the pipeline and the parameter grid and train a Logistic Regression model and compare the performance of the two models. You'll need to replace the clasifier with LogisticRegression. We have supplied the parameter grid for you.</p>
<p>Complete the following code:</p>
<div class="highlight"><pre><span></span><span class="c1"># Replace RandomForestClassifier with LogisticRegression</span>
<span class="n">pipeline</span><span class="o">.</span><span class="n">set_params</span><span class="p">(</span><span class="o">...=</span><span class="n">LogisticRegression</span><span class="p">(</span><span class="n">random_state</span><span class="o">=</span><span class="mi">42</span><span class="p">))</span>

<span class="c1"># update the model's estimator to use the new pipeline</span>
<span class="n">grid_search</span><span class="o">.</span><span class="n">estimator</span> <span class="o">=</span> <span class="o">...</span>

<span class="c1"># Define a new grid with Logistic Regression parameters</span>
<span class="n">param_grid</span> <span class="o">=</span> <span class="p">{</span>
    <span class="c1"># 'classifier__n_estimators': [50, 100],</span>
    <span class="c1"># 'classifier__max_depth': [None, 10, 20],</span>
    <span class="c1"># 'classifier__min_samples_split': [2, 5],</span>
    <span class="s1">'classifier__solver'</span> <span class="p">:</span> <span class="p">[</span><span class="s1">'liblinear'</span><span class="p">],</span>
    <span class="s1">'classifier__penalty'</span><span class="p">:</span> <span class="p">[</span><span class="s1">'l1'</span><span class="p">,</span> <span class="s1">'l2'</span><span class="p">],</span>
    <span class="s1">'classifier__class_weight'</span> <span class="p">:</span> <span class="p">[</span><span class="kc">None</span><span class="p">,</span> <span class="s1">'balanced'</span><span class="p">]</span>
<span class="p">}</span>

<span class="n">grid_search</span><span class="o">.</span><span class="n">param_grid</span> <span class="o">=</span> <span class="o">...</span>

<span class="c1"># Fit the updated pipeline with LogisticRegression</span>
<span class="n">model</span><span class="o">.</span><span class="n">fit</span><span class="p">(</span><span class="o">...</span><span class="p">,</span> <span class="o">...</span><span class="p">)</span>

<span class="c1"># Make predictions</span>
<span class="n">y_pred</span> <span class="o">=</span> <span class="n">model</span><span class="o">.</span><span class="n">predict</span><span class="p">(</span><span class="n">X_test</span><span class="p">)</span>
</pre></div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [52]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="c1">## Write your response</span>
<span class="kn">from</span><span class="w"> </span><span class="nn">sklearn.linear_model</span><span class="w"> </span><span class="kn">import</span> <span class="n">LogisticRegression</span>

<span class="c1"># Replace RandomForestClassifier with LogisticRegression</span>
<span class="n">pipeline</span><span class="o">.</span><span class="n">set_params</span><span class="p">(</span><span class="n">classifier</span><span class="o">=</span><span class="n">LogisticRegression</span><span class="p">(</span><span class="n">random_state</span><span class="o">=</span><span class="mi">42</span><span class="p">))</span>

<span class="c1"># Update the model's estimator to use the new pipeline</span>
<span class="n">grid_search</span><span class="o">.</span><span class="n">estimator</span> <span class="o">=</span> <span class="n">pipeline</span>

<span class="c1"># Define a new grid with Logistic Regression parameters</span>
<span class="n">param_grid</span> <span class="o">=</span> <span class="p">{</span>
    <span class="s1">'classifier__solver'</span> <span class="p">:</span> <span class="p">[</span><span class="s1">'liblinear'</span><span class="p">],</span>
    <span class="s1">'classifier__penalty'</span><span class="p">:</span> <span class="p">[</span><span class="s1">'l1'</span><span class="p">,</span> <span class="s1">'l2'</span><span class="p">],</span>
    <span class="s1">'classifier__class_weight'</span> <span class="p">:</span> <span class="p">[</span><span class="kc">None</span><span class="p">,</span> <span class="s1">'balanced'</span><span class="p">]</span>
<span class="p">}</span>

<span class="n">grid_search</span><span class="o">.</span><span class="n">param_grid</span> <span class="o">=</span> <span class="n">param_grid</span>

<span class="c1"># Fit the updated pipeline with LogisticRegression</span>
<span class="n">model</span> <span class="o">=</span> <span class="n">grid_search</span><span class="o">.</span><span class="n">fit</span><span class="p">(</span><span class="n">X_train</span><span class="p">,</span> <span class="n">y_train</span><span class="p">)</span>

<span class="c1"># Make predictions</span>
<span class="n">y_pred</span> <span class="o">=</span> <span class="n">model</span><span class="o">.</span><span class="n">predict</span><span class="p">(</span><span class="n">X_test</span><span class="p">)</span>
</pre></div>
</div>
</div>
</div>
</div>
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
<div class="jp-OutputPrompt jp-OutputArea-prompt"></div>
<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="text/plain" tabindex="0">
<pre>Fitting 5 folds for each of 4 candidates, totalling 20 fits
[CV] END classifier__class_weight=None, classifier__penalty=l1, classifier__solver=liblinear; total time=   0.1s
[CV] END classifier__class_weight=None, classifier__penalty=l1, classifier__solver=liblinear; total time=   0.0s
[CV] END classifier__class_weight=None, classifier__penalty=l1, classifier__solver=liblinear; total time=   0.0s
[CV] END classifier__class_weight=None, classifier__penalty=l1, classifier__solver=liblinear; total time=   0.0s
[CV] END classifier__class_weight=None, classifier__penalty=l1, classifier__solver=liblinear; total time=   0.0s
[CV] END classifier__class_weight=None, classifier__penalty=l2, classifier__solver=liblinear; total time=   0.1s
[CV] END classifier__class_weight=None, classifier__penalty=l2, classifier__solver=liblinear; total time=   0.0s
[CV] END classifier__class_weight=None, classifier__penalty=l2, classifier__solver=liblinear; total time=   0.1s
[CV] END classifier__class_weight=None, classifier__penalty=l2, classifier__solver=liblinear; total time=   0.1s
[CV] END classifier__class_weight=None, classifier__penalty=l2, classifier__solver=liblinear; total time=   0.0s
[CV] END classifier__class_weight=balanced, classifier__penalty=l1, classifier__solver=liblinear; total time=   0.0s
[CV] END classifier__class_weight=balanced, classifier__penalty=l1, classifier__solver=liblinear; total time=   0.0s
[CV] END classifier__class_weight=balanced, classifier__penalty=l1, classifier__solver=liblinear; total time=   0.0s
[CV] END classifier__class_weight=balanced, classifier__penalty=l1, classifier__solver=liblinear; total time=   0.0s
[CV] END classifier__class_weight=balanced, classifier__penalty=l1, classifier__solver=liblinear; total time=   0.0s
[CV] END classifier__class_weight=balanced, classifier__penalty=l2, classifier__solver=liblinear; total time=   0.1s
[CV] END classifier__class_weight=balanced, classifier__penalty=l2, classifier__solver=liblinear; total time=   0.1s
[CV] END classifier__class_weight=balanced, classifier__penalty=l2, classifier__solver=liblinear; total time=   0.1s
[CV] END classifier__class_weight=balanced, classifier__penalty=l2, classifier__solver=liblinear; total time=   0.1s
[CV] END classifier__class_weight=balanced, classifier__penalty=l2, classifier__solver=liblinear; total time=   0.1s
</pre>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h3 id="Compare-the-results-to-your-previous-model.">Compare the results to your previous model.<a class="anchor-link" href="#Compare-the-results-to-your-previous-model.">¶</a></h3><p>Display the clasification report and the confusion matrix for the new model and compare your results with the previous model.</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [53]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="nb">print</span><span class="p">(</span><span class="n">classification_report</span><span class="p">(</span><span class="n">y_test</span><span class="p">,</span> <span class="n">y_pred</span><span class="p">))</span>

<span class="c1"># Generate the confusion matrix </span>
<span class="n">conf_matrix</span> <span class="o">=</span> <span class="n">confusion_matrix</span><span class="p">(</span><span class="n">y_test</span><span class="p">,</span> <span class="n">y_pred</span><span class="p">)</span>

<span class="n">plt</span><span class="o">.</span><span class="n">figure</span><span class="p">()</span>
<span class="n">sns</span><span class="o">.</span><span class="n">heatmap</span><span class="p">(</span><span class="n">conf_matrix</span><span class="p">,</span> <span class="n">annot</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">cmap</span><span class="o">=</span><span class="s1">'Blues'</span><span class="p">,</span> <span class="n">fmt</span><span class="o">=</span><span class="s1">'d'</span><span class="p">)</span>

<span class="c1"># Set the title and labels</span>
<span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s1">'Titanic Classification Confusion Matrix'</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s1">'Predicted'</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s1">'Actual'</span><span class="p">)</span>

<span class="c1"># Show the plot</span>
<span class="n">plt</span><span class="o">.</span><span class="n">tight_layout</span><span class="p">()</span>
<span class="n">plt</span><span class="o">.</span><span class="n">show</span><span class="p">()</span>
</pre></div>
</div>
</div>
</div>
</div>
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
<div class="jp-OutputPrompt jp-OutputArea-prompt"></div>
<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="text/plain" tabindex="0">
<pre>              precision    recall  f1-score   support

          No       1.00      1.00      1.00      1154
         Yes       1.00      1.00      1.00       358

    accuracy                           1.00      1512
   macro avg       1.00      1.00      1.00      1512
weighted avg       1.00      1.00      1.00      1512

</pre>
</div>
</div>
<div class="jp-OutputArea-child">
<div class="jp-OutputPrompt jp-OutputArea-prompt"></div>
<div class="jp-RenderedImage jp-OutputArea-output" tabindex="0">
<img alt="No description has been provided for this image" class="" src="data:image/png;base64,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WJgCAwMveRySufP7T48++qiSkpK0f/9+JSYm6tFHH73g2P3796tz584KCgpSiRIlFBwcrIYNG0oq2O/UuX83zAgKCtKECRP0888/KyAgQBMmTDC9LlCYkIThX2nfvr3efvttPfHEE/r000/19ddfa8mSJZKUb4Jxoet5jCvwpJSqVatKkrZs2XJZ66enp6thw4bavHmzRo4cqc8//1xJSUmu69fOP75x48bp559/1nPPPae///5b/fr1U40aNXTgwAFJZ6sFycnJ+uabb9SpUyf9/PPPeuSRR9S4cWPl5OT8yyM1Z/fu3br//vuVlpam119/XV988YWSkpI0YMCAPMdzpVzuYwb+7Wt5KVfi9/Kfr+s999yj3bt3691331XNmjU1Y8YM3XbbbZoxY8Ylt2X2Aa5WHcdDDz0kp9OpuLg4ZWZmqn379vmOy8nJUePGjfXFF1/omWeeUWJiopKSklzPmCvI79T5FTUzli5dKulsonzufQZca0jCcEkX+gA4duyYli1bpmeffVYvvviiWrdurcaNG+vGG2+0dP+VKlXS//73vwKv17RpU3l6euZ5RppZK1as0JEjRzRr1iw99dRTevDBBxUTE+OqkvxTrVq19MILLyg5OVkrV67UH3/8oWnTprmWe3h46P7779frr7+uX375RS+//LKWL1+ub7/99rLiO1+lSpX0559/6ujRoxcc8/nnnyszM1OLFi3S448/rmbNmikmJibfDz+zH/rnWlQ7duzIs2zHjh0XbGEV1F133aVSpUpp7ty5ppLWiIiIfGM610K2Ki7pbKUpPT3dbV5WVpYOHjyYZ2xQUJC6dOmiuXPn6vfff9ctt9xy0WfvRUREKDc3N08LMzU1Venp6ZYex/l8fX3VqlUrrVixQo0bN77gzS9btmzRzp07NW7cOD3zzDNq2bKlYmJiFB4enmesld8EsGTJEs2YMUNPP/20goODFRcXp+zsbMu2D1wtJGG4pOLFi0tSng+ac391//Ov7PHjx1u6/7Zt22rz5s157gTLb9/nK1++vHr06KGvv/5aEydOzLM8NzdX48aNu+Bf0fkdX1ZWVp47sDIyMvJ8ANSqVUseHh7KzMyUpHyTo1tvvVWSXGP+jbZt28owDL344ot5lp2LP7/jOX78uGbOnJlnHT8/vzyvd37q1q2rkJAQTZs2ze04vvrqK23btk3N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SEiIBg8erOzs7H8ZTV4kYQAAwFIOh3XT5Vq3bp3eeust3XLLLW7zBwwYoM8//1yffPKJvvvuO/35559q06aNa3lOTo6aN2+urKws/fjjj5o9e7ZmzZqlYcOGXX4wF0ASBgAAipQTJ06oY8eOevvtt1WqVCnX/OPHj+udd97R66+/rvvuu09RUVGaOXOmfvzxR61evVqS9PXXX+uXX37R+++/r1tvvVVNmzbVSy+9pMmTJysrK8vSOEnCAACApRwOh2VTZmamMjIy3KbMzMyL7r93795q3ry5YmJi3OavX79eZ86ccZtftWpVVahQQatWrZIkrVq1SrVq1VJoaKhrTGxsrDIyMrR161YLzxJJGAAAsJiHhVNCQoICAgLcpoSEhAvu+6OPPtKGDRvyHZOSkiJvb28FBga6zQ8NDVVKSoprzPkJ2Lnl55ZZiUdUAACAQmvIkCGKj493m+d0OvMd+/vvv+upp55SUlKSfHx8rkZ4/wqVMAAAYCkr25FOp1P+/v5u04WSsPXr1+vQoUO67bbbVKxYMRUrVkzfffedJkyYoGLFiik0NFRZWVlKT093Wy81NVVhYWGSpLCwsDx3S577+dwYq5CEAQAAS9n1iIr7779fW7Zs0aZNm1xT3bp11bFjR9f/e3l5admyZa51duzYof379ys6OlqSFB0drS1btujQoUOuMUlJSfL391f16tULfjIugnYkAAAoEkqWLKmaNWu6zfPz81Pp0qVd87t166b4+HgFBQXJ399fffv2VXR0tOrXry9JeuCBB1S9enV16tRJY8eOVUpKil544QX17t37ghW4y0USBgAALOUoxF9b9MYbb8jDw0Nt27ZVZmamYmNjNWXKFNdyT09PLV68WL169VJ0dLT8/PwUFxenkSNHWh6LwzAMw/Kt2uy09Q+1BXAZvtmeeulBAK64B2uGXnqQhT7dfNCybbWpXdaybRU2XBMGAABgA9qRAADAUoW5HVmYkIQBAABLkYKZQzsSAADABlTCAACApehGmkMSBgAALOVBQ9IU2pEAAAA2oBIGAAAsRTvSHJIwAABgKQftSFNoRwIAANiAShgAALAU7UhzSMIAAICluDvSHNqRAAAANqASBgAALEU70hySMAAAYCmSMHNoRwIAANiAShgAALAUzwkzhyQMAABYyoMczBTakQAAADagEgYAACxFO9IckjAA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7d69W8ePH9fBgwdVr14917JixYqpbt26eVqS52zatEmenp5q2LCh6Zh//fVXnTp1So0bN3abn5WVpTp16kiStm3b5haHJFfCBgCFHUkYcB1o1KiRpk6dKm9vb4WHh6tYsf976/v5+bmNPXHihKKiovTBBx/k2U5wcPBl7d/X17fA65w4cUKS9MUXX6hcuXJuy5xO52XFAQCFCUkYcB3w8/NT5cqVTY297bbbNG/ePIWEhMjf3z/fMWXLltWaNWt0zz33SJKys7O1fv163XbbbfmOr1WrlnJzc/Xdd9+52pHnO1eJy8nJcc2rXr26nE6n9u/ff8EKWrVq1bRo0SK3eatXr770QQJAIcCF+QDcdOzYUWXKlFHLli21cuVK7d27VytWrFC/fv104MABSdJTTz2lV155RYmJidq+fbuefPLJiz7jq2LFioqLi1PXrl2VmJjo2ubHH38sSYqIiJDD4dDixYt1+PBhnThxQiVLltSgQYM0YMAAzZ49W7t379aGDRs0ceJEzZ49W5L0xBNPaNeuXRo8eLB27NihDz/8ULNmzbrSpwgALEESBsBN8eLFlZycrAoVKqhNmzaqVq2aunXrptOnT7sqYwMHDlSnTp0UFxen6OholSxZUq1bt77odqdOnap27drpySefVNWqVdWjRw+dPHlSklSuXDm9+OKLevbZZxUaGqo+ffpIkl566SUNHTpUCQkJqlatmpo0aaIvvvhCkZGRkqQKFSpowYIFSkxMVO3atTVt2jSNHj36Cp4dALCOw7jQlbQAAAC4YqiEAQAA2IAkDAAAwAYkYQAAADYgCQMAALABSRgAAIANSMIAAABsQBIGAABgA5IwAAAAG5CEAQAA2IAkDAAAwAYkYQAAADYgCQMAALDB/wP1ABwLccSMYwAAAABJRU5ErkJggg=="/>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>What can you conclude about the model performances?</p>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h2 id="Points-to-note---4">Points to note - 4<a class="anchor-link" href="#Points-to-note---4">¶</a></h2><p>Compare the accuracy and true positive rate of rainfall predictions between the LogisticRegression model and the RandomForestClassifier model.</p>
<p><strong>Note: Make sure to provide the answer in the form of a list using either bullets or numbers.</strong></p>
<p>There will be a question on this in the assignment that follows.</p>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<details><summary>Click here for Hints</summary>
<pre><code>    </code></pre>
<p>Compare the accuracy percentages of both the classifiers.</p>
<p>Provide the details of the number of correct predictions.</p>
<p>Provide the true positive rate of LogisticRegression Classifier.</p>
</details>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h3 id="Congratulations!-You've-made-it-the-end-of-your-final-project!">Congratulations! You've made it the end of your final project!<a class="anchor-link" href="#Congratulations!-You've-made-it-the-end-of-your-final-project!">¶</a></h3><p>Well done! You now have some great tools to use for tackling complex real-world problems with machine learning.</p>
<h2 id="Author">Author<a class="anchor-link" href="#Author">¶</a></h2><p><a href="https://www.linkedin.com/in/jpgrossman/" target="_blank">Jeff Grossman</a></p>
<h3 id="Other-Contributor(s)">Other Contributor(s)<a class="anchor-link" href="#Other-Contributor(s)">¶</a></h3><p><a href="https://www.linkedin.com/in/abhishek-gagneja-23051987/" taget="_blank">Abhishek Gagneja</a></p>
<!-- ## Changelog

| Date | Version | Changed by | Change Description |
|:------------|:------|:------------------|:---------------------------------------|
| 2024-11-26 | 0.2  | Anita Verma    | Fixed the variable used before definition in Exercise 14|
| 2024-11-26 | 0.1  | Jeff Grossman    | Create lab |

 -->
<h3 align="center"> © IBM Corporation. All rights reserved. <h3></h3>
</h3></div>
</div>
</div>
</div></section></section>
</div>
</div>
</main>
</body>
<script>
require(
    {
      // it makes sense to wait a little bit when you are loading
      // reveal from a cdn in a slow connection environment
      waitSeconds: 15
    },
    [
      "https://unpkg.com/reveal.js@4.0.2/dist/reveal.js",
      "https://unpkg.com/reveal.js@4.0.2/plugin/notes/notes.js"
    ],

    function(Reveal, RevealNotes){
        // Full list of configuration options available here: https://github.com/hakimel/reveal.js#configuration
        Reveal.initialize({
            controls: true,
            progress: true,
            history: true,
            transition: "slide",
            slideNumber: "",
            plugins: [RevealNotes],
            width: 960,
			      height: 700,

        });

        var update = function(event){
          if(MathJax.Hub.getAllJax(Reveal.getCurrentSlide())){
            MathJax.Hub.Rerender(Reveal.getCurrentSlide());
          }
        };

        Reveal.addEventListener('slidechanged', update);

        function setScrollingSlide() {
            var scroll = false
            if (scroll === true) {
              var h = $('.reveal').height() * 0.95;
              $('section.present').find('section')
                .filter(function() {
                  return $(this).height() > h;
                })
                .css('height', 'calc(95vh)')
                .css('overflow-y', 'scroll')
                .css('margin-top', '20px');
            }
        }

        // check and set the scrolling slide every time the slide change
        Reveal.addEventListener('slidechanged', setScrollingSlide);
    }
);
</script>
</html>
