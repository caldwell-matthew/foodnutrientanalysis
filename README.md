<!DOCTYPE html>
<html>
<head><meta charset="utf-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>FINAL</title><script src="https://cdnjs.cloudflare.com/ajax/libs/require.js/2.1.10/require.min.js"></script>




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

/*
 * Webkit scrollbar styling
 */

/* use standard opaque scrollbars for most nodes */

[data-jp-theme-scrollbars='true'] ::-webkit-scrollbar,
[data-jp-theme-scrollbars='true'] ::-webkit-scrollbar-corner {
  background: var(--jp-scrollbar-background-color);
}

[data-jp-theme-scrollbars='true'] ::-webkit-scrollbar-thumb {
  background: rgb(var(--jp-scrollbar-thumb-color));
  border: var(--jp-scrollbar-thumb-margin) solid transparent;
  background-clip: content-box;
  border-radius: var(--jp-scrollbar-thumb-radius);
}

[data-jp-theme-scrollbars='true'] ::-webkit-scrollbar-track:horizontal {
  border-left: var(--jp-scrollbar-endpad) solid
    var(--jp-scrollbar-background-color);
  border-right: var(--jp-scrollbar-endpad) solid
    var(--jp-scrollbar-background-color);
}

[data-jp-theme-scrollbars='true'] ::-webkit-scrollbar-track:vertical {
  border-top: var(--jp-scrollbar-endpad) solid
    var(--jp-scrollbar-background-color);
  border-bottom: var(--jp-scrollbar-endpad) solid
    var(--jp-scrollbar-background-color);
}

/* for code nodes, use a transparent style of scrollbar */

[data-jp-theme-scrollbars='true'] .CodeMirror-hscrollbar::-webkit-scrollbar,
[data-jp-theme-scrollbars='true'] .CodeMirror-vscrollbar::-webkit-scrollbar,
[data-jp-theme-scrollbars='true']
  .CodeMirror-hscrollbar::-webkit-scrollbar-corner,
[data-jp-theme-scrollbars='true']
  .CodeMirror-vscrollbar::-webkit-scrollbar-corner {
  background-color: transparent;
}

[data-jp-theme-scrollbars='true']
  .CodeMirror-hscrollbar::-webkit-scrollbar-thumb,
[data-jp-theme-scrollbars='true']
  .CodeMirror-vscrollbar::-webkit-scrollbar-thumb {
  background: rgba(var(--jp-scrollbar-thumb-color), 0.5);
  border: var(--jp-scrollbar-thumb-margin) solid transparent;
  background-clip: content-box;
  border-radius: var(--jp-scrollbar-thumb-radius);
}

[data-jp-theme-scrollbars='true']
  .CodeMirror-hscrollbar::-webkit-scrollbar-track:horizontal {
  border-left: var(--jp-scrollbar-endpad) solid transparent;
  border-right: var(--jp-scrollbar-endpad) solid transparent;
}

[data-jp-theme-scrollbars='true']
  .CodeMirror-vscrollbar::-webkit-scrollbar-track:vertical {
  border-top: var(--jp-scrollbar-endpad) solid transparent;
  border-bottom: var(--jp-scrollbar-endpad) solid transparent;
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
  border-left: 0px solid transparent;
  border-right: 0px solid transparent;
}

.jp-scrollbar-tiny::-webkit-scrollbar-track:vertical {
  border-top: 0px solid transparent;
  border-bottom: 0px solid transparent;
}

/*
 * Phosphor
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

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/


/* <DEPRECATED> */ .p-Widget, /* </DEPRECATED> */
.lm-Widget {
  box-sizing: border-box;
  position: relative;
  overflow: hidden;
  cursor: default;
}


/* <DEPRECATED> */ .p-Widget.p-mod-hidden, /* </DEPRECATED> */
.lm-Widget.lm-mod-hidden {
  display: none !important;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/


/* <DEPRECATED> */ .p-CommandPalette, /* </DEPRECATED> */
.lm-CommandPalette {
  display: flex;
  flex-direction: column;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}


/* <DEPRECATED> */ .p-CommandPalette-search, /* </DEPRECATED> */
.lm-CommandPalette-search {
  flex: 0 0 auto;
}


/* <DEPRECATED> */ .p-CommandPalette-content, /* </DEPRECATED> */
.lm-CommandPalette-content {
  flex: 1 1 auto;
  margin: 0;
  padding: 0;
  min-height: 0;
  overflow: auto;
  list-style-type: none;
}


/* <DEPRECATED> */ .p-CommandPalette-header, /* </DEPRECATED> */
.lm-CommandPalette-header {
  overflow: hidden;
  white-space: nowrap;
  text-overflow: ellipsis;
}


/* <DEPRECATED> */ .p-CommandPalette-item, /* </DEPRECATED> */
.lm-CommandPalette-item {
  display: flex;
  flex-direction: row;
}


/* <DEPRECATED> */ .p-CommandPalette-itemIcon, /* </DEPRECATED> */
.lm-CommandPalette-itemIcon {
  flex: 0 0 auto;
}


/* <DEPRECATED> */ .p-CommandPalette-itemContent, /* </DEPRECATED> */
.lm-CommandPalette-itemContent {
  flex: 1 1 auto;
  overflow: hidden;
}


/* <DEPRECATED> */ .p-CommandPalette-itemShortcut, /* </DEPRECATED> */
.lm-CommandPalette-itemShortcut {
  flex: 0 0 auto;
}


/* <DEPRECATED> */ .p-CommandPalette-itemLabel, /* </DEPRECATED> */
.lm-CommandPalette-itemLabel {
  overflow: hidden;
  white-space: nowrap;
  text-overflow: ellipsis;
}

.lm-close-icon {
	border:1px solid transparent;
  background-color: transparent;
  position: absolute;
	z-index:1;
	right:3%;
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
	content: "X";
	display: block;
	width: 15px;
	height: 15px;
	text-align: center;
	color:#000;
	font-weight: normal;
	font-size: 12px;
	cursor: pointer;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/


/* <DEPRECATED> */ .p-DockPanel, /* </DEPRECATED> */
.lm-DockPanel {
  z-index: 0;
}


/* <DEPRECATED> */ .p-DockPanel-widget, /* </DEPRECATED> */
.lm-DockPanel-widget {
  z-index: 0;
}


/* <DEPRECATED> */ .p-DockPanel-tabBar, /* </DEPRECATED> */
.lm-DockPanel-tabBar {
  z-index: 1;
}


/* <DEPRECATED> */ .p-DockPanel-handle, /* </DEPRECATED> */
.lm-DockPanel-handle {
  z-index: 2;
}


/* <DEPRECATED> */ .p-DockPanel-handle.p-mod-hidden, /* </DEPRECATED> */
.lm-DockPanel-handle.lm-mod-hidden {
  display: none !important;
}


/* <DEPRECATED> */ .p-DockPanel-handle:after, /* </DEPRECATED> */
.lm-DockPanel-handle:after {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  content: '';
}


/* <DEPRECATED> */
.p-DockPanel-handle[data-orientation='horizontal'],
/* </DEPRECATED> */
.lm-DockPanel-handle[data-orientation='horizontal'] {
  cursor: ew-resize;
}


/* <DEPRECATED> */
.p-DockPanel-handle[data-orientation='vertical'],
/* </DEPRECATED> */
.lm-DockPanel-handle[data-orientation='vertical'] {
  cursor: ns-resize;
}


/* <DEPRECATED> */
.p-DockPanel-handle[data-orientation='horizontal']:after,
/* </DEPRECATED> */
.lm-DockPanel-handle[data-orientation='horizontal']:after {
  left: 50%;
  min-width: 8px;
  transform: translateX(-50%);
}


/* <DEPRECATED> */
.p-DockPanel-handle[data-orientation='vertical']:after,
/* </DEPRECATED> */
.lm-DockPanel-handle[data-orientation='vertical']:after {
  top: 50%;
  min-height: 8px;
  transform: translateY(-50%);
}


/* <DEPRECATED> */ .p-DockPanel-overlay, /* </DEPRECATED> */
.lm-DockPanel-overlay {
  z-index: 3;
  box-sizing: border-box;
  pointer-events: none;
}


/* <DEPRECATED> */ .p-DockPanel-overlay.p-mod-hidden, /* </DEPRECATED> */
.lm-DockPanel-overlay.lm-mod-hidden {
  display: none !important;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/


/* <DEPRECATED> */ .p-Menu, /* </DEPRECATED> */
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


/* <DEPRECATED> */ .p-Menu-content, /* </DEPRECATED> */
.lm-Menu-content {
  margin: 0;
  padding: 0;
  display: table;
  list-style-type: none;
}


/* <DEPRECATED> */ .p-Menu-item, /* </DEPRECATED> */
.lm-Menu-item {
  display: table-row;
}


/* <DEPRECATED> */
.p-Menu-item.p-mod-hidden,
.p-Menu-item.p-mod-collapsed,
/* </DEPRECATED> */
.lm-Menu-item.lm-mod-hidden,
.lm-Menu-item.lm-mod-collapsed {
  display: none !important;
}


/* <DEPRECATED> */
.p-Menu-itemIcon,
.p-Menu-itemSubmenuIcon,
/* </DEPRECATED> */
.lm-Menu-itemIcon,
.lm-Menu-itemSubmenuIcon {
  display: table-cell;
  text-align: center;
}


/* <DEPRECATED> */ .p-Menu-itemLabel, /* </DEPRECATED> */
.lm-Menu-itemLabel {
  display: table-cell;
  text-align: left;
}


/* <DEPRECATED> */ .p-Menu-itemShortcut, /* </DEPRECATED> */
.lm-Menu-itemShortcut {
  display: table-cell;
  text-align: right;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/


/* <DEPRECATED> */ .p-MenuBar, /* </DEPRECATED> */
.lm-MenuBar {
  outline: none;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}


/* <DEPRECATED> */ .p-MenuBar-content, /* </DEPRECATED> */
.lm-MenuBar-content {
  margin: 0;
  padding: 0;
  display: flex;
  flex-direction: row;
  list-style-type: none;
}


/* <DEPRECATED> */ .p--MenuBar-item, /* </DEPRECATED> */
.lm-MenuBar-item {
  box-sizing: border-box;
}


/* <DEPRECATED> */
.p-MenuBar-itemIcon,
.p-MenuBar-itemLabel,
/* </DEPRECATED> */
.lm-MenuBar-itemIcon,
.lm-MenuBar-itemLabel {
  display: inline-block;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/


/* <DEPRECATED> */ .p-ScrollBar, /* </DEPRECATED> */
.lm-ScrollBar {
  display: flex;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}


/* <DEPRECATED> */
.p-ScrollBar[data-orientation='horizontal'],
/* </DEPRECATED> */
.lm-ScrollBar[data-orientation='horizontal'] {
  flex-direction: row;
}


/* <DEPRECATED> */
.p-ScrollBar[data-orientation='vertical'],
/* </DEPRECATED> */
.lm-ScrollBar[data-orientation='vertical'] {
  flex-direction: column;
}


/* <DEPRECATED> */ .p-ScrollBar-button, /* </DEPRECATED> */
.lm-ScrollBar-button {
  box-sizing: border-box;
  flex: 0 0 auto;
}


/* <DEPRECATED> */ .p-ScrollBar-track, /* </DEPRECATED> */
.lm-ScrollBar-track {
  box-sizing: border-box;
  position: relative;
  overflow: hidden;
  flex: 1 1 auto;
}


/* <DEPRECATED> */ .p-ScrollBar-thumb, /* </DEPRECATED> */
.lm-ScrollBar-thumb {
  box-sizing: border-box;
  position: absolute;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/


/* <DEPRECATED> */ .p-SplitPanel-child, /* </DEPRECATED> */
.lm-SplitPanel-child {
  z-index: 0;
}


/* <DEPRECATED> */ .p-SplitPanel-handle, /* </DEPRECATED> */
.lm-SplitPanel-handle {
  z-index: 1;
}


/* <DEPRECATED> */ .p-SplitPanel-handle.p-mod-hidden, /* </DEPRECATED> */
.lm-SplitPanel-handle.lm-mod-hidden {
  display: none !important;
}


/* <DEPRECATED> */ .p-SplitPanel-handle:after, /* </DEPRECATED> */
.lm-SplitPanel-handle:after {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  content: '';
}


/* <DEPRECATED> */
.p-SplitPanel[data-orientation='horizontal'] > .p-SplitPanel-handle,
/* </DEPRECATED> */
.lm-SplitPanel[data-orientation='horizontal'] > .lm-SplitPanel-handle {
  cursor: ew-resize;
}


/* <DEPRECATED> */
.p-SplitPanel[data-orientation='vertical'] > .p-SplitPanel-handle,
/* </DEPRECATED> */
.lm-SplitPanel[data-orientation='vertical'] > .lm-SplitPanel-handle {
  cursor: ns-resize;
}


/* <DEPRECATED> */
.p-SplitPanel[data-orientation='horizontal'] > .p-SplitPanel-handle:after,
/* </DEPRECATED> */
.lm-SplitPanel[data-orientation='horizontal'] > .lm-SplitPanel-handle:after {
  left: 50%;
  min-width: 8px;
  transform: translateX(-50%);
}


/* <DEPRECATED> */
.p-SplitPanel[data-orientation='vertical'] > .p-SplitPanel-handle:after,
/* </DEPRECATED> */
.lm-SplitPanel[data-orientation='vertical'] > .lm-SplitPanel-handle:after {
  top: 50%;
  min-height: 8px;
  transform: translateY(-50%);
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/


/* <DEPRECATED> */ .p-TabBar, /* </DEPRECATED> */
.lm-TabBar {
  display: flex;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}


/* <DEPRECATED> */ .p-TabBar[data-orientation='horizontal'], /* </DEPRECATED> */
.lm-TabBar[data-orientation='horizontal'] {
  flex-direction: row;
  align-items: flex-end;
}


/* <DEPRECATED> */ .p-TabBar[data-orientation='vertical'], /* </DEPRECATED> */
.lm-TabBar[data-orientation='vertical'] {
  flex-direction: column;
  align-items: flex-end;
}


/* <DEPRECATED> */ .p-TabBar-content, /* </DEPRECATED> */
.lm-TabBar-content {
  margin: 0;
  padding: 0;
  display: flex;
  flex: 1 1 auto;
  list-style-type: none;
}


/* <DEPRECATED> */
.p-TabBar[data-orientation='horizontal'] > .p-TabBar-content,
/* </DEPRECATED> */
.lm-TabBar[data-orientation='horizontal'] > .lm-TabBar-content {
  flex-direction: row;
}


/* <DEPRECATED> */
.p-TabBar[data-orientation='vertical'] > .p-TabBar-content,
/* </DEPRECATED> */
.lm-TabBar[data-orientation='vertical'] > .lm-TabBar-content {
  flex-direction: column;
}


/* <DEPRECATED> */ .p-TabBar-tab, /* </DEPRECATED> */
.lm-TabBar-tab {
  display: flex;
  flex-direction: row;
  box-sizing: border-box;
  overflow: hidden;
}


/* <DEPRECATED> */
.p-TabBar-tabIcon,
.p-TabBar-tabCloseIcon,
/* </DEPRECATED> */
.lm-TabBar-tabIcon,
.lm-TabBar-tabCloseIcon {
  flex: 0 0 auto;
}


/* <DEPRECATED> */ .p-TabBar-tabLabel, /* </DEPRECATED> */
.lm-TabBar-tabLabel {
  flex: 1 1 auto;
  overflow: hidden;
  white-space: nowrap;
}


.lm-TabBar-tabInput {
  user-select: all;
  width: 100%;
  box-sizing : border-box;
}


/* <DEPRECATED> */ .p-TabBar-tab.p-mod-hidden, /* </DEPRECATED> */
.lm-TabBar-tab.lm-mod-hidden {
  display: none !important;
}


.lm-TabBar-addButton.lm-mod-hidden {
  display: none !important;
}


/* <DEPRECATED> */ .p-TabBar.p-mod-dragging .p-TabBar-tab, /* </DEPRECATED> */
.lm-TabBar.lm-mod-dragging .lm-TabBar-tab {
  position: relative;
}


/* <DEPRECATED> */
.p-TabBar.p-mod-dragging[data-orientation='horizontal'] .p-TabBar-tab,
/* </DEPRECATED> */
.lm-TabBar.lm-mod-dragging[data-orientation='horizontal'] .lm-TabBar-tab {
  left: 0;
  transition: left 150ms ease;
}


/* <DEPRECATED> */
.p-TabBar.p-mod-dragging[data-orientation='vertical'] .p-TabBar-tab,
/* </DEPRECATED> */
.lm-TabBar.lm-mod-dragging[data-orientation='vertical'] .lm-TabBar-tab {
  top: 0;
  transition: top 150ms ease;
}


/* <DEPRECATED> */
.p-TabBar.p-mod-dragging .p-TabBar-tab.p-mod-dragging,
/* </DEPRECATED> */
.lm-TabBar.lm-mod-dragging .lm-TabBar-tab.lm-mod-dragging {
  transition: none;
}

.lm-TabBar-tabLabel .lm-TabBar-tabInput {
  user-select: all;
  width: 100%;
  box-sizing : border-box;
  background: inherit;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/


/* <DEPRECATED> */ .p-TabPanel-tabBar, /* </DEPRECATED> */
.lm-TabPanel-tabBar {
  z-index: 1;
}


/* <DEPRECATED> */ .p-TabPanel-stackedPanel, /* </DEPRECATED> */
.lm-TabPanel-stackedPanel {
  z-index: 0;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

@charset "UTF-8";
html{
  -webkit-box-sizing:border-box;
          box-sizing:border-box; }

*,
*::before,
*::after{
  -webkit-box-sizing:inherit;
          box-sizing:inherit; }

body{
  font-size:14px;
  font-weight:400;
  letter-spacing:0;
  line-height:1.28581;
  text-transform:none;
  color:#182026;
  font-family:-apple-system, "BlinkMacSystemFont", "Segoe UI", "Roboto", "Oxygen", "Ubuntu", "Cantarell", "Open Sans", "Helvetica Neue", "Icons16", sans-serif; }

p{
  margin-bottom:10px;
  margin-top:0; }

small{
  font-size:12px; }

strong{
  font-weight:600; }

::-moz-selection{
  background:rgba(125, 188, 255, 0.6); }

::selection{
  background:rgba(125, 188, 255, 0.6); }
.bp3-heading{
  color:#182026;
  font-weight:600;
  margin:0 0 10px;
  padding:0; }
  .bp3-dark .bp3-heading{
    color:#f5f8fa; }

h1.bp3-heading, .bp3-running-text h1{
  font-size:36px;
  line-height:40px; }

h2.bp3-heading, .bp3-running-text h2{
  font-size:28px;
  line-height:32px; }

h3.bp3-heading, .bp3-running-text h3{
  font-size:22px;
  line-height:25px; }

h4.bp3-heading, .bp3-running-text h4{
  font-size:18px;
  line-height:21px; }

h5.bp3-heading, .bp3-running-text h5{
  font-size:16px;
  line-height:19px; }

h6.bp3-heading, .bp3-running-text h6{
  font-size:14px;
  line-height:16px; }
.bp3-ui-text{
  font-size:14px;
  font-weight:400;
  letter-spacing:0;
  line-height:1.28581;
  text-transform:none; }

.bp3-monospace-text{
  font-family:monospace;
  text-transform:none; }

.bp3-text-muted{
  color:#5c7080; }
  .bp3-dark .bp3-text-muted{
    color:#a7b6c2; }

.bp3-text-disabled{
  color:rgba(92, 112, 128, 0.6); }
  .bp3-dark .bp3-text-disabled{
    color:rgba(167, 182, 194, 0.6); }

.bp3-text-overflow-ellipsis{
  overflow:hidden;
  text-overflow:ellipsis;
  white-space:nowrap;
  word-wrap:normal; }
.bp3-running-text{
  font-size:14px;
  line-height:1.5; }
  .bp3-running-text h1{
    color:#182026;
    font-weight:600;
    margin-bottom:20px;
    margin-top:40px; }
    .bp3-dark .bp3-running-text h1{
      color:#f5f8fa; }
  .bp3-running-text h2{
    color:#182026;
    font-weight:600;
    margin-bottom:20px;
    margin-top:40px; }
    .bp3-dark .bp3-running-text h2{
      color:#f5f8fa; }
  .bp3-running-text h3{
    color:#182026;
    font-weight:600;
    margin-bottom:20px;
    margin-top:40px; }
    .bp3-dark .bp3-running-text h3{
      color:#f5f8fa; }
  .bp3-running-text h4{
    color:#182026;
    font-weight:600;
    margin-bottom:20px;
    margin-top:40px; }
    .bp3-dark .bp3-running-text h4{
      color:#f5f8fa; }
  .bp3-running-text h5{
    color:#182026;
    font-weight:600;
    margin-bottom:20px;
    margin-top:40px; }
    .bp3-dark .bp3-running-text h5{
      color:#f5f8fa; }
  .bp3-running-text h6{
    color:#182026;
    font-weight:600;
    margin-bottom:20px;
    margin-top:40px; }
    .bp3-dark .bp3-running-text h6{
      color:#f5f8fa; }
  .bp3-running-text hr{
    border:none;
    border-bottom:1px solid rgba(16, 22, 26, 0.15);
    margin:20px 0; }
    .bp3-dark .bp3-running-text hr{
      border-color:rgba(255, 255, 255, 0.15); }
  .bp3-running-text p{
    margin:0 0 10px;
    padding:0; }

.bp3-text-large{
  font-size:16px; }

.bp3-text-small{
  font-size:12px; }
a{
  color:#106ba3;
  text-decoration:none; }
  a:hover{
    color:#106ba3;
    cursor:pointer;
    text-decoration:underline; }
  a .bp3-icon, a .bp3-icon-standard, a .bp3-icon-large{
    color:inherit; }
  a code,
  .bp3-dark a code{
    color:inherit; }
  .bp3-dark a,
  .bp3-dark a:hover{
    color:#48aff0; }
    .bp3-dark a .bp3-icon, .bp3-dark a .bp3-icon-standard, .bp3-dark a .bp3-icon-large,
    .bp3-dark a:hover .bp3-icon,
    .bp3-dark a:hover .bp3-icon-standard,
    .bp3-dark a:hover .bp3-icon-large{
      color:inherit; }
.bp3-running-text code, .bp3-code{
  font-family:monospace;
  text-transform:none;
  background:rgba(255, 255, 255, 0.7);
  border-radius:3px;
  -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2);
          box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2);
  color:#5c7080;
  font-size:smaller;
  padding:2px 5px; }
  .bp3-dark .bp3-running-text code, .bp3-running-text .bp3-dark code, .bp3-dark .bp3-code{
    background:rgba(16, 22, 26, 0.3);
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4);
    color:#a7b6c2; }
  .bp3-running-text a > code, a > .bp3-code{
    color:#137cbd; }
    .bp3-dark .bp3-running-text a > code, .bp3-running-text .bp3-dark a > code, .bp3-dark a > .bp3-code{
      color:inherit; }

.bp3-running-text pre, .bp3-code-block{
  font-family:monospace;
  text-transform:none;
  background:rgba(255, 255, 255, 0.7);
  border-radius:3px;
  -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.15);
          box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.15);
  color:#182026;
  display:block;
  font-size:13px;
  line-height:1.4;
  margin:10px 0;
  padding:13px 15px 12px;
  word-break:break-all;
  word-wrap:break-word; }
  .bp3-dark .bp3-running-text pre, .bp3-running-text .bp3-dark pre, .bp3-dark .bp3-code-block{
    background:rgba(16, 22, 26, 0.3);
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4);
    color:#f5f8fa; }
  .bp3-running-text pre > code, .bp3-code-block > code{
    background:none;
    -webkit-box-shadow:none;
            box-shadow:none;
    color:inherit;
    font-size:inherit;
    padding:0; }

.bp3-running-text kbd, .bp3-key{
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  background:#ffffff;
  border-radius:3px;
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.2);
  color:#5c7080;
  display:-webkit-inline-box;
  display:-ms-inline-flexbox;
  display:inline-flex;
  font-family:inherit;
  font-size:12px;
  height:24px;
  -webkit-box-pack:center;
      -ms-flex-pack:center;
          justify-content:center;
  line-height:24px;
  min-width:24px;
  padding:3px 6px;
  vertical-align:middle; }
  .bp3-running-text kbd .bp3-icon, .bp3-key .bp3-icon, .bp3-running-text kbd .bp3-icon-standard, .bp3-key .bp3-icon-standard, .bp3-running-text kbd .bp3-icon-large, .bp3-key .bp3-icon-large{
    margin-right:5px; }
  .bp3-dark .bp3-running-text kbd, .bp3-running-text .bp3-dark kbd, .bp3-dark .bp3-key{
    background:#394b59;
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.4);
    color:#a7b6c2; }
.bp3-running-text blockquote, .bp3-blockquote{
  border-left:solid 4px rgba(167, 182, 194, 0.5);
  margin:0 0 10px;
  padding:0 20px; }
  .bp3-dark .bp3-running-text blockquote, .bp3-running-text .bp3-dark blockquote, .bp3-dark .bp3-blockquote{
    border-color:rgba(115, 134, 148, 0.5); }
.bp3-running-text ul,
.bp3-running-text ol, .bp3-list{
  margin:10px 0;
  padding-left:30px; }
  .bp3-running-text ul li:not(:last-child), .bp3-running-text ol li:not(:last-child), .bp3-list li:not(:last-child){
    margin-bottom:5px; }
  .bp3-running-text ul ol, .bp3-running-text ol ol, .bp3-list ol,
  .bp3-running-text ul ul,
  .bp3-running-text ol ul,
  .bp3-list ul{
    margin-top:5px; }

.bp3-list-unstyled{
  list-style:none;
  margin:0;
  padding:0; }
  .bp3-list-unstyled li{
    padding:0; }
.bp3-rtl{
  text-align:right; }

.bp3-dark{
  color:#f5f8fa; }

:focus{
  outline:rgba(19, 124, 189, 0.6) auto 2px;
  outline-offset:2px;
  -moz-outline-radius:6px; }

.bp3-focus-disabled :focus{
  outline:none !important; }
  .bp3-focus-disabled :focus ~ .bp3-control-indicator{
    outline:none !important; }

.bp3-alert{
  max-width:400px;
  padding:20px; }

.bp3-alert-body{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex; }
  .bp3-alert-body .bp3-icon{
    font-size:40px;
    margin-right:20px;
    margin-top:0; }

.bp3-alert-contents{
  word-break:break-word; }

.bp3-alert-footer{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-orient:horizontal;
  -webkit-box-direction:reverse;
      -ms-flex-direction:row-reverse;
          flex-direction:row-reverse;
  margin-top:10px; }
  .bp3-alert-footer .bp3-button{
    margin-left:10px; }
.bp3-breadcrumbs{
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  cursor:default;
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -ms-flex-wrap:wrap;
      flex-wrap:wrap;
  height:30px;
  list-style:none;
  margin:0;
  padding:0; }
  .bp3-breadcrumbs > li{
    -webkit-box-align:center;
        -ms-flex-align:center;
            align-items:center;
    display:-webkit-box;
    display:-ms-flexbox;
    display:flex; }
    .bp3-breadcrumbs > li::after{
      background:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16'%3e%3cpath fill-rule='evenodd' clip-rule='evenodd' d='M10.71 7.29l-4-4a1.003 1.003 0 00-1.42 1.42L8.59 8 5.3 11.29c-.19.18-.3.43-.3.71a1.003 1.003 0 001.71.71l4-4c.18-.18.29-.43.29-.71 0-.28-.11-.53-.29-.71z' fill='%235C7080'/%3e%3c/svg%3e");
      content:"";
      display:block;
      height:16px;
      margin:0 5px;
      width:16px; }
    .bp3-breadcrumbs > li:last-of-type::after{
      display:none; }

.bp3-breadcrumb,
.bp3-breadcrumb-current,
.bp3-breadcrumbs-collapsed{
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  display:-webkit-inline-box;
  display:-ms-inline-flexbox;
  display:inline-flex;
  font-size:16px; }

.bp3-breadcrumb,
.bp3-breadcrumbs-collapsed{
  color:#5c7080; }

.bp3-breadcrumb:hover{
  text-decoration:none; }

.bp3-breadcrumb.bp3-disabled{
  color:rgba(92, 112, 128, 0.6);
  cursor:not-allowed; }

.bp3-breadcrumb .bp3-icon{
  margin-right:5px; }

.bp3-breadcrumb-current{
  color:inherit;
  font-weight:600; }
  .bp3-breadcrumb-current .bp3-input{
    font-size:inherit;
    font-weight:inherit;
    vertical-align:baseline; }

.bp3-breadcrumbs-collapsed{
  background:#ced9e0;
  border:none;
  border-radius:3px;
  cursor:pointer;
  margin-right:2px;
  padding:1px 5px;
  vertical-align:text-bottom; }
  .bp3-breadcrumbs-collapsed::before{
    background:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16'%3e%3cg fill='%235C7080'%3e%3ccircle cx='2' cy='8.03' r='2'/%3e%3ccircle cx='14' cy='8.03' r='2'/%3e%3ccircle cx='8' cy='8.03' r='2'/%3e%3c/g%3e%3c/svg%3e") center no-repeat;
    content:"";
    display:block;
    height:16px;
    width:16px; }
  .bp3-breadcrumbs-collapsed:hover{
    background:#bfccd6;
    color:#182026;
    text-decoration:none; }

.bp3-dark .bp3-breadcrumb,
.bp3-dark .bp3-breadcrumbs-collapsed{
  color:#a7b6c2; }

.bp3-dark .bp3-breadcrumbs > li::after{
  color:#a7b6c2; }

.bp3-dark .bp3-breadcrumb.bp3-disabled{
  color:rgba(167, 182, 194, 0.6); }

.bp3-dark .bp3-breadcrumb-current{
  color:#f5f8fa; }

.bp3-dark .bp3-breadcrumbs-collapsed{
  background:rgba(16, 22, 26, 0.4); }
  .bp3-dark .bp3-breadcrumbs-collapsed:hover{
    background:rgba(16, 22, 26, 0.6);
    color:#f5f8fa; }
.bp3-button{
  display:-webkit-inline-box;
  display:-ms-inline-flexbox;
  display:inline-flex;
  -webkit-box-orient:horizontal;
  -webkit-box-direction:normal;
      -ms-flex-direction:row;
          flex-direction:row;
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  border:none;
  border-radius:3px;
  cursor:pointer;
  font-size:14px;
  -webkit-box-pack:center;
      -ms-flex-pack:center;
          justify-content:center;
  padding:5px 10px;
  text-align:left;
  vertical-align:middle;
  min-height:30px;
  min-width:30px; }
  .bp3-button > *{
    -webkit-box-flex:0;
        -ms-flex-positive:0;
            flex-grow:0;
    -ms-flex-negative:0;
        flex-shrink:0; }
  .bp3-button > .bp3-fill{
    -webkit-box-flex:1;
        -ms-flex-positive:1;
            flex-grow:1;
    -ms-flex-negative:1;
        flex-shrink:1; }
  .bp3-button::before,
  .bp3-button > *{
    margin-right:7px; }
  .bp3-button:empty::before,
  .bp3-button > :last-child{
    margin-right:0; }
  .bp3-button:empty{
    padding:0 !important; }
  .bp3-button:disabled, .bp3-button.bp3-disabled{
    cursor:not-allowed; }
  .bp3-button.bp3-fill{
    display:-webkit-box;
    display:-ms-flexbox;
    display:flex;
    width:100%; }
  .bp3-button.bp3-align-right,
  .bp3-align-right .bp3-button{
    text-align:right; }
  .bp3-button.bp3-align-left,
  .bp3-align-left .bp3-button{
    text-align:left; }
  .bp3-button:not([class*="bp3-intent-"]){
    background-color:#f5f8fa;
    background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.8)), to(rgba(255, 255, 255, 0)));
    background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.8), rgba(255, 255, 255, 0));
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
    color:#182026; }
    .bp3-button:not([class*="bp3-intent-"]):hover{
      background-clip:padding-box;
      background-color:#ebf1f5;
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1); }
    .bp3-button:not([class*="bp3-intent-"]):active, .bp3-button:not([class*="bp3-intent-"]).bp3-active{
      background-color:#d8e1e8;
      background-image:none;
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
    .bp3-button:not([class*="bp3-intent-"]):disabled, .bp3-button:not([class*="bp3-intent-"]).bp3-disabled{
      background-color:rgba(206, 217, 224, 0.5);
      background-image:none;
      -webkit-box-shadow:none;
              box-shadow:none;
      color:rgba(92, 112, 128, 0.6);
      cursor:not-allowed;
      outline:none; }
      .bp3-button:not([class*="bp3-intent-"]):disabled.bp3-active, .bp3-button:not([class*="bp3-intent-"]):disabled.bp3-active:hover, .bp3-button:not([class*="bp3-intent-"]).bp3-disabled.bp3-active, .bp3-button:not([class*="bp3-intent-"]).bp3-disabled.bp3-active:hover{
        background:rgba(206, 217, 224, 0.7); }
  .bp3-button.bp3-intent-primary{
    background-color:#137cbd;
    background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.1)), to(rgba(255, 255, 255, 0)));
    background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.1), rgba(255, 255, 255, 0));
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
    color:#ffffff; }
    .bp3-button.bp3-intent-primary:hover, .bp3-button.bp3-intent-primary:active, .bp3-button.bp3-intent-primary.bp3-active{
      color:#ffffff; }
    .bp3-button.bp3-intent-primary:hover{
      background-color:#106ba3;
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2); }
    .bp3-button.bp3-intent-primary:active, .bp3-button.bp3-intent-primary.bp3-active{
      background-color:#0e5a8a;
      background-image:none;
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
    .bp3-button.bp3-intent-primary:disabled, .bp3-button.bp3-intent-primary.bp3-disabled{
      background-color:rgba(19, 124, 189, 0.5);
      background-image:none;
      border-color:transparent;
      -webkit-box-shadow:none;
              box-shadow:none;
      color:rgba(255, 255, 255, 0.6); }
  .bp3-button.bp3-intent-success{
    background-color:#0f9960;
    background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.1)), to(rgba(255, 255, 255, 0)));
    background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.1), rgba(255, 255, 255, 0));
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
    color:#ffffff; }
    .bp3-button.bp3-intent-success:hover, .bp3-button.bp3-intent-success:active, .bp3-button.bp3-intent-success.bp3-active{
      color:#ffffff; }
    .bp3-button.bp3-intent-success:hover{
      background-color:#0d8050;
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2); }
    .bp3-button.bp3-intent-success:active, .bp3-button.bp3-intent-success.bp3-active{
      background-color:#0a6640;
      background-image:none;
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
    .bp3-button.bp3-intent-success:disabled, .bp3-button.bp3-intent-success.bp3-disabled{
      background-color:rgba(15, 153, 96, 0.5);
      background-image:none;
      border-color:transparent;
      -webkit-box-shadow:none;
              box-shadow:none;
      color:rgba(255, 255, 255, 0.6); }
  .bp3-button.bp3-intent-warning{
    background-color:#d9822b;
    background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.1)), to(rgba(255, 255, 255, 0)));
    background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.1), rgba(255, 255, 255, 0));
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
    color:#ffffff; }
    .bp3-button.bp3-intent-warning:hover, .bp3-button.bp3-intent-warning:active, .bp3-button.bp3-intent-warning.bp3-active{
      color:#ffffff; }
    .bp3-button.bp3-intent-warning:hover{
      background-color:#bf7326;
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2); }
    .bp3-button.bp3-intent-warning:active, .bp3-button.bp3-intent-warning.bp3-active{
      background-color:#a66321;
      background-image:none;
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
    .bp3-button.bp3-intent-warning:disabled, .bp3-button.bp3-intent-warning.bp3-disabled{
      background-color:rgba(217, 130, 43, 0.5);
      background-image:none;
      border-color:transparent;
      -webkit-box-shadow:none;
              box-shadow:none;
      color:rgba(255, 255, 255, 0.6); }
  .bp3-button.bp3-intent-danger{
    background-color:#db3737;
    background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.1)), to(rgba(255, 255, 255, 0)));
    background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.1), rgba(255, 255, 255, 0));
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
    color:#ffffff; }
    .bp3-button.bp3-intent-danger:hover, .bp3-button.bp3-intent-danger:active, .bp3-button.bp3-intent-danger.bp3-active{
      color:#ffffff; }
    .bp3-button.bp3-intent-danger:hover{
      background-color:#c23030;
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2); }
    .bp3-button.bp3-intent-danger:active, .bp3-button.bp3-intent-danger.bp3-active{
      background-color:#a82a2a;
      background-image:none;
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
    .bp3-button.bp3-intent-danger:disabled, .bp3-button.bp3-intent-danger.bp3-disabled{
      background-color:rgba(219, 55, 55, 0.5);
      background-image:none;
      border-color:transparent;
      -webkit-box-shadow:none;
              box-shadow:none;
      color:rgba(255, 255, 255, 0.6); }
  .bp3-button[class*="bp3-intent-"] .bp3-button-spinner .bp3-spinner-head{
    stroke:#ffffff; }
  .bp3-button.bp3-large,
  .bp3-large .bp3-button{
    min-height:40px;
    min-width:40px;
    font-size:16px;
    padding:5px 15px; }
    .bp3-button.bp3-large::before,
    .bp3-button.bp3-large > *,
    .bp3-large .bp3-button::before,
    .bp3-large .bp3-button > *{
      margin-right:10px; }
    .bp3-button.bp3-large:empty::before,
    .bp3-button.bp3-large > :last-child,
    .bp3-large .bp3-button:empty::before,
    .bp3-large .bp3-button > :last-child{
      margin-right:0; }
  .bp3-button.bp3-small,
  .bp3-small .bp3-button{
    min-height:24px;
    min-width:24px;
    padding:0 7px; }
  .bp3-button.bp3-loading{
    position:relative; }
    .bp3-button.bp3-loading[class*="bp3-icon-"]::before{
      visibility:hidden; }
    .bp3-button.bp3-loading .bp3-button-spinner{
      margin:0;
      position:absolute; }
    .bp3-button.bp3-loading > :not(.bp3-button-spinner){
      visibility:hidden; }
  .bp3-button[class*="bp3-icon-"]::before{
    font-family:"Icons16", sans-serif;
    font-size:16px;
    font-style:normal;
    font-weight:400;
    line-height:1;
    -moz-osx-font-smoothing:grayscale;
    -webkit-font-smoothing:antialiased;
    color:#5c7080; }
  .bp3-button .bp3-icon, .bp3-button .bp3-icon-standard, .bp3-button .bp3-icon-large{
    color:#5c7080; }
    .bp3-button .bp3-icon.bp3-align-right, .bp3-button .bp3-icon-standard.bp3-align-right, .bp3-button .bp3-icon-large.bp3-align-right{
      margin-left:7px; }
  .bp3-button .bp3-icon:first-child:last-child,
  .bp3-button .bp3-spinner + .bp3-icon:last-child{
    margin:0 -7px; }
  .bp3-dark .bp3-button:not([class*="bp3-intent-"]){
    background-color:#394b59;
    background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.05)), to(rgba(255, 255, 255, 0)));
    background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.05), rgba(255, 255, 255, 0));
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
    color:#f5f8fa; }
    .bp3-dark .bp3-button:not([class*="bp3-intent-"]):hover, .bp3-dark .bp3-button:not([class*="bp3-intent-"]):active, .bp3-dark .bp3-button:not([class*="bp3-intent-"]).bp3-active{
      color:#f5f8fa; }
    .bp3-dark .bp3-button:not([class*="bp3-intent-"]):hover{
      background-color:#30404d;
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-button:not([class*="bp3-intent-"]):active, .bp3-dark .bp3-button:not([class*="bp3-intent-"]).bp3-active{
      background-color:#202b33;
      background-image:none;
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
    .bp3-dark .bp3-button:not([class*="bp3-intent-"]):disabled, .bp3-dark .bp3-button:not([class*="bp3-intent-"]).bp3-disabled{
      background-color:rgba(57, 75, 89, 0.5);
      background-image:none;
      -webkit-box-shadow:none;
              box-shadow:none;
      color:rgba(167, 182, 194, 0.6); }
      .bp3-dark .bp3-button:not([class*="bp3-intent-"]):disabled.bp3-active, .bp3-dark .bp3-button:not([class*="bp3-intent-"]).bp3-disabled.bp3-active{
        background:rgba(57, 75, 89, 0.7); }
    .bp3-dark .bp3-button:not([class*="bp3-intent-"]) .bp3-button-spinner .bp3-spinner-head{
      background:rgba(16, 22, 26, 0.5);
      stroke:#8a9ba8; }
    .bp3-dark .bp3-button:not([class*="bp3-intent-"])[class*="bp3-icon-"]::before{
      color:#a7b6c2; }
    .bp3-dark .bp3-button:not([class*="bp3-intent-"]) .bp3-icon, .bp3-dark .bp3-button:not([class*="bp3-intent-"]) .bp3-icon-standard, .bp3-dark .bp3-button:not([class*="bp3-intent-"]) .bp3-icon-large{
      color:#a7b6c2; }
  .bp3-dark .bp3-button[class*="bp3-intent-"]{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-button[class*="bp3-intent-"]:hover{
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-button[class*="bp3-intent-"]:active, .bp3-dark .bp3-button[class*="bp3-intent-"].bp3-active{
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
    .bp3-dark .bp3-button[class*="bp3-intent-"]:disabled, .bp3-dark .bp3-button[class*="bp3-intent-"].bp3-disabled{
      background-image:none;
      -webkit-box-shadow:none;
              box-shadow:none;
      color:rgba(255, 255, 255, 0.3); }
    .bp3-dark .bp3-button[class*="bp3-intent-"] .bp3-button-spinner .bp3-spinner-head{
      stroke:#8a9ba8; }
  .bp3-button:disabled::before,
  .bp3-button:disabled .bp3-icon, .bp3-button:disabled .bp3-icon-standard, .bp3-button:disabled .bp3-icon-large, .bp3-button.bp3-disabled::before,
  .bp3-button.bp3-disabled .bp3-icon, .bp3-button.bp3-disabled .bp3-icon-standard, .bp3-button.bp3-disabled .bp3-icon-large, .bp3-button[class*="bp3-intent-"]::before,
  .bp3-button[class*="bp3-intent-"] .bp3-icon, .bp3-button[class*="bp3-intent-"] .bp3-icon-standard, .bp3-button[class*="bp3-intent-"] .bp3-icon-large{
    color:inherit !important; }
  .bp3-button.bp3-minimal{
    background:none;
    -webkit-box-shadow:none;
            box-shadow:none; }
    .bp3-button.bp3-minimal:hover{
      background:rgba(167, 182, 194, 0.3);
      -webkit-box-shadow:none;
              box-shadow:none;
      color:#182026;
      text-decoration:none; }
    .bp3-button.bp3-minimal:active, .bp3-button.bp3-minimal.bp3-active{
      background:rgba(115, 134, 148, 0.3);
      -webkit-box-shadow:none;
              box-shadow:none;
      color:#182026; }
    .bp3-button.bp3-minimal:disabled, .bp3-button.bp3-minimal:disabled:hover, .bp3-button.bp3-minimal.bp3-disabled, .bp3-button.bp3-minimal.bp3-disabled:hover{
      background:none;
      color:rgba(92, 112, 128, 0.6);
      cursor:not-allowed; }
      .bp3-button.bp3-minimal:disabled.bp3-active, .bp3-button.bp3-minimal:disabled:hover.bp3-active, .bp3-button.bp3-minimal.bp3-disabled.bp3-active, .bp3-button.bp3-minimal.bp3-disabled:hover.bp3-active{
        background:rgba(115, 134, 148, 0.3); }
    .bp3-dark .bp3-button.bp3-minimal{
      background:none;
      -webkit-box-shadow:none;
              box-shadow:none;
      color:inherit; }
      .bp3-dark .bp3-button.bp3-minimal:hover, .bp3-dark .bp3-button.bp3-minimal:active, .bp3-dark .bp3-button.bp3-minimal.bp3-active{
        background:none;
        -webkit-box-shadow:none;
                box-shadow:none; }
      .bp3-dark .bp3-button.bp3-minimal:hover{
        background:rgba(138, 155, 168, 0.15); }
      .bp3-dark .bp3-button.bp3-minimal:active, .bp3-dark .bp3-button.bp3-minimal.bp3-active{
        background:rgba(138, 155, 168, 0.3);
        color:#f5f8fa; }
      .bp3-dark .bp3-button.bp3-minimal:disabled, .bp3-dark .bp3-button.bp3-minimal:disabled:hover, .bp3-dark .bp3-button.bp3-minimal.bp3-disabled, .bp3-dark .bp3-button.bp3-minimal.bp3-disabled:hover{
        background:none;
        color:rgba(167, 182, 194, 0.6);
        cursor:not-allowed; }
        .bp3-dark .bp3-button.bp3-minimal:disabled.bp3-active, .bp3-dark .bp3-button.bp3-minimal:disabled:hover.bp3-active, .bp3-dark .bp3-button.bp3-minimal.bp3-disabled.bp3-active, .bp3-dark .bp3-button.bp3-minimal.bp3-disabled:hover.bp3-active{
          background:rgba(138, 155, 168, 0.3); }
    .bp3-button.bp3-minimal.bp3-intent-primary{
      color:#106ba3; }
      .bp3-button.bp3-minimal.bp3-intent-primary:hover, .bp3-button.bp3-minimal.bp3-intent-primary:active, .bp3-button.bp3-minimal.bp3-intent-primary.bp3-active{
        background:none;
        -webkit-box-shadow:none;
                box-shadow:none;
        color:#106ba3; }
      .bp3-button.bp3-minimal.bp3-intent-primary:hover{
        background:rgba(19, 124, 189, 0.15);
        color:#106ba3; }
      .bp3-button.bp3-minimal.bp3-intent-primary:active, .bp3-button.bp3-minimal.bp3-intent-primary.bp3-active{
        background:rgba(19, 124, 189, 0.3);
        color:#106ba3; }
      .bp3-button.bp3-minimal.bp3-intent-primary:disabled, .bp3-button.bp3-minimal.bp3-intent-primary.bp3-disabled{
        background:none;
        color:rgba(16, 107, 163, 0.5); }
        .bp3-button.bp3-minimal.bp3-intent-primary:disabled.bp3-active, .bp3-button.bp3-minimal.bp3-intent-primary.bp3-disabled.bp3-active{
          background:rgba(19, 124, 189, 0.3); }
      .bp3-button.bp3-minimal.bp3-intent-primary .bp3-button-spinner .bp3-spinner-head{
        stroke:#106ba3; }
      .bp3-dark .bp3-button.bp3-minimal.bp3-intent-primary{
        color:#48aff0; }
        .bp3-dark .bp3-button.bp3-minimal.bp3-intent-primary:hover{
          background:rgba(19, 124, 189, 0.2);
          color:#48aff0; }
        .bp3-dark .bp3-button.bp3-minimal.bp3-intent-primary:active, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-primary.bp3-active{
          background:rgba(19, 124, 189, 0.3);
          color:#48aff0; }
        .bp3-dark .bp3-button.bp3-minimal.bp3-intent-primary:disabled, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-primary.bp3-disabled{
          background:none;
          color:rgba(72, 175, 240, 0.5); }
          .bp3-dark .bp3-button.bp3-minimal.bp3-intent-primary:disabled.bp3-active, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-primary.bp3-disabled.bp3-active{
            background:rgba(19, 124, 189, 0.3); }
    .bp3-button.bp3-minimal.bp3-intent-success{
      color:#0d8050; }
      .bp3-button.bp3-minimal.bp3-intent-success:hover, .bp3-button.bp3-minimal.bp3-intent-success:active, .bp3-button.bp3-minimal.bp3-intent-success.bp3-active{
        background:none;
        -webkit-box-shadow:none;
                box-shadow:none;
        color:#0d8050; }
      .bp3-button.bp3-minimal.bp3-intent-success:hover{
        background:rgba(15, 153, 96, 0.15);
        color:#0d8050; }
      .bp3-button.bp3-minimal.bp3-intent-success:active, .bp3-button.bp3-minimal.bp3-intent-success.bp3-active{
        background:rgba(15, 153, 96, 0.3);
        color:#0d8050; }
      .bp3-button.bp3-minimal.bp3-intent-success:disabled, .bp3-button.bp3-minimal.bp3-intent-success.bp3-disabled{
        background:none;
        color:rgba(13, 128, 80, 0.5); }
        .bp3-button.bp3-minimal.bp3-intent-success:disabled.bp3-active, .bp3-button.bp3-minimal.bp3-intent-success.bp3-disabled.bp3-active{
          background:rgba(15, 153, 96, 0.3); }
      .bp3-button.bp3-minimal.bp3-intent-success .bp3-button-spinner .bp3-spinner-head{
        stroke:#0d8050; }
      .bp3-dark .bp3-button.bp3-minimal.bp3-intent-success{
        color:#3dcc91; }
        .bp3-dark .bp3-button.bp3-minimal.bp3-intent-success:hover{
          background:rgba(15, 153, 96, 0.2);
          color:#3dcc91; }
        .bp3-dark .bp3-button.bp3-minimal.bp3-intent-success:active, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-success.bp3-active{
          background:rgba(15, 153, 96, 0.3);
          color:#3dcc91; }
        .bp3-dark .bp3-button.bp3-minimal.bp3-intent-success:disabled, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-success.bp3-disabled{
          background:none;
          color:rgba(61, 204, 145, 0.5); }
          .bp3-dark .bp3-button.bp3-minimal.bp3-intent-success:disabled.bp3-active, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-success.bp3-disabled.bp3-active{
            background:rgba(15, 153, 96, 0.3); }
    .bp3-button.bp3-minimal.bp3-intent-warning{
      color:#bf7326; }
      .bp3-button.bp3-minimal.bp3-intent-warning:hover, .bp3-button.bp3-minimal.bp3-intent-warning:active, .bp3-button.bp3-minimal.bp3-intent-warning.bp3-active{
        background:none;
        -webkit-box-shadow:none;
                box-shadow:none;
        color:#bf7326; }
      .bp3-button.bp3-minimal.bp3-intent-warning:hover{
        background:rgba(217, 130, 43, 0.15);
        color:#bf7326; }
      .bp3-button.bp3-minimal.bp3-intent-warning:active, .bp3-button.bp3-minimal.bp3-intent-warning.bp3-active{
        background:rgba(217, 130, 43, 0.3);
        color:#bf7326; }
      .bp3-button.bp3-minimal.bp3-intent-warning:disabled, .bp3-button.bp3-minimal.bp3-intent-warning.bp3-disabled{
        background:none;
        color:rgba(191, 115, 38, 0.5); }
        .bp3-button.bp3-minimal.bp3-intent-warning:disabled.bp3-active, .bp3-button.bp3-minimal.bp3-intent-warning.bp3-disabled.bp3-active{
          background:rgba(217, 130, 43, 0.3); }
      .bp3-button.bp3-minimal.bp3-intent-warning .bp3-button-spinner .bp3-spinner-head{
        stroke:#bf7326; }
      .bp3-dark .bp3-button.bp3-minimal.bp3-intent-warning{
        color:#ffb366; }
        .bp3-dark .bp3-button.bp3-minimal.bp3-intent-warning:hover{
          background:rgba(217, 130, 43, 0.2);
          color:#ffb366; }
        .bp3-dark .bp3-button.bp3-minimal.bp3-intent-warning:active, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-warning.bp3-active{
          background:rgba(217, 130, 43, 0.3);
          color:#ffb366; }
        .bp3-dark .bp3-button.bp3-minimal.bp3-intent-warning:disabled, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-warning.bp3-disabled{
          background:none;
          color:rgba(255, 179, 102, 0.5); }
          .bp3-dark .bp3-button.bp3-minimal.bp3-intent-warning:disabled.bp3-active, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-warning.bp3-disabled.bp3-active{
            background:rgba(217, 130, 43, 0.3); }
    .bp3-button.bp3-minimal.bp3-intent-danger{
      color:#c23030; }
      .bp3-button.bp3-minimal.bp3-intent-danger:hover, .bp3-button.bp3-minimal.bp3-intent-danger:active, .bp3-button.bp3-minimal.bp3-intent-danger.bp3-active{
        background:none;
        -webkit-box-shadow:none;
                box-shadow:none;
        color:#c23030; }
      .bp3-button.bp3-minimal.bp3-intent-danger:hover{
        background:rgba(219, 55, 55, 0.15);
        color:#c23030; }
      .bp3-button.bp3-minimal.bp3-intent-danger:active, .bp3-button.bp3-minimal.bp3-intent-danger.bp3-active{
        background:rgba(219, 55, 55, 0.3);
        color:#c23030; }
      .bp3-button.bp3-minimal.bp3-intent-danger:disabled, .bp3-button.bp3-minimal.bp3-intent-danger.bp3-disabled{
        background:none;
        color:rgba(194, 48, 48, 0.5); }
        .bp3-button.bp3-minimal.bp3-intent-danger:disabled.bp3-active, .bp3-button.bp3-minimal.bp3-intent-danger.bp3-disabled.bp3-active{
          background:rgba(219, 55, 55, 0.3); }
      .bp3-button.bp3-minimal.bp3-intent-danger .bp3-button-spinner .bp3-spinner-head{
        stroke:#c23030; }
      .bp3-dark .bp3-button.bp3-minimal.bp3-intent-danger{
        color:#ff7373; }
        .bp3-dark .bp3-button.bp3-minimal.bp3-intent-danger:hover{
          background:rgba(219, 55, 55, 0.2);
          color:#ff7373; }
        .bp3-dark .bp3-button.bp3-minimal.bp3-intent-danger:active, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-danger.bp3-active{
          background:rgba(219, 55, 55, 0.3);
          color:#ff7373; }
        .bp3-dark .bp3-button.bp3-minimal.bp3-intent-danger:disabled, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-danger.bp3-disabled{
          background:none;
          color:rgba(255, 115, 115, 0.5); }
          .bp3-dark .bp3-button.bp3-minimal.bp3-intent-danger:disabled.bp3-active, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-danger.bp3-disabled.bp3-active{
            background:rgba(219, 55, 55, 0.3); }
  .bp3-button.bp3-outlined{
    background:none;
    -webkit-box-shadow:none;
            box-shadow:none;
    border:1px solid rgba(24, 32, 38, 0.2);
    -webkit-box-sizing:border-box;
            box-sizing:border-box; }
    .bp3-button.bp3-outlined:hover{
      background:rgba(167, 182, 194, 0.3);
      -webkit-box-shadow:none;
              box-shadow:none;
      color:#182026;
      text-decoration:none; }
    .bp3-button.bp3-outlined:active, .bp3-button.bp3-outlined.bp3-active{
      background:rgba(115, 134, 148, 0.3);
      -webkit-box-shadow:none;
              box-shadow:none;
      color:#182026; }
    .bp3-button.bp3-outlined:disabled, .bp3-button.bp3-outlined:disabled:hover, .bp3-button.bp3-outlined.bp3-disabled, .bp3-button.bp3-outlined.bp3-disabled:hover{
      background:none;
      color:rgba(92, 112, 128, 0.6);
      cursor:not-allowed; }
      .bp3-button.bp3-outlined:disabled.bp3-active, .bp3-button.bp3-outlined:disabled:hover.bp3-active, .bp3-button.bp3-outlined.bp3-disabled.bp3-active, .bp3-button.bp3-outlined.bp3-disabled:hover.bp3-active{
        background:rgba(115, 134, 148, 0.3); }
    .bp3-dark .bp3-button.bp3-outlined{
      background:none;
      -webkit-box-shadow:none;
              box-shadow:none;
      color:inherit; }
      .bp3-dark .bp3-button.bp3-outlined:hover, .bp3-dark .bp3-button.bp3-outlined:active, .bp3-dark .bp3-button.bp3-outlined.bp3-active{
        background:none;
        -webkit-box-shadow:none;
                box-shadow:none; }
      .bp3-dark .bp3-button.bp3-outlined:hover{
        background:rgba(138, 155, 168, 0.15); }
      .bp3-dark .bp3-button.bp3-outlined:active, .bp3-dark .bp3-button.bp3-outlined.bp3-active{
        background:rgba(138, 155, 168, 0.3);
        color:#f5f8fa; }
      .bp3-dark .bp3-button.bp3-outlined:disabled, .bp3-dark .bp3-button.bp3-outlined:disabled:hover, .bp3-dark .bp3-button.bp3-outlined.bp3-disabled, .bp3-dark .bp3-button.bp3-outlined.bp3-disabled:hover{
        background:none;
        color:rgba(167, 182, 194, 0.6);
        cursor:not-allowed; }
        .bp3-dark .bp3-button.bp3-outlined:disabled.bp3-active, .bp3-dark .bp3-button.bp3-outlined:disabled:hover.bp3-active, .bp3-dark .bp3-button.bp3-outlined.bp3-disabled.bp3-active, .bp3-dark .bp3-button.bp3-outlined.bp3-disabled:hover.bp3-active{
          background:rgba(138, 155, 168, 0.3); }
    .bp3-button.bp3-outlined.bp3-intent-primary{
      color:#106ba3; }
      .bp3-button.bp3-outlined.bp3-intent-primary:hover, .bp3-button.bp3-outlined.bp3-intent-primary:active, .bp3-button.bp3-outlined.bp3-intent-primary.bp3-active{
        background:none;
        -webkit-box-shadow:none;
                box-shadow:none;
        color:#106ba3; }
      .bp3-button.bp3-outlined.bp3-intent-primary:hover{
        background:rgba(19, 124, 189, 0.15);
        color:#106ba3; }
      .bp3-button.bp3-outlined.bp3-intent-primary:active, .bp3-button.bp3-outlined.bp3-intent-primary.bp3-active{
        background:rgba(19, 124, 189, 0.3);
        color:#106ba3; }
      .bp3-button.bp3-outlined.bp3-intent-primary:disabled, .bp3-button.bp3-outlined.bp3-intent-primary.bp3-disabled{
        background:none;
        color:rgba(16, 107, 163, 0.5); }
        .bp3-button.bp3-outlined.bp3-intent-primary:disabled.bp3-active, .bp3-button.bp3-outlined.bp3-intent-primary.bp3-disabled.bp3-active{
          background:rgba(19, 124, 189, 0.3); }
      .bp3-button.bp3-outlined.bp3-intent-primary .bp3-button-spinner .bp3-spinner-head{
        stroke:#106ba3; }
      .bp3-dark .bp3-button.bp3-outlined.bp3-intent-primary{
        color:#48aff0; }
        .bp3-dark .bp3-button.bp3-outlined.bp3-intent-primary:hover{
          background:rgba(19, 124, 189, 0.2);
          color:#48aff0; }
        .bp3-dark .bp3-button.bp3-outlined.bp3-intent-primary:active, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-primary.bp3-active{
          background:rgba(19, 124, 189, 0.3);
          color:#48aff0; }
        .bp3-dark .bp3-button.bp3-outlined.bp3-intent-primary:disabled, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-primary.bp3-disabled{
          background:none;
          color:rgba(72, 175, 240, 0.5); }
          .bp3-dark .bp3-button.bp3-outlined.bp3-intent-primary:disabled.bp3-active, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-primary.bp3-disabled.bp3-active{
            background:rgba(19, 124, 189, 0.3); }
    .bp3-button.bp3-outlined.bp3-intent-success{
      color:#0d8050; }
      .bp3-button.bp3-outlined.bp3-intent-success:hover, .bp3-button.bp3-outlined.bp3-intent-success:active, .bp3-button.bp3-outlined.bp3-intent-success.bp3-active{
        background:none;
        -webkit-box-shadow:none;
                box-shadow:none;
        color:#0d8050; }
      .bp3-button.bp3-outlined.bp3-intent-success:hover{
        background:rgba(15, 153, 96, 0.15);
        color:#0d8050; }
      .bp3-button.bp3-outlined.bp3-intent-success:active, .bp3-button.bp3-outlined.bp3-intent-success.bp3-active{
        background:rgba(15, 153, 96, 0.3);
        color:#0d8050; }
      .bp3-button.bp3-outlined.bp3-intent-success:disabled, .bp3-button.bp3-outlined.bp3-intent-success.bp3-disabled{
        background:none;
        color:rgba(13, 128, 80, 0.5); }
        .bp3-button.bp3-outlined.bp3-intent-success:disabled.bp3-active, .bp3-button.bp3-outlined.bp3-intent-success.bp3-disabled.bp3-active{
          background:rgba(15, 153, 96, 0.3); }
      .bp3-button.bp3-outlined.bp3-intent-success .bp3-button-spinner .bp3-spinner-head{
        stroke:#0d8050; }
      .bp3-dark .bp3-button.bp3-outlined.bp3-intent-success{
        color:#3dcc91; }
        .bp3-dark .bp3-button.bp3-outlined.bp3-intent-success:hover{
          background:rgba(15, 153, 96, 0.2);
          color:#3dcc91; }
        .bp3-dark .bp3-button.bp3-outlined.bp3-intent-success:active, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-success.bp3-active{
          background:rgba(15, 153, 96, 0.3);
          color:#3dcc91; }
        .bp3-dark .bp3-button.bp3-outlined.bp3-intent-success:disabled, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-success.bp3-disabled{
          background:none;
          color:rgba(61, 204, 145, 0.5); }
          .bp3-dark .bp3-button.bp3-outlined.bp3-intent-success:disabled.bp3-active, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-success.bp3-disabled.bp3-active{
            background:rgba(15, 153, 96, 0.3); }
    .bp3-button.bp3-outlined.bp3-intent-warning{
      color:#bf7326; }
      .bp3-button.bp3-outlined.bp3-intent-warning:hover, .bp3-button.bp3-outlined.bp3-intent-warning:active, .bp3-button.bp3-outlined.bp3-intent-warning.bp3-active{
        background:none;
        -webkit-box-shadow:none;
                box-shadow:none;
        color:#bf7326; }
      .bp3-button.bp3-outlined.bp3-intent-warning:hover{
        background:rgba(217, 130, 43, 0.15);
        color:#bf7326; }
      .bp3-button.bp3-outlined.bp3-intent-warning:active, .bp3-button.bp3-outlined.bp3-intent-warning.bp3-active{
        background:rgba(217, 130, 43, 0.3);
        color:#bf7326; }
      .bp3-button.bp3-outlined.bp3-intent-warning:disabled, .bp3-button.bp3-outlined.bp3-intent-warning.bp3-disabled{
        background:none;
        color:rgba(191, 115, 38, 0.5); }
        .bp3-button.bp3-outlined.bp3-intent-warning:disabled.bp3-active, .bp3-button.bp3-outlined.bp3-intent-warning.bp3-disabled.bp3-active{
          background:rgba(217, 130, 43, 0.3); }
      .bp3-button.bp3-outlined.bp3-intent-warning .bp3-button-spinner .bp3-spinner-head{
        stroke:#bf7326; }
      .bp3-dark .bp3-button.bp3-outlined.bp3-intent-warning{
        color:#ffb366; }
        .bp3-dark .bp3-button.bp3-outlined.bp3-intent-warning:hover{
          background:rgba(217, 130, 43, 0.2);
          color:#ffb366; }
        .bp3-dark .bp3-button.bp3-outlined.bp3-intent-warning:active, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-warning.bp3-active{
          background:rgba(217, 130, 43, 0.3);
          color:#ffb366; }
        .bp3-dark .bp3-button.bp3-outlined.bp3-intent-warning:disabled, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-warning.bp3-disabled{
          background:none;
          color:rgba(255, 179, 102, 0.5); }
          .bp3-dark .bp3-button.bp3-outlined.bp3-intent-warning:disabled.bp3-active, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-warning.bp3-disabled.bp3-active{
            background:rgba(217, 130, 43, 0.3); }
    .bp3-button.bp3-outlined.bp3-intent-danger{
      color:#c23030; }
      .bp3-button.bp3-outlined.bp3-intent-danger:hover, .bp3-button.bp3-outlined.bp3-intent-danger:active, .bp3-button.bp3-outlined.bp3-intent-danger.bp3-active{
        background:none;
        -webkit-box-shadow:none;
                box-shadow:none;
        color:#c23030; }
      .bp3-button.bp3-outlined.bp3-intent-danger:hover{
        background:rgba(219, 55, 55, 0.15);
        color:#c23030; }
      .bp3-button.bp3-outlined.bp3-intent-danger:active, .bp3-button.bp3-outlined.bp3-intent-danger.bp3-active{
        background:rgba(219, 55, 55, 0.3);
        color:#c23030; }
      .bp3-button.bp3-outlined.bp3-intent-danger:disabled, .bp3-button.bp3-outlined.bp3-intent-danger.bp3-disabled{
        background:none;
        color:rgba(194, 48, 48, 0.5); }
        .bp3-button.bp3-outlined.bp3-intent-danger:disabled.bp3-active, .bp3-button.bp3-outlined.bp3-intent-danger.bp3-disabled.bp3-active{
          background:rgba(219, 55, 55, 0.3); }
      .bp3-button.bp3-outlined.bp3-intent-danger .bp3-button-spinner .bp3-spinner-head{
        stroke:#c23030; }
      .bp3-dark .bp3-button.bp3-outlined.bp3-intent-danger{
        color:#ff7373; }
        .bp3-dark .bp3-button.bp3-outlined.bp3-intent-danger:hover{
          background:rgba(219, 55, 55, 0.2);
          color:#ff7373; }
        .bp3-dark .bp3-button.bp3-outlined.bp3-intent-danger:active, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-danger.bp3-active{
          background:rgba(219, 55, 55, 0.3);
          color:#ff7373; }
        .bp3-dark .bp3-button.bp3-outlined.bp3-intent-danger:disabled, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-danger.bp3-disabled{
          background:none;
          color:rgba(255, 115, 115, 0.5); }
          .bp3-dark .bp3-button.bp3-outlined.bp3-intent-danger:disabled.bp3-active, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-danger.bp3-disabled.bp3-active{
            background:rgba(219, 55, 55, 0.3); }
    .bp3-button.bp3-outlined:disabled, .bp3-button.bp3-outlined.bp3-disabled, .bp3-button.bp3-outlined:disabled:hover, .bp3-button.bp3-outlined.bp3-disabled:hover{
      border-color:rgba(92, 112, 128, 0.1); }
    .bp3-dark .bp3-button.bp3-outlined{
      border-color:rgba(255, 255, 255, 0.4); }
      .bp3-dark .bp3-button.bp3-outlined:disabled, .bp3-dark .bp3-button.bp3-outlined:disabled:hover, .bp3-dark .bp3-button.bp3-outlined.bp3-disabled, .bp3-dark .bp3-button.bp3-outlined.bp3-disabled:hover{
        border-color:rgba(255, 255, 255, 0.2); }
    .bp3-button.bp3-outlined.bp3-intent-primary{
      border-color:rgba(16, 107, 163, 0.6); }
      .bp3-button.bp3-outlined.bp3-intent-primary:disabled, .bp3-button.bp3-outlined.bp3-intent-primary.bp3-disabled{
        border-color:rgba(16, 107, 163, 0.2); }
      .bp3-dark .bp3-button.bp3-outlined.bp3-intent-primary{
        border-color:rgba(72, 175, 240, 0.6); }
        .bp3-dark .bp3-button.bp3-outlined.bp3-intent-primary:disabled, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-primary.bp3-disabled{
          border-color:rgba(72, 175, 240, 0.2); }
    .bp3-button.bp3-outlined.bp3-intent-success{
      border-color:rgba(13, 128, 80, 0.6); }
      .bp3-button.bp3-outlined.bp3-intent-success:disabled, .bp3-button.bp3-outlined.bp3-intent-success.bp3-disabled{
        border-color:rgba(13, 128, 80, 0.2); }
      .bp3-dark .bp3-button.bp3-outlined.bp3-intent-success{
        border-color:rgba(61, 204, 145, 0.6); }
        .bp3-dark .bp3-button.bp3-outlined.bp3-intent-success:disabled, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-success.bp3-disabled{
          border-color:rgba(61, 204, 145, 0.2); }
    .bp3-button.bp3-outlined.bp3-intent-warning{
      border-color:rgba(191, 115, 38, 0.6); }
      .bp3-button.bp3-outlined.bp3-intent-warning:disabled, .bp3-button.bp3-outlined.bp3-intent-warning.bp3-disabled{
        border-color:rgba(191, 115, 38, 0.2); }
      .bp3-dark .bp3-button.bp3-outlined.bp3-intent-warning{
        border-color:rgba(255, 179, 102, 0.6); }
        .bp3-dark .bp3-button.bp3-outlined.bp3-intent-warning:disabled, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-warning.bp3-disabled{
          border-color:rgba(255, 179, 102, 0.2); }
    .bp3-button.bp3-outlined.bp3-intent-danger{
      border-color:rgba(194, 48, 48, 0.6); }
      .bp3-button.bp3-outlined.bp3-intent-danger:disabled, .bp3-button.bp3-outlined.bp3-intent-danger.bp3-disabled{
        border-color:rgba(194, 48, 48, 0.2); }
      .bp3-dark .bp3-button.bp3-outlined.bp3-intent-danger{
        border-color:rgba(255, 115, 115, 0.6); }
        .bp3-dark .bp3-button.bp3-outlined.bp3-intent-danger:disabled, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-danger.bp3-disabled{
          border-color:rgba(255, 115, 115, 0.2); }

a.bp3-button{
  text-align:center;
  text-decoration:none;
  -webkit-transition:none;
  transition:none; }
  a.bp3-button, a.bp3-button:hover, a.bp3-button:active{
    color:#182026; }
  a.bp3-button.bp3-disabled{
    color:rgba(92, 112, 128, 0.6); }

.bp3-button-text{
  -webkit-box-flex:0;
      -ms-flex:0 1 auto;
          flex:0 1 auto; }

.bp3-button.bp3-align-left .bp3-button-text, .bp3-button.bp3-align-right .bp3-button-text,
.bp3-button-group.bp3-align-left .bp3-button-text,
.bp3-button-group.bp3-align-right .bp3-button-text{
  -webkit-box-flex:1;
      -ms-flex:1 1 auto;
          flex:1 1 auto; }
.bp3-button-group{
  display:-webkit-inline-box;
  display:-ms-inline-flexbox;
  display:inline-flex; }
  .bp3-button-group .bp3-button{
    -webkit-box-flex:0;
        -ms-flex:0 0 auto;
            flex:0 0 auto;
    position:relative;
    z-index:4; }
    .bp3-button-group .bp3-button:focus{
      z-index:5; }
    .bp3-button-group .bp3-button:hover{
      z-index:6; }
    .bp3-button-group .bp3-button:active, .bp3-button-group .bp3-button.bp3-active{
      z-index:7; }
    .bp3-button-group .bp3-button:disabled, .bp3-button-group .bp3-button.bp3-disabled{
      z-index:3; }
    .bp3-button-group .bp3-button[class*="bp3-intent-"]{
      z-index:9; }
      .bp3-button-group .bp3-button[class*="bp3-intent-"]:focus{
        z-index:10; }
      .bp3-button-group .bp3-button[class*="bp3-intent-"]:hover{
        z-index:11; }
      .bp3-button-group .bp3-button[class*="bp3-intent-"]:active, .bp3-button-group .bp3-button[class*="bp3-intent-"].bp3-active{
        z-index:12; }
      .bp3-button-group .bp3-button[class*="bp3-intent-"]:disabled, .bp3-button-group .bp3-button[class*="bp3-intent-"].bp3-disabled{
        z-index:8; }
  .bp3-button-group:not(.bp3-minimal) > .bp3-popover-wrapper:not(:first-child) .bp3-button,
  .bp3-button-group:not(.bp3-minimal) > .bp3-button:not(:first-child){
    border-bottom-left-radius:0;
    border-top-left-radius:0; }
  .bp3-button-group:not(.bp3-minimal) > .bp3-popover-wrapper:not(:last-child) .bp3-button,
  .bp3-button-group:not(.bp3-minimal) > .bp3-button:not(:last-child){
    border-bottom-right-radius:0;
    border-top-right-radius:0;
    margin-right:-1px; }
  .bp3-button-group.bp3-minimal .bp3-button{
    background:none;
    -webkit-box-shadow:none;
            box-shadow:none; }
    .bp3-button-group.bp3-minimal .bp3-button:hover{
      background:rgba(167, 182, 194, 0.3);
      -webkit-box-shadow:none;
              box-shadow:none;
      color:#182026;
      text-decoration:none; }
    .bp3-button-group.bp3-minimal .bp3-button:active, .bp3-button-group.bp3-minimal .bp3-button.bp3-active{
      background:rgba(115, 134, 148, 0.3);
      -webkit-box-shadow:none;
              box-shadow:none;
      color:#182026; }
    .bp3-button-group.bp3-minimal .bp3-button:disabled, .bp3-button-group.bp3-minimal .bp3-button:disabled:hover, .bp3-button-group.bp3-minimal .bp3-button.bp3-disabled, .bp3-button-group.bp3-minimal .bp3-button.bp3-disabled:hover{
      background:none;
      color:rgba(92, 112, 128, 0.6);
      cursor:not-allowed; }
      .bp3-button-group.bp3-minimal .bp3-button:disabled.bp3-active, .bp3-button-group.bp3-minimal .bp3-button:disabled:hover.bp3-active, .bp3-button-group.bp3-minimal .bp3-button.bp3-disabled.bp3-active, .bp3-button-group.bp3-minimal .bp3-button.bp3-disabled:hover.bp3-active{
        background:rgba(115, 134, 148, 0.3); }
    .bp3-dark .bp3-button-group.bp3-minimal .bp3-button{
      background:none;
      -webkit-box-shadow:none;
              box-shadow:none;
      color:inherit; }
      .bp3-dark .bp3-button-group.bp3-minimal .bp3-button:hover, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button:active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-active{
        background:none;
        -webkit-box-shadow:none;
                box-shadow:none; }
      .bp3-dark .bp3-button-group.bp3-minimal .bp3-button:hover{
        background:rgba(138, 155, 168, 0.15); }
      .bp3-dark .bp3-button-group.bp3-minimal .bp3-button:active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-active{
        background:rgba(138, 155, 168, 0.3);
        color:#f5f8fa; }
      .bp3-dark .bp3-button-group.bp3-minimal .bp3-button:disabled, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button:disabled:hover, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-disabled, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-disabled:hover{
        background:none;
        color:rgba(167, 182, 194, 0.6);
        cursor:not-allowed; }
        .bp3-dark .bp3-button-group.bp3-minimal .bp3-button:disabled.bp3-active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button:disabled:hover.bp3-active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-disabled.bp3-active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-disabled:hover.bp3-active{
          background:rgba(138, 155, 168, 0.3); }
    .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary{
      color:#106ba3; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary:hover, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary:active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary.bp3-active{
        background:none;
        -webkit-box-shadow:none;
                box-shadow:none;
        color:#106ba3; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary:hover{
        background:rgba(19, 124, 189, 0.15);
        color:#106ba3; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary:active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary.bp3-active{
        background:rgba(19, 124, 189, 0.3);
        color:#106ba3; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary:disabled, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary.bp3-disabled{
        background:none;
        color:rgba(16, 107, 163, 0.5); }
        .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary:disabled.bp3-active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary.bp3-disabled.bp3-active{
          background:rgba(19, 124, 189, 0.3); }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary .bp3-button-spinner .bp3-spinner-head{
        stroke:#106ba3; }
      .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary{
        color:#48aff0; }
        .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary:hover{
          background:rgba(19, 124, 189, 0.2);
          color:#48aff0; }
        .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary:active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary.bp3-active{
          background:rgba(19, 124, 189, 0.3);
          color:#48aff0; }
        .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary:disabled, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary.bp3-disabled{
          background:none;
          color:rgba(72, 175, 240, 0.5); }
          .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary:disabled.bp3-active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary.bp3-disabled.bp3-active{
            background:rgba(19, 124, 189, 0.3); }
    .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success{
      color:#0d8050; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success:hover, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success:active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success.bp3-active{
        background:none;
        -webkit-box-shadow:none;
                box-shadow:none;
        color:#0d8050; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success:hover{
        background:rgba(15, 153, 96, 0.15);
        color:#0d8050; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success:active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success.bp3-active{
        background:rgba(15, 153, 96, 0.3);
        color:#0d8050; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success:disabled, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success.bp3-disabled{
        background:none;
        color:rgba(13, 128, 80, 0.5); }
        .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success:disabled.bp3-active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success.bp3-disabled.bp3-active{
          background:rgba(15, 153, 96, 0.3); }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success .bp3-button-spinner .bp3-spinner-head{
        stroke:#0d8050; }
      .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success{
        color:#3dcc91; }
        .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success:hover{
          background:rgba(15, 153, 96, 0.2);
          color:#3dcc91; }
        .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success:active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success.bp3-active{
          background:rgba(15, 153, 96, 0.3);
          color:#3dcc91; }
        .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success:disabled, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success.bp3-disabled{
          background:none;
          color:rgba(61, 204, 145, 0.5); }
          .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success:disabled.bp3-active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success.bp3-disabled.bp3-active{
            background:rgba(15, 153, 96, 0.3); }
    .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning{
      color:#bf7326; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning:hover, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning:active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning.bp3-active{
        background:none;
        -webkit-box-shadow:none;
                box-shadow:none;
        color:#bf7326; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning:hover{
        background:rgba(217, 130, 43, 0.15);
        color:#bf7326; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning:active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning.bp3-active{
        background:rgba(217, 130, 43, 0.3);
        color:#bf7326; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning:disabled, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning.bp3-disabled{
        background:none;
        color:rgba(191, 115, 38, 0.5); }
        .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning:disabled.bp3-active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning.bp3-disabled.bp3-active{
          background:rgba(217, 130, 43, 0.3); }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning .bp3-button-spinner .bp3-spinner-head{
        stroke:#bf7326; }
      .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning{
        color:#ffb366; }
        .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning:hover{
          background:rgba(217, 130, 43, 0.2);
          color:#ffb366; }
        .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning:active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning.bp3-active{
          background:rgba(217, 130, 43, 0.3);
          color:#ffb366; }
        .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning:disabled, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning.bp3-disabled{
          background:none;
          color:rgba(255, 179, 102, 0.5); }
          .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning:disabled.bp3-active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning.bp3-disabled.bp3-active{
            background:rgba(217, 130, 43, 0.3); }
    .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger{
      color:#c23030; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger:hover, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger:active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger.bp3-active{
        background:none;
        -webkit-box-shadow:none;
                box-shadow:none;
        color:#c23030; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger:hover{
        background:rgba(219, 55, 55, 0.15);
        color:#c23030; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger:active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger.bp3-active{
        background:rgba(219, 55, 55, 0.3);
        color:#c23030; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger:disabled, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger.bp3-disabled{
        background:none;
        color:rgba(194, 48, 48, 0.5); }
        .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger:disabled.bp3-active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger.bp3-disabled.bp3-active{
          background:rgba(219, 55, 55, 0.3); }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger .bp3-button-spinner .bp3-spinner-head{
        stroke:#c23030; }
      .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger{
        color:#ff7373; }
        .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger:hover{
          background:rgba(219, 55, 55, 0.2);
          color:#ff7373; }
        .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger:active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger.bp3-active{
          background:rgba(219, 55, 55, 0.3);
          color:#ff7373; }
        .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger:disabled, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger.bp3-disabled{
          background:none;
          color:rgba(255, 115, 115, 0.5); }
          .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger:disabled.bp3-active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger.bp3-disabled.bp3-active{
            background:rgba(219, 55, 55, 0.3); }
  .bp3-button-group .bp3-popover-wrapper,
  .bp3-button-group .bp3-popover-target{
    display:-webkit-box;
    display:-ms-flexbox;
    display:flex;
    -webkit-box-flex:1;
        -ms-flex:1 1 auto;
            flex:1 1 auto; }
  .bp3-button-group.bp3-fill{
    display:-webkit-box;
    display:-ms-flexbox;
    display:flex;
    width:100%; }
  .bp3-button-group .bp3-button.bp3-fill,
  .bp3-button-group.bp3-fill .bp3-button:not(.bp3-fixed){
    -webkit-box-flex:1;
        -ms-flex:1 1 auto;
            flex:1 1 auto; }
  .bp3-button-group.bp3-vertical{
    -webkit-box-align:stretch;
        -ms-flex-align:stretch;
            align-items:stretch;
    -webkit-box-orient:vertical;
    -webkit-box-direction:normal;
        -ms-flex-direction:column;
            flex-direction:column;
    vertical-align:top; }
    .bp3-button-group.bp3-vertical.bp3-fill{
      height:100%;
      width:unset; }
    .bp3-button-group.bp3-vertical .bp3-button{
      margin-right:0 !important;
      width:100%; }
    .bp3-button-group.bp3-vertical:not(.bp3-minimal) > .bp3-popover-wrapper:first-child .bp3-button,
    .bp3-button-group.bp3-vertical:not(.bp3-minimal) > .bp3-button:first-child{
      border-radius:3px 3px 0 0; }
    .bp3-button-group.bp3-vertical:not(.bp3-minimal) > .bp3-popover-wrapper:last-child .bp3-button,
    .bp3-button-group.bp3-vertical:not(.bp3-minimal) > .bp3-button:last-child{
      border-radius:0 0 3px 3px; }
    .bp3-button-group.bp3-vertical:not(.bp3-minimal) > .bp3-popover-wrapper:not(:last-child) .bp3-button,
    .bp3-button-group.bp3-vertical:not(.bp3-minimal) > .bp3-button:not(:last-child){
      margin-bottom:-1px; }
  .bp3-button-group.bp3-align-left .bp3-button{
    text-align:left; }
  .bp3-dark .bp3-button-group:not(.bp3-minimal) > .bp3-popover-wrapper:not(:last-child) .bp3-button,
  .bp3-dark .bp3-button-group:not(.bp3-minimal) > .bp3-button:not(:last-child){
    margin-right:1px; }
  .bp3-dark .bp3-button-group.bp3-vertical > .bp3-popover-wrapper:not(:last-child) .bp3-button,
  .bp3-dark .bp3-button-group.bp3-vertical > .bp3-button:not(:last-child){
    margin-bottom:1px; }
.bp3-callout{
  font-size:14px;
  line-height:1.5;
  background-color:rgba(138, 155, 168, 0.15);
  border-radius:3px;
  padding:10px 12px 9px;
  position:relative;
  width:100%; }
  .bp3-callout[class*="bp3-icon-"]{
    padding-left:40px; }
    .bp3-callout[class*="bp3-icon-"]::before{
      font-family:"Icons20", sans-serif;
      font-size:20px;
      font-style:normal;
      font-weight:400;
      line-height:1;
      -moz-osx-font-smoothing:grayscale;
      -webkit-font-smoothing:antialiased;
      color:#5c7080;
      left:10px;
      position:absolute;
      top:10px; }
  .bp3-callout.bp3-callout-icon{
    padding-left:40px; }
    .bp3-callout.bp3-callout-icon > .bp3-icon:first-child{
      color:#5c7080;
      left:10px;
      position:absolute;
      top:10px; }
  .bp3-callout .bp3-heading{
    line-height:20px;
    margin-bottom:5px;
    margin-top:0; }
    .bp3-callout .bp3-heading:last-child{
      margin-bottom:0; }
  .bp3-dark .bp3-callout{
    background-color:rgba(138, 155, 168, 0.2); }
    .bp3-dark .bp3-callout[class*="bp3-icon-"]::before{
      color:#a7b6c2; }
  .bp3-callout.bp3-intent-primary{
    background-color:rgba(19, 124, 189, 0.15); }
    .bp3-callout.bp3-intent-primary[class*="bp3-icon-"]::before,
    .bp3-callout.bp3-intent-primary > .bp3-icon:first-child,
    .bp3-callout.bp3-intent-primary .bp3-heading{
      color:#106ba3; }
    .bp3-dark .bp3-callout.bp3-intent-primary{
      background-color:rgba(19, 124, 189, 0.25); }
      .bp3-dark .bp3-callout.bp3-intent-primary[class*="bp3-icon-"]::before,
      .bp3-dark .bp3-callout.bp3-intent-primary > .bp3-icon:first-child,
      .bp3-dark .bp3-callout.bp3-intent-primary .bp3-heading{
        color:#48aff0; }
  .bp3-callout.bp3-intent-success{
    background-color:rgba(15, 153, 96, 0.15); }
    .bp3-callout.bp3-intent-success[class*="bp3-icon-"]::before,
    .bp3-callout.bp3-intent-success > .bp3-icon:first-child,
    .bp3-callout.bp3-intent-success .bp3-heading{
      color:#0d8050; }
    .bp3-dark .bp3-callout.bp3-intent-success{
      background-color:rgba(15, 153, 96, 0.25); }
      .bp3-dark .bp3-callout.bp3-intent-success[class*="bp3-icon-"]::before,
      .bp3-dark .bp3-callout.bp3-intent-success > .bp3-icon:first-child,
      .bp3-dark .bp3-callout.bp3-intent-success .bp3-heading{
        color:#3dcc91; }
  .bp3-callout.bp3-intent-warning{
    background-color:rgba(217, 130, 43, 0.15); }
    .bp3-callout.bp3-intent-warning[class*="bp3-icon-"]::before,
    .bp3-callout.bp3-intent-warning > .bp3-icon:first-child,
    .bp3-callout.bp3-intent-warning .bp3-heading{
      color:#bf7326; }
    .bp3-dark .bp3-callout.bp3-intent-warning{
      background-color:rgba(217, 130, 43, 0.25); }
      .bp3-dark .bp3-callout.bp3-intent-warning[class*="bp3-icon-"]::before,
      .bp3-dark .bp3-callout.bp3-intent-warning > .bp3-icon:first-child,
      .bp3-dark .bp3-callout.bp3-intent-warning .bp3-heading{
        color:#ffb366; }
  .bp3-callout.bp3-intent-danger{
    background-color:rgba(219, 55, 55, 0.15); }
    .bp3-callout.bp3-intent-danger[class*="bp3-icon-"]::before,
    .bp3-callout.bp3-intent-danger > .bp3-icon:first-child,
    .bp3-callout.bp3-intent-danger .bp3-heading{
      color:#c23030; }
    .bp3-dark .bp3-callout.bp3-intent-danger{
      background-color:rgba(219, 55, 55, 0.25); }
      .bp3-dark .bp3-callout.bp3-intent-danger[class*="bp3-icon-"]::before,
      .bp3-dark .bp3-callout.bp3-intent-danger > .bp3-icon:first-child,
      .bp3-dark .bp3-callout.bp3-intent-danger .bp3-heading{
        color:#ff7373; }
  .bp3-running-text .bp3-callout{
    margin:20px 0; }
.bp3-card{
  background-color:#ffffff;
  border-radius:3px;
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.15), 0 0 0 rgba(16, 22, 26, 0), 0 0 0 rgba(16, 22, 26, 0);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.15), 0 0 0 rgba(16, 22, 26, 0), 0 0 0 rgba(16, 22, 26, 0);
  padding:20px;
  -webkit-transition:-webkit-transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-box-shadow 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
  transition:-webkit-transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-box-shadow 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
  transition:transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9), box-shadow 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
  transition:transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9), box-shadow 200ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-box-shadow 200ms cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-card.bp3-dark,
  .bp3-dark .bp3-card{
    background-color:#30404d;
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4), 0 0 0 rgba(16, 22, 26, 0), 0 0 0 rgba(16, 22, 26, 0);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4), 0 0 0 rgba(16, 22, 26, 0), 0 0 0 rgba(16, 22, 26, 0); }

.bp3-elevation-0{
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.15), 0 0 0 rgba(16, 22, 26, 0), 0 0 0 rgba(16, 22, 26, 0);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.15), 0 0 0 rgba(16, 22, 26, 0), 0 0 0 rgba(16, 22, 26, 0); }
  .bp3-elevation-0.bp3-dark,
  .bp3-dark .bp3-elevation-0{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4), 0 0 0 rgba(16, 22, 26, 0), 0 0 0 rgba(16, 22, 26, 0);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4), 0 0 0 rgba(16, 22, 26, 0), 0 0 0 rgba(16, 22, 26, 0); }

.bp3-elevation-1{
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.2); }
  .bp3-elevation-1.bp3-dark,
  .bp3-dark .bp3-elevation-1{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.4); }

.bp3-elevation-2{
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 1px 1px rgba(16, 22, 26, 0.2), 0 2px 6px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 1px 1px rgba(16, 22, 26, 0.2), 0 2px 6px rgba(16, 22, 26, 0.2); }
  .bp3-elevation-2.bp3-dark,
  .bp3-dark .bp3-elevation-2{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 1px 1px rgba(16, 22, 26, 0.4), 0 2px 6px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 1px 1px rgba(16, 22, 26, 0.4), 0 2px 6px rgba(16, 22, 26, 0.4); }

.bp3-elevation-3{
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2); }
  .bp3-elevation-3.bp3-dark,
  .bp3-dark .bp3-elevation-3{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4); }

.bp3-elevation-4{
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 4px 8px rgba(16, 22, 26, 0.2), 0 18px 46px 6px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 4px 8px rgba(16, 22, 26, 0.2), 0 18px 46px 6px rgba(16, 22, 26, 0.2); }
  .bp3-elevation-4.bp3-dark,
  .bp3-dark .bp3-elevation-4{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 4px 8px rgba(16, 22, 26, 0.4), 0 18px 46px 6px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 4px 8px rgba(16, 22, 26, 0.4), 0 18px 46px 6px rgba(16, 22, 26, 0.4); }

.bp3-card.bp3-interactive:hover{
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
  cursor:pointer; }
  .bp3-card.bp3-interactive:hover.bp3-dark,
  .bp3-dark .bp3-card.bp3-interactive:hover{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4); }

.bp3-card.bp3-interactive:active{
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.2);
  opacity:0.9;
  -webkit-transition-duration:0;
          transition-duration:0; }
  .bp3-card.bp3-interactive:active.bp3-dark,
  .bp3-dark .bp3-card.bp3-interactive:active{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.4); }

.bp3-collapse{
  height:0;
  overflow-y:hidden;
  -webkit-transition:height 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
  transition:height 200ms cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-collapse .bp3-collapse-body{
    -webkit-transition:-webkit-transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
    transition:-webkit-transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
    transition:transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
    transition:transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9); }
    .bp3-collapse .bp3-collapse-body[aria-hidden="true"]{
      display:none; }

.bp3-context-menu .bp3-popover-target{
  display:block; }

.bp3-context-menu-popover-target{
  position:fixed; }

.bp3-divider{
  border-bottom:1px solid rgba(16, 22, 26, 0.15);
  border-right:1px solid rgba(16, 22, 26, 0.15);
  margin:5px; }
  .bp3-dark .bp3-divider{
    border-color:rgba(16, 22, 26, 0.4); }
.bp3-dialog-container{
  opacity:1;
  -webkit-transform:scale(1);
          transform:scale(1);
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-pack:center;
      -ms-flex-pack:center;
          justify-content:center;
  min-height:100%;
  pointer-events:none;
  -webkit-user-select:none;
     -moz-user-select:none;
      -ms-user-select:none;
          user-select:none;
  width:100%; }
  .bp3-dialog-container.bp3-overlay-enter > .bp3-dialog, .bp3-dialog-container.bp3-overlay-appear > .bp3-dialog{
    opacity:0;
    -webkit-transform:scale(0.5);
            transform:scale(0.5); }
  .bp3-dialog-container.bp3-overlay-enter-active > .bp3-dialog, .bp3-dialog-container.bp3-overlay-appear-active > .bp3-dialog{
    opacity:1;
    -webkit-transform:scale(1);
            transform:scale(1);
    -webkit-transition-delay:0;
            transition-delay:0;
    -webkit-transition-duration:300ms;
            transition-duration:300ms;
    -webkit-transition-property:opacity, -webkit-transform;
    transition-property:opacity, -webkit-transform;
    transition-property:opacity, transform;
    transition-property:opacity, transform, -webkit-transform;
    -webkit-transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11);
            transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11); }
  .bp3-dialog-container.bp3-overlay-exit > .bp3-dialog{
    opacity:1;
    -webkit-transform:scale(1);
            transform:scale(1); }
  .bp3-dialog-container.bp3-overlay-exit-active > .bp3-dialog{
    opacity:0;
    -webkit-transform:scale(0.5);
            transform:scale(0.5);
    -webkit-transition-delay:0;
            transition-delay:0;
    -webkit-transition-duration:300ms;
            transition-duration:300ms;
    -webkit-transition-property:opacity, -webkit-transform;
    transition-property:opacity, -webkit-transform;
    transition-property:opacity, transform;
    transition-property:opacity, transform, -webkit-transform;
    -webkit-transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11);
            transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11); }

.bp3-dialog{
  background:#ebf1f5;
  border-radius:6px;
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 4px 8px rgba(16, 22, 26, 0.2), 0 18px 46px 6px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 4px 8px rgba(16, 22, 26, 0.2), 0 18px 46px 6px rgba(16, 22, 26, 0.2);
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-orient:vertical;
  -webkit-box-direction:normal;
      -ms-flex-direction:column;
          flex-direction:column;
  margin:30px 0;
  padding-bottom:20px;
  pointer-events:all;
  -webkit-user-select:text;
     -moz-user-select:text;
      -ms-user-select:text;
          user-select:text;
  width:500px; }
  .bp3-dialog:focus{
    outline:0; }
  .bp3-dialog.bp3-dark,
  .bp3-dark .bp3-dialog{
    background:#293742;
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 4px 8px rgba(16, 22, 26, 0.4), 0 18px 46px 6px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 4px 8px rgba(16, 22, 26, 0.4), 0 18px 46px 6px rgba(16, 22, 26, 0.4);
    color:#f5f8fa; }

.bp3-dialog-header{
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  background:#ffffff;
  border-radius:6px 6px 0 0;
  -webkit-box-shadow:0 1px 0 rgba(16, 22, 26, 0.15);
          box-shadow:0 1px 0 rgba(16, 22, 26, 0.15);
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-flex:0;
      -ms-flex:0 0 auto;
          flex:0 0 auto;
  min-height:40px;
  padding-left:20px;
  padding-right:5px;
  z-index:30; }
  .bp3-dialog-header .bp3-icon-large,
  .bp3-dialog-header .bp3-icon{
    color:#5c7080;
    -webkit-box-flex:0;
        -ms-flex:0 0 auto;
            flex:0 0 auto;
    margin-right:10px; }
  .bp3-dialog-header .bp3-heading{
    overflow:hidden;
    text-overflow:ellipsis;
    white-space:nowrap;
    word-wrap:normal;
    -webkit-box-flex:1;
        -ms-flex:1 1 auto;
            flex:1 1 auto;
    line-height:inherit;
    margin:0; }
    .bp3-dialog-header .bp3-heading:last-child{
      margin-right:20px; }
  .bp3-dark .bp3-dialog-header{
    background:#30404d;
    -webkit-box-shadow:0 1px 0 rgba(16, 22, 26, 0.4);
            box-shadow:0 1px 0 rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-dialog-header .bp3-icon-large,
    .bp3-dark .bp3-dialog-header .bp3-icon{
      color:#a7b6c2; }

.bp3-dialog-body{
  -webkit-box-flex:1;
      -ms-flex:1 1 auto;
          flex:1 1 auto;
  line-height:18px;
  margin:20px; }

.bp3-dialog-footer{
  -webkit-box-flex:0;
      -ms-flex:0 0 auto;
          flex:0 0 auto;
  margin:0 20px; }

.bp3-dialog-footer-actions{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-pack:end;
      -ms-flex-pack:end;
          justify-content:flex-end; }
  .bp3-dialog-footer-actions .bp3-button{
    margin-left:10px; }
.bp3-multistep-dialog-panels{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex; }

.bp3-multistep-dialog-left-panel{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-flex:1;
      -ms-flex:1;
          flex:1;
  -webkit-box-orient:vertical;
  -webkit-box-direction:normal;
      -ms-flex-direction:column;
          flex-direction:column; }
  .bp3-dark .bp3-multistep-dialog-left-panel{
    background:#202b33; }

.bp3-multistep-dialog-right-panel{
  background-color:#f5f8fa;
  border-left:1px solid rgba(16, 22, 26, 0.15);
  border-radius:0 0 6px 0;
  -webkit-box-flex:3;
      -ms-flex:3;
          flex:3;
  min-width:0; }
  .bp3-dark .bp3-multistep-dialog-right-panel{
    background-color:#293742;
    border-left:1px solid rgba(16, 22, 26, 0.4); }

.bp3-multistep-dialog-footer{
  background-color:#ffffff;
  border-radius:0 0 6px 0;
  border-top:1px solid rgba(16, 22, 26, 0.15);
  padding:10px; }
  .bp3-dark .bp3-multistep-dialog-footer{
    background:#30404d;
    border-top:1px solid rgba(16, 22, 26, 0.4); }

.bp3-dialog-step-container{
  background-color:#f5f8fa;
  border-bottom:1px solid rgba(16, 22, 26, 0.15); }
  .bp3-dark .bp3-dialog-step-container{
    background:#293742;
    border-bottom:1px solid rgba(16, 22, 26, 0.4); }
  .bp3-dialog-step-container.bp3-dialog-step-viewed{
    background-color:#ffffff; }
    .bp3-dark .bp3-dialog-step-container.bp3-dialog-step-viewed{
      background:#30404d; }

.bp3-dialog-step{
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  background-color:#f5f8fa;
  border-radius:6px;
  cursor:not-allowed;
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  margin:4px;
  padding:6px 14px; }
  .bp3-dark .bp3-dialog-step{
    background:#293742; }
  .bp3-dialog-step-viewed .bp3-dialog-step{
    background-color:#ffffff;
    cursor:pointer; }
    .bp3-dark .bp3-dialog-step-viewed .bp3-dialog-step{
      background:#30404d; }
  .bp3-dialog-step:hover{
    background-color:#f5f8fa; }
    .bp3-dark .bp3-dialog-step:hover{
      background:#293742; }

.bp3-dialog-step-icon{
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  background-color:rgba(92, 112, 128, 0.6);
  border-radius:50%;
  color:#ffffff;
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  height:25px;
  -webkit-box-pack:center;
      -ms-flex-pack:center;
          justify-content:center;
  width:25px; }
  .bp3-dark .bp3-dialog-step-icon{
    background-color:rgba(167, 182, 194, 0.6); }
  .bp3-active.bp3-dialog-step-viewed .bp3-dialog-step-icon{
    background-color:#2b95d6; }
  .bp3-dialog-step-viewed .bp3-dialog-step-icon{
    background-color:#8a9ba8; }

.bp3-dialog-step-title{
  color:rgba(92, 112, 128, 0.6);
  -webkit-box-flex:1;
      -ms-flex:1;
          flex:1;
  padding-left:10px; }
  .bp3-dark .bp3-dialog-step-title{
    color:rgba(167, 182, 194, 0.6); }
  .bp3-active.bp3-dialog-step-viewed .bp3-dialog-step-title{
    color:#2b95d6; }
  .bp3-dialog-step-viewed:not(.bp3-active) .bp3-dialog-step-title{
    color:#182026; }
    .bp3-dark .bp3-dialog-step-viewed:not(.bp3-active) .bp3-dialog-step-title{
      color:#f5f8fa; }
.bp3-drawer{
  background:#ffffff;
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 4px 8px rgba(16, 22, 26, 0.2), 0 18px 46px 6px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 4px 8px rgba(16, 22, 26, 0.2), 0 18px 46px 6px rgba(16, 22, 26, 0.2);
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-orient:vertical;
  -webkit-box-direction:normal;
      -ms-flex-direction:column;
          flex-direction:column;
  margin:0;
  padding:0; }
  .bp3-drawer:focus{
    outline:0; }
  .bp3-drawer.bp3-position-top{
    height:50%;
    left:0;
    right:0;
    top:0; }
    .bp3-drawer.bp3-position-top.bp3-overlay-enter, .bp3-drawer.bp3-position-top.bp3-overlay-appear{
      -webkit-transform:translateY(-100%);
              transform:translateY(-100%); }
    .bp3-drawer.bp3-position-top.bp3-overlay-enter-active, .bp3-drawer.bp3-position-top.bp3-overlay-appear-active{
      -webkit-transform:translateY(0);
              transform:translateY(0);
      -webkit-transition-delay:0;
              transition-delay:0;
      -webkit-transition-duration:200ms;
              transition-duration:200ms;
      -webkit-transition-property:-webkit-transform;
      transition-property:-webkit-transform;
      transition-property:transform;
      transition-property:transform, -webkit-transform;
      -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
              transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
    .bp3-drawer.bp3-position-top.bp3-overlay-exit{
      -webkit-transform:translateY(0);
              transform:translateY(0); }
    .bp3-drawer.bp3-position-top.bp3-overlay-exit-active{
      -webkit-transform:translateY(-100%);
              transform:translateY(-100%);
      -webkit-transition-delay:0;
              transition-delay:0;
      -webkit-transition-duration:100ms;
              transition-duration:100ms;
      -webkit-transition-property:-webkit-transform;
      transition-property:-webkit-transform;
      transition-property:transform;
      transition-property:transform, -webkit-transform;
      -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
              transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-drawer.bp3-position-bottom{
    bottom:0;
    height:50%;
    left:0;
    right:0; }
    .bp3-drawer.bp3-position-bottom.bp3-overlay-enter, .bp3-drawer.bp3-position-bottom.bp3-overlay-appear{
      -webkit-transform:translateY(100%);
              transform:translateY(100%); }
    .bp3-drawer.bp3-position-bottom.bp3-overlay-enter-active, .bp3-drawer.bp3-position-bottom.bp3-overlay-appear-active{
      -webkit-transform:translateY(0);
              transform:translateY(0);
      -webkit-transition-delay:0;
              transition-delay:0;
      -webkit-transition-duration:200ms;
              transition-duration:200ms;
      -webkit-transition-property:-webkit-transform;
      transition-property:-webkit-transform;
      transition-property:transform;
      transition-property:transform, -webkit-transform;
      -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
              transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
    .bp3-drawer.bp3-position-bottom.bp3-overlay-exit{
      -webkit-transform:translateY(0);
              transform:translateY(0); }
    .bp3-drawer.bp3-position-bottom.bp3-overlay-exit-active{
      -webkit-transform:translateY(100%);
              transform:translateY(100%);
      -webkit-transition-delay:0;
              transition-delay:0;
      -webkit-transition-duration:100ms;
              transition-duration:100ms;
      -webkit-transition-property:-webkit-transform;
      transition-property:-webkit-transform;
      transition-property:transform;
      transition-property:transform, -webkit-transform;
      -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
              transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-drawer.bp3-position-left{
    bottom:0;
    left:0;
    top:0;
    width:50%; }
    .bp3-drawer.bp3-position-left.bp3-overlay-enter, .bp3-drawer.bp3-position-left.bp3-overlay-appear{
      -webkit-transform:translateX(-100%);
              transform:translateX(-100%); }
    .bp3-drawer.bp3-position-left.bp3-overlay-enter-active, .bp3-drawer.bp3-position-left.bp3-overlay-appear-active{
      -webkit-transform:translateX(0);
              transform:translateX(0);
      -webkit-transition-delay:0;
              transition-delay:0;
      -webkit-transition-duration:200ms;
              transition-duration:200ms;
      -webkit-transition-property:-webkit-transform;
      transition-property:-webkit-transform;
      transition-property:transform;
      transition-property:transform, -webkit-transform;
      -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
              transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
    .bp3-drawer.bp3-position-left.bp3-overlay-exit{
      -webkit-transform:translateX(0);
              transform:translateX(0); }
    .bp3-drawer.bp3-position-left.bp3-overlay-exit-active{
      -webkit-transform:translateX(-100%);
              transform:translateX(-100%);
      -webkit-transition-delay:0;
              transition-delay:0;
      -webkit-transition-duration:100ms;
              transition-duration:100ms;
      -webkit-transition-property:-webkit-transform;
      transition-property:-webkit-transform;
      transition-property:transform;
      transition-property:transform, -webkit-transform;
      -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
              transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-drawer.bp3-position-right{
    bottom:0;
    right:0;
    top:0;
    width:50%; }
    .bp3-drawer.bp3-position-right.bp3-overlay-enter, .bp3-drawer.bp3-position-right.bp3-overlay-appear{
      -webkit-transform:translateX(100%);
              transform:translateX(100%); }
    .bp3-drawer.bp3-position-right.bp3-overlay-enter-active, .bp3-drawer.bp3-position-right.bp3-overlay-appear-active{
      -webkit-transform:translateX(0);
              transform:translateX(0);
      -webkit-transition-delay:0;
              transition-delay:0;
      -webkit-transition-duration:200ms;
              transition-duration:200ms;
      -webkit-transition-property:-webkit-transform;
      transition-property:-webkit-transform;
      transition-property:transform;
      transition-property:transform, -webkit-transform;
      -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
              transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
    .bp3-drawer.bp3-position-right.bp3-overlay-exit{
      -webkit-transform:translateX(0);
              transform:translateX(0); }
    .bp3-drawer.bp3-position-right.bp3-overlay-exit-active{
      -webkit-transform:translateX(100%);
              transform:translateX(100%);
      -webkit-transition-delay:0;
              transition-delay:0;
      -webkit-transition-duration:100ms;
              transition-duration:100ms;
      -webkit-transition-property:-webkit-transform;
      transition-property:-webkit-transform;
      transition-property:transform;
      transition-property:transform, -webkit-transform;
      -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
              transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
  .bp3-position-right):not(.bp3-vertical){
    bottom:0;
    right:0;
    top:0;
    width:50%; }
    .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
    .bp3-position-right):not(.bp3-vertical).bp3-overlay-enter, .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
    .bp3-position-right):not(.bp3-vertical).bp3-overlay-appear{
      -webkit-transform:translateX(100%);
              transform:translateX(100%); }
    .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
    .bp3-position-right):not(.bp3-vertical).bp3-overlay-enter-active, .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
    .bp3-position-right):not(.bp3-vertical).bp3-overlay-appear-active{
      -webkit-transform:translateX(0);
              transform:translateX(0);
      -webkit-transition-delay:0;
              transition-delay:0;
      -webkit-transition-duration:200ms;
              transition-duration:200ms;
      -webkit-transition-property:-webkit-transform;
      transition-property:-webkit-transform;
      transition-property:transform;
      transition-property:transform, -webkit-transform;
      -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
              transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
    .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
    .bp3-position-right):not(.bp3-vertical).bp3-overlay-exit{
      -webkit-transform:translateX(0);
              transform:translateX(0); }
    .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
    .bp3-position-right):not(.bp3-vertical).bp3-overlay-exit-active{
      -webkit-transform:translateX(100%);
              transform:translateX(100%);
      -webkit-transition-delay:0;
              transition-delay:0;
      -webkit-transition-duration:100ms;
              transition-duration:100ms;
      -webkit-transition-property:-webkit-transform;
      transition-property:-webkit-transform;
      transition-property:transform;
      transition-property:transform, -webkit-transform;
      -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
              transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
  .bp3-position-right).bp3-vertical{
    bottom:0;
    height:50%;
    left:0;
    right:0; }
    .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
    .bp3-position-right).bp3-vertical.bp3-overlay-enter, .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
    .bp3-position-right).bp3-vertical.bp3-overlay-appear{
      -webkit-transform:translateY(100%);
              transform:translateY(100%); }
    .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
    .bp3-position-right).bp3-vertical.bp3-overlay-enter-active, .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
    .bp3-position-right).bp3-vertical.bp3-overlay-appear-active{
      -webkit-transform:translateY(0);
              transform:translateY(0);
      -webkit-transition-delay:0;
              transition-delay:0;
      -webkit-transition-duration:200ms;
              transition-duration:200ms;
      -webkit-transition-property:-webkit-transform;
      transition-property:-webkit-transform;
      transition-property:transform;
      transition-property:transform, -webkit-transform;
      -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
              transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
    .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
    .bp3-position-right).bp3-vertical.bp3-overlay-exit{
      -webkit-transform:translateY(0);
              transform:translateY(0); }
    .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
    .bp3-position-right).bp3-vertical.bp3-overlay-exit-active{
      -webkit-transform:translateY(100%);
              transform:translateY(100%);
      -webkit-transition-delay:0;
              transition-delay:0;
      -webkit-transition-duration:100ms;
              transition-duration:100ms;
      -webkit-transition-property:-webkit-transform;
      transition-property:-webkit-transform;
      transition-property:transform;
      transition-property:transform, -webkit-transform;
      -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
              transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-drawer.bp3-dark,
  .bp3-dark .bp3-drawer{
    background:#30404d;
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 4px 8px rgba(16, 22, 26, 0.4), 0 18px 46px 6px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 4px 8px rgba(16, 22, 26, 0.4), 0 18px 46px 6px rgba(16, 22, 26, 0.4);
    color:#f5f8fa; }

.bp3-drawer-header{
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  border-radius:0;
  -webkit-box-shadow:0 1px 0 rgba(16, 22, 26, 0.15);
          box-shadow:0 1px 0 rgba(16, 22, 26, 0.15);
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-flex:0;
      -ms-flex:0 0 auto;
          flex:0 0 auto;
  min-height:40px;
  padding:5px;
  padding-left:20px;
  position:relative; }
  .bp3-drawer-header .bp3-icon-large,
  .bp3-drawer-header .bp3-icon{
    color:#5c7080;
    -webkit-box-flex:0;
        -ms-flex:0 0 auto;
            flex:0 0 auto;
    margin-right:10px; }
  .bp3-drawer-header .bp3-heading{
    overflow:hidden;
    text-overflow:ellipsis;
    white-space:nowrap;
    word-wrap:normal;
    -webkit-box-flex:1;
        -ms-flex:1 1 auto;
            flex:1 1 auto;
    line-height:inherit;
    margin:0; }
    .bp3-drawer-header .bp3-heading:last-child{
      margin-right:20px; }
  .bp3-dark .bp3-drawer-header{
    -webkit-box-shadow:0 1px 0 rgba(16, 22, 26, 0.4);
            box-shadow:0 1px 0 rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-drawer-header .bp3-icon-large,
    .bp3-dark .bp3-drawer-header .bp3-icon{
      color:#a7b6c2; }

.bp3-drawer-body{
  -webkit-box-flex:1;
      -ms-flex:1 1 auto;
          flex:1 1 auto;
  line-height:18px;
  overflow:auto; }

.bp3-drawer-footer{
  -webkit-box-shadow:inset 0 1px 0 rgba(16, 22, 26, 0.15);
          box-shadow:inset 0 1px 0 rgba(16, 22, 26, 0.15);
  -webkit-box-flex:0;
      -ms-flex:0 0 auto;
          flex:0 0 auto;
  padding:10px 20px;
  position:relative; }
  .bp3-dark .bp3-drawer-footer{
    -webkit-box-shadow:inset 0 1px 0 rgba(16, 22, 26, 0.4);
            box-shadow:inset 0 1px 0 rgba(16, 22, 26, 0.4); }
.bp3-editable-text{
  cursor:text;
  display:inline-block;
  max-width:100%;
  position:relative;
  vertical-align:top;
  white-space:nowrap; }
  .bp3-editable-text::before{
    bottom:-3px;
    left:-3px;
    position:absolute;
    right:-3px;
    top:-3px;
    border-radius:3px;
    content:"";
    -webkit-transition:background-color 100ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
    transition:background-color 100ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
    transition:background-color 100ms cubic-bezier(0.4, 1, 0.75, 0.9), box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
    transition:background-color 100ms cubic-bezier(0.4, 1, 0.75, 0.9), box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-editable-text:hover::before{
    -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.15);
            box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.15); }
  .bp3-editable-text.bp3-editable-text-editing::before{
    background-color:#ffffff;
    -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
  .bp3-editable-text.bp3-disabled::before{
    -webkit-box-shadow:none;
            box-shadow:none; }
  .bp3-editable-text.bp3-intent-primary .bp3-editable-text-input,
  .bp3-editable-text.bp3-intent-primary .bp3-editable-text-content{
    color:#137cbd; }
  .bp3-editable-text.bp3-intent-primary:hover::before{
    -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(19, 124, 189, 0.4);
            box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(19, 124, 189, 0.4); }
  .bp3-editable-text.bp3-intent-primary.bp3-editable-text-editing::before{
    -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
  .bp3-editable-text.bp3-intent-success .bp3-editable-text-input,
  .bp3-editable-text.bp3-intent-success .bp3-editable-text-content{
    color:#0f9960; }
  .bp3-editable-text.bp3-intent-success:hover::before{
    -webkit-box-shadow:0 0 0 0 rgba(15, 153, 96, 0), 0 0 0 0 rgba(15, 153, 96, 0), inset 0 0 0 1px rgba(15, 153, 96, 0.4);
            box-shadow:0 0 0 0 rgba(15, 153, 96, 0), 0 0 0 0 rgba(15, 153, 96, 0), inset 0 0 0 1px rgba(15, 153, 96, 0.4); }
  .bp3-editable-text.bp3-intent-success.bp3-editable-text-editing::before{
    -webkit-box-shadow:0 0 0 1px #0f9960, 0 0 0 3px rgba(15, 153, 96, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px #0f9960, 0 0 0 3px rgba(15, 153, 96, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
  .bp3-editable-text.bp3-intent-warning .bp3-editable-text-input,
  .bp3-editable-text.bp3-intent-warning .bp3-editable-text-content{
    color:#d9822b; }
  .bp3-editable-text.bp3-intent-warning:hover::before{
    -webkit-box-shadow:0 0 0 0 rgba(217, 130, 43, 0), 0 0 0 0 rgba(217, 130, 43, 0), inset 0 0 0 1px rgba(217, 130, 43, 0.4);
            box-shadow:0 0 0 0 rgba(217, 130, 43, 0), 0 0 0 0 rgba(217, 130, 43, 0), inset 0 0 0 1px rgba(217, 130, 43, 0.4); }
  .bp3-editable-text.bp3-intent-warning.bp3-editable-text-editing::before{
    -webkit-box-shadow:0 0 0 1px #d9822b, 0 0 0 3px rgba(217, 130, 43, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px #d9822b, 0 0 0 3px rgba(217, 130, 43, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
  .bp3-editable-text.bp3-intent-danger .bp3-editable-text-input,
  .bp3-editable-text.bp3-intent-danger .bp3-editable-text-content{
    color:#db3737; }
  .bp3-editable-text.bp3-intent-danger:hover::before{
    -webkit-box-shadow:0 0 0 0 rgba(219, 55, 55, 0), 0 0 0 0 rgba(219, 55, 55, 0), inset 0 0 0 1px rgba(219, 55, 55, 0.4);
            box-shadow:0 0 0 0 rgba(219, 55, 55, 0), 0 0 0 0 rgba(219, 55, 55, 0), inset 0 0 0 1px rgba(219, 55, 55, 0.4); }
  .bp3-editable-text.bp3-intent-danger.bp3-editable-text-editing::before{
    -webkit-box-shadow:0 0 0 1px #db3737, 0 0 0 3px rgba(219, 55, 55, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px #db3737, 0 0 0 3px rgba(219, 55, 55, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
  .bp3-dark .bp3-editable-text:hover::before{
    -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(255, 255, 255, 0.15);
            box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(255, 255, 255, 0.15); }
  .bp3-dark .bp3-editable-text.bp3-editable-text-editing::before{
    background-color:rgba(16, 22, 26, 0.3);
    -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
  .bp3-dark .bp3-editable-text.bp3-disabled::before{
    -webkit-box-shadow:none;
            box-shadow:none; }
  .bp3-dark .bp3-editable-text.bp3-intent-primary .bp3-editable-text-content{
    color:#48aff0; }
  .bp3-dark .bp3-editable-text.bp3-intent-primary:hover::before{
    -webkit-box-shadow:0 0 0 0 rgba(72, 175, 240, 0), 0 0 0 0 rgba(72, 175, 240, 0), inset 0 0 0 1px rgba(72, 175, 240, 0.4);
            box-shadow:0 0 0 0 rgba(72, 175, 240, 0), 0 0 0 0 rgba(72, 175, 240, 0), inset 0 0 0 1px rgba(72, 175, 240, 0.4); }
  .bp3-dark .bp3-editable-text.bp3-intent-primary.bp3-editable-text-editing::before{
    -webkit-box-shadow:0 0 0 1px #48aff0, 0 0 0 3px rgba(72, 175, 240, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px #48aff0, 0 0 0 3px rgba(72, 175, 240, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
  .bp3-dark .bp3-editable-text.bp3-intent-success .bp3-editable-text-content{
    color:#3dcc91; }
  .bp3-dark .bp3-editable-text.bp3-intent-success:hover::before{
    -webkit-box-shadow:0 0 0 0 rgba(61, 204, 145, 0), 0 0 0 0 rgba(61, 204, 145, 0), inset 0 0 0 1px rgba(61, 204, 145, 0.4);
            box-shadow:0 0 0 0 rgba(61, 204, 145, 0), 0 0 0 0 rgba(61, 204, 145, 0), inset 0 0 0 1px rgba(61, 204, 145, 0.4); }
  .bp3-dark .bp3-editable-text.bp3-intent-success.bp3-editable-text-editing::before{
    -webkit-box-shadow:0 0 0 1px #3dcc91, 0 0 0 3px rgba(61, 204, 145, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px #3dcc91, 0 0 0 3px rgba(61, 204, 145, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
  .bp3-dark .bp3-editable-text.bp3-intent-warning .bp3-editable-text-content{
    color:#ffb366; }
  .bp3-dark .bp3-editable-text.bp3-intent-warning:hover::before{
    -webkit-box-shadow:0 0 0 0 rgba(255, 179, 102, 0), 0 0 0 0 rgba(255, 179, 102, 0), inset 0 0 0 1px rgba(255, 179, 102, 0.4);
            box-shadow:0 0 0 0 rgba(255, 179, 102, 0), 0 0 0 0 rgba(255, 179, 102, 0), inset 0 0 0 1px rgba(255, 179, 102, 0.4); }
  .bp3-dark .bp3-editable-text.bp3-intent-warning.bp3-editable-text-editing::before{
    -webkit-box-shadow:0 0 0 1px #ffb366, 0 0 0 3px rgba(255, 179, 102, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px #ffb366, 0 0 0 3px rgba(255, 179, 102, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
  .bp3-dark .bp3-editable-text.bp3-intent-danger .bp3-editable-text-content{
    color:#ff7373; }
  .bp3-dark .bp3-editable-text.bp3-intent-danger:hover::before{
    -webkit-box-shadow:0 0 0 0 rgba(255, 115, 115, 0), 0 0 0 0 rgba(255, 115, 115, 0), inset 0 0 0 1px rgba(255, 115, 115, 0.4);
            box-shadow:0 0 0 0 rgba(255, 115, 115, 0), 0 0 0 0 rgba(255, 115, 115, 0), inset 0 0 0 1px rgba(255, 115, 115, 0.4); }
  .bp3-dark .bp3-editable-text.bp3-intent-danger.bp3-editable-text-editing::before{
    -webkit-box-shadow:0 0 0 1px #ff7373, 0 0 0 3px rgba(255, 115, 115, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px #ff7373, 0 0 0 3px rgba(255, 115, 115, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }

.bp3-editable-text-input,
.bp3-editable-text-content{
  color:inherit;
  display:inherit;
  font:inherit;
  letter-spacing:inherit;
  max-width:inherit;
  min-width:inherit;
  position:relative;
  resize:none;
  text-transform:inherit;
  vertical-align:top; }

.bp3-editable-text-input{
  background:none;
  border:none;
  -webkit-box-shadow:none;
          box-shadow:none;
  padding:0;
  white-space:pre-wrap;
  width:100%; }
  .bp3-editable-text-input::-webkit-input-placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-editable-text-input::-moz-placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-editable-text-input:-ms-input-placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-editable-text-input::-ms-input-placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-editable-text-input::placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-editable-text-input:focus{
    outline:none; }
  .bp3-editable-text-input::-ms-clear{
    display:none; }

.bp3-editable-text-content{
  overflow:hidden;
  padding-right:2px;
  text-overflow:ellipsis;
  white-space:pre; }
  .bp3-editable-text-editing > .bp3-editable-text-content{
    left:0;
    position:absolute;
    visibility:hidden; }
  .bp3-editable-text-placeholder > .bp3-editable-text-content{
    color:rgba(92, 112, 128, 0.6); }
    .bp3-dark .bp3-editable-text-placeholder > .bp3-editable-text-content{
      color:rgba(167, 182, 194, 0.6); }

.bp3-editable-text.bp3-multiline{
  display:block; }
  .bp3-editable-text.bp3-multiline .bp3-editable-text-content{
    overflow:auto;
    white-space:pre-wrap;
    word-wrap:break-word; }
.bp3-divider{
  border-bottom:1px solid rgba(16, 22, 26, 0.15);
  border-right:1px solid rgba(16, 22, 26, 0.15);
  margin:5px; }
  .bp3-dark .bp3-divider{
    border-color:rgba(16, 22, 26, 0.4); }
.bp3-control-group{
  -webkit-transform:translateZ(0);
          transform:translateZ(0);
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-orient:horizontal;
  -webkit-box-direction:normal;
      -ms-flex-direction:row;
          flex-direction:row;
  -webkit-box-align:stretch;
      -ms-flex-align:stretch;
          align-items:stretch; }
  .bp3-control-group > *{
    -webkit-box-flex:0;
        -ms-flex-positive:0;
            flex-grow:0;
    -ms-flex-negative:0;
        flex-shrink:0; }
  .bp3-control-group > .bp3-fill{
    -webkit-box-flex:1;
        -ms-flex-positive:1;
            flex-grow:1;
    -ms-flex-negative:1;
        flex-shrink:1; }
  .bp3-control-group .bp3-button,
  .bp3-control-group .bp3-html-select,
  .bp3-control-group .bp3-input,
  .bp3-control-group .bp3-select{
    position:relative; }
  .bp3-control-group .bp3-input{
    border-radius:inherit;
    z-index:2; }
    .bp3-control-group .bp3-input:focus{
      border-radius:3px;
      z-index:14; }
    .bp3-control-group .bp3-input[class*="bp3-intent"]{
      z-index:13; }
      .bp3-control-group .bp3-input[class*="bp3-intent"]:focus{
        z-index:15; }
    .bp3-control-group .bp3-input[readonly], .bp3-control-group .bp3-input:disabled, .bp3-control-group .bp3-input.bp3-disabled{
      z-index:1; }
  .bp3-control-group .bp3-input-group[class*="bp3-intent"] .bp3-input{
    z-index:13; }
    .bp3-control-group .bp3-input-group[class*="bp3-intent"] .bp3-input:focus{
      z-index:15; }
  .bp3-control-group .bp3-button,
  .bp3-control-group .bp3-html-select select,
  .bp3-control-group .bp3-select select{
    -webkit-transform:translateZ(0);
            transform:translateZ(0);
    border-radius:inherit;
    z-index:4; }
    .bp3-control-group .bp3-button:focus,
    .bp3-control-group .bp3-html-select select:focus,
    .bp3-control-group .bp3-select select:focus{
      z-index:5; }
    .bp3-control-group .bp3-button:hover,
    .bp3-control-group .bp3-html-select select:hover,
    .bp3-control-group .bp3-select select:hover{
      z-index:6; }
    .bp3-control-group .bp3-button:active,
    .bp3-control-group .bp3-html-select select:active,
    .bp3-control-group .bp3-select select:active{
      z-index:7; }
    .bp3-control-group .bp3-button[readonly], .bp3-control-group .bp3-button:disabled, .bp3-control-group .bp3-button.bp3-disabled,
    .bp3-control-group .bp3-html-select select[readonly],
    .bp3-control-group .bp3-html-select select:disabled,
    .bp3-control-group .bp3-html-select select.bp3-disabled,
    .bp3-control-group .bp3-select select[readonly],
    .bp3-control-group .bp3-select select:disabled,
    .bp3-control-group .bp3-select select.bp3-disabled{
      z-index:3; }
    .bp3-control-group .bp3-button[class*="bp3-intent"],
    .bp3-control-group .bp3-html-select select[class*="bp3-intent"],
    .bp3-control-group .bp3-select select[class*="bp3-intent"]{
      z-index:9; }
      .bp3-control-group .bp3-button[class*="bp3-intent"]:focus,
      .bp3-control-group .bp3-html-select select[class*="bp3-intent"]:focus,
      .bp3-control-group .bp3-select select[class*="bp3-intent"]:focus{
        z-index:10; }
      .bp3-control-group .bp3-button[class*="bp3-intent"]:hover,
      .bp3-control-group .bp3-html-select select[class*="bp3-intent"]:hover,
      .bp3-control-group .bp3-select select[class*="bp3-intent"]:hover{
        z-index:11; }
      .bp3-control-group .bp3-button[class*="bp3-intent"]:active,
      .bp3-control-group .bp3-html-select select[class*="bp3-intent"]:active,
      .bp3-control-group .bp3-select select[class*="bp3-intent"]:active{
        z-index:12; }
      .bp3-control-group .bp3-button[class*="bp3-intent"][readonly], .bp3-control-group .bp3-button[class*="bp3-intent"]:disabled, .bp3-control-group .bp3-button[class*="bp3-intent"].bp3-disabled,
      .bp3-control-group .bp3-html-select select[class*="bp3-intent"][readonly],
      .bp3-control-group .bp3-html-select select[class*="bp3-intent"]:disabled,
      .bp3-control-group .bp3-html-select select[class*="bp3-intent"].bp3-disabled,
      .bp3-control-group .bp3-select select[class*="bp3-intent"][readonly],
      .bp3-control-group .bp3-select select[class*="bp3-intent"]:disabled,
      .bp3-control-group .bp3-select select[class*="bp3-intent"].bp3-disabled{
        z-index:8; }
  .bp3-control-group .bp3-input-group > .bp3-icon,
  .bp3-control-group .bp3-input-group > .bp3-button,
  .bp3-control-group .bp3-input-group > .bp3-input-left-container,
  .bp3-control-group .bp3-input-group > .bp3-input-action{
    z-index:16; }
  .bp3-control-group .bp3-select::after,
  .bp3-control-group .bp3-html-select::after,
  .bp3-control-group .bp3-select > .bp3-icon,
  .bp3-control-group .bp3-html-select > .bp3-icon{
    z-index:17; }
  .bp3-control-group .bp3-select:focus-within{
    z-index:5; }
  .bp3-control-group:not(.bp3-vertical) > *:not(.bp3-divider){
    margin-right:-1px; }
  .bp3-control-group:not(.bp3-vertical) > .bp3-divider:not(:first-child){
    margin-left:6px; }
  .bp3-dark .bp3-control-group:not(.bp3-vertical) > *:not(.bp3-divider){
    margin-right:0; }
  .bp3-dark .bp3-control-group:not(.bp3-vertical) > .bp3-button + .bp3-button{
    margin-left:1px; }
  .bp3-control-group .bp3-popover-wrapper,
  .bp3-control-group .bp3-popover-target{
    border-radius:inherit; }
  .bp3-control-group > :first-child{
    border-radius:3px 0 0 3px; }
  .bp3-control-group > :last-child{
    border-radius:0 3px 3px 0;
    margin-right:0; }
  .bp3-control-group > :only-child{
    border-radius:3px;
    margin-right:0; }
  .bp3-control-group .bp3-input-group .bp3-button{
    border-radius:3px; }
  .bp3-control-group .bp3-numeric-input:not(:first-child) .bp3-input-group{
    border-bottom-left-radius:0;
    border-top-left-radius:0; }
  .bp3-control-group.bp3-fill{
    width:100%; }
  .bp3-control-group > .bp3-fill{
    -webkit-box-flex:1;
        -ms-flex:1 1 auto;
            flex:1 1 auto; }
  .bp3-control-group.bp3-fill > *:not(.bp3-fixed){
    -webkit-box-flex:1;
        -ms-flex:1 1 auto;
            flex:1 1 auto; }
  .bp3-control-group.bp3-vertical{
    -webkit-box-orient:vertical;
    -webkit-box-direction:normal;
        -ms-flex-direction:column;
            flex-direction:column; }
    .bp3-control-group.bp3-vertical > *{
      margin-top:-1px; }
    .bp3-control-group.bp3-vertical > :first-child{
      border-radius:3px 3px 0 0;
      margin-top:0; }
    .bp3-control-group.bp3-vertical > :last-child{
      border-radius:0 0 3px 3px; }
.bp3-control{
  cursor:pointer;
  display:block;
  margin-bottom:10px;
  position:relative;
  text-transform:none; }
  .bp3-control input:checked ~ .bp3-control-indicator{
    background-color:#137cbd;
    background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.1)), to(rgba(255, 255, 255, 0)));
    background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.1), rgba(255, 255, 255, 0));
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
    color:#ffffff; }
  .bp3-control:hover input:checked ~ .bp3-control-indicator{
    background-color:#106ba3;
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2); }
  .bp3-control input:not(:disabled):active:checked ~ .bp3-control-indicator{
    background:#0e5a8a;
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
  .bp3-control input:disabled:checked ~ .bp3-control-indicator{
    background:rgba(19, 124, 189, 0.5);
    -webkit-box-shadow:none;
            box-shadow:none; }
  .bp3-dark .bp3-control input:checked ~ .bp3-control-indicator{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
  .bp3-dark .bp3-control:hover input:checked ~ .bp3-control-indicator{
    background-color:#106ba3;
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
  .bp3-dark .bp3-control input:not(:disabled):active:checked ~ .bp3-control-indicator{
    background-color:#0e5a8a;
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
  .bp3-dark .bp3-control input:disabled:checked ~ .bp3-control-indicator{
    background:rgba(14, 90, 138, 0.5);
    -webkit-box-shadow:none;
            box-shadow:none; }
  .bp3-control:not(.bp3-align-right){
    padding-left:26px; }
    .bp3-control:not(.bp3-align-right) .bp3-control-indicator{
      margin-left:-26px; }
  .bp3-control.bp3-align-right{
    padding-right:26px; }
    .bp3-control.bp3-align-right .bp3-control-indicator{
      margin-right:-26px; }
  .bp3-control.bp3-disabled{
    color:rgba(92, 112, 128, 0.6);
    cursor:not-allowed; }
  .bp3-control.bp3-inline{
    display:inline-block;
    margin-right:20px; }
  .bp3-control input{
    left:0;
    opacity:0;
    position:absolute;
    top:0;
    z-index:-1; }
  .bp3-control .bp3-control-indicator{
    background-clip:padding-box;
    background-color:#f5f8fa;
    background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.8)), to(rgba(255, 255, 255, 0)));
    background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.8), rgba(255, 255, 255, 0));
    border:none;
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
    cursor:pointer;
    display:inline-block;
    font-size:16px;
    height:1em;
    margin-right:10px;
    margin-top:-3px;
    position:relative;
    -webkit-user-select:none;
       -moz-user-select:none;
        -ms-user-select:none;
            user-select:none;
    vertical-align:middle;
    width:1em; }
    .bp3-control .bp3-control-indicator::before{
      content:"";
      display:block;
      height:1em;
      width:1em; }
  .bp3-control:hover .bp3-control-indicator{
    background-color:#ebf1f5; }
  .bp3-control input:not(:disabled):active ~ .bp3-control-indicator{
    background:#d8e1e8;
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
  .bp3-control input:disabled ~ .bp3-control-indicator{
    background:rgba(206, 217, 224, 0.5);
    -webkit-box-shadow:none;
            box-shadow:none;
    cursor:not-allowed; }
  .bp3-control input:focus ~ .bp3-control-indicator{
    outline:rgba(19, 124, 189, 0.6) auto 2px;
    outline-offset:2px;
    -moz-outline-radius:6px; }
  .bp3-control.bp3-align-right .bp3-control-indicator{
    float:right;
    margin-left:10px;
    margin-top:1px; }
  .bp3-control.bp3-large{
    font-size:16px; }
    .bp3-control.bp3-large:not(.bp3-align-right){
      padding-left:30px; }
      .bp3-control.bp3-large:not(.bp3-align-right) .bp3-control-indicator{
        margin-left:-30px; }
    .bp3-control.bp3-large.bp3-align-right{
      padding-right:30px; }
      .bp3-control.bp3-large.bp3-align-right .bp3-control-indicator{
        margin-right:-30px; }
    .bp3-control.bp3-large .bp3-control-indicator{
      font-size:20px; }
    .bp3-control.bp3-large.bp3-align-right .bp3-control-indicator{
      margin-top:0; }
  .bp3-control.bp3-checkbox input:indeterminate ~ .bp3-control-indicator{
    background-color:#137cbd;
    background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.1)), to(rgba(255, 255, 255, 0)));
    background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.1), rgba(255, 255, 255, 0));
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
    color:#ffffff; }
  .bp3-control.bp3-checkbox:hover input:indeterminate ~ .bp3-control-indicator{
    background-color:#106ba3;
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2); }
  .bp3-control.bp3-checkbox input:not(:disabled):active:indeterminate ~ .bp3-control-indicator{
    background:#0e5a8a;
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
  .bp3-control.bp3-checkbox input:disabled:indeterminate ~ .bp3-control-indicator{
    background:rgba(19, 124, 189, 0.5);
    -webkit-box-shadow:none;
            box-shadow:none; }
  .bp3-dark .bp3-control.bp3-checkbox input:indeterminate ~ .bp3-control-indicator{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
  .bp3-dark .bp3-control.bp3-checkbox:hover input:indeterminate ~ .bp3-control-indicator{
    background-color:#106ba3;
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
  .bp3-dark .bp3-control.bp3-checkbox input:not(:disabled):active:indeterminate ~ .bp3-control-indicator{
    background-color:#0e5a8a;
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
  .bp3-dark .bp3-control.bp3-checkbox input:disabled:indeterminate ~ .bp3-control-indicator{
    background:rgba(14, 90, 138, 0.5);
    -webkit-box-shadow:none;
            box-shadow:none; }
  .bp3-control.bp3-checkbox .bp3-control-indicator{
    border-radius:3px; }
  .bp3-control.bp3-checkbox input:checked ~ .bp3-control-indicator::before{
    background-image:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16'%3e%3cpath fill-rule='evenodd' clip-rule='evenodd' d='M12 5c-.28 0-.53.11-.71.29L7 9.59l-2.29-2.3a1.003 1.003 0 00-1.42 1.42l3 3c.18.18.43.29.71.29s.53-.11.71-.29l5-5A1.003 1.003 0 0012 5z' fill='white'/%3e%3c/svg%3e"); }
  .bp3-control.bp3-checkbox input:indeterminate ~ .bp3-control-indicator::before{
    background-image:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16'%3e%3cpath fill-rule='evenodd' clip-rule='evenodd' d='M11 7H5c-.55 0-1 .45-1 1s.45 1 1 1h6c.55 0 1-.45 1-1s-.45-1-1-1z' fill='white'/%3e%3c/svg%3e"); }
  .bp3-control.bp3-radio .bp3-control-indicator{
    border-radius:50%; }
  .bp3-control.bp3-radio input:checked ~ .bp3-control-indicator::before{
    background-image:radial-gradient(#ffffff, #ffffff 28%, transparent 32%); }
  .bp3-control.bp3-radio input:checked:disabled ~ .bp3-control-indicator::before{
    opacity:0.5; }
  .bp3-control.bp3-radio input:focus ~ .bp3-control-indicator{
    -moz-outline-radius:16px; }
  .bp3-control.bp3-switch input ~ .bp3-control-indicator{
    background:rgba(167, 182, 194, 0.5); }
  .bp3-control.bp3-switch:hover input ~ .bp3-control-indicator{
    background:rgba(115, 134, 148, 0.5); }
  .bp3-control.bp3-switch input:not(:disabled):active ~ .bp3-control-indicator{
    background:rgba(92, 112, 128, 0.5); }
  .bp3-control.bp3-switch input:disabled ~ .bp3-control-indicator{
    background:rgba(206, 217, 224, 0.5); }
    .bp3-control.bp3-switch input:disabled ~ .bp3-control-indicator::before{
      background:rgba(255, 255, 255, 0.8); }
  .bp3-control.bp3-switch input:checked ~ .bp3-control-indicator{
    background:#137cbd; }
  .bp3-control.bp3-switch:hover input:checked ~ .bp3-control-indicator{
    background:#106ba3; }
  .bp3-control.bp3-switch input:checked:not(:disabled):active ~ .bp3-control-indicator{
    background:#0e5a8a; }
  .bp3-control.bp3-switch input:checked:disabled ~ .bp3-control-indicator{
    background:rgba(19, 124, 189, 0.5); }
    .bp3-control.bp3-switch input:checked:disabled ~ .bp3-control-indicator::before{
      background:rgba(255, 255, 255, 0.8); }
  .bp3-control.bp3-switch:not(.bp3-align-right){
    padding-left:38px; }
    .bp3-control.bp3-switch:not(.bp3-align-right) .bp3-control-indicator{
      margin-left:-38px; }
  .bp3-control.bp3-switch.bp3-align-right{
    padding-right:38px; }
    .bp3-control.bp3-switch.bp3-align-right .bp3-control-indicator{
      margin-right:-38px; }
  .bp3-control.bp3-switch .bp3-control-indicator{
    border:none;
    border-radius:1.75em;
    -webkit-box-shadow:none !important;
            box-shadow:none !important;
    min-width:1.75em;
    -webkit-transition:background-color 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
    transition:background-color 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
    width:auto; }
    .bp3-control.bp3-switch .bp3-control-indicator::before{
      background:#ffffff;
      border-radius:50%;
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 1px 1px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 1px 1px rgba(16, 22, 26, 0.2);
      height:calc(1em - 4px);
      left:0;
      margin:2px;
      position:absolute;
      -webkit-transition:left 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
      transition:left 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
      width:calc(1em - 4px); }
  .bp3-control.bp3-switch input:checked ~ .bp3-control-indicator::before{
    left:calc(100% - 1em); }
  .bp3-control.bp3-switch.bp3-large:not(.bp3-align-right){
    padding-left:45px; }
    .bp3-control.bp3-switch.bp3-large:not(.bp3-align-right) .bp3-control-indicator{
      margin-left:-45px; }
  .bp3-control.bp3-switch.bp3-large.bp3-align-right{
    padding-right:45px; }
    .bp3-control.bp3-switch.bp3-large.bp3-align-right .bp3-control-indicator{
      margin-right:-45px; }
  .bp3-dark .bp3-control.bp3-switch input ~ .bp3-control-indicator{
    background:rgba(16, 22, 26, 0.5); }
  .bp3-dark .bp3-control.bp3-switch:hover input ~ .bp3-control-indicator{
    background:rgba(16, 22, 26, 0.7); }
  .bp3-dark .bp3-control.bp3-switch input:not(:disabled):active ~ .bp3-control-indicator{
    background:rgba(16, 22, 26, 0.9); }
  .bp3-dark .bp3-control.bp3-switch input:disabled ~ .bp3-control-indicator{
    background:rgba(57, 75, 89, 0.5); }
    .bp3-dark .bp3-control.bp3-switch input:disabled ~ .bp3-control-indicator::before{
      background:rgba(16, 22, 26, 0.4); }
  .bp3-dark .bp3-control.bp3-switch input:checked ~ .bp3-control-indicator{
    background:#137cbd; }
  .bp3-dark .bp3-control.bp3-switch:hover input:checked ~ .bp3-control-indicator{
    background:#106ba3; }
  .bp3-dark .bp3-control.bp3-switch input:checked:not(:disabled):active ~ .bp3-control-indicator{
    background:#0e5a8a; }
  .bp3-dark .bp3-control.bp3-switch input:checked:disabled ~ .bp3-control-indicator{
    background:rgba(14, 90, 138, 0.5); }
    .bp3-dark .bp3-control.bp3-switch input:checked:disabled ~ .bp3-control-indicator::before{
      background:rgba(16, 22, 26, 0.4); }
  .bp3-dark .bp3-control.bp3-switch .bp3-control-indicator::before{
    background:#394b59;
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
  .bp3-dark .bp3-control.bp3-switch input:checked ~ .bp3-control-indicator::before{
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4); }
  .bp3-control.bp3-switch .bp3-switch-inner-text{
    font-size:0.7em;
    text-align:center; }
  .bp3-control.bp3-switch .bp3-control-indicator-child:first-child{
    line-height:0;
    margin-left:0.5em;
    margin-right:1.2em;
    visibility:hidden; }
  .bp3-control.bp3-switch .bp3-control-indicator-child:last-child{
    line-height:1em;
    margin-left:1.2em;
    margin-right:0.5em;
    visibility:visible; }
  .bp3-control.bp3-switch input:checked ~ .bp3-control-indicator .bp3-control-indicator-child:first-child{
    line-height:1em;
    visibility:visible; }
  .bp3-control.bp3-switch input:checked ~ .bp3-control-indicator .bp3-control-indicator-child:last-child{
    line-height:0;
    visibility:hidden; }
  .bp3-dark .bp3-control{
    color:#f5f8fa; }
    .bp3-dark .bp3-control.bp3-disabled{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-control .bp3-control-indicator{
      background-color:#394b59;
      background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.05)), to(rgba(255, 255, 255, 0)));
      background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.05), rgba(255, 255, 255, 0));
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-control:hover .bp3-control-indicator{
      background-color:#30404d; }
    .bp3-dark .bp3-control input:not(:disabled):active ~ .bp3-control-indicator{
      background:#202b33;
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
    .bp3-dark .bp3-control input:disabled ~ .bp3-control-indicator{
      background:rgba(57, 75, 89, 0.5);
      -webkit-box-shadow:none;
              box-shadow:none;
      cursor:not-allowed; }
    .bp3-dark .bp3-control.bp3-checkbox input:disabled:checked ~ .bp3-control-indicator, .bp3-dark .bp3-control.bp3-checkbox input:disabled:indeterminate ~ .bp3-control-indicator{
      color:rgba(167, 182, 194, 0.6); }
.bp3-file-input{
  cursor:pointer;
  display:inline-block;
  height:30px;
  position:relative; }
  .bp3-file-input input{
    margin:0;
    min-width:200px;
    opacity:0; }
    .bp3-file-input input:disabled + .bp3-file-upload-input,
    .bp3-file-input input.bp3-disabled + .bp3-file-upload-input{
      background:rgba(206, 217, 224, 0.5);
      -webkit-box-shadow:none;
              box-shadow:none;
      color:rgba(92, 112, 128, 0.6);
      cursor:not-allowed;
      resize:none; }
      .bp3-file-input input:disabled + .bp3-file-upload-input::after,
      .bp3-file-input input.bp3-disabled + .bp3-file-upload-input::after{
        background-color:rgba(206, 217, 224, 0.5);
        background-image:none;
        -webkit-box-shadow:none;
                box-shadow:none;
        color:rgba(92, 112, 128, 0.6);
        cursor:not-allowed;
        outline:none; }
        .bp3-file-input input:disabled + .bp3-file-upload-input::after.bp3-active, .bp3-file-input input:disabled + .bp3-file-upload-input::after.bp3-active:hover,
        .bp3-file-input input.bp3-disabled + .bp3-file-upload-input::after.bp3-active,
        .bp3-file-input input.bp3-disabled + .bp3-file-upload-input::after.bp3-active:hover{
          background:rgba(206, 217, 224, 0.7); }
      .bp3-dark .bp3-file-input input:disabled + .bp3-file-upload-input, .bp3-dark
      .bp3-file-input input.bp3-disabled + .bp3-file-upload-input{
        background:rgba(57, 75, 89, 0.5);
        -webkit-box-shadow:none;
                box-shadow:none;
        color:rgba(167, 182, 194, 0.6); }
        .bp3-dark .bp3-file-input input:disabled + .bp3-file-upload-input::after, .bp3-dark
        .bp3-file-input input.bp3-disabled + .bp3-file-upload-input::after{
          background-color:rgba(57, 75, 89, 0.5);
          background-image:none;
          -webkit-box-shadow:none;
                  box-shadow:none;
          color:rgba(167, 182, 194, 0.6); }
          .bp3-dark .bp3-file-input input:disabled + .bp3-file-upload-input::after.bp3-active, .bp3-dark
          .bp3-file-input input.bp3-disabled + .bp3-file-upload-input::after.bp3-active{
            background:rgba(57, 75, 89, 0.7); }
  .bp3-file-input.bp3-file-input-has-selection .bp3-file-upload-input{
    color:#182026; }
  .bp3-dark .bp3-file-input.bp3-file-input-has-selection .bp3-file-upload-input{
    color:#f5f8fa; }
  .bp3-file-input.bp3-fill{
    width:100%; }
  .bp3-file-input.bp3-large,
  .bp3-large .bp3-file-input{
    height:40px; }
  .bp3-file-input .bp3-file-upload-input-custom-text::after{
    content:attr(bp3-button-text); }

.bp3-file-upload-input{
  -webkit-appearance:none;
     -moz-appearance:none;
          appearance:none;
  background:#ffffff;
  border:none;
  border-radius:3px;
  -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
  color:#182026;
  font-size:14px;
  font-weight:400;
  height:30px;
  line-height:30px;
  outline:none;
  padding:0 10px;
  -webkit-transition:-webkit-box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
  transition:-webkit-box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
  transition:box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
  transition:box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
  vertical-align:middle;
  overflow:hidden;
  text-overflow:ellipsis;
  white-space:nowrap;
  word-wrap:normal;
  color:rgba(92, 112, 128, 0.6);
  left:0;
  padding-right:80px;
  position:absolute;
  right:0;
  top:0;
  -webkit-user-select:none;
     -moz-user-select:none;
      -ms-user-select:none;
          user-select:none; }
  .bp3-file-upload-input::-webkit-input-placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-file-upload-input::-moz-placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-file-upload-input:-ms-input-placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-file-upload-input::-ms-input-placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-file-upload-input::placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-file-upload-input:focus, .bp3-file-upload-input.bp3-active{
    -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
  .bp3-file-upload-input[type="search"], .bp3-file-upload-input.bp3-round{
    border-radius:30px;
    -webkit-box-sizing:border-box;
            box-sizing:border-box;
    padding-left:10px; }
  .bp3-file-upload-input[readonly]{
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.15);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.15); }
  .bp3-file-upload-input:disabled, .bp3-file-upload-input.bp3-disabled{
    background:rgba(206, 217, 224, 0.5);
    -webkit-box-shadow:none;
            box-shadow:none;
    color:rgba(92, 112, 128, 0.6);
    cursor:not-allowed;
    resize:none; }
  .bp3-file-upload-input::after{
    background-color:#f5f8fa;
    background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.8)), to(rgba(255, 255, 255, 0)));
    background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.8), rgba(255, 255, 255, 0));
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
    color:#182026;
    min-height:24px;
    min-width:24px;
    overflow:hidden;
    text-overflow:ellipsis;
    white-space:nowrap;
    word-wrap:normal;
    border-radius:3px;
    content:"Browse";
    line-height:24px;
    margin:3px;
    position:absolute;
    right:0;
    text-align:center;
    top:0;
    width:70px; }
    .bp3-file-upload-input::after:hover{
      background-clip:padding-box;
      background-color:#ebf1f5;
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1); }
    .bp3-file-upload-input::after:active, .bp3-file-upload-input::after.bp3-active{
      background-color:#d8e1e8;
      background-image:none;
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
    .bp3-file-upload-input::after:disabled, .bp3-file-upload-input::after.bp3-disabled{
      background-color:rgba(206, 217, 224, 0.5);
      background-image:none;
      -webkit-box-shadow:none;
              box-shadow:none;
      color:rgba(92, 112, 128, 0.6);
      cursor:not-allowed;
      outline:none; }
      .bp3-file-upload-input::after:disabled.bp3-active, .bp3-file-upload-input::after:disabled.bp3-active:hover, .bp3-file-upload-input::after.bp3-disabled.bp3-active, .bp3-file-upload-input::after.bp3-disabled.bp3-active:hover{
        background:rgba(206, 217, 224, 0.7); }
  .bp3-file-upload-input:hover::after{
    background-clip:padding-box;
    background-color:#ebf1f5;
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1); }
  .bp3-file-upload-input:active::after{
    background-color:#d8e1e8;
    background-image:none;
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
  .bp3-large .bp3-file-upload-input{
    font-size:16px;
    height:40px;
    line-height:40px;
    padding-right:95px; }
    .bp3-large .bp3-file-upload-input[type="search"], .bp3-large .bp3-file-upload-input.bp3-round{
      padding:0 15px; }
    .bp3-large .bp3-file-upload-input::after{
      min-height:30px;
      min-width:30px;
      line-height:30px;
      margin:5px;
      width:85px; }
  .bp3-dark .bp3-file-upload-input{
    background:rgba(16, 22, 26, 0.3);
    -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
    color:#f5f8fa;
    color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-file-upload-input::-webkit-input-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-file-upload-input::-moz-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-file-upload-input:-ms-input-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-file-upload-input::-ms-input-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-file-upload-input::placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-file-upload-input:focus{
      -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px #137cbd, 0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-file-upload-input[readonly]{
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-file-upload-input:disabled, .bp3-dark .bp3-file-upload-input.bp3-disabled{
      background:rgba(57, 75, 89, 0.5);
      -webkit-box-shadow:none;
              box-shadow:none;
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-file-upload-input::after{
      background-color:#394b59;
      background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.05)), to(rgba(255, 255, 255, 0)));
      background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.05), rgba(255, 255, 255, 0));
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
      color:#f5f8fa; }
      .bp3-dark .bp3-file-upload-input::after:hover, .bp3-dark .bp3-file-upload-input::after:active, .bp3-dark .bp3-file-upload-input::after.bp3-active{
        color:#f5f8fa; }
      .bp3-dark .bp3-file-upload-input::after:hover{
        background-color:#30404d;
        -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
                box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
      .bp3-dark .bp3-file-upload-input::after:active, .bp3-dark .bp3-file-upload-input::after.bp3-active{
        background-color:#202b33;
        background-image:none;
        -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2);
                box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
      .bp3-dark .bp3-file-upload-input::after:disabled, .bp3-dark .bp3-file-upload-input::after.bp3-disabled{
        background-color:rgba(57, 75, 89, 0.5);
        background-image:none;
        -webkit-box-shadow:none;
                box-shadow:none;
        color:rgba(167, 182, 194, 0.6); }
        .bp3-dark .bp3-file-upload-input::after:disabled.bp3-active, .bp3-dark .bp3-file-upload-input::after.bp3-disabled.bp3-active{
          background:rgba(57, 75, 89, 0.7); }
      .bp3-dark .bp3-file-upload-input::after .bp3-button-spinner .bp3-spinner-head{
        background:rgba(16, 22, 26, 0.5);
        stroke:#8a9ba8; }
    .bp3-dark .bp3-file-upload-input:hover::after{
      background-color:#30404d;
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-file-upload-input:active::after{
      background-color:#202b33;
      background-image:none;
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
.bp3-file-upload-input::after{
  -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
          box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1); }
.bp3-form-group{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-orient:vertical;
  -webkit-box-direction:normal;
      -ms-flex-direction:column;
          flex-direction:column;
  margin:0 0 15px; }
  .bp3-form-group label.bp3-label{
    margin-bottom:5px; }
  .bp3-form-group .bp3-control{
    margin-top:7px; }
  .bp3-form-group .bp3-form-helper-text{
    color:#5c7080;
    font-size:12px;
    margin-top:5px; }
  .bp3-form-group.bp3-intent-primary .bp3-form-helper-text{
    color:#106ba3; }
  .bp3-form-group.bp3-intent-success .bp3-form-helper-text{
    color:#0d8050; }
  .bp3-form-group.bp3-intent-warning .bp3-form-helper-text{
    color:#bf7326; }
  .bp3-form-group.bp3-intent-danger .bp3-form-helper-text{
    color:#c23030; }
  .bp3-form-group.bp3-inline{
    -webkit-box-align:start;
        -ms-flex-align:start;
            align-items:flex-start;
    -webkit-box-orient:horizontal;
    -webkit-box-direction:normal;
        -ms-flex-direction:row;
            flex-direction:row; }
    .bp3-form-group.bp3-inline.bp3-large label.bp3-label{
      line-height:40px;
      margin:0 10px 0 0; }
    .bp3-form-group.bp3-inline label.bp3-label{
      line-height:30px;
      margin:0 10px 0 0; }
  .bp3-form-group.bp3-disabled .bp3-label,
  .bp3-form-group.bp3-disabled .bp3-text-muted,
  .bp3-form-group.bp3-disabled .bp3-form-helper-text{
    color:rgba(92, 112, 128, 0.6) !important; }
  .bp3-dark .bp3-form-group.bp3-intent-primary .bp3-form-helper-text{
    color:#48aff0; }
  .bp3-dark .bp3-form-group.bp3-intent-success .bp3-form-helper-text{
    color:#3dcc91; }
  .bp3-dark .bp3-form-group.bp3-intent-warning .bp3-form-helper-text{
    color:#ffb366; }
  .bp3-dark .bp3-form-group.bp3-intent-danger .bp3-form-helper-text{
    color:#ff7373; }
  .bp3-dark .bp3-form-group .bp3-form-helper-text{
    color:#a7b6c2; }
  .bp3-dark .bp3-form-group.bp3-disabled .bp3-label,
  .bp3-dark .bp3-form-group.bp3-disabled .bp3-text-muted,
  .bp3-dark .bp3-form-group.bp3-disabled .bp3-form-helper-text{
    color:rgba(167, 182, 194, 0.6) !important; }
.bp3-input-group{
  display:block;
  position:relative; }
  .bp3-input-group .bp3-input{
    position:relative;
    width:100%; }
    .bp3-input-group .bp3-input:not(:first-child){
      padding-left:30px; }
    .bp3-input-group .bp3-input:not(:last-child){
      padding-right:30px; }
  .bp3-input-group .bp3-input-action,
  .bp3-input-group > .bp3-input-left-container,
  .bp3-input-group > .bp3-button,
  .bp3-input-group > .bp3-icon{
    position:absolute;
    top:0; }
    .bp3-input-group .bp3-input-action:first-child,
    .bp3-input-group > .bp3-input-left-container:first-child,
    .bp3-input-group > .bp3-button:first-child,
    .bp3-input-group > .bp3-icon:first-child{
      left:0; }
    .bp3-input-group .bp3-input-action:last-child,
    .bp3-input-group > .bp3-input-left-container:last-child,
    .bp3-input-group > .bp3-button:last-child,
    .bp3-input-group > .bp3-icon:last-child{
      right:0; }
  .bp3-input-group .bp3-button{
    min-height:24px;
    min-width:24px;
    margin:3px;
    padding:0 7px; }
    .bp3-input-group .bp3-button:empty{
      padding:0; }
  .bp3-input-group > .bp3-input-left-container,
  .bp3-input-group > .bp3-icon{
    z-index:1; }
  .bp3-input-group > .bp3-input-left-container > .bp3-icon,
  .bp3-input-group > .bp3-icon{
    color:#5c7080; }
    .bp3-input-group > .bp3-input-left-container > .bp3-icon:empty,
    .bp3-input-group > .bp3-icon:empty{
      font-family:"Icons16", sans-serif;
      font-size:16px;
      font-style:normal;
      font-weight:400;
      line-height:1;
      -moz-osx-font-smoothing:grayscale;
      -webkit-font-smoothing:antialiased; }
  .bp3-input-group > .bp3-input-left-container > .bp3-icon,
  .bp3-input-group > .bp3-icon,
  .bp3-input-group .bp3-input-action > .bp3-spinner{
    margin:7px; }
  .bp3-input-group .bp3-tag{
    margin:5px; }
  .bp3-input-group .bp3-input:not(:focus) + .bp3-button.bp3-minimal:not(:hover):not(:focus),
  .bp3-input-group .bp3-input:not(:focus) + .bp3-input-action .bp3-button.bp3-minimal:not(:hover):not(:focus){
    color:#5c7080; }
    .bp3-dark .bp3-input-group .bp3-input:not(:focus) + .bp3-button.bp3-minimal:not(:hover):not(:focus), .bp3-dark
    .bp3-input-group .bp3-input:not(:focus) + .bp3-input-action .bp3-button.bp3-minimal:not(:hover):not(:focus){
      color:#a7b6c2; }
    .bp3-input-group .bp3-input:not(:focus) + .bp3-button.bp3-minimal:not(:hover):not(:focus) .bp3-icon, .bp3-input-group .bp3-input:not(:focus) + .bp3-button.bp3-minimal:not(:hover):not(:focus) .bp3-icon-standard, .bp3-input-group .bp3-input:not(:focus) + .bp3-button.bp3-minimal:not(:hover):not(:focus) .bp3-icon-large,
    .bp3-input-group .bp3-input:not(:focus) + .bp3-input-action .bp3-button.bp3-minimal:not(:hover):not(:focus) .bp3-icon,
    .bp3-input-group .bp3-input:not(:focus) + .bp3-input-action .bp3-button.bp3-minimal:not(:hover):not(:focus) .bp3-icon-standard,
    .bp3-input-group .bp3-input:not(:focus) + .bp3-input-action .bp3-button.bp3-minimal:not(:hover):not(:focus) .bp3-icon-large{
      color:#5c7080; }
  .bp3-input-group .bp3-input:not(:focus) + .bp3-button.bp3-minimal:disabled,
  .bp3-input-group .bp3-input:not(:focus) + .bp3-input-action .bp3-button.bp3-minimal:disabled{
    color:rgba(92, 112, 128, 0.6) !important; }
    .bp3-input-group .bp3-input:not(:focus) + .bp3-button.bp3-minimal:disabled .bp3-icon, .bp3-input-group .bp3-input:not(:focus) + .bp3-button.bp3-minimal:disabled .bp3-icon-standard, .bp3-input-group .bp3-input:not(:focus) + .bp3-button.bp3-minimal:disabled .bp3-icon-large,
    .bp3-input-group .bp3-input:not(:focus) + .bp3-input-action .bp3-button.bp3-minimal:disabled .bp3-icon,
    .bp3-input-group .bp3-input:not(:focus) + .bp3-input-action .bp3-button.bp3-minimal:disabled .bp3-icon-standard,
    .bp3-input-group .bp3-input:not(:focus) + .bp3-input-action .bp3-button.bp3-minimal:disabled .bp3-icon-large{
      color:rgba(92, 112, 128, 0.6) !important; }
  .bp3-input-group.bp3-disabled{
    cursor:not-allowed; }
    .bp3-input-group.bp3-disabled .bp3-icon{
      color:rgba(92, 112, 128, 0.6); }
  .bp3-input-group.bp3-large .bp3-button{
    min-height:30px;
    min-width:30px;
    margin:5px; }
  .bp3-input-group.bp3-large > .bp3-input-left-container > .bp3-icon,
  .bp3-input-group.bp3-large > .bp3-icon,
  .bp3-input-group.bp3-large .bp3-input-action > .bp3-spinner{
    margin:12px; }
  .bp3-input-group.bp3-large .bp3-input{
    font-size:16px;
    height:40px;
    line-height:40px; }
    .bp3-input-group.bp3-large .bp3-input[type="search"], .bp3-input-group.bp3-large .bp3-input.bp3-round{
      padding:0 15px; }
    .bp3-input-group.bp3-large .bp3-input:not(:first-child){
      padding-left:40px; }
    .bp3-input-group.bp3-large .bp3-input:not(:last-child){
      padding-right:40px; }
  .bp3-input-group.bp3-small .bp3-button{
    min-height:20px;
    min-width:20px;
    margin:2px; }
  .bp3-input-group.bp3-small .bp3-tag{
    min-height:20px;
    min-width:20px;
    margin:2px; }
  .bp3-input-group.bp3-small > .bp3-input-left-container > .bp3-icon,
  .bp3-input-group.bp3-small > .bp3-icon,
  .bp3-input-group.bp3-small .bp3-input-action > .bp3-spinner{
    margin:4px; }
  .bp3-input-group.bp3-small .bp3-input{
    font-size:12px;
    height:24px;
    line-height:24px;
    padding-left:8px;
    padding-right:8px; }
    .bp3-input-group.bp3-small .bp3-input[type="search"], .bp3-input-group.bp3-small .bp3-input.bp3-round{
      padding:0 12px; }
    .bp3-input-group.bp3-small .bp3-input:not(:first-child){
      padding-left:24px; }
    .bp3-input-group.bp3-small .bp3-input:not(:last-child){
      padding-right:24px; }
  .bp3-input-group.bp3-fill{
    -webkit-box-flex:1;
        -ms-flex:1 1 auto;
            flex:1 1 auto;
    width:100%; }
  .bp3-input-group.bp3-round .bp3-button,
  .bp3-input-group.bp3-round .bp3-input,
  .bp3-input-group.bp3-round .bp3-tag{
    border-radius:30px; }
  .bp3-dark .bp3-input-group .bp3-icon{
    color:#a7b6c2; }
  .bp3-dark .bp3-input-group.bp3-disabled .bp3-icon{
    color:rgba(167, 182, 194, 0.6); }
  .bp3-input-group.bp3-intent-primary .bp3-input{
    -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px #137cbd, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px #137cbd, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input-group.bp3-intent-primary .bp3-input:focus{
      -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input-group.bp3-intent-primary .bp3-input[readonly]{
      -webkit-box-shadow:inset 0 0 0 1px #137cbd;
              box-shadow:inset 0 0 0 1px #137cbd; }
    .bp3-input-group.bp3-intent-primary .bp3-input:disabled, .bp3-input-group.bp3-intent-primary .bp3-input.bp3-disabled{
      -webkit-box-shadow:none;
              box-shadow:none; }
  .bp3-input-group.bp3-intent-primary > .bp3-icon{
    color:#106ba3; }
    .bp3-dark .bp3-input-group.bp3-intent-primary > .bp3-icon{
      color:#48aff0; }
  .bp3-input-group.bp3-intent-success .bp3-input{
    -webkit-box-shadow:0 0 0 0 rgba(15, 153, 96, 0), 0 0 0 0 rgba(15, 153, 96, 0), inset 0 0 0 1px #0f9960, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 0 rgba(15, 153, 96, 0), 0 0 0 0 rgba(15, 153, 96, 0), inset 0 0 0 1px #0f9960, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input-group.bp3-intent-success .bp3-input:focus{
      -webkit-box-shadow:0 0 0 1px #0f9960, 0 0 0 3px rgba(15, 153, 96, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px #0f9960, 0 0 0 3px rgba(15, 153, 96, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input-group.bp3-intent-success .bp3-input[readonly]{
      -webkit-box-shadow:inset 0 0 0 1px #0f9960;
              box-shadow:inset 0 0 0 1px #0f9960; }
    .bp3-input-group.bp3-intent-success .bp3-input:disabled, .bp3-input-group.bp3-intent-success .bp3-input.bp3-disabled{
      -webkit-box-shadow:none;
              box-shadow:none; }
  .bp3-input-group.bp3-intent-success > .bp3-icon{
    color:#0d8050; }
    .bp3-dark .bp3-input-group.bp3-intent-success > .bp3-icon{
      color:#3dcc91; }
  .bp3-input-group.bp3-intent-warning .bp3-input{
    -webkit-box-shadow:0 0 0 0 rgba(217, 130, 43, 0), 0 0 0 0 rgba(217, 130, 43, 0), inset 0 0 0 1px #d9822b, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 0 rgba(217, 130, 43, 0), 0 0 0 0 rgba(217, 130, 43, 0), inset 0 0 0 1px #d9822b, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input-group.bp3-intent-warning .bp3-input:focus{
      -webkit-box-shadow:0 0 0 1px #d9822b, 0 0 0 3px rgba(217, 130, 43, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px #d9822b, 0 0 0 3px rgba(217, 130, 43, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input-group.bp3-intent-warning .bp3-input[readonly]{
      -webkit-box-shadow:inset 0 0 0 1px #d9822b;
              box-shadow:inset 0 0 0 1px #d9822b; }
    .bp3-input-group.bp3-intent-warning .bp3-input:disabled, .bp3-input-group.bp3-intent-warning .bp3-input.bp3-disabled{
      -webkit-box-shadow:none;
              box-shadow:none; }
  .bp3-input-group.bp3-intent-warning > .bp3-icon{
    color:#bf7326; }
    .bp3-dark .bp3-input-group.bp3-intent-warning > .bp3-icon{
      color:#ffb366; }
  .bp3-input-group.bp3-intent-danger .bp3-input{
    -webkit-box-shadow:0 0 0 0 rgba(219, 55, 55, 0), 0 0 0 0 rgba(219, 55, 55, 0), inset 0 0 0 1px #db3737, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 0 rgba(219, 55, 55, 0), 0 0 0 0 rgba(219, 55, 55, 0), inset 0 0 0 1px #db3737, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input-group.bp3-intent-danger .bp3-input:focus{
      -webkit-box-shadow:0 0 0 1px #db3737, 0 0 0 3px rgba(219, 55, 55, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px #db3737, 0 0 0 3px rgba(219, 55, 55, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input-group.bp3-intent-danger .bp3-input[readonly]{
      -webkit-box-shadow:inset 0 0 0 1px #db3737;
              box-shadow:inset 0 0 0 1px #db3737; }
    .bp3-input-group.bp3-intent-danger .bp3-input:disabled, .bp3-input-group.bp3-intent-danger .bp3-input.bp3-disabled{
      -webkit-box-shadow:none;
              box-shadow:none; }
  .bp3-input-group.bp3-intent-danger > .bp3-icon{
    color:#c23030; }
    .bp3-dark .bp3-input-group.bp3-intent-danger > .bp3-icon{
      color:#ff7373; }
.bp3-input{
  -webkit-appearance:none;
     -moz-appearance:none;
          appearance:none;
  background:#ffffff;
  border:none;
  border-radius:3px;
  -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
  color:#182026;
  font-size:14px;
  font-weight:400;
  height:30px;
  line-height:30px;
  outline:none;
  padding:0 10px;
  -webkit-transition:-webkit-box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
  transition:-webkit-box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
  transition:box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
  transition:box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
  vertical-align:middle; }
  .bp3-input::-webkit-input-placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-input::-moz-placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-input:-ms-input-placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-input::-ms-input-placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-input::placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-input:focus, .bp3-input.bp3-active{
    -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
  .bp3-input[type="search"], .bp3-input.bp3-round{
    border-radius:30px;
    -webkit-box-sizing:border-box;
            box-sizing:border-box;
    padding-left:10px; }
  .bp3-input[readonly]{
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.15);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.15); }
  .bp3-input:disabled, .bp3-input.bp3-disabled{
    background:rgba(206, 217, 224, 0.5);
    -webkit-box-shadow:none;
            box-shadow:none;
    color:rgba(92, 112, 128, 0.6);
    cursor:not-allowed;
    resize:none; }
  .bp3-input.bp3-large{
    font-size:16px;
    height:40px;
    line-height:40px; }
    .bp3-input.bp3-large[type="search"], .bp3-input.bp3-large.bp3-round{
      padding:0 15px; }
  .bp3-input.bp3-small{
    font-size:12px;
    height:24px;
    line-height:24px;
    padding-left:8px;
    padding-right:8px; }
    .bp3-input.bp3-small[type="search"], .bp3-input.bp3-small.bp3-round{
      padding:0 12px; }
  .bp3-input.bp3-fill{
    -webkit-box-flex:1;
        -ms-flex:1 1 auto;
            flex:1 1 auto;
    width:100%; }
  .bp3-dark .bp3-input{
    background:rgba(16, 22, 26, 0.3);
    -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
    color:#f5f8fa; }
    .bp3-dark .bp3-input::-webkit-input-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-input::-moz-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-input:-ms-input-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-input::-ms-input-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-input::placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-input:focus{
      -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px #137cbd, 0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-input[readonly]{
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-input:disabled, .bp3-dark .bp3-input.bp3-disabled{
      background:rgba(57, 75, 89, 0.5);
      -webkit-box-shadow:none;
              box-shadow:none;
      color:rgba(167, 182, 194, 0.6); }
  .bp3-input.bp3-intent-primary{
    -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px #137cbd, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px #137cbd, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input.bp3-intent-primary:focus{
      -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input.bp3-intent-primary[readonly]{
      -webkit-box-shadow:inset 0 0 0 1px #137cbd;
              box-shadow:inset 0 0 0 1px #137cbd; }
    .bp3-input.bp3-intent-primary:disabled, .bp3-input.bp3-intent-primary.bp3-disabled{
      -webkit-box-shadow:none;
              box-shadow:none; }
    .bp3-dark .bp3-input.bp3-intent-primary{
      -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px #137cbd, inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px #137cbd, inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
      .bp3-dark .bp3-input.bp3-intent-primary:focus{
        -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
                box-shadow:0 0 0 1px #137cbd, 0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
      .bp3-dark .bp3-input.bp3-intent-primary[readonly]{
        -webkit-box-shadow:inset 0 0 0 1px #137cbd;
                box-shadow:inset 0 0 0 1px #137cbd; }
      .bp3-dark .bp3-input.bp3-intent-primary:disabled, .bp3-dark .bp3-input.bp3-intent-primary.bp3-disabled{
        -webkit-box-shadow:none;
                box-shadow:none; }
  .bp3-input.bp3-intent-success{
    -webkit-box-shadow:0 0 0 0 rgba(15, 153, 96, 0), 0 0 0 0 rgba(15, 153, 96, 0), inset 0 0 0 1px #0f9960, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 0 rgba(15, 153, 96, 0), 0 0 0 0 rgba(15, 153, 96, 0), inset 0 0 0 1px #0f9960, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input.bp3-intent-success:focus{
      -webkit-box-shadow:0 0 0 1px #0f9960, 0 0 0 3px rgba(15, 153, 96, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px #0f9960, 0 0 0 3px rgba(15, 153, 96, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input.bp3-intent-success[readonly]{
      -webkit-box-shadow:inset 0 0 0 1px #0f9960;
              box-shadow:inset 0 0 0 1px #0f9960; }
    .bp3-input.bp3-intent-success:disabled, .bp3-input.bp3-intent-success.bp3-disabled{
      -webkit-box-shadow:none;
              box-shadow:none; }
    .bp3-dark .bp3-input.bp3-intent-success{
      -webkit-box-shadow:0 0 0 0 rgba(15, 153, 96, 0), 0 0 0 0 rgba(15, 153, 96, 0), 0 0 0 0 rgba(15, 153, 96, 0), inset 0 0 0 1px #0f9960, inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 0 rgba(15, 153, 96, 0), 0 0 0 0 rgba(15, 153, 96, 0), 0 0 0 0 rgba(15, 153, 96, 0), inset 0 0 0 1px #0f9960, inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
      .bp3-dark .bp3-input.bp3-intent-success:focus{
        -webkit-box-shadow:0 0 0 1px #0f9960, 0 0 0 1px #0f9960, 0 0 0 3px rgba(15, 153, 96, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
                box-shadow:0 0 0 1px #0f9960, 0 0 0 1px #0f9960, 0 0 0 3px rgba(15, 153, 96, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
      .bp3-dark .bp3-input.bp3-intent-success[readonly]{
        -webkit-box-shadow:inset 0 0 0 1px #0f9960;
                box-shadow:inset 0 0 0 1px #0f9960; }
      .bp3-dark .bp3-input.bp3-intent-success:disabled, .bp3-dark .bp3-input.bp3-intent-success.bp3-disabled{
        -webkit-box-shadow:none;
                box-shadow:none; }
  .bp3-input.bp3-intent-warning{
    -webkit-box-shadow:0 0 0 0 rgba(217, 130, 43, 0), 0 0 0 0 rgba(217, 130, 43, 0), inset 0 0 0 1px #d9822b, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 0 rgba(217, 130, 43, 0), 0 0 0 0 rgba(217, 130, 43, 0), inset 0 0 0 1px #d9822b, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input.bp3-intent-warning:focus{
      -webkit-box-shadow:0 0 0 1px #d9822b, 0 0 0 3px rgba(217, 130, 43, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px #d9822b, 0 0 0 3px rgba(217, 130, 43, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input.bp3-intent-warning[readonly]{
      -webkit-box-shadow:inset 0 0 0 1px #d9822b;
              box-shadow:inset 0 0 0 1px #d9822b; }
    .bp3-input.bp3-intent-warning:disabled, .bp3-input.bp3-intent-warning.bp3-disabled{
      -webkit-box-shadow:none;
              box-shadow:none; }
    .bp3-dark .bp3-input.bp3-intent-warning{
      -webkit-box-shadow:0 0 0 0 rgba(217, 130, 43, 0), 0 0 0 0 rgba(217, 130, 43, 0), 0 0 0 0 rgba(217, 130, 43, 0), inset 0 0 0 1px #d9822b, inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 0 rgba(217, 130, 43, 0), 0 0 0 0 rgba(217, 130, 43, 0), 0 0 0 0 rgba(217, 130, 43, 0), inset 0 0 0 1px #d9822b, inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
      .bp3-dark .bp3-input.bp3-intent-warning:focus{
        -webkit-box-shadow:0 0 0 1px #d9822b, 0 0 0 1px #d9822b, 0 0 0 3px rgba(217, 130, 43, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
                box-shadow:0 0 0 1px #d9822b, 0 0 0 1px #d9822b, 0 0 0 3px rgba(217, 130, 43, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
      .bp3-dark .bp3-input.bp3-intent-warning[readonly]{
        -webkit-box-shadow:inset 0 0 0 1px #d9822b;
                box-shadow:inset 0 0 0 1px #d9822b; }
      .bp3-dark .bp3-input.bp3-intent-warning:disabled, .bp3-dark .bp3-input.bp3-intent-warning.bp3-disabled{
        -webkit-box-shadow:none;
                box-shadow:none; }
  .bp3-input.bp3-intent-danger{
    -webkit-box-shadow:0 0 0 0 rgba(219, 55, 55, 0), 0 0 0 0 rgba(219, 55, 55, 0), inset 0 0 0 1px #db3737, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 0 rgba(219, 55, 55, 0), 0 0 0 0 rgba(219, 55, 55, 0), inset 0 0 0 1px #db3737, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input.bp3-intent-danger:focus{
      -webkit-box-shadow:0 0 0 1px #db3737, 0 0 0 3px rgba(219, 55, 55, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px #db3737, 0 0 0 3px rgba(219, 55, 55, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input.bp3-intent-danger[readonly]{
      -webkit-box-shadow:inset 0 0 0 1px #db3737;
              box-shadow:inset 0 0 0 1px #db3737; }
    .bp3-input.bp3-intent-danger:disabled, .bp3-input.bp3-intent-danger.bp3-disabled{
      -webkit-box-shadow:none;
              box-shadow:none; }
    .bp3-dark .bp3-input.bp3-intent-danger{
      -webkit-box-shadow:0 0 0 0 rgba(219, 55, 55, 0), 0 0 0 0 rgba(219, 55, 55, 0), 0 0 0 0 rgba(219, 55, 55, 0), inset 0 0 0 1px #db3737, inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 0 rgba(219, 55, 55, 0), 0 0 0 0 rgba(219, 55, 55, 0), 0 0 0 0 rgba(219, 55, 55, 0), inset 0 0 0 1px #db3737, inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
      .bp3-dark .bp3-input.bp3-intent-danger:focus{
        -webkit-box-shadow:0 0 0 1px #db3737, 0 0 0 1px #db3737, 0 0 0 3px rgba(219, 55, 55, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
                box-shadow:0 0 0 1px #db3737, 0 0 0 1px #db3737, 0 0 0 3px rgba(219, 55, 55, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
      .bp3-dark .bp3-input.bp3-intent-danger[readonly]{
        -webkit-box-shadow:inset 0 0 0 1px #db3737;
                box-shadow:inset 0 0 0 1px #db3737; }
      .bp3-dark .bp3-input.bp3-intent-danger:disabled, .bp3-dark .bp3-input.bp3-intent-danger.bp3-disabled{
        -webkit-box-shadow:none;
                box-shadow:none; }
  .bp3-input::-ms-clear{
    display:none; }
textarea.bp3-input{
  max-width:100%;
  padding:10px; }
  textarea.bp3-input, textarea.bp3-input.bp3-large, textarea.bp3-input.bp3-small{
    height:auto;
    line-height:inherit; }
  textarea.bp3-input.bp3-small{
    padding:8px; }
  .bp3-dark textarea.bp3-input{
    background:rgba(16, 22, 26, 0.3);
    -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
    color:#f5f8fa; }
    .bp3-dark textarea.bp3-input::-webkit-input-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark textarea.bp3-input::-moz-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark textarea.bp3-input:-ms-input-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark textarea.bp3-input::-ms-input-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark textarea.bp3-input::placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark textarea.bp3-input:focus{
      -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px #137cbd, 0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark textarea.bp3-input[readonly]{
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark textarea.bp3-input:disabled, .bp3-dark textarea.bp3-input.bp3-disabled{
      background:rgba(57, 75, 89, 0.5);
      -webkit-box-shadow:none;
              box-shadow:none;
      color:rgba(167, 182, 194, 0.6); }
label.bp3-label{
  display:block;
  margin-bottom:15px;
  margin-top:0; }
  label.bp3-label .bp3-html-select,
  label.bp3-label .bp3-input,
  label.bp3-label .bp3-select,
  label.bp3-label .bp3-slider,
  label.bp3-label .bp3-popover-wrapper{
    display:block;
    margin-top:5px;
    text-transform:none; }
  label.bp3-label .bp3-button-group{
    margin-top:5px; }
  label.bp3-label .bp3-select select,
  label.bp3-label .bp3-html-select select{
    font-weight:400;
    vertical-align:top;
    width:100%; }
  label.bp3-label.bp3-disabled,
  label.bp3-label.bp3-disabled .bp3-text-muted{
    color:rgba(92, 112, 128, 0.6); }
  label.bp3-label.bp3-inline{
    line-height:30px; }
    label.bp3-label.bp3-inline .bp3-html-select,
    label.bp3-label.bp3-inline .bp3-input,
    label.bp3-label.bp3-inline .bp3-input-group,
    label.bp3-label.bp3-inline .bp3-select,
    label.bp3-label.bp3-inline .bp3-popover-wrapper{
      display:inline-block;
      margin:0 0 0 5px;
      vertical-align:top; }
    label.bp3-label.bp3-inline .bp3-button-group{
      margin:0 0 0 5px; }
    label.bp3-label.bp3-inline .bp3-input-group .bp3-input{
      margin-left:0; }
    label.bp3-label.bp3-inline.bp3-large{
      line-height:40px; }
  label.bp3-label:not(.bp3-inline) .bp3-popover-target{
    display:block; }
  .bp3-dark label.bp3-label{
    color:#f5f8fa; }
    .bp3-dark label.bp3-label.bp3-disabled,
    .bp3-dark label.bp3-label.bp3-disabled .bp3-text-muted{
      color:rgba(167, 182, 194, 0.6); }
.bp3-numeric-input .bp3-button-group.bp3-vertical > .bp3-button{
  -webkit-box-flex:1;
      -ms-flex:1 1 14px;
          flex:1 1 14px;
  min-height:0;
  padding:0;
  width:30px; }
  .bp3-numeric-input .bp3-button-group.bp3-vertical > .bp3-button:first-child{
    border-radius:0 3px 0 0; }
  .bp3-numeric-input .bp3-button-group.bp3-vertical > .bp3-button:last-child{
    border-radius:0 0 3px 0; }

.bp3-numeric-input .bp3-button-group.bp3-vertical:first-child > .bp3-button:first-child{
  border-radius:3px 0 0 0; }

.bp3-numeric-input .bp3-button-group.bp3-vertical:first-child > .bp3-button:last-child{
  border-radius:0 0 0 3px; }

.bp3-numeric-input.bp3-large .bp3-button-group.bp3-vertical > .bp3-button{
  width:40px; }

form{
  display:block; }
.bp3-html-select select,
.bp3-select select{
  display:-webkit-inline-box;
  display:-ms-inline-flexbox;
  display:inline-flex;
  -webkit-box-orient:horizontal;
  -webkit-box-direction:normal;
      -ms-flex-direction:row;
          flex-direction:row;
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  border:none;
  border-radius:3px;
  cursor:pointer;
  font-size:14px;
  -webkit-box-pack:center;
      -ms-flex-pack:center;
          justify-content:center;
  padding:5px 10px;
  text-align:left;
  vertical-align:middle;
  background-color:#f5f8fa;
  background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.8)), to(rgba(255, 255, 255, 0)));
  background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.8), rgba(255, 255, 255, 0));
  -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
          box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
  color:#182026;
  -moz-appearance:none;
  -webkit-appearance:none;
  border-radius:3px;
  height:30px;
  padding:0 25px 0 10px;
  width:100%; }
  .bp3-html-select select > *, .bp3-select select > *{
    -webkit-box-flex:0;
        -ms-flex-positive:0;
            flex-grow:0;
    -ms-flex-negative:0;
        flex-shrink:0; }
  .bp3-html-select select > .bp3-fill, .bp3-select select > .bp3-fill{
    -webkit-box-flex:1;
        -ms-flex-positive:1;
            flex-grow:1;
    -ms-flex-negative:1;
        flex-shrink:1; }
  .bp3-html-select select::before,
  .bp3-select select::before, .bp3-html-select select > *, .bp3-select select > *{
    margin-right:7px; }
  .bp3-html-select select:empty::before,
  .bp3-select select:empty::before,
  .bp3-html-select select > :last-child,
  .bp3-select select > :last-child{
    margin-right:0; }
  .bp3-html-select select:hover,
  .bp3-select select:hover{
    background-clip:padding-box;
    background-color:#ebf1f5;
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1); }
  .bp3-html-select select:active,
  .bp3-select select:active, .bp3-html-select select.bp3-active,
  .bp3-select select.bp3-active{
    background-color:#d8e1e8;
    background-image:none;
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
  .bp3-html-select select:disabled,
  .bp3-select select:disabled, .bp3-html-select select.bp3-disabled,
  .bp3-select select.bp3-disabled{
    background-color:rgba(206, 217, 224, 0.5);
    background-image:none;
    -webkit-box-shadow:none;
            box-shadow:none;
    color:rgba(92, 112, 128, 0.6);
    cursor:not-allowed;
    outline:none; }
    .bp3-html-select select:disabled.bp3-active,
    .bp3-select select:disabled.bp3-active, .bp3-html-select select:disabled.bp3-active:hover,
    .bp3-select select:disabled.bp3-active:hover, .bp3-html-select select.bp3-disabled.bp3-active,
    .bp3-select select.bp3-disabled.bp3-active, .bp3-html-select select.bp3-disabled.bp3-active:hover,
    .bp3-select select.bp3-disabled.bp3-active:hover{
      background:rgba(206, 217, 224, 0.7); }

.bp3-html-select.bp3-minimal select,
.bp3-select.bp3-minimal select{
  background:none;
  -webkit-box-shadow:none;
          box-shadow:none; }
  .bp3-html-select.bp3-minimal select:hover,
  .bp3-select.bp3-minimal select:hover{
    background:rgba(167, 182, 194, 0.3);
    -webkit-box-shadow:none;
            box-shadow:none;
    color:#182026;
    text-decoration:none; }
  .bp3-html-select.bp3-minimal select:active,
  .bp3-select.bp3-minimal select:active, .bp3-html-select.bp3-minimal select.bp3-active,
  .bp3-select.bp3-minimal select.bp3-active{
    background:rgba(115, 134, 148, 0.3);
    -webkit-box-shadow:none;
            box-shadow:none;
    color:#182026; }
  .bp3-html-select.bp3-minimal select:disabled,
  .bp3-select.bp3-minimal select:disabled, .bp3-html-select.bp3-minimal select:disabled:hover,
  .bp3-select.bp3-minimal select:disabled:hover, .bp3-html-select.bp3-minimal select.bp3-disabled,
  .bp3-select.bp3-minimal select.bp3-disabled, .bp3-html-select.bp3-minimal select.bp3-disabled:hover,
  .bp3-select.bp3-minimal select.bp3-disabled:hover{
    background:none;
    color:rgba(92, 112, 128, 0.6);
    cursor:not-allowed; }
    .bp3-html-select.bp3-minimal select:disabled.bp3-active,
    .bp3-select.bp3-minimal select:disabled.bp3-active, .bp3-html-select.bp3-minimal select:disabled:hover.bp3-active,
    .bp3-select.bp3-minimal select:disabled:hover.bp3-active, .bp3-html-select.bp3-minimal select.bp3-disabled.bp3-active,
    .bp3-select.bp3-minimal select.bp3-disabled.bp3-active, .bp3-html-select.bp3-minimal select.bp3-disabled:hover.bp3-active,
    .bp3-select.bp3-minimal select.bp3-disabled:hover.bp3-active{
      background:rgba(115, 134, 148, 0.3); }
  .bp3-dark .bp3-html-select.bp3-minimal select, .bp3-html-select.bp3-minimal .bp3-dark select,
  .bp3-dark .bp3-select.bp3-minimal select, .bp3-select.bp3-minimal .bp3-dark select{
    background:none;
    -webkit-box-shadow:none;
            box-shadow:none;
    color:inherit; }
    .bp3-dark .bp3-html-select.bp3-minimal select:hover, .bp3-html-select.bp3-minimal .bp3-dark select:hover,
    .bp3-dark .bp3-select.bp3-minimal select:hover, .bp3-select.bp3-minimal .bp3-dark select:hover, .bp3-dark .bp3-html-select.bp3-minimal select:active, .bp3-html-select.bp3-minimal .bp3-dark select:active,
    .bp3-dark .bp3-select.bp3-minimal select:active, .bp3-select.bp3-minimal .bp3-dark select:active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-active,
    .bp3-dark .bp3-select.bp3-minimal select.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-active{
      background:none;
      -webkit-box-shadow:none;
              box-shadow:none; }
    .bp3-dark .bp3-html-select.bp3-minimal select:hover, .bp3-html-select.bp3-minimal .bp3-dark select:hover,
    .bp3-dark .bp3-select.bp3-minimal select:hover, .bp3-select.bp3-minimal .bp3-dark select:hover{
      background:rgba(138, 155, 168, 0.15); }
    .bp3-dark .bp3-html-select.bp3-minimal select:active, .bp3-html-select.bp3-minimal .bp3-dark select:active,
    .bp3-dark .bp3-select.bp3-minimal select:active, .bp3-select.bp3-minimal .bp3-dark select:active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-active,
    .bp3-dark .bp3-select.bp3-minimal select.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-active{
      background:rgba(138, 155, 168, 0.3);
      color:#f5f8fa; }
    .bp3-dark .bp3-html-select.bp3-minimal select:disabled, .bp3-html-select.bp3-minimal .bp3-dark select:disabled,
    .bp3-dark .bp3-select.bp3-minimal select:disabled, .bp3-select.bp3-minimal .bp3-dark select:disabled, .bp3-dark .bp3-html-select.bp3-minimal select:disabled:hover, .bp3-html-select.bp3-minimal .bp3-dark select:disabled:hover,
    .bp3-dark .bp3-select.bp3-minimal select:disabled:hover, .bp3-select.bp3-minimal .bp3-dark select:disabled:hover, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-disabled, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-disabled,
    .bp3-dark .bp3-select.bp3-minimal select.bp3-disabled, .bp3-select.bp3-minimal .bp3-dark select.bp3-disabled, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-disabled:hover, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-disabled:hover,
    .bp3-dark .bp3-select.bp3-minimal select.bp3-disabled:hover, .bp3-select.bp3-minimal .bp3-dark select.bp3-disabled:hover{
      background:none;
      color:rgba(167, 182, 194, 0.6);
      cursor:not-allowed; }
      .bp3-dark .bp3-html-select.bp3-minimal select:disabled.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select:disabled.bp3-active,
      .bp3-dark .bp3-select.bp3-minimal select:disabled.bp3-active, .bp3-select.bp3-minimal .bp3-dark select:disabled.bp3-active, .bp3-dark .bp3-html-select.bp3-minimal select:disabled:hover.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select:disabled:hover.bp3-active,
      .bp3-dark .bp3-select.bp3-minimal select:disabled:hover.bp3-active, .bp3-select.bp3-minimal .bp3-dark select:disabled:hover.bp3-active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-disabled.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-disabled.bp3-active,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-disabled.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-disabled.bp3-active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-disabled:hover.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-disabled:hover.bp3-active,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-disabled:hover.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-disabled:hover.bp3-active{
        background:rgba(138, 155, 168, 0.3); }
  .bp3-html-select.bp3-minimal select.bp3-intent-primary,
  .bp3-select.bp3-minimal select.bp3-intent-primary{
    color:#106ba3; }
    .bp3-html-select.bp3-minimal select.bp3-intent-primary:hover,
    .bp3-select.bp3-minimal select.bp3-intent-primary:hover, .bp3-html-select.bp3-minimal select.bp3-intent-primary:active,
    .bp3-select.bp3-minimal select.bp3-intent-primary:active, .bp3-html-select.bp3-minimal select.bp3-intent-primary.bp3-active,
    .bp3-select.bp3-minimal select.bp3-intent-primary.bp3-active{
      background:none;
      -webkit-box-shadow:none;
              box-shadow:none;
      color:#106ba3; }
    .bp3-html-select.bp3-minimal select.bp3-intent-primary:hover,
    .bp3-select.bp3-minimal select.bp3-intent-primary:hover{
      background:rgba(19, 124, 189, 0.15);
      color:#106ba3; }
    .bp3-html-select.bp3-minimal select.bp3-intent-primary:active,
    .bp3-select.bp3-minimal select.bp3-intent-primary:active, .bp3-html-select.bp3-minimal select.bp3-intent-primary.bp3-active,
    .bp3-select.bp3-minimal select.bp3-intent-primary.bp3-active{
      background:rgba(19, 124, 189, 0.3);
      color:#106ba3; }
    .bp3-html-select.bp3-minimal select.bp3-intent-primary:disabled,
    .bp3-select.bp3-minimal select.bp3-intent-primary:disabled, .bp3-html-select.bp3-minimal select.bp3-intent-primary.bp3-disabled,
    .bp3-select.bp3-minimal select.bp3-intent-primary.bp3-disabled{
      background:none;
      color:rgba(16, 107, 163, 0.5); }
      .bp3-html-select.bp3-minimal select.bp3-intent-primary:disabled.bp3-active,
      .bp3-select.bp3-minimal select.bp3-intent-primary:disabled.bp3-active, .bp3-html-select.bp3-minimal select.bp3-intent-primary.bp3-disabled.bp3-active,
      .bp3-select.bp3-minimal select.bp3-intent-primary.bp3-disabled.bp3-active{
        background:rgba(19, 124, 189, 0.3); }
    .bp3-html-select.bp3-minimal select.bp3-intent-primary .bp3-button-spinner .bp3-spinner-head, .bp3-select.bp3-minimal select.bp3-intent-primary .bp3-button-spinner .bp3-spinner-head{
      stroke:#106ba3; }
    .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-primary, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-primary,
    .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-primary, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-primary{
      color:#48aff0; }
      .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-primary:hover, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-primary:hover,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-primary:hover, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-primary:hover{
        background:rgba(19, 124, 189, 0.2);
        color:#48aff0; }
      .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-primary:active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-primary:active,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-primary:active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-primary:active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-primary.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-primary.bp3-active,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-primary.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-primary.bp3-active{
        background:rgba(19, 124, 189, 0.3);
        color:#48aff0; }
      .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-primary:disabled, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-primary:disabled,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-primary:disabled, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-primary:disabled, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-primary.bp3-disabled, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-primary.bp3-disabled,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-primary.bp3-disabled, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-primary.bp3-disabled{
        background:none;
        color:rgba(72, 175, 240, 0.5); }
        .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-primary:disabled.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-primary:disabled.bp3-active,
        .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-primary:disabled.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-primary:disabled.bp3-active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-primary.bp3-disabled.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-primary.bp3-disabled.bp3-active,
        .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-primary.bp3-disabled.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-primary.bp3-disabled.bp3-active{
          background:rgba(19, 124, 189, 0.3); }
  .bp3-html-select.bp3-minimal select.bp3-intent-success,
  .bp3-select.bp3-minimal select.bp3-intent-success{
    color:#0d8050; }
    .bp3-html-select.bp3-minimal select.bp3-intent-success:hover,
    .bp3-select.bp3-minimal select.bp3-intent-success:hover, .bp3-html-select.bp3-minimal select.bp3-intent-success:active,
    .bp3-select.bp3-minimal select.bp3-intent-success:active, .bp3-html-select.bp3-minimal select.bp3-intent-success.bp3-active,
    .bp3-select.bp3-minimal select.bp3-intent-success.bp3-active{
      background:none;
      -webkit-box-shadow:none;
              box-shadow:none;
      color:#0d8050; }
    .bp3-html-select.bp3-minimal select.bp3-intent-success:hover,
    .bp3-select.bp3-minimal select.bp3-intent-success:hover{
      background:rgba(15, 153, 96, 0.15);
      color:#0d8050; }
    .bp3-html-select.bp3-minimal select.bp3-intent-success:active,
    .bp3-select.bp3-minimal select.bp3-intent-success:active, .bp3-html-select.bp3-minimal select.bp3-intent-success.bp3-active,
    .bp3-select.bp3-minimal select.bp3-intent-success.bp3-active{
      background:rgba(15, 153, 96, 0.3);
      color:#0d8050; }
    .bp3-html-select.bp3-minimal select.bp3-intent-success:disabled,
    .bp3-select.bp3-minimal select.bp3-intent-success:disabled, .bp3-html-select.bp3-minimal select.bp3-intent-success.bp3-disabled,
    .bp3-select.bp3-minimal select.bp3-intent-success.bp3-disabled{
      background:none;
      color:rgba(13, 128, 80, 0.5); }
      .bp3-html-select.bp3-minimal select.bp3-intent-success:disabled.bp3-active,
      .bp3-select.bp3-minimal select.bp3-intent-success:disabled.bp3-active, .bp3-html-select.bp3-minimal select.bp3-intent-success.bp3-disabled.bp3-active,
      .bp3-select.bp3-minimal select.bp3-intent-success.bp3-disabled.bp3-active{
        background:rgba(15, 153, 96, 0.3); }
    .bp3-html-select.bp3-minimal select.bp3-intent-success .bp3-button-spinner .bp3-spinner-head, .bp3-select.bp3-minimal select.bp3-intent-success .bp3-button-spinner .bp3-spinner-head{
      stroke:#0d8050; }
    .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-success, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-success,
    .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-success, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-success{
      color:#3dcc91; }
      .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-success:hover, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-success:hover,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-success:hover, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-success:hover{
        background:rgba(15, 153, 96, 0.2);
        color:#3dcc91; }
      .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-success:active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-success:active,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-success:active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-success:active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-success.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-success.bp3-active,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-success.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-success.bp3-active{
        background:rgba(15, 153, 96, 0.3);
        color:#3dcc91; }
      .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-success:disabled, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-success:disabled,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-success:disabled, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-success:disabled, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-success.bp3-disabled, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-success.bp3-disabled,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-success.bp3-disabled, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-success.bp3-disabled{
        background:none;
        color:rgba(61, 204, 145, 0.5); }
        .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-success:disabled.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-success:disabled.bp3-active,
        .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-success:disabled.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-success:disabled.bp3-active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-success.bp3-disabled.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-success.bp3-disabled.bp3-active,
        .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-success.bp3-disabled.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-success.bp3-disabled.bp3-active{
          background:rgba(15, 153, 96, 0.3); }
  .bp3-html-select.bp3-minimal select.bp3-intent-warning,
  .bp3-select.bp3-minimal select.bp3-intent-warning{
    color:#bf7326; }
    .bp3-html-select.bp3-minimal select.bp3-intent-warning:hover,
    .bp3-select.bp3-minimal select.bp3-intent-warning:hover, .bp3-html-select.bp3-minimal select.bp3-intent-warning:active,
    .bp3-select.bp3-minimal select.bp3-intent-warning:active, .bp3-html-select.bp3-minimal select.bp3-intent-warning.bp3-active,
    .bp3-select.bp3-minimal select.bp3-intent-warning.bp3-active{
      background:none;
      -webkit-box-shadow:none;
              box-shadow:none;
      color:#bf7326; }
    .bp3-html-select.bp3-minimal select.bp3-intent-warning:hover,
    .bp3-select.bp3-minimal select.bp3-intent-warning:hover{
      background:rgba(217, 130, 43, 0.15);
      color:#bf7326; }
    .bp3-html-select.bp3-minimal select.bp3-intent-warning:active,
    .bp3-select.bp3-minimal select.bp3-intent-warning:active, .bp3-html-select.bp3-minimal select.bp3-intent-warning.bp3-active,
    .bp3-select.bp3-minimal select.bp3-intent-warning.bp3-active{
      background:rgba(217, 130, 43, 0.3);
      color:#bf7326; }
    .bp3-html-select.bp3-minimal select.bp3-intent-warning:disabled,
    .bp3-select.bp3-minimal select.bp3-intent-warning:disabled, .bp3-html-select.bp3-minimal select.bp3-intent-warning.bp3-disabled,
    .bp3-select.bp3-minimal select.bp3-intent-warning.bp3-disabled{
      background:none;
      color:rgba(191, 115, 38, 0.5); }
      .bp3-html-select.bp3-minimal select.bp3-intent-warning:disabled.bp3-active,
      .bp3-select.bp3-minimal select.bp3-intent-warning:disabled.bp3-active, .bp3-html-select.bp3-minimal select.bp3-intent-warning.bp3-disabled.bp3-active,
      .bp3-select.bp3-minimal select.bp3-intent-warning.bp3-disabled.bp3-active{
        background:rgba(217, 130, 43, 0.3); }
    .bp3-html-select.bp3-minimal select.bp3-intent-warning .bp3-button-spinner .bp3-spinner-head, .bp3-select.bp3-minimal select.bp3-intent-warning .bp3-button-spinner .bp3-spinner-head{
      stroke:#bf7326; }
    .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-warning, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-warning,
    .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-warning, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-warning{
      color:#ffb366; }
      .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-warning:hover, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-warning:hover,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-warning:hover, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-warning:hover{
        background:rgba(217, 130, 43, 0.2);
        color:#ffb366; }
      .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-warning:active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-warning:active,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-warning:active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-warning:active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-warning.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-warning.bp3-active,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-warning.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-warning.bp3-active{
        background:rgba(217, 130, 43, 0.3);
        color:#ffb366; }
      .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-warning:disabled, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-warning:disabled,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-warning:disabled, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-warning:disabled, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-warning.bp3-disabled, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-warning.bp3-disabled,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-warning.bp3-disabled, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-warning.bp3-disabled{
        background:none;
        color:rgba(255, 179, 102, 0.5); }
        .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-warning:disabled.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-warning:disabled.bp3-active,
        .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-warning:disabled.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-warning:disabled.bp3-active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-warning.bp3-disabled.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-warning.bp3-disabled.bp3-active,
        .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-warning.bp3-disabled.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-warning.bp3-disabled.bp3-active{
          background:rgba(217, 130, 43, 0.3); }
  .bp3-html-select.bp3-minimal select.bp3-intent-danger,
  .bp3-select.bp3-minimal select.bp3-intent-danger{
    color:#c23030; }
    .bp3-html-select.bp3-minimal select.bp3-intent-danger:hover,
    .bp3-select.bp3-minimal select.bp3-intent-danger:hover, .bp3-html-select.bp3-minimal select.bp3-intent-danger:active,
    .bp3-select.bp3-minimal select.bp3-intent-danger:active, .bp3-html-select.bp3-minimal select.bp3-intent-danger.bp3-active,
    .bp3-select.bp3-minimal select.bp3-intent-danger.bp3-active{
      background:none;
      -webkit-box-shadow:none;
              box-shadow:none;
      color:#c23030; }
    .bp3-html-select.bp3-minimal select.bp3-intent-danger:hover,
    .bp3-select.bp3-minimal select.bp3-intent-danger:hover{
      background:rgba(219, 55, 55, 0.15);
      color:#c23030; }
    .bp3-html-select.bp3-minimal select.bp3-intent-danger:active,
    .bp3-select.bp3-minimal select.bp3-intent-danger:active, .bp3-html-select.bp3-minimal select.bp3-intent-danger.bp3-active,
    .bp3-select.bp3-minimal select.bp3-intent-danger.bp3-active{
      background:rgba(219, 55, 55, 0.3);
      color:#c23030; }
    .bp3-html-select.bp3-minimal select.bp3-intent-danger:disabled,
    .bp3-select.bp3-minimal select.bp3-intent-danger:disabled, .bp3-html-select.bp3-minimal select.bp3-intent-danger.bp3-disabled,
    .bp3-select.bp3-minimal select.bp3-intent-danger.bp3-disabled{
      background:none;
      color:rgba(194, 48, 48, 0.5); }
      .bp3-html-select.bp3-minimal select.bp3-intent-danger:disabled.bp3-active,
      .bp3-select.bp3-minimal select.bp3-intent-danger:disabled.bp3-active, .bp3-html-select.bp3-minimal select.bp3-intent-danger.bp3-disabled.bp3-active,
      .bp3-select.bp3-minimal select.bp3-intent-danger.bp3-disabled.bp3-active{
        background:rgba(219, 55, 55, 0.3); }
    .bp3-html-select.bp3-minimal select.bp3-intent-danger .bp3-button-spinner .bp3-spinner-head, .bp3-select.bp3-minimal select.bp3-intent-danger .bp3-button-spinner .bp3-spinner-head{
      stroke:#c23030; }
    .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-danger, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-danger,
    .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-danger, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-danger{
      color:#ff7373; }
      .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-danger:hover, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-danger:hover,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-danger:hover, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-danger:hover{
        background:rgba(219, 55, 55, 0.2);
        color:#ff7373; }
      .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-danger:active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-danger:active,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-danger:active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-danger:active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-danger.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-danger.bp3-active,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-danger.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-danger.bp3-active{
        background:rgba(219, 55, 55, 0.3);
        color:#ff7373; }
      .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-danger:disabled, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-danger:disabled,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-danger:disabled, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-danger:disabled, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-danger.bp3-disabled, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-danger.bp3-disabled,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-danger.bp3-disabled, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-danger.bp3-disabled{
        background:none;
        color:rgba(255, 115, 115, 0.5); }
        .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-danger:disabled.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-danger:disabled.bp3-active,
        .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-danger:disabled.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-danger:disabled.bp3-active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-danger.bp3-disabled.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-danger.bp3-disabled.bp3-active,
        .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-danger.bp3-disabled.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-danger.bp3-disabled.bp3-active{
          background:rgba(219, 55, 55, 0.3); }

.bp3-html-select.bp3-large select,
.bp3-select.bp3-large select{
  font-size:16px;
  height:40px;
  padding-right:35px; }

.bp3-dark .bp3-html-select select, .bp3-dark .bp3-select select{
  background-color:#394b59;
  background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.05)), to(rgba(255, 255, 255, 0)));
  background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.05), rgba(255, 255, 255, 0));
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
  color:#f5f8fa; }
  .bp3-dark .bp3-html-select select:hover, .bp3-dark .bp3-select select:hover, .bp3-dark .bp3-html-select select:active, .bp3-dark .bp3-select select:active, .bp3-dark .bp3-html-select select.bp3-active, .bp3-dark .bp3-select select.bp3-active{
    color:#f5f8fa; }
  .bp3-dark .bp3-html-select select:hover, .bp3-dark .bp3-select select:hover{
    background-color:#30404d;
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
  .bp3-dark .bp3-html-select select:active, .bp3-dark .bp3-select select:active, .bp3-dark .bp3-html-select select.bp3-active, .bp3-dark .bp3-select select.bp3-active{
    background-color:#202b33;
    background-image:none;
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
  .bp3-dark .bp3-html-select select:disabled, .bp3-dark .bp3-select select:disabled, .bp3-dark .bp3-html-select select.bp3-disabled, .bp3-dark .bp3-select select.bp3-disabled{
    background-color:rgba(57, 75, 89, 0.5);
    background-image:none;
    -webkit-box-shadow:none;
            box-shadow:none;
    color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-html-select select:disabled.bp3-active, .bp3-dark .bp3-select select:disabled.bp3-active, .bp3-dark .bp3-html-select select.bp3-disabled.bp3-active, .bp3-dark .bp3-select select.bp3-disabled.bp3-active{
      background:rgba(57, 75, 89, 0.7); }
  .bp3-dark .bp3-html-select select .bp3-button-spinner .bp3-spinner-head, .bp3-dark .bp3-select select .bp3-button-spinner .bp3-spinner-head{
    background:rgba(16, 22, 26, 0.5);
    stroke:#8a9ba8; }

.bp3-html-select select:disabled,
.bp3-select select:disabled{
  background-color:rgba(206, 217, 224, 0.5);
  -webkit-box-shadow:none;
          box-shadow:none;
  color:rgba(92, 112, 128, 0.6);
  cursor:not-allowed; }

.bp3-html-select .bp3-icon,
.bp3-select .bp3-icon, .bp3-select::after{
  color:#5c7080;
  pointer-events:none;
  position:absolute;
  right:7px;
  top:7px; }
  .bp3-html-select .bp3-disabled.bp3-icon,
  .bp3-select .bp3-disabled.bp3-icon, .bp3-disabled.bp3-select::after{
    color:rgba(92, 112, 128, 0.6); }
.bp3-html-select,
.bp3-select{
  display:inline-block;
  letter-spacing:normal;
  position:relative;
  vertical-align:middle; }
  .bp3-html-select select::-ms-expand,
  .bp3-select select::-ms-expand{
    display:none; }
  .bp3-html-select .bp3-icon,
  .bp3-select .bp3-icon{
    color:#5c7080; }
    .bp3-html-select .bp3-icon:hover,
    .bp3-select .bp3-icon:hover{
      color:#182026; }
    .bp3-dark .bp3-html-select .bp3-icon, .bp3-dark
    .bp3-select .bp3-icon{
      color:#a7b6c2; }
      .bp3-dark .bp3-html-select .bp3-icon:hover, .bp3-dark
      .bp3-select .bp3-icon:hover{
        color:#f5f8fa; }
  .bp3-html-select.bp3-large::after,
  .bp3-html-select.bp3-large .bp3-icon,
  .bp3-select.bp3-large::after,
  .bp3-select.bp3-large .bp3-icon{
    right:12px;
    top:12px; }
  .bp3-html-select.bp3-fill,
  .bp3-html-select.bp3-fill select,
  .bp3-select.bp3-fill,
  .bp3-select.bp3-fill select{
    width:100%; }
  .bp3-dark .bp3-html-select option, .bp3-dark
  .bp3-select option{
    background-color:#30404d;
    color:#f5f8fa; }
  .bp3-dark .bp3-html-select option:disabled, .bp3-dark
  .bp3-select option:disabled{
    color:rgba(167, 182, 194, 0.6); }
  .bp3-dark .bp3-html-select::after, .bp3-dark
  .bp3-select::after{
    color:#a7b6c2; }

.bp3-select::after{
  font-family:"Icons16", sans-serif;
  font-size:16px;
  font-style:normal;
  font-weight:400;
  line-height:1;
  -moz-osx-font-smoothing:grayscale;
  -webkit-font-smoothing:antialiased;
  content:""; }
.bp3-running-text table, table.bp3-html-table{
  border-spacing:0;
  font-size:14px; }
  .bp3-running-text table th, table.bp3-html-table th,
  .bp3-running-text table td,
  table.bp3-html-table td{
    padding:11px;
    text-align:left;
    vertical-align:top; }
  .bp3-running-text table th, table.bp3-html-table th{
    color:#182026;
    font-weight:600; }
  
  .bp3-running-text table td,
  table.bp3-html-table td{
    color:#182026; }
  .bp3-running-text table tbody tr:first-child th, table.bp3-html-table tbody tr:first-child th,
  .bp3-running-text table tbody tr:first-child td,
  table.bp3-html-table tbody tr:first-child td,
  .bp3-running-text table tfoot tr:first-child th,
  table.bp3-html-table tfoot tr:first-child th,
  .bp3-running-text table tfoot tr:first-child td,
  table.bp3-html-table tfoot tr:first-child td{
    -webkit-box-shadow:inset 0 1px 0 0 rgba(16, 22, 26, 0.15);
            box-shadow:inset 0 1px 0 0 rgba(16, 22, 26, 0.15); }
  .bp3-dark .bp3-running-text table th, .bp3-running-text .bp3-dark table th, .bp3-dark table.bp3-html-table th{
    color:#f5f8fa; }
  .bp3-dark .bp3-running-text table td, .bp3-running-text .bp3-dark table td, .bp3-dark table.bp3-html-table td{
    color:#f5f8fa; }
  .bp3-dark .bp3-running-text table tbody tr:first-child th, .bp3-running-text .bp3-dark table tbody tr:first-child th, .bp3-dark table.bp3-html-table tbody tr:first-child th,
  .bp3-dark .bp3-running-text table tbody tr:first-child td,
  .bp3-running-text .bp3-dark table tbody tr:first-child td,
  .bp3-dark table.bp3-html-table tbody tr:first-child td,
  .bp3-dark .bp3-running-text table tfoot tr:first-child th,
  .bp3-running-text .bp3-dark table tfoot tr:first-child th,
  .bp3-dark table.bp3-html-table tfoot tr:first-child th,
  .bp3-dark .bp3-running-text table tfoot tr:first-child td,
  .bp3-running-text .bp3-dark table tfoot tr:first-child td,
  .bp3-dark table.bp3-html-table tfoot tr:first-child td{
    -webkit-box-shadow:inset 0 1px 0 0 rgba(255, 255, 255, 0.15);
            box-shadow:inset 0 1px 0 0 rgba(255, 255, 255, 0.15); }

table.bp3-html-table.bp3-html-table-condensed th,
table.bp3-html-table.bp3-html-table-condensed td, table.bp3-html-table.bp3-small th,
table.bp3-html-table.bp3-small td{
  padding-bottom:6px;
  padding-top:6px; }

table.bp3-html-table.bp3-html-table-striped tbody tr:nth-child(odd) td{
  background:rgba(191, 204, 214, 0.15); }

table.bp3-html-table.bp3-html-table-bordered th:not(:first-child){
  -webkit-box-shadow:inset 1px 0 0 0 rgba(16, 22, 26, 0.15);
          box-shadow:inset 1px 0 0 0 rgba(16, 22, 26, 0.15); }

table.bp3-html-table.bp3-html-table-bordered tbody tr td,
table.bp3-html-table.bp3-html-table-bordered tfoot tr td{
  -webkit-box-shadow:inset 0 1px 0 0 rgba(16, 22, 26, 0.15);
          box-shadow:inset 0 1px 0 0 rgba(16, 22, 26, 0.15); }
  table.bp3-html-table.bp3-html-table-bordered tbody tr td:not(:first-child),
  table.bp3-html-table.bp3-html-table-bordered tfoot tr td:not(:first-child){
    -webkit-box-shadow:inset 1px 1px 0 0 rgba(16, 22, 26, 0.15);
            box-shadow:inset 1px 1px 0 0 rgba(16, 22, 26, 0.15); }

table.bp3-html-table.bp3-html-table-bordered.bp3-html-table-striped tbody tr:not(:first-child) td{
  -webkit-box-shadow:none;
          box-shadow:none; }
  table.bp3-html-table.bp3-html-table-bordered.bp3-html-table-striped tbody tr:not(:first-child) td:not(:first-child){
    -webkit-box-shadow:inset 1px 0 0 0 rgba(16, 22, 26, 0.15);
            box-shadow:inset 1px 0 0 0 rgba(16, 22, 26, 0.15); }

table.bp3-html-table.bp3-interactive tbody tr:hover td{
  background-color:rgba(191, 204, 214, 0.3);
  cursor:pointer; }

table.bp3-html-table.bp3-interactive tbody tr:active td{
  background-color:rgba(191, 204, 214, 0.4); }

.bp3-dark table.bp3-html-table{ }
  .bp3-dark table.bp3-html-table.bp3-html-table-striped tbody tr:nth-child(odd) td{
    background:rgba(92, 112, 128, 0.15); }
  .bp3-dark table.bp3-html-table.bp3-html-table-bordered th:not(:first-child){
    -webkit-box-shadow:inset 1px 0 0 0 rgba(255, 255, 255, 0.15);
            box-shadow:inset 1px 0 0 0 rgba(255, 255, 255, 0.15); }
  .bp3-dark table.bp3-html-table.bp3-html-table-bordered tbody tr td,
  .bp3-dark table.bp3-html-table.bp3-html-table-bordered tfoot tr td{
    -webkit-box-shadow:inset 0 1px 0 0 rgba(255, 255, 255, 0.15);
            box-shadow:inset 0 1px 0 0 rgba(255, 255, 255, 0.15); }
    .bp3-dark table.bp3-html-table.bp3-html-table-bordered tbody tr td:not(:first-child),
    .bp3-dark table.bp3-html-table.bp3-html-table-bordered tfoot tr td:not(:first-child){
      -webkit-box-shadow:inset 1px 1px 0 0 rgba(255, 255, 255, 0.15);
              box-shadow:inset 1px 1px 0 0 rgba(255, 255, 255, 0.15); }
  .bp3-dark table.bp3-html-table.bp3-html-table-bordered.bp3-html-table-striped tbody tr:not(:first-child) td{
    -webkit-box-shadow:inset 1px 0 0 0 rgba(255, 255, 255, 0.15);
            box-shadow:inset 1px 0 0 0 rgba(255, 255, 255, 0.15); }
    .bp3-dark table.bp3-html-table.bp3-html-table-bordered.bp3-html-table-striped tbody tr:not(:first-child) td:first-child{
      -webkit-box-shadow:none;
              box-shadow:none; }
  .bp3-dark table.bp3-html-table.bp3-interactive tbody tr:hover td{
    background-color:rgba(92, 112, 128, 0.3);
    cursor:pointer; }
  .bp3-dark table.bp3-html-table.bp3-interactive tbody tr:active td{
    background-color:rgba(92, 112, 128, 0.4); }

.bp3-key-combo{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-orient:horizontal;
  -webkit-box-direction:normal;
      -ms-flex-direction:row;
          flex-direction:row;
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center; }
  .bp3-key-combo > *{
    -webkit-box-flex:0;
        -ms-flex-positive:0;
            flex-grow:0;
    -ms-flex-negative:0;
        flex-shrink:0; }
  .bp3-key-combo > .bp3-fill{
    -webkit-box-flex:1;
        -ms-flex-positive:1;
            flex-grow:1;
    -ms-flex-negative:1;
        flex-shrink:1; }
  .bp3-key-combo::before,
  .bp3-key-combo > *{
    margin-right:5px; }
  .bp3-key-combo:empty::before,
  .bp3-key-combo > :last-child{
    margin-right:0; }

.bp3-hotkey-dialog{
  padding-bottom:0;
  top:40px; }
  .bp3-hotkey-dialog .bp3-dialog-body{
    margin:0;
    padding:0; }
  .bp3-hotkey-dialog .bp3-hotkey-label{
    -webkit-box-flex:1;
        -ms-flex-positive:1;
            flex-grow:1; }

.bp3-hotkey-column{
  margin:auto;
  max-height:80vh;
  overflow-y:auto;
  padding:30px; }
  .bp3-hotkey-column .bp3-heading{
    margin-bottom:20px; }
    .bp3-hotkey-column .bp3-heading:not(:first-child){
      margin-top:40px; }

.bp3-hotkey{
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-pack:justify;
      -ms-flex-pack:justify;
          justify-content:space-between;
  margin-left:0;
  margin-right:0; }
  .bp3-hotkey:not(:last-child){
    margin-bottom:10px; }
.bp3-icon{
  display:inline-block;
  -webkit-box-flex:0;
      -ms-flex:0 0 auto;
          flex:0 0 auto;
  vertical-align:text-bottom; }
  .bp3-icon:not(:empty)::before{
    content:"" !important;
    content:unset !important; }
  .bp3-icon > svg{
    display:block; }
    .bp3-icon > svg:not([fill]){
      fill:currentColor; }

.bp3-icon.bp3-intent-primary, .bp3-icon-standard.bp3-intent-primary, .bp3-icon-large.bp3-intent-primary{
  color:#106ba3; }
  .bp3-dark .bp3-icon.bp3-intent-primary, .bp3-dark .bp3-icon-standard.bp3-intent-primary, .bp3-dark .bp3-icon-large.bp3-intent-primary{
    color:#48aff0; }

.bp3-icon.bp3-intent-success, .bp3-icon-standard.bp3-intent-success, .bp3-icon-large.bp3-intent-success{
  color:#0d8050; }
  .bp3-dark .bp3-icon.bp3-intent-success, .bp3-dark .bp3-icon-standard.bp3-intent-success, .bp3-dark .bp3-icon-large.bp3-intent-success{
    color:#3dcc91; }

.bp3-icon.bp3-intent-warning, .bp3-icon-standard.bp3-intent-warning, .bp3-icon-large.bp3-intent-warning{
  color:#bf7326; }
  .bp3-dark .bp3-icon.bp3-intent-warning, .bp3-dark .bp3-icon-standard.bp3-intent-warning, .bp3-dark .bp3-icon-large.bp3-intent-warning{
    color:#ffb366; }

.bp3-icon.bp3-intent-danger, .bp3-icon-standard.bp3-intent-danger, .bp3-icon-large.bp3-intent-danger{
  color:#c23030; }
  .bp3-dark .bp3-icon.bp3-intent-danger, .bp3-dark .bp3-icon-standard.bp3-intent-danger, .bp3-dark .bp3-icon-large.bp3-intent-danger{
    color:#ff7373; }

span.bp3-icon-standard{
  font-family:"Icons16", sans-serif;
  font-size:16px;
  font-style:normal;
  font-weight:400;
  line-height:1;
  -moz-osx-font-smoothing:grayscale;
  -webkit-font-smoothing:antialiased;
  display:inline-block; }

span.bp3-icon-large{
  font-family:"Icons20", sans-serif;
  font-size:20px;
  font-style:normal;
  font-weight:400;
  line-height:1;
  -moz-osx-font-smoothing:grayscale;
  -webkit-font-smoothing:antialiased;
  display:inline-block; }

span.bp3-icon:empty{
  font-family:"Icons20";
  font-size:inherit;
  font-style:normal;
  font-weight:400;
  line-height:1; }
  span.bp3-icon:empty::before{
    -moz-osx-font-smoothing:grayscale;
    -webkit-font-smoothing:antialiased; }

.bp3-icon-add::before{
  content:""; }

.bp3-icon-add-column-left::before{
  content:""; }

.bp3-icon-add-column-right::before{
  content:""; }

.bp3-icon-add-row-bottom::before{
  content:""; }

.bp3-icon-add-row-top::before{
  content:""; }

.bp3-icon-add-to-artifact::before{
  content:""; }

.bp3-icon-add-to-folder::before{
  content:""; }

.bp3-icon-airplane::before{
  content:""; }

.bp3-icon-align-center::before{
  content:""; }

.bp3-icon-align-justify::before{
  content:""; }

.bp3-icon-align-left::before{
  content:""; }

.bp3-icon-align-right::before{
  content:""; }

.bp3-icon-alignment-bottom::before{
  content:""; }

.bp3-icon-alignment-horizontal-center::before{
  content:""; }

.bp3-icon-alignment-left::before{
  content:""; }

.bp3-icon-alignment-right::before{
  content:""; }

.bp3-icon-alignment-top::before{
  content:""; }

.bp3-icon-alignment-vertical-center::before{
  content:""; }

.bp3-icon-annotation::before{
  content:""; }

.bp3-icon-application::before{
  content:""; }

.bp3-icon-applications::before{
  content:""; }

.bp3-icon-archive::before{
  content:""; }

.bp3-icon-arrow-bottom-left::before{
  content:"↙"; }

.bp3-icon-arrow-bottom-right::before{
  content:"↘"; }

.bp3-icon-arrow-down::before{
  content:"↓"; }

.bp3-icon-arrow-left::before{
  content:"←"; }

.bp3-icon-arrow-right::before{
  content:"→"; }

.bp3-icon-arrow-top-left::before{
  content:"↖"; }

.bp3-icon-arrow-top-right::before{
  content:"↗"; }

.bp3-icon-arrow-up::before{
  content:"↑"; }

.bp3-icon-arrows-horizontal::before{
  content:"↔"; }

.bp3-icon-arrows-vertical::before{
  content:"↕"; }

.bp3-icon-asterisk::before{
  content:"*"; }

.bp3-icon-automatic-updates::before{
  content:""; }

.bp3-icon-badge::before{
  content:""; }

.bp3-icon-ban-circle::before{
  content:""; }

.bp3-icon-bank-account::before{
  content:""; }

.bp3-icon-barcode::before{
  content:""; }

.bp3-icon-blank::before{
  content:""; }

.bp3-icon-blocked-person::before{
  content:""; }

.bp3-icon-bold::before{
  content:""; }

.bp3-icon-book::before{
  content:""; }

.bp3-icon-bookmark::before{
  content:""; }

.bp3-icon-box::before{
  content:""; }

.bp3-icon-briefcase::before{
  content:""; }

.bp3-icon-bring-data::before{
  content:""; }

.bp3-icon-build::before{
  content:""; }

.bp3-icon-calculator::before{
  content:""; }

.bp3-icon-calendar::before{
  content:""; }

.bp3-icon-camera::before{
  content:""; }

.bp3-icon-caret-down::before{
  content:"⌄"; }

.bp3-icon-caret-left::before{
  content:"〈"; }

.bp3-icon-caret-right::before{
  content:"〉"; }

.bp3-icon-caret-up::before{
  content:"⌃"; }

.bp3-icon-cell-tower::before{
  content:""; }

.bp3-icon-changes::before{
  content:""; }

.bp3-icon-chart::before{
  content:""; }

.bp3-icon-chat::before{
  content:""; }

.bp3-icon-chevron-backward::before{
  content:""; }

.bp3-icon-chevron-down::before{
  content:""; }

.bp3-icon-chevron-forward::before{
  content:""; }

.bp3-icon-chevron-left::before{
  content:""; }

.bp3-icon-chevron-right::before{
  content:""; }

.bp3-icon-chevron-up::before{
  content:""; }

.bp3-icon-circle::before{
  content:""; }

.bp3-icon-circle-arrow-down::before{
  content:""; }

.bp3-icon-circle-arrow-left::before{
  content:""; }

.bp3-icon-circle-arrow-right::before{
  content:""; }

.bp3-icon-circle-arrow-up::before{
  content:""; }

.bp3-icon-citation::before{
  content:""; }

.bp3-icon-clean::before{
  content:""; }

.bp3-icon-clipboard::before{
  content:""; }

.bp3-icon-cloud::before{
  content:"☁"; }

.bp3-icon-cloud-download::before{
  content:""; }

.bp3-icon-cloud-upload::before{
  content:""; }

.bp3-icon-code::before{
  content:""; }

.bp3-icon-code-block::before{
  content:""; }

.bp3-icon-cog::before{
  content:""; }

.bp3-icon-collapse-all::before{
  content:""; }

.bp3-icon-column-layout::before{
  content:""; }

.bp3-icon-comment::before{
  content:""; }

.bp3-icon-comparison::before{
  content:""; }

.bp3-icon-compass::before{
  content:""; }

.bp3-icon-compressed::before{
  content:""; }

.bp3-icon-confirm::before{
  content:""; }

.bp3-icon-console::before{
  content:""; }

.bp3-icon-contrast::before{
  content:""; }

.bp3-icon-control::before{
  content:""; }

.bp3-icon-credit-card::before{
  content:""; }

.bp3-icon-cross::before{
  content:"✗"; }

.bp3-icon-crown::before{
  content:""; }

.bp3-icon-cube::before{
  content:""; }

.bp3-icon-cube-add::before{
  content:""; }

.bp3-icon-cube-remove::before{
  content:""; }

.bp3-icon-curved-range-chart::before{
  content:""; }

.bp3-icon-cut::before{
  content:""; }

.bp3-icon-dashboard::before{
  content:""; }

.bp3-icon-data-lineage::before{
  content:""; }

.bp3-icon-database::before{
  content:""; }

.bp3-icon-delete::before{
  content:""; }

.bp3-icon-delta::before{
  content:"Δ"; }

.bp3-icon-derive-column::before{
  content:""; }

.bp3-icon-desktop::before{
  content:""; }

.bp3-icon-diagnosis::before{
  content:""; }

.bp3-icon-diagram-tree::before{
  content:""; }

.bp3-icon-direction-left::before{
  content:""; }

.bp3-icon-direction-right::before{
  content:""; }

.bp3-icon-disable::before{
  content:""; }

.bp3-icon-document::before{
  content:""; }

.bp3-icon-document-open::before{
  content:""; }

.bp3-icon-document-share::before{
  content:""; }

.bp3-icon-dollar::before{
  content:"$"; }

.bp3-icon-dot::before{
  content:"•"; }

.bp3-icon-double-caret-horizontal::before{
  content:""; }

.bp3-icon-double-caret-vertical::before{
  content:""; }

.bp3-icon-double-chevron-down::before{
  content:""; }

.bp3-icon-double-chevron-left::before{
  content:""; }

.bp3-icon-double-chevron-right::before{
  content:""; }

.bp3-icon-double-chevron-up::before{
  content:""; }

.bp3-icon-doughnut-chart::before{
  content:""; }

.bp3-icon-download::before{
  content:""; }

.bp3-icon-drag-handle-horizontal::before{
  content:""; }

.bp3-icon-drag-handle-vertical::before{
  content:""; }

.bp3-icon-draw::before{
  content:""; }

.bp3-icon-drive-time::before{
  content:""; }

.bp3-icon-duplicate::before{
  content:""; }

.bp3-icon-edit::before{
  content:"✎"; }

.bp3-icon-eject::before{
  content:"⏏"; }

.bp3-icon-endorsed::before{
  content:""; }

.bp3-icon-envelope::before{
  content:"✉"; }

.bp3-icon-equals::before{
  content:""; }

.bp3-icon-eraser::before{
  content:""; }

.bp3-icon-error::before{
  content:""; }

.bp3-icon-euro::before{
  content:"€"; }

.bp3-icon-exchange::before{
  content:""; }

.bp3-icon-exclude-row::before{
  content:""; }

.bp3-icon-expand-all::before{
  content:""; }

.bp3-icon-export::before{
  content:""; }

.bp3-icon-eye-off::before{
  content:""; }

.bp3-icon-eye-on::before{
  content:""; }

.bp3-icon-eye-open::before{
  content:""; }

.bp3-icon-fast-backward::before{
  content:""; }

.bp3-icon-fast-forward::before{
  content:""; }

.bp3-icon-feed::before{
  content:""; }

.bp3-icon-feed-subscribed::before{
  content:""; }

.bp3-icon-film::before{
  content:""; }

.bp3-icon-filter::before{
  content:""; }

.bp3-icon-filter-keep::before{
  content:""; }

.bp3-icon-filter-list::before{
  content:""; }

.bp3-icon-filter-open::before{
  content:""; }

.bp3-icon-filter-remove::before{
  content:""; }

.bp3-icon-flag::before{
  content:"⚑"; }

.bp3-icon-flame::before{
  content:""; }

.bp3-icon-flash::before{
  content:""; }

.bp3-icon-floppy-disk::before{
  content:""; }

.bp3-icon-flow-branch::before{
  content:""; }

.bp3-icon-flow-end::before{
  content:""; }

.bp3-icon-flow-linear::before{
  content:""; }

.bp3-icon-flow-review::before{
  content:""; }

.bp3-icon-flow-review-branch::before{
  content:""; }

.bp3-icon-flows::before{
  content:""; }

.bp3-icon-folder-close::before{
  content:""; }

.bp3-icon-folder-new::before{
  content:""; }

.bp3-icon-folder-open::before{
  content:""; }

.bp3-icon-folder-shared::before{
  content:""; }

.bp3-icon-folder-shared-open::before{
  content:""; }

.bp3-icon-follower::before{
  content:""; }

.bp3-icon-following::before{
  content:""; }

.bp3-icon-font::before{
  content:""; }

.bp3-icon-fork::before{
  content:""; }

.bp3-icon-form::before{
  content:""; }

.bp3-icon-full-circle::before{
  content:""; }

.bp3-icon-full-stacked-chart::before{
  content:""; }

.bp3-icon-fullscreen::before{
  content:""; }

.bp3-icon-function::before{
  content:""; }

.bp3-icon-gantt-chart::before{
  content:""; }

.bp3-icon-geolocation::before{
  content:""; }

.bp3-icon-geosearch::before{
  content:""; }

.bp3-icon-git-branch::before{
  content:""; }

.bp3-icon-git-commit::before{
  content:""; }

.bp3-icon-git-merge::before{
  content:""; }

.bp3-icon-git-new-branch::before{
  content:""; }

.bp3-icon-git-pull::before{
  content:""; }

.bp3-icon-git-push::before{
  content:""; }

.bp3-icon-git-repo::before{
  content:""; }

.bp3-icon-glass::before{
  content:""; }

.bp3-icon-globe::before{
  content:""; }

.bp3-icon-globe-network::before{
  content:""; }

.bp3-icon-graph::before{
  content:""; }

.bp3-icon-graph-remove::before{
  content:""; }

.bp3-icon-greater-than::before{
  content:""; }

.bp3-icon-greater-than-or-equal-to::before{
  content:""; }

.bp3-icon-grid::before{
  content:""; }

.bp3-icon-grid-view::before{
  content:""; }

.bp3-icon-group-objects::before{
  content:""; }

.bp3-icon-grouped-bar-chart::before{
  content:""; }

.bp3-icon-hand::before{
  content:""; }

.bp3-icon-hand-down::before{
  content:""; }

.bp3-icon-hand-left::before{
  content:""; }

.bp3-icon-hand-right::before{
  content:""; }

.bp3-icon-hand-up::before{
  content:""; }

.bp3-icon-header::before{
  content:""; }

.bp3-icon-header-one::before{
  content:""; }

.bp3-icon-header-two::before{
  content:""; }

.bp3-icon-headset::before{
  content:""; }

.bp3-icon-heart::before{
  content:"♥"; }

.bp3-icon-heart-broken::before{
  content:""; }

.bp3-icon-heat-grid::before{
  content:""; }

.bp3-icon-heatmap::before{
  content:""; }

.bp3-icon-help::before{
  content:"?"; }

.bp3-icon-helper-management::before{
  content:""; }

.bp3-icon-highlight::before{
  content:""; }

.bp3-icon-history::before{
  content:""; }

.bp3-icon-home::before{
  content:"⌂"; }

.bp3-icon-horizontal-bar-chart::before{
  content:""; }

.bp3-icon-horizontal-bar-chart-asc::before{
  content:""; }

.bp3-icon-horizontal-bar-chart-desc::before{
  content:""; }

.bp3-icon-horizontal-distribution::before{
  content:""; }

.bp3-icon-id-number::before{
  content:""; }

.bp3-icon-image-rotate-left::before{
  content:""; }

.bp3-icon-image-rotate-right::before{
  content:""; }

.bp3-icon-import::before{
  content:""; }

.bp3-icon-inbox::before{
  content:""; }

.bp3-icon-inbox-filtered::before{
  content:""; }

.bp3-icon-inbox-geo::before{
  content:""; }

.bp3-icon-inbox-search::before{
  content:""; }

.bp3-icon-inbox-update::before{
  content:""; }

.bp3-icon-info-sign::before{
  content:"ℹ"; }

.bp3-icon-inheritance::before{
  content:""; }

.bp3-icon-inner-join::before{
  content:""; }

.bp3-icon-insert::before{
  content:""; }

.bp3-icon-intersection::before{
  content:""; }

.bp3-icon-ip-address::before{
  content:""; }

.bp3-icon-issue::before{
  content:""; }

.bp3-icon-issue-closed::before{
  content:""; }

.bp3-icon-issue-new::before{
  content:""; }

.bp3-icon-italic::before{
  content:""; }

.bp3-icon-join-table::before{
  content:""; }

.bp3-icon-key::before{
  content:""; }

.bp3-icon-key-backspace::before{
  content:""; }

.bp3-icon-key-command::before{
  content:""; }

.bp3-icon-key-control::before{
  content:""; }

.bp3-icon-key-delete::before{
  content:""; }

.bp3-icon-key-enter::before{
  content:""; }

.bp3-icon-key-escape::before{
  content:""; }

.bp3-icon-key-option::before{
  content:""; }

.bp3-icon-key-shift::before{
  content:""; }

.bp3-icon-key-tab::before{
  content:""; }

.bp3-icon-known-vehicle::before{
  content:""; }

.bp3-icon-lab-test::before{
  content:""; }

.bp3-icon-label::before{
  content:""; }

.bp3-icon-layer::before{
  content:""; }

.bp3-icon-layers::before{
  content:""; }

.bp3-icon-layout::before{
  content:""; }

.bp3-icon-layout-auto::before{
  content:""; }

.bp3-icon-layout-balloon::before{
  content:""; }

.bp3-icon-layout-circle::before{
  content:""; }

.bp3-icon-layout-grid::before{
  content:""; }

.bp3-icon-layout-group-by::before{
  content:""; }

.bp3-icon-layout-hierarchy::before{
  content:""; }

.bp3-icon-layout-linear::before{
  content:""; }

.bp3-icon-layout-skew-grid::before{
  content:""; }

.bp3-icon-layout-sorted-clusters::before{
  content:""; }

.bp3-icon-learning::before{
  content:""; }

.bp3-icon-left-join::before{
  content:""; }

.bp3-icon-less-than::before{
  content:""; }

.bp3-icon-less-than-or-equal-to::before{
  content:""; }

.bp3-icon-lifesaver::before{
  content:""; }

.bp3-icon-lightbulb::before{
  content:""; }

.bp3-icon-link::before{
  content:""; }

.bp3-icon-list::before{
  content:"☰"; }

.bp3-icon-list-columns::before{
  content:""; }

.bp3-icon-list-detail-view::before{
  content:""; }

.bp3-icon-locate::before{
  content:""; }

.bp3-icon-lock::before{
  content:""; }

.bp3-icon-log-in::before{
  content:""; }

.bp3-icon-log-out::before{
  content:""; }

.bp3-icon-manual::before{
  content:""; }

.bp3-icon-manually-entered-data::before{
  content:""; }

.bp3-icon-map::before{
  content:""; }

.bp3-icon-map-create::before{
  content:""; }

.bp3-icon-map-marker::before{
  content:""; }

.bp3-icon-maximize::before{
  content:""; }

.bp3-icon-media::before{
  content:""; }

.bp3-icon-menu::before{
  content:""; }

.bp3-icon-menu-closed::before{
  content:""; }

.bp3-icon-menu-open::before{
  content:""; }

.bp3-icon-merge-columns::before{
  content:""; }

.bp3-icon-merge-links::before{
  content:""; }

.bp3-icon-minimize::before{
  content:""; }

.bp3-icon-minus::before{
  content:"−"; }

.bp3-icon-mobile-phone::before{
  content:""; }

.bp3-icon-mobile-video::before{
  content:""; }

.bp3-icon-moon::before{
  content:""; }

.bp3-icon-more::before{
  content:""; }

.bp3-icon-mountain::before{
  content:""; }

.bp3-icon-move::before{
  content:""; }

.bp3-icon-mugshot::before{
  content:""; }

.bp3-icon-multi-select::before{
  content:""; }

.bp3-icon-music::before{
  content:""; }

.bp3-icon-new-drawing::before{
  content:""; }

.bp3-icon-new-grid-item::before{
  content:""; }

.bp3-icon-new-layer::before{
  content:""; }

.bp3-icon-new-layers::before{
  content:""; }

.bp3-icon-new-link::before{
  content:""; }

.bp3-icon-new-object::before{
  content:""; }

.bp3-icon-new-person::before{
  content:""; }

.bp3-icon-new-prescription::before{
  content:""; }

.bp3-icon-new-text-box::before{
  content:""; }

.bp3-icon-ninja::before{
  content:""; }

.bp3-icon-not-equal-to::before{
  content:""; }

.bp3-icon-notifications::before{
  content:""; }

.bp3-icon-notifications-updated::before{
  content:""; }

.bp3-icon-numbered-list::before{
  content:""; }

.bp3-icon-numerical::before{
  content:""; }

.bp3-icon-office::before{
  content:""; }

.bp3-icon-offline::before{
  content:""; }

.bp3-icon-oil-field::before{
  content:""; }

.bp3-icon-one-column::before{
  content:""; }

.bp3-icon-outdated::before{
  content:""; }

.bp3-icon-page-layout::before{
  content:""; }

.bp3-icon-panel-stats::before{
  content:""; }

.bp3-icon-panel-table::before{
  content:""; }

.bp3-icon-paperclip::before{
  content:""; }

.bp3-icon-paragraph::before{
  content:""; }

.bp3-icon-path::before{
  content:""; }

.bp3-icon-path-search::before{
  content:""; }

.bp3-icon-pause::before{
  content:""; }

.bp3-icon-people::before{
  content:""; }

.bp3-icon-percentage::before{
  content:""; }

.bp3-icon-person::before{
  content:""; }

.bp3-icon-phone::before{
  content:"☎"; }

.bp3-icon-pie-chart::before{
  content:""; }

.bp3-icon-pin::before{
  content:""; }

.bp3-icon-pivot::before{
  content:""; }

.bp3-icon-pivot-table::before{
  content:""; }

.bp3-icon-play::before{
  content:""; }

.bp3-icon-plus::before{
  content:"+"; }

.bp3-icon-polygon-filter::before{
  content:""; }

.bp3-icon-power::before{
  content:""; }

.bp3-icon-predictive-analysis::before{
  content:""; }

.bp3-icon-prescription::before{
  content:""; }

.bp3-icon-presentation::before{
  content:""; }

.bp3-icon-print::before{
  content:"⎙"; }

.bp3-icon-projects::before{
  content:""; }

.bp3-icon-properties::before{
  content:""; }

.bp3-icon-property::before{
  content:""; }

.bp3-icon-publish-function::before{
  content:""; }

.bp3-icon-pulse::before{
  content:""; }

.bp3-icon-random::before{
  content:""; }

.bp3-icon-record::before{
  content:""; }

.bp3-icon-redo::before{
  content:""; }

.bp3-icon-refresh::before{
  content:""; }

.bp3-icon-regression-chart::before{
  content:""; }

.bp3-icon-remove::before{
  content:""; }

.bp3-icon-remove-column::before{
  content:""; }

.bp3-icon-remove-column-left::before{
  content:""; }

.bp3-icon-remove-column-right::before{
  content:""; }

.bp3-icon-remove-row-bottom::before{
  content:""; }

.bp3-icon-remove-row-top::before{
  content:""; }

.bp3-icon-repeat::before{
  content:""; }

.bp3-icon-reset::before{
  content:""; }

.bp3-icon-resolve::before{
  content:""; }

.bp3-icon-rig::before{
  content:""; }

.bp3-icon-right-join::before{
  content:""; }

.bp3-icon-ring::before{
  content:""; }

.bp3-icon-rotate-document::before{
  content:""; }

.bp3-icon-rotate-page::before{
  content:""; }

.bp3-icon-satellite::before{
  content:""; }

.bp3-icon-saved::before{
  content:""; }

.bp3-icon-scatter-plot::before{
  content:""; }

.bp3-icon-search::before{
  content:""; }

.bp3-icon-search-around::before{
  content:""; }

.bp3-icon-search-template::before{
  content:""; }

.bp3-icon-search-text::before{
  content:""; }

.bp3-icon-segmented-control::before{
  content:""; }

.bp3-icon-select::before{
  content:""; }

.bp3-icon-selection::before{
  content:"⦿"; }

.bp3-icon-send-to::before{
  content:""; }

.bp3-icon-send-to-graph::before{
  content:""; }

.bp3-icon-send-to-map::before{
  content:""; }

.bp3-icon-series-add::before{
  content:""; }

.bp3-icon-series-configuration::before{
  content:""; }

.bp3-icon-series-derived::before{
  content:""; }

.bp3-icon-series-filtered::before{
  content:""; }

.bp3-icon-series-search::before{
  content:""; }

.bp3-icon-settings::before{
  content:""; }

.bp3-icon-share::before{
  content:""; }

.bp3-icon-shield::before{
  content:""; }

.bp3-icon-shop::before{
  content:""; }

.bp3-icon-shopping-cart::before{
  content:""; }

.bp3-icon-signal-search::before{
  content:""; }

.bp3-icon-sim-card::before{
  content:""; }

.bp3-icon-slash::before{
  content:""; }

.bp3-icon-small-cross::before{
  content:""; }

.bp3-icon-small-minus::before{
  content:""; }

.bp3-icon-small-plus::before{
  content:""; }

.bp3-icon-small-tick::before{
  content:""; }

.bp3-icon-snowflake::before{
  content:""; }

.bp3-icon-social-media::before{
  content:""; }

.bp3-icon-sort::before{
  content:""; }

.bp3-icon-sort-alphabetical::before{
  content:""; }

.bp3-icon-sort-alphabetical-desc::before{
  content:""; }

.bp3-icon-sort-asc::before{
  content:""; }

.bp3-icon-sort-desc::before{
  content:""; }

.bp3-icon-sort-numerical::before{
  content:""; }

.bp3-icon-sort-numerical-desc::before{
  content:""; }

.bp3-icon-split-columns::before{
  content:""; }

.bp3-icon-square::before{
  content:""; }

.bp3-icon-stacked-chart::before{
  content:""; }

.bp3-icon-star::before{
  content:"★"; }

.bp3-icon-star-empty::before{
  content:"☆"; }

.bp3-icon-step-backward::before{
  content:""; }

.bp3-icon-step-chart::before{
  content:""; }

.bp3-icon-step-forward::before{
  content:""; }

.bp3-icon-stop::before{
  content:""; }

.bp3-icon-stopwatch::before{
  content:""; }

.bp3-icon-strikethrough::before{
  content:""; }

.bp3-icon-style::before{
  content:""; }

.bp3-icon-swap-horizontal::before{
  content:""; }

.bp3-icon-swap-vertical::before{
  content:""; }

.bp3-icon-symbol-circle::before{
  content:""; }

.bp3-icon-symbol-cross::before{
  content:""; }

.bp3-icon-symbol-diamond::before{
  content:""; }

.bp3-icon-symbol-square::before{
  content:""; }

.bp3-icon-symbol-triangle-down::before{
  content:""; }

.bp3-icon-symbol-triangle-up::before{
  content:""; }

.bp3-icon-tag::before{
  content:""; }

.bp3-icon-take-action::before{
  content:""; }

.bp3-icon-taxi::before{
  content:""; }

.bp3-icon-text-highlight::before{
  content:""; }

.bp3-icon-th::before{
  content:""; }

.bp3-icon-th-derived::before{
  content:""; }

.bp3-icon-th-disconnect::before{
  content:""; }

.bp3-icon-th-filtered::before{
  content:""; }

.bp3-icon-th-list::before{
  content:""; }

.bp3-icon-thumbs-down::before{
  content:""; }

.bp3-icon-thumbs-up::before{
  content:""; }

.bp3-icon-tick::before{
  content:"✓"; }

.bp3-icon-tick-circle::before{
  content:""; }

.bp3-icon-time::before{
  content:"⏲"; }

.bp3-icon-timeline-area-chart::before{
  content:""; }

.bp3-icon-timeline-bar-chart::before{
  content:""; }

.bp3-icon-timeline-events::before{
  content:""; }

.bp3-icon-timeline-line-chart::before{
  content:""; }

.bp3-icon-tint::before{
  content:""; }

.bp3-icon-torch::before{
  content:""; }

.bp3-icon-tractor::before{
  content:""; }

.bp3-icon-train::before{
  content:""; }

.bp3-icon-translate::before{
  content:""; }

.bp3-icon-trash::before{
  content:""; }

.bp3-icon-tree::before{
  content:""; }

.bp3-icon-trending-down::before{
  content:""; }

.bp3-icon-trending-up::before{
  content:""; }

.bp3-icon-truck::before{
  content:""; }

.bp3-icon-two-columns::before{
  content:""; }

.bp3-icon-unarchive::before{
  content:""; }

.bp3-icon-underline::before{
  content:"⎁"; }

.bp3-icon-undo::before{
  content:"⎌"; }

.bp3-icon-ungroup-objects::before{
  content:""; }

.bp3-icon-unknown-vehicle::before{
  content:""; }

.bp3-icon-unlock::before{
  content:""; }

.bp3-icon-unpin::before{
  content:""; }

.bp3-icon-unresolve::before{
  content:""; }

.bp3-icon-updated::before{
  content:""; }

.bp3-icon-upload::before{
  content:""; }

.bp3-icon-user::before{
  content:""; }

.bp3-icon-variable::before{
  content:""; }

.bp3-icon-vertical-bar-chart-asc::before{
  content:""; }

.bp3-icon-vertical-bar-chart-desc::before{
  content:""; }

.bp3-icon-vertical-distribution::before{
  content:""; }

.bp3-icon-video::before{
  content:""; }

.bp3-icon-volume-down::before{
  content:""; }

.bp3-icon-volume-off::before{
  content:""; }

.bp3-icon-volume-up::before{
  content:""; }

.bp3-icon-walk::before{
  content:""; }

.bp3-icon-warning-sign::before{
  content:""; }

.bp3-icon-waterfall-chart::before{
  content:""; }

.bp3-icon-widget::before{
  content:""; }

.bp3-icon-widget-button::before{
  content:""; }

.bp3-icon-widget-footer::before{
  content:""; }

.bp3-icon-widget-header::before{
  content:""; }

.bp3-icon-wrench::before{
  content:""; }

.bp3-icon-zoom-in::before{
  content:""; }

.bp3-icon-zoom-out::before{
  content:""; }

.bp3-icon-zoom-to-fit::before{
  content:""; }
.bp3-submenu > .bp3-popover-wrapper{
  display:block; }

.bp3-submenu .bp3-popover-target{
  display:block; }
  .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-menu-item{ }

.bp3-submenu.bp3-popover{
  -webkit-box-shadow:none;
          box-shadow:none;
  padding:0 5px; }
  .bp3-submenu.bp3-popover > .bp3-popover-content{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2); }
  .bp3-dark .bp3-submenu.bp3-popover, .bp3-submenu.bp3-popover.bp3-dark{
    -webkit-box-shadow:none;
            box-shadow:none; }
    .bp3-dark .bp3-submenu.bp3-popover > .bp3-popover-content, .bp3-submenu.bp3-popover.bp3-dark > .bp3-popover-content{
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4); }
.bp3-menu{
  background:#ffffff;
  border-radius:3px;
  color:#182026;
  list-style:none;
  margin:0;
  min-width:180px;
  padding:5px;
  text-align:left; }

.bp3-menu-divider{
  border-top:1px solid rgba(16, 22, 26, 0.15);
  display:block;
  margin:5px; }
  .bp3-dark .bp3-menu-divider{
    border-top-color:rgba(255, 255, 255, 0.15); }

.bp3-menu-item{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-orient:horizontal;
  -webkit-box-direction:normal;
      -ms-flex-direction:row;
          flex-direction:row;
  -webkit-box-align:start;
      -ms-flex-align:start;
          align-items:flex-start;
  border-radius:2px;
  color:inherit;
  line-height:20px;
  padding:5px 7px;
  text-decoration:none;
  -webkit-user-select:none;
     -moz-user-select:none;
      -ms-user-select:none;
          user-select:none; }
  .bp3-menu-item > *{
    -webkit-box-flex:0;
        -ms-flex-positive:0;
            flex-grow:0;
    -ms-flex-negative:0;
        flex-shrink:0; }
  .bp3-menu-item > .bp3-fill{
    -webkit-box-flex:1;
        -ms-flex-positive:1;
            flex-grow:1;
    -ms-flex-negative:1;
        flex-shrink:1; }
  .bp3-menu-item::before,
  .bp3-menu-item > *{
    margin-right:7px; }
  .bp3-menu-item:empty::before,
  .bp3-menu-item > :last-child{
    margin-right:0; }
  .bp3-menu-item > .bp3-fill{
    word-break:break-word; }
  .bp3-menu-item:hover, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-menu-item{
    background-color:rgba(167, 182, 194, 0.3);
    cursor:pointer;
    text-decoration:none; }
  .bp3-menu-item.bp3-disabled{
    background-color:inherit;
    color:rgba(92, 112, 128, 0.6);
    cursor:not-allowed; }
  .bp3-dark .bp3-menu-item{
    color:inherit; }
    .bp3-dark .bp3-menu-item:hover, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-menu-item, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-menu-item{
      background-color:rgba(138, 155, 168, 0.15);
      color:inherit; }
    .bp3-dark .bp3-menu-item.bp3-disabled{
      background-color:inherit;
      color:rgba(167, 182, 194, 0.6); }
  .bp3-menu-item.bp3-intent-primary{
    color:#106ba3; }
    .bp3-menu-item.bp3-intent-primary .bp3-icon{
      color:inherit; }
    .bp3-menu-item.bp3-intent-primary::before, .bp3-menu-item.bp3-intent-primary::after,
    .bp3-menu-item.bp3-intent-primary .bp3-menu-item-label{
      color:#106ba3; }
    .bp3-menu-item.bp3-intent-primary:hover, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item, .bp3-menu-item.bp3-intent-primary.bp3-active{
      background-color:#137cbd; }
    .bp3-menu-item.bp3-intent-primary:active{
      background-color:#106ba3; }
    .bp3-menu-item.bp3-intent-primary:hover, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item, .bp3-menu-item.bp3-intent-primary:hover::before, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item::before, .bp3-menu-item.bp3-intent-primary:hover::after, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item::after,
    .bp3-menu-item.bp3-intent-primary:hover .bp3-menu-item-label,
    .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item .bp3-menu-item-label, .bp3-menu-item.bp3-intent-primary:active, .bp3-menu-item.bp3-intent-primary:active::before, .bp3-menu-item.bp3-intent-primary:active::after,
    .bp3-menu-item.bp3-intent-primary:active .bp3-menu-item-label, .bp3-menu-item.bp3-intent-primary.bp3-active, .bp3-menu-item.bp3-intent-primary.bp3-active::before, .bp3-menu-item.bp3-intent-primary.bp3-active::after,
    .bp3-menu-item.bp3-intent-primary.bp3-active .bp3-menu-item-label{
      color:#ffffff; }
  .bp3-menu-item.bp3-intent-success{
    color:#0d8050; }
    .bp3-menu-item.bp3-intent-success .bp3-icon{
      color:inherit; }
    .bp3-menu-item.bp3-intent-success::before, .bp3-menu-item.bp3-intent-success::after,
    .bp3-menu-item.bp3-intent-success .bp3-menu-item-label{
      color:#0d8050; }
    .bp3-menu-item.bp3-intent-success:hover, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item, .bp3-menu-item.bp3-intent-success.bp3-active{
      background-color:#0f9960; }
    .bp3-menu-item.bp3-intent-success:active{
      background-color:#0d8050; }
    .bp3-menu-item.bp3-intent-success:hover, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item, .bp3-menu-item.bp3-intent-success:hover::before, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item::before, .bp3-menu-item.bp3-intent-success:hover::after, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item::after,
    .bp3-menu-item.bp3-intent-success:hover .bp3-menu-item-label,
    .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item .bp3-menu-item-label, .bp3-menu-item.bp3-intent-success:active, .bp3-menu-item.bp3-intent-success:active::before, .bp3-menu-item.bp3-intent-success:active::after,
    .bp3-menu-item.bp3-intent-success:active .bp3-menu-item-label, .bp3-menu-item.bp3-intent-success.bp3-active, .bp3-menu-item.bp3-intent-success.bp3-active::before, .bp3-menu-item.bp3-intent-success.bp3-active::after,
    .bp3-menu-item.bp3-intent-success.bp3-active .bp3-menu-item-label{
      color:#ffffff; }
  .bp3-menu-item.bp3-intent-warning{
    color:#bf7326; }
    .bp3-menu-item.bp3-intent-warning .bp3-icon{
      color:inherit; }
    .bp3-menu-item.bp3-intent-warning::before, .bp3-menu-item.bp3-intent-warning::after,
    .bp3-menu-item.bp3-intent-warning .bp3-menu-item-label{
      color:#bf7326; }
    .bp3-menu-item.bp3-intent-warning:hover, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item, .bp3-menu-item.bp3-intent-warning.bp3-active{
      background-color:#d9822b; }
    .bp3-menu-item.bp3-intent-warning:active{
      background-color:#bf7326; }
    .bp3-menu-item.bp3-intent-warning:hover, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item, .bp3-menu-item.bp3-intent-warning:hover::before, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item::before, .bp3-menu-item.bp3-intent-warning:hover::after, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item::after,
    .bp3-menu-item.bp3-intent-warning:hover .bp3-menu-item-label,
    .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item .bp3-menu-item-label, .bp3-menu-item.bp3-intent-warning:active, .bp3-menu-item.bp3-intent-warning:active::before, .bp3-menu-item.bp3-intent-warning:active::after,
    .bp3-menu-item.bp3-intent-warning:active .bp3-menu-item-label, .bp3-menu-item.bp3-intent-warning.bp3-active, .bp3-menu-item.bp3-intent-warning.bp3-active::before, .bp3-menu-item.bp3-intent-warning.bp3-active::after,
    .bp3-menu-item.bp3-intent-warning.bp3-active .bp3-menu-item-label{
      color:#ffffff; }
  .bp3-menu-item.bp3-intent-danger{
    color:#c23030; }
    .bp3-menu-item.bp3-intent-danger .bp3-icon{
      color:inherit; }
    .bp3-menu-item.bp3-intent-danger::before, .bp3-menu-item.bp3-intent-danger::after,
    .bp3-menu-item.bp3-intent-danger .bp3-menu-item-label{
      color:#c23030; }
    .bp3-menu-item.bp3-intent-danger:hover, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item, .bp3-menu-item.bp3-intent-danger.bp3-active{
      background-color:#db3737; }
    .bp3-menu-item.bp3-intent-danger:active{
      background-color:#c23030; }
    .bp3-menu-item.bp3-intent-danger:hover, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item, .bp3-menu-item.bp3-intent-danger:hover::before, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item::before, .bp3-menu-item.bp3-intent-danger:hover::after, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item::after,
    .bp3-menu-item.bp3-intent-danger:hover .bp3-menu-item-label,
    .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item .bp3-menu-item-label, .bp3-menu-item.bp3-intent-danger:active, .bp3-menu-item.bp3-intent-danger:active::before, .bp3-menu-item.bp3-intent-danger:active::after,
    .bp3-menu-item.bp3-intent-danger:active .bp3-menu-item-label, .bp3-menu-item.bp3-intent-danger.bp3-active, .bp3-menu-item.bp3-intent-danger.bp3-active::before, .bp3-menu-item.bp3-intent-danger.bp3-active::after,
    .bp3-menu-item.bp3-intent-danger.bp3-active .bp3-menu-item-label{
      color:#ffffff; }
  .bp3-menu-item::before{
    font-family:"Icons16", sans-serif;
    font-size:16px;
    font-style:normal;
    font-weight:400;
    line-height:1;
    -moz-osx-font-smoothing:grayscale;
    -webkit-font-smoothing:antialiased;
    margin-right:7px; }
  .bp3-menu-item::before,
  .bp3-menu-item > .bp3-icon{
    color:#5c7080;
    margin-top:2px; }
  .bp3-menu-item .bp3-menu-item-label{
    color:#5c7080; }
  .bp3-menu-item:hover, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-menu-item{
    color:inherit; }
  .bp3-menu-item.bp3-active, .bp3-menu-item:active{
    background-color:rgba(115, 134, 148, 0.3); }
  .bp3-menu-item.bp3-disabled{
    background-color:inherit !important;
    color:rgba(92, 112, 128, 0.6) !important;
    cursor:not-allowed !important;
    outline:none !important; }
    .bp3-menu-item.bp3-disabled::before,
    .bp3-menu-item.bp3-disabled > .bp3-icon,
    .bp3-menu-item.bp3-disabled .bp3-menu-item-label{
      color:rgba(92, 112, 128, 0.6) !important; }
  .bp3-large .bp3-menu-item{
    font-size:16px;
    line-height:22px;
    padding:9px 7px; }
    .bp3-large .bp3-menu-item .bp3-icon{
      margin-top:3px; }
    .bp3-large .bp3-menu-item::before{
      font-family:"Icons20", sans-serif;
      font-size:20px;
      font-style:normal;
      font-weight:400;
      line-height:1;
      -moz-osx-font-smoothing:grayscale;
      -webkit-font-smoothing:antialiased;
      margin-right:10px;
      margin-top:1px; }

button.bp3-menu-item{
  background:none;
  border:none;
  text-align:left;
  width:100%; }
.bp3-menu-header{
  border-top:1px solid rgba(16, 22, 26, 0.15);
  display:block;
  margin:5px;
  cursor:default;
  padding-left:2px; }
  .bp3-dark .bp3-menu-header{
    border-top-color:rgba(255, 255, 255, 0.15); }
  .bp3-menu-header:first-of-type{
    border-top:none; }
  .bp3-menu-header > h6{
    color:#182026;
    font-weight:600;
    overflow:hidden;
    text-overflow:ellipsis;
    white-space:nowrap;
    word-wrap:normal;
    line-height:17px;
    margin:0;
    padding:10px 7px 0 1px; }
    .bp3-dark .bp3-menu-header > h6{
      color:#f5f8fa; }
  .bp3-menu-header:first-of-type > h6{
    padding-top:0; }
  .bp3-large .bp3-menu-header > h6{
    font-size:18px;
    padding-bottom:5px;
    padding-top:15px; }
  .bp3-large .bp3-menu-header:first-of-type > h6{
    padding-top:0; }

.bp3-dark .bp3-menu{
  background:#30404d;
  color:#f5f8fa; }

.bp3-dark .bp3-menu-item{ }
  .bp3-dark .bp3-menu-item.bp3-intent-primary{
    color:#48aff0; }
    .bp3-dark .bp3-menu-item.bp3-intent-primary .bp3-icon{
      color:inherit; }
    .bp3-dark .bp3-menu-item.bp3-intent-primary::before, .bp3-dark .bp3-menu-item.bp3-intent-primary::after,
    .bp3-dark .bp3-menu-item.bp3-intent-primary .bp3-menu-item-label{
      color:#48aff0; }
    .bp3-dark .bp3-menu-item.bp3-intent-primary:hover, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item, .bp3-dark .bp3-menu-item.bp3-intent-primary.bp3-active{
      background-color:#137cbd; }
    .bp3-dark .bp3-menu-item.bp3-intent-primary:active{
      background-color:#106ba3; }
    .bp3-dark .bp3-menu-item.bp3-intent-primary:hover, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item, .bp3-dark .bp3-menu-item.bp3-intent-primary:hover::before, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item::before, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item::before, .bp3-dark .bp3-menu-item.bp3-intent-primary:hover::after, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item::after, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item::after,
    .bp3-dark .bp3-menu-item.bp3-intent-primary:hover .bp3-menu-item-label,
    .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item .bp3-menu-item-label,
    .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item .bp3-menu-item-label, .bp3-dark .bp3-menu-item.bp3-intent-primary:active, .bp3-dark .bp3-menu-item.bp3-intent-primary:active::before, .bp3-dark .bp3-menu-item.bp3-intent-primary:active::after,
    .bp3-dark .bp3-menu-item.bp3-intent-primary:active .bp3-menu-item-label, .bp3-dark .bp3-menu-item.bp3-intent-primary.bp3-active, .bp3-dark .bp3-menu-item.bp3-intent-primary.bp3-active::before, .bp3-dark .bp3-menu-item.bp3-intent-primary.bp3-active::after,
    .bp3-dark .bp3-menu-item.bp3-intent-primary.bp3-active .bp3-menu-item-label{
      color:#ffffff; }
  .bp3-dark .bp3-menu-item.bp3-intent-success{
    color:#3dcc91; }
    .bp3-dark .bp3-menu-item.bp3-intent-success .bp3-icon{
      color:inherit; }
    .bp3-dark .bp3-menu-item.bp3-intent-success::before, .bp3-dark .bp3-menu-item.bp3-intent-success::after,
    .bp3-dark .bp3-menu-item.bp3-intent-success .bp3-menu-item-label{
      color:#3dcc91; }
    .bp3-dark .bp3-menu-item.bp3-intent-success:hover, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item, .bp3-dark .bp3-menu-item.bp3-intent-success.bp3-active{
      background-color:#0f9960; }
    .bp3-dark .bp3-menu-item.bp3-intent-success:active{
      background-color:#0d8050; }
    .bp3-dark .bp3-menu-item.bp3-intent-success:hover, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item, .bp3-dark .bp3-menu-item.bp3-intent-success:hover::before, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item::before, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item::before, .bp3-dark .bp3-menu-item.bp3-intent-success:hover::after, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item::after, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item::after,
    .bp3-dark .bp3-menu-item.bp3-intent-success:hover .bp3-menu-item-label,
    .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item .bp3-menu-item-label,
    .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item .bp3-menu-item-label, .bp3-dark .bp3-menu-item.bp3-intent-success:active, .bp3-dark .bp3-menu-item.bp3-intent-success:active::before, .bp3-dark .bp3-menu-item.bp3-intent-success:active::after,
    .bp3-dark .bp3-menu-item.bp3-intent-success:active .bp3-menu-item-label, .bp3-dark .bp3-menu-item.bp3-intent-success.bp3-active, .bp3-dark .bp3-menu-item.bp3-intent-success.bp3-active::before, .bp3-dark .bp3-menu-item.bp3-intent-success.bp3-active::after,
    .bp3-dark .bp3-menu-item.bp3-intent-success.bp3-active .bp3-menu-item-label{
      color:#ffffff; }
  .bp3-dark .bp3-menu-item.bp3-intent-warning{
    color:#ffb366; }
    .bp3-dark .bp3-menu-item.bp3-intent-warning .bp3-icon{
      color:inherit; }
    .bp3-dark .bp3-menu-item.bp3-intent-warning::before, .bp3-dark .bp3-menu-item.bp3-intent-warning::after,
    .bp3-dark .bp3-menu-item.bp3-intent-warning .bp3-menu-item-label{
      color:#ffb366; }
    .bp3-dark .bp3-menu-item.bp3-intent-warning:hover, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item, .bp3-dark .bp3-menu-item.bp3-intent-warning.bp3-active{
      background-color:#d9822b; }
    .bp3-dark .bp3-menu-item.bp3-intent-warning:active{
      background-color:#bf7326; }
    .bp3-dark .bp3-menu-item.bp3-intent-warning:hover, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item, .bp3-dark .bp3-menu-item.bp3-intent-warning:hover::before, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item::before, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item::before, .bp3-dark .bp3-menu-item.bp3-intent-warning:hover::after, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item::after, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item::after,
    .bp3-dark .bp3-menu-item.bp3-intent-warning:hover .bp3-menu-item-label,
    .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item .bp3-menu-item-label,
    .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item .bp3-menu-item-label, .bp3-dark .bp3-menu-item.bp3-intent-warning:active, .bp3-dark .bp3-menu-item.bp3-intent-warning:active::before, .bp3-dark .bp3-menu-item.bp3-intent-warning:active::after,
    .bp3-dark .bp3-menu-item.bp3-intent-warning:active .bp3-menu-item-label, .bp3-dark .bp3-menu-item.bp3-intent-warning.bp3-active, .bp3-dark .bp3-menu-item.bp3-intent-warning.bp3-active::before, .bp3-dark .bp3-menu-item.bp3-intent-warning.bp3-active::after,
    .bp3-dark .bp3-menu-item.bp3-intent-warning.bp3-active .bp3-menu-item-label{
      color:#ffffff; }
  .bp3-dark .bp3-menu-item.bp3-intent-danger{
    color:#ff7373; }
    .bp3-dark .bp3-menu-item.bp3-intent-danger .bp3-icon{
      color:inherit; }
    .bp3-dark .bp3-menu-item.bp3-intent-danger::before, .bp3-dark .bp3-menu-item.bp3-intent-danger::after,
    .bp3-dark .bp3-menu-item.bp3-intent-danger .bp3-menu-item-label{
      color:#ff7373; }
    .bp3-dark .bp3-menu-item.bp3-intent-danger:hover, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item, .bp3-dark .bp3-menu-item.bp3-intent-danger.bp3-active{
      background-color:#db3737; }
    .bp3-dark .bp3-menu-item.bp3-intent-danger:active{
      background-color:#c23030; }
    .bp3-dark .bp3-menu-item.bp3-intent-danger:hover, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item, .bp3-dark .bp3-menu-item.bp3-intent-danger:hover::before, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item::before, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item::before, .bp3-dark .bp3-menu-item.bp3-intent-danger:hover::after, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item::after, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item::after,
    .bp3-dark .bp3-menu-item.bp3-intent-danger:hover .bp3-menu-item-label,
    .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item .bp3-menu-item-label,
    .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item .bp3-menu-item-label, .bp3-dark .bp3-menu-item.bp3-intent-danger:active, .bp3-dark .bp3-menu-item.bp3-intent-danger:active::before, .bp3-dark .bp3-menu-item.bp3-intent-danger:active::after,
    .bp3-dark .bp3-menu-item.bp3-intent-danger:active .bp3-menu-item-label, .bp3-dark .bp3-menu-item.bp3-intent-danger.bp3-active, .bp3-dark .bp3-menu-item.bp3-intent-danger.bp3-active::before, .bp3-dark .bp3-menu-item.bp3-intent-danger.bp3-active::after,
    .bp3-dark .bp3-menu-item.bp3-intent-danger.bp3-active .bp3-menu-item-label{
      color:#ffffff; }
  .bp3-dark .bp3-menu-item::before,
  .bp3-dark .bp3-menu-item > .bp3-icon{
    color:#a7b6c2; }
  .bp3-dark .bp3-menu-item .bp3-menu-item-label{
    color:#a7b6c2; }
  .bp3-dark .bp3-menu-item.bp3-active, .bp3-dark .bp3-menu-item:active{
    background-color:rgba(138, 155, 168, 0.3); }
  .bp3-dark .bp3-menu-item.bp3-disabled{
    color:rgba(167, 182, 194, 0.6) !important; }
    .bp3-dark .bp3-menu-item.bp3-disabled::before,
    .bp3-dark .bp3-menu-item.bp3-disabled > .bp3-icon,
    .bp3-dark .bp3-menu-item.bp3-disabled .bp3-menu-item-label{
      color:rgba(167, 182, 194, 0.6) !important; }

.bp3-dark .bp3-menu-divider,
.bp3-dark .bp3-menu-header{
  border-color:rgba(255, 255, 255, 0.15); }

.bp3-dark .bp3-menu-header > h6{
  color:#f5f8fa; }

.bp3-label .bp3-menu{
  margin-top:5px; }
.bp3-navbar{
  background-color:#ffffff;
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.2);
  height:50px;
  padding:0 15px;
  position:relative;
  width:100%;
  z-index:10; }
  .bp3-navbar.bp3-dark,
  .bp3-dark .bp3-navbar{
    background-color:#394b59; }
  .bp3-navbar.bp3-dark{
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.4); }
  .bp3-dark .bp3-navbar{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.4); }
  .bp3-navbar.bp3-fixed-top{
    left:0;
    position:fixed;
    right:0;
    top:0; }

.bp3-navbar-heading{
  font-size:16px;
  margin-right:15px; }

.bp3-navbar-group{
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  height:50px; }
  .bp3-navbar-group.bp3-align-left{
    float:left; }
  .bp3-navbar-group.bp3-align-right{
    float:right; }

.bp3-navbar-divider{
  border-left:1px solid rgba(16, 22, 26, 0.15);
  height:20px;
  margin:0 10px; }
  .bp3-dark .bp3-navbar-divider{
    border-left-color:rgba(255, 255, 255, 0.15); }
.bp3-non-ideal-state{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-orient:vertical;
  -webkit-box-direction:normal;
      -ms-flex-direction:column;
          flex-direction:column;
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  height:100%;
  -webkit-box-pack:center;
      -ms-flex-pack:center;
          justify-content:center;
  text-align:center;
  width:100%; }
  .bp3-non-ideal-state > *{
    -webkit-box-flex:0;
        -ms-flex-positive:0;
            flex-grow:0;
    -ms-flex-negative:0;
        flex-shrink:0; }
  .bp3-non-ideal-state > .bp3-fill{
    -webkit-box-flex:1;
        -ms-flex-positive:1;
            flex-grow:1;
    -ms-flex-negative:1;
        flex-shrink:1; }
  .bp3-non-ideal-state::before,
  .bp3-non-ideal-state > *{
    margin-bottom:20px; }
  .bp3-non-ideal-state:empty::before,
  .bp3-non-ideal-state > :last-child{
    margin-bottom:0; }
  .bp3-non-ideal-state > *{
    max-width:400px; }

.bp3-non-ideal-state-visual{
  color:rgba(92, 112, 128, 0.6);
  font-size:60px; }
  .bp3-dark .bp3-non-ideal-state-visual{
    color:rgba(167, 182, 194, 0.6); }

.bp3-overflow-list{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -ms-flex-wrap:nowrap;
      flex-wrap:nowrap;
  min-width:0; }

.bp3-overflow-list-spacer{
  -ms-flex-negative:1;
      flex-shrink:1;
  width:1px; }

body.bp3-overlay-open{
  overflow:hidden; }

.bp3-overlay{
  bottom:0;
  left:0;
  position:static;
  right:0;
  top:0;
  z-index:20; }
  .bp3-overlay:not(.bp3-overlay-open){
    pointer-events:none; }
  .bp3-overlay.bp3-overlay-container{
    overflow:hidden;
    position:fixed; }
    .bp3-overlay.bp3-overlay-container.bp3-overlay-inline{
      position:absolute; }
  .bp3-overlay.bp3-overlay-scroll-container{
    overflow:auto;
    position:fixed; }
    .bp3-overlay.bp3-overlay-scroll-container.bp3-overlay-inline{
      position:absolute; }
  .bp3-overlay.bp3-overlay-inline{
    display:inline;
    overflow:visible; }

.bp3-overlay-content{
  position:fixed;
  z-index:20; }
  .bp3-overlay-inline .bp3-overlay-content,
  .bp3-overlay-scroll-container .bp3-overlay-content{
    position:absolute; }

.bp3-overlay-backdrop{
  bottom:0;
  left:0;
  position:fixed;
  right:0;
  top:0;
  opacity:1;
  background-color:rgba(16, 22, 26, 0.7);
  overflow:auto;
  -webkit-user-select:none;
     -moz-user-select:none;
      -ms-user-select:none;
          user-select:none;
  z-index:20; }
  .bp3-overlay-backdrop.bp3-overlay-enter, .bp3-overlay-backdrop.bp3-overlay-appear{
    opacity:0; }
  .bp3-overlay-backdrop.bp3-overlay-enter-active, .bp3-overlay-backdrop.bp3-overlay-appear-active{
    opacity:1;
    -webkit-transition-delay:0;
            transition-delay:0;
    -webkit-transition-duration:200ms;
            transition-duration:200ms;
    -webkit-transition-property:opacity;
    transition-property:opacity;
    -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
            transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-overlay-backdrop.bp3-overlay-exit{
    opacity:1; }
  .bp3-overlay-backdrop.bp3-overlay-exit-active{
    opacity:0;
    -webkit-transition-delay:0;
            transition-delay:0;
    -webkit-transition-duration:200ms;
            transition-duration:200ms;
    -webkit-transition-property:opacity;
    transition-property:opacity;
    -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
            transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-overlay-backdrop:focus{
    outline:none; }
  .bp3-overlay-inline .bp3-overlay-backdrop{
    position:absolute; }
.bp3-panel-stack{
  overflow:hidden;
  position:relative; }

.bp3-panel-stack-header{
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  -webkit-box-shadow:0 1px rgba(16, 22, 26, 0.15);
          box-shadow:0 1px rgba(16, 22, 26, 0.15);
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -ms-flex-negative:0;
      flex-shrink:0;
  height:30px;
  z-index:1; }
  .bp3-dark .bp3-panel-stack-header{
    -webkit-box-shadow:0 1px rgba(255, 255, 255, 0.15);
            box-shadow:0 1px rgba(255, 255, 255, 0.15); }
  .bp3-panel-stack-header > span{
    -webkit-box-align:stretch;
        -ms-flex-align:stretch;
            align-items:stretch;
    display:-webkit-box;
    display:-ms-flexbox;
    display:flex;
    -webkit-box-flex:1;
        -ms-flex:1;
            flex:1; }
  .bp3-panel-stack-header .bp3-heading{
    margin:0 5px; }

.bp3-button.bp3-panel-stack-header-back{
  margin-left:5px;
  padding-left:0;
  white-space:nowrap; }
  .bp3-button.bp3-panel-stack-header-back .bp3-icon{
    margin:0 2px; }

.bp3-panel-stack-view{
  bottom:0;
  left:0;
  position:absolute;
  right:0;
  top:0;
  background-color:#ffffff;
  border-right:1px solid rgba(16, 22, 26, 0.15);
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-orient:vertical;
  -webkit-box-direction:normal;
      -ms-flex-direction:column;
          flex-direction:column;
  margin-right:-1px;
  overflow-y:auto;
  z-index:1; }
  .bp3-dark .bp3-panel-stack-view{
    background-color:#30404d; }
  .bp3-panel-stack-view:nth-last-child(n + 4){
    display:none; }

.bp3-panel-stack-push .bp3-panel-stack-enter, .bp3-panel-stack-push .bp3-panel-stack-appear{
  -webkit-transform:translateX(100%);
          transform:translateX(100%);
  opacity:0; }

.bp3-panel-stack-push .bp3-panel-stack-enter-active, .bp3-panel-stack-push .bp3-panel-stack-appear-active{
  -webkit-transform:translate(0%);
          transform:translate(0%);
  opacity:1;
  -webkit-transition-delay:0;
          transition-delay:0;
  -webkit-transition-duration:400ms;
          transition-duration:400ms;
  -webkit-transition-property:opacity, -webkit-transform;
  transition-property:opacity, -webkit-transform;
  transition-property:transform, opacity;
  transition-property:transform, opacity, -webkit-transform;
  -webkit-transition-timing-function:ease;
          transition-timing-function:ease; }

.bp3-panel-stack-push .bp3-panel-stack-exit{
  -webkit-transform:translate(0%);
          transform:translate(0%);
  opacity:1; }

.bp3-panel-stack-push .bp3-panel-stack-exit-active{
  -webkit-transform:translateX(-50%);
          transform:translateX(-50%);
  opacity:0;
  -webkit-transition-delay:0;
          transition-delay:0;
  -webkit-transition-duration:400ms;
          transition-duration:400ms;
  -webkit-transition-property:opacity, -webkit-transform;
  transition-property:opacity, -webkit-transform;
  transition-property:transform, opacity;
  transition-property:transform, opacity, -webkit-transform;
  -webkit-transition-timing-function:ease;
          transition-timing-function:ease; }

.bp3-panel-stack-pop .bp3-panel-stack-enter, .bp3-panel-stack-pop .bp3-panel-stack-appear{
  -webkit-transform:translateX(-50%);
          transform:translateX(-50%);
  opacity:0; }

.bp3-panel-stack-pop .bp3-panel-stack-enter-active, .bp3-panel-stack-pop .bp3-panel-stack-appear-active{
  -webkit-transform:translate(0%);
          transform:translate(0%);
  opacity:1;
  -webkit-transition-delay:0;
          transition-delay:0;
  -webkit-transition-duration:400ms;
          transition-duration:400ms;
  -webkit-transition-property:opacity, -webkit-transform;
  transition-property:opacity, -webkit-transform;
  transition-property:transform, opacity;
  transition-property:transform, opacity, -webkit-transform;
  -webkit-transition-timing-function:ease;
          transition-timing-function:ease; }

.bp3-panel-stack-pop .bp3-panel-stack-exit{
  -webkit-transform:translate(0%);
          transform:translate(0%);
  opacity:1; }

.bp3-panel-stack-pop .bp3-panel-stack-exit-active{
  -webkit-transform:translateX(100%);
          transform:translateX(100%);
  opacity:0;
  -webkit-transition-delay:0;
          transition-delay:0;
  -webkit-transition-duration:400ms;
          transition-duration:400ms;
  -webkit-transition-property:opacity, -webkit-transform;
  transition-property:opacity, -webkit-transform;
  transition-property:transform, opacity;
  transition-property:transform, opacity, -webkit-transform;
  -webkit-transition-timing-function:ease;
          transition-timing-function:ease; }
.bp3-panel-stack2{
  overflow:hidden;
  position:relative; }

.bp3-panel-stack2-header{
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  -webkit-box-shadow:0 1px rgba(16, 22, 26, 0.15);
          box-shadow:0 1px rgba(16, 22, 26, 0.15);
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -ms-flex-negative:0;
      flex-shrink:0;
  height:30px;
  z-index:1; }
  .bp3-dark .bp3-panel-stack2-header{
    -webkit-box-shadow:0 1px rgba(255, 255, 255, 0.15);
            box-shadow:0 1px rgba(255, 255, 255, 0.15); }
  .bp3-panel-stack2-header > span{
    -webkit-box-align:stretch;
        -ms-flex-align:stretch;
            align-items:stretch;
    display:-webkit-box;
    display:-ms-flexbox;
    display:flex;
    -webkit-box-flex:1;
        -ms-flex:1;
            flex:1; }
  .bp3-panel-stack2-header .bp3-heading{
    margin:0 5px; }

.bp3-button.bp3-panel-stack2-header-back{
  margin-left:5px;
  padding-left:0;
  white-space:nowrap; }
  .bp3-button.bp3-panel-stack2-header-back .bp3-icon{
    margin:0 2px; }

.bp3-panel-stack2-view{
  bottom:0;
  left:0;
  position:absolute;
  right:0;
  top:0;
  background-color:#ffffff;
  border-right:1px solid rgba(16, 22, 26, 0.15);
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-orient:vertical;
  -webkit-box-direction:normal;
      -ms-flex-direction:column;
          flex-direction:column;
  margin-right:-1px;
  overflow-y:auto;
  z-index:1; }
  .bp3-dark .bp3-panel-stack2-view{
    background-color:#30404d; }
  .bp3-panel-stack2-view:nth-last-child(n + 4){
    display:none; }

.bp3-panel-stack2-push .bp3-panel-stack2-enter, .bp3-panel-stack2-push .bp3-panel-stack2-appear{
  -webkit-transform:translateX(100%);
          transform:translateX(100%);
  opacity:0; }

.bp3-panel-stack2-push .bp3-panel-stack2-enter-active, .bp3-panel-stack2-push .bp3-panel-stack2-appear-active{
  -webkit-transform:translate(0%);
          transform:translate(0%);
  opacity:1;
  -webkit-transition-delay:0;
          transition-delay:0;
  -webkit-transition-duration:400ms;
          transition-duration:400ms;
  -webkit-transition-property:opacity, -webkit-transform;
  transition-property:opacity, -webkit-transform;
  transition-property:transform, opacity;
  transition-property:transform, opacity, -webkit-transform;
  -webkit-transition-timing-function:ease;
          transition-timing-function:ease; }

.bp3-panel-stack2-push .bp3-panel-stack2-exit{
  -webkit-transform:translate(0%);
          transform:translate(0%);
  opacity:1; }

.bp3-panel-stack2-push .bp3-panel-stack2-exit-active{
  -webkit-transform:translateX(-50%);
          transform:translateX(-50%);
  opacity:0;
  -webkit-transition-delay:0;
          transition-delay:0;
  -webkit-transition-duration:400ms;
          transition-duration:400ms;
  -webkit-transition-property:opacity, -webkit-transform;
  transition-property:opacity, -webkit-transform;
  transition-property:transform, opacity;
  transition-property:transform, opacity, -webkit-transform;
  -webkit-transition-timing-function:ease;
          transition-timing-function:ease; }

.bp3-panel-stack2-pop .bp3-panel-stack2-enter, .bp3-panel-stack2-pop .bp3-panel-stack2-appear{
  -webkit-transform:translateX(-50%);
          transform:translateX(-50%);
  opacity:0; }

.bp3-panel-stack2-pop .bp3-panel-stack2-enter-active, .bp3-panel-stack2-pop .bp3-panel-stack2-appear-active{
  -webkit-transform:translate(0%);
          transform:translate(0%);
  opacity:1;
  -webkit-transition-delay:0;
          transition-delay:0;
  -webkit-transition-duration:400ms;
          transition-duration:400ms;
  -webkit-transition-property:opacity, -webkit-transform;
  transition-property:opacity, -webkit-transform;
  transition-property:transform, opacity;
  transition-property:transform, opacity, -webkit-transform;
  -webkit-transition-timing-function:ease;
          transition-timing-function:ease; }

.bp3-panel-stack2-pop .bp3-panel-stack2-exit{
  -webkit-transform:translate(0%);
          transform:translate(0%);
  opacity:1; }

.bp3-panel-stack2-pop .bp3-panel-stack2-exit-active{
  -webkit-transform:translateX(100%);
          transform:translateX(100%);
  opacity:0;
  -webkit-transition-delay:0;
          transition-delay:0;
  -webkit-transition-duration:400ms;
          transition-duration:400ms;
  -webkit-transition-property:opacity, -webkit-transform;
  transition-property:opacity, -webkit-transform;
  transition-property:transform, opacity;
  transition-property:transform, opacity, -webkit-transform;
  -webkit-transition-timing-function:ease;
          transition-timing-function:ease; }
.bp3-popover{
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
  -webkit-transform:scale(1);
          transform:scale(1);
  border-radius:3px;
  display:inline-block;
  z-index:20; }
  .bp3-popover .bp3-popover-arrow{
    height:30px;
    position:absolute;
    width:30px; }
    .bp3-popover .bp3-popover-arrow::before{
      height:20px;
      margin:5px;
      width:20px; }
  .bp3-tether-element-attached-bottom.bp3-tether-target-attached-top > .bp3-popover{
    margin-bottom:17px;
    margin-top:-17px; }
    .bp3-tether-element-attached-bottom.bp3-tether-target-attached-top > .bp3-popover > .bp3-popover-arrow{
      bottom:-11px; }
      .bp3-tether-element-attached-bottom.bp3-tether-target-attached-top > .bp3-popover > .bp3-popover-arrow svg{
        -webkit-transform:rotate(-90deg);
                transform:rotate(-90deg); }
  .bp3-tether-element-attached-left.bp3-tether-target-attached-right > .bp3-popover{
    margin-left:17px; }
    .bp3-tether-element-attached-left.bp3-tether-target-attached-right > .bp3-popover > .bp3-popover-arrow{
      left:-11px; }
      .bp3-tether-element-attached-left.bp3-tether-target-attached-right > .bp3-popover > .bp3-popover-arrow svg{
        -webkit-transform:rotate(0);
                transform:rotate(0); }
  .bp3-tether-element-attached-top.bp3-tether-target-attached-bottom > .bp3-popover{
    margin-top:17px; }
    .bp3-tether-element-attached-top.bp3-tether-target-attached-bottom > .bp3-popover > .bp3-popover-arrow{
      top:-11px; }
      .bp3-tether-element-attached-top.bp3-tether-target-attached-bottom > .bp3-popover > .bp3-popover-arrow svg{
        -webkit-transform:rotate(90deg);
                transform:rotate(90deg); }
  .bp3-tether-element-attached-right.bp3-tether-target-attached-left > .bp3-popover{
    margin-left:-17px;
    margin-right:17px; }
    .bp3-tether-element-attached-right.bp3-tether-target-attached-left > .bp3-popover > .bp3-popover-arrow{
      right:-11px; }
      .bp3-tether-element-attached-right.bp3-tether-target-attached-left > .bp3-popover > .bp3-popover-arrow svg{
        -webkit-transform:rotate(180deg);
                transform:rotate(180deg); }
  .bp3-tether-element-attached-middle > .bp3-popover > .bp3-popover-arrow{
    top:50%;
    -webkit-transform:translateY(-50%);
            transform:translateY(-50%); }
  .bp3-tether-element-attached-center > .bp3-popover > .bp3-popover-arrow{
    right:50%;
    -webkit-transform:translateX(50%);
            transform:translateX(50%); }
  .bp3-tether-element-attached-top.bp3-tether-target-attached-top > .bp3-popover > .bp3-popover-arrow{
    top:-0.3934px; }
  .bp3-tether-element-attached-right.bp3-tether-target-attached-right > .bp3-popover > .bp3-popover-arrow{
    right:-0.3934px; }
  .bp3-tether-element-attached-left.bp3-tether-target-attached-left > .bp3-popover > .bp3-popover-arrow{
    left:-0.3934px; }
  .bp3-tether-element-attached-bottom.bp3-tether-target-attached-bottom > .bp3-popover > .bp3-popover-arrow{
    bottom:-0.3934px; }
  .bp3-tether-element-attached-top.bp3-tether-element-attached-left > .bp3-popover{
    -webkit-transform-origin:top left;
            transform-origin:top left; }
  .bp3-tether-element-attached-top.bp3-tether-element-attached-center > .bp3-popover{
    -webkit-transform-origin:top center;
            transform-origin:top center; }
  .bp3-tether-element-attached-top.bp3-tether-element-attached-right > .bp3-popover{
    -webkit-transform-origin:top right;
            transform-origin:top right; }
  .bp3-tether-element-attached-middle.bp3-tether-element-attached-left > .bp3-popover{
    -webkit-transform-origin:center left;
            transform-origin:center left; }
  .bp3-tether-element-attached-middle.bp3-tether-element-attached-center > .bp3-popover{
    -webkit-transform-origin:center center;
            transform-origin:center center; }
  .bp3-tether-element-attached-middle.bp3-tether-element-attached-right > .bp3-popover{
    -webkit-transform-origin:center right;
            transform-origin:center right; }
  .bp3-tether-element-attached-bottom.bp3-tether-element-attached-left > .bp3-popover{
    -webkit-transform-origin:bottom left;
            transform-origin:bottom left; }
  .bp3-tether-element-attached-bottom.bp3-tether-element-attached-center > .bp3-popover{
    -webkit-transform-origin:bottom center;
            transform-origin:bottom center; }
  .bp3-tether-element-attached-bottom.bp3-tether-element-attached-right > .bp3-popover{
    -webkit-transform-origin:bottom right;
            transform-origin:bottom right; }
  .bp3-popover .bp3-popover-content{
    background:#ffffff;
    color:inherit; }
  .bp3-popover .bp3-popover-arrow::before{
    -webkit-box-shadow:1px 1px 6px rgba(16, 22, 26, 0.2);
            box-shadow:1px 1px 6px rgba(16, 22, 26, 0.2); }
  .bp3-popover .bp3-popover-arrow-border{
    fill:#10161a;
    fill-opacity:0.1; }
  .bp3-popover .bp3-popover-arrow-fill{
    fill:#ffffff; }
  .bp3-popover-enter > .bp3-popover, .bp3-popover-appear > .bp3-popover{
    -webkit-transform:scale(0.3);
            transform:scale(0.3); }
  .bp3-popover-enter-active > .bp3-popover, .bp3-popover-appear-active > .bp3-popover{
    -webkit-transform:scale(1);
            transform:scale(1);
    -webkit-transition-delay:0;
            transition-delay:0;
    -webkit-transition-duration:300ms;
            transition-duration:300ms;
    -webkit-transition-property:-webkit-transform;
    transition-property:-webkit-transform;
    transition-property:transform;
    transition-property:transform, -webkit-transform;
    -webkit-transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11);
            transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11); }
  .bp3-popover-exit > .bp3-popover{
    -webkit-transform:scale(1);
            transform:scale(1); }
  .bp3-popover-exit-active > .bp3-popover{
    -webkit-transform:scale(0.3);
            transform:scale(0.3);
    -webkit-transition-delay:0;
            transition-delay:0;
    -webkit-transition-duration:300ms;
            transition-duration:300ms;
    -webkit-transition-property:-webkit-transform;
    transition-property:-webkit-transform;
    transition-property:transform;
    transition-property:transform, -webkit-transform;
    -webkit-transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11);
            transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11); }
  .bp3-popover .bp3-popover-content{
    border-radius:3px;
    position:relative; }
  .bp3-popover.bp3-popover-content-sizing .bp3-popover-content{
    max-width:350px;
    padding:20px; }
  .bp3-popover-target + .bp3-overlay .bp3-popover.bp3-popover-content-sizing{
    width:350px; }
  .bp3-popover.bp3-minimal{
    margin:0 !important; }
    .bp3-popover.bp3-minimal .bp3-popover-arrow{
      display:none; }
    .bp3-popover.bp3-minimal.bp3-popover{
      -webkit-transform:scale(1);
              transform:scale(1); }
      .bp3-popover-enter > .bp3-popover.bp3-minimal.bp3-popover, .bp3-popover-appear > .bp3-popover.bp3-minimal.bp3-popover{
        -webkit-transform:scale(1);
                transform:scale(1); }
      .bp3-popover-enter-active > .bp3-popover.bp3-minimal.bp3-popover, .bp3-popover-appear-active > .bp3-popover.bp3-minimal.bp3-popover{
        -webkit-transform:scale(1);
                transform:scale(1);
        -webkit-transition-delay:0;
                transition-delay:0;
        -webkit-transition-duration:100ms;
                transition-duration:100ms;
        -webkit-transition-property:-webkit-transform;
        transition-property:-webkit-transform;
        transition-property:transform;
        transition-property:transform, -webkit-transform;
        -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
                transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
      .bp3-popover-exit > .bp3-popover.bp3-minimal.bp3-popover{
        -webkit-transform:scale(1);
                transform:scale(1); }
      .bp3-popover-exit-active > .bp3-popover.bp3-minimal.bp3-popover{
        -webkit-transform:scale(1);
                transform:scale(1);
        -webkit-transition-delay:0;
                transition-delay:0;
        -webkit-transition-duration:100ms;
                transition-duration:100ms;
        -webkit-transition-property:-webkit-transform;
        transition-property:-webkit-transform;
        transition-property:transform;
        transition-property:transform, -webkit-transform;
        -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
                transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-popover.bp3-dark,
  .bp3-dark .bp3-popover{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4); }
    .bp3-popover.bp3-dark .bp3-popover-content,
    .bp3-dark .bp3-popover .bp3-popover-content{
      background:#30404d;
      color:inherit; }
    .bp3-popover.bp3-dark .bp3-popover-arrow::before,
    .bp3-dark .bp3-popover .bp3-popover-arrow::before{
      -webkit-box-shadow:1px 1px 6px rgba(16, 22, 26, 0.4);
              box-shadow:1px 1px 6px rgba(16, 22, 26, 0.4); }
    .bp3-popover.bp3-dark .bp3-popover-arrow-border,
    .bp3-dark .bp3-popover .bp3-popover-arrow-border{
      fill:#10161a;
      fill-opacity:0.2; }
    .bp3-popover.bp3-dark .bp3-popover-arrow-fill,
    .bp3-dark .bp3-popover .bp3-popover-arrow-fill{
      fill:#30404d; }

.bp3-popover-arrow::before{
  border-radius:2px;
  content:"";
  display:block;
  position:absolute;
  -webkit-transform:rotate(45deg);
          transform:rotate(45deg); }

.bp3-tether-pinned .bp3-popover-arrow{
  display:none; }

.bp3-popover-backdrop{
  background:rgba(255, 255, 255, 0); }

.bp3-transition-container{
  opacity:1;
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  z-index:20; }
  .bp3-transition-container.bp3-popover-enter, .bp3-transition-container.bp3-popover-appear{
    opacity:0; }
  .bp3-transition-container.bp3-popover-enter-active, .bp3-transition-container.bp3-popover-appear-active{
    opacity:1;
    -webkit-transition-delay:0;
            transition-delay:0;
    -webkit-transition-duration:100ms;
            transition-duration:100ms;
    -webkit-transition-property:opacity;
    transition-property:opacity;
    -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
            transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-transition-container.bp3-popover-exit{
    opacity:1; }
  .bp3-transition-container.bp3-popover-exit-active{
    opacity:0;
    -webkit-transition-delay:0;
            transition-delay:0;
    -webkit-transition-duration:100ms;
            transition-duration:100ms;
    -webkit-transition-property:opacity;
    transition-property:opacity;
    -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
            transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-transition-container:focus{
    outline:none; }
  .bp3-transition-container.bp3-popover-leave .bp3-popover-content{
    pointer-events:none; }
  .bp3-transition-container[data-x-out-of-boundaries]{
    display:none; }

span.bp3-popover-target{
  display:inline-block; }

.bp3-popover-wrapper.bp3-fill{
  width:100%; }

.bp3-portal{
  left:0;
  position:absolute;
  right:0;
  top:0; }
@-webkit-keyframes linear-progress-bar-stripes{
  from{
    background-position:0 0; }
  to{
    background-position:30px 0; } }
@keyframes linear-progress-bar-stripes{
  from{
    background-position:0 0; }
  to{
    background-position:30px 0; } }

.bp3-progress-bar{
  background:rgba(92, 112, 128, 0.2);
  border-radius:40px;
  display:block;
  height:8px;
  overflow:hidden;
  position:relative;
  width:100%; }
  .bp3-progress-bar .bp3-progress-meter{
    background:linear-gradient(-45deg, rgba(255, 255, 255, 0.2) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.2) 50%, rgba(255, 255, 255, 0.2) 75%, transparent 75%);
    background-color:rgba(92, 112, 128, 0.8);
    background-size:30px 30px;
    border-radius:40px;
    height:100%;
    position:absolute;
    -webkit-transition:width 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
    transition:width 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
    width:100%; }
  .bp3-progress-bar:not(.bp3-no-animation):not(.bp3-no-stripes) .bp3-progress-meter{
    animation:linear-progress-bar-stripes 300ms linear infinite reverse; }
  .bp3-progress-bar.bp3-no-stripes .bp3-progress-meter{
    background-image:none; }

.bp3-dark .bp3-progress-bar{
  background:rgba(16, 22, 26, 0.5); }
  .bp3-dark .bp3-progress-bar .bp3-progress-meter{
    background-color:#8a9ba8; }

.bp3-progress-bar.bp3-intent-primary .bp3-progress-meter{
  background-color:#137cbd; }

.bp3-progress-bar.bp3-intent-success .bp3-progress-meter{
  background-color:#0f9960; }

.bp3-progress-bar.bp3-intent-warning .bp3-progress-meter{
  background-color:#d9822b; }

.bp3-progress-bar.bp3-intent-danger .bp3-progress-meter{
  background-color:#db3737; }
@-webkit-keyframes skeleton-glow{
  from{
    background:rgba(206, 217, 224, 0.2);
    border-color:rgba(206, 217, 224, 0.2); }
  to{
    background:rgba(92, 112, 128, 0.2);
    border-color:rgba(92, 112, 128, 0.2); } }
@keyframes skeleton-glow{
  from{
    background:rgba(206, 217, 224, 0.2);
    border-color:rgba(206, 217, 224, 0.2); }
  to{
    background:rgba(92, 112, 128, 0.2);
    border-color:rgba(92, 112, 128, 0.2); } }
.bp3-skeleton{
  -webkit-animation:1000ms linear infinite alternate skeleton-glow;
          animation:1000ms linear infinite alternate skeleton-glow;
  background:rgba(206, 217, 224, 0.2);
  background-clip:padding-box !important;
  border-color:rgba(206, 217, 224, 0.2) !important;
  border-radius:2px;
  -webkit-box-shadow:none !important;
          box-shadow:none !important;
  color:transparent !important;
  cursor:default;
  pointer-events:none;
  -webkit-user-select:none;
     -moz-user-select:none;
      -ms-user-select:none;
          user-select:none; }
  .bp3-skeleton::before, .bp3-skeleton::after,
  .bp3-skeleton *{
    visibility:hidden !important; }
.bp3-slider{
  height:40px;
  min-width:150px;
  width:100%;
  cursor:default;
  outline:none;
  position:relative;
  -webkit-user-select:none;
     -moz-user-select:none;
      -ms-user-select:none;
          user-select:none; }
  .bp3-slider:hover{
    cursor:pointer; }
  .bp3-slider:active{
    cursor:-webkit-grabbing;
    cursor:grabbing; }
  .bp3-slider.bp3-disabled{
    cursor:not-allowed;
    opacity:0.5; }
  .bp3-slider.bp3-slider-unlabeled{
    height:16px; }

.bp3-slider-track,
.bp3-slider-progress{
  height:6px;
  left:0;
  right:0;
  top:5px;
  position:absolute; }

.bp3-slider-track{
  border-radius:3px;
  overflow:hidden; }

.bp3-slider-progress{
  background:rgba(92, 112, 128, 0.2); }
  .bp3-dark .bp3-slider-progress{
    background:rgba(16, 22, 26, 0.5); }
  .bp3-slider-progress.bp3-intent-primary{
    background-color:#137cbd; }
  .bp3-slider-progress.bp3-intent-success{
    background-color:#0f9960; }
  .bp3-slider-progress.bp3-intent-warning{
    background-color:#d9822b; }
  .bp3-slider-progress.bp3-intent-danger{
    background-color:#db3737; }

.bp3-slider-handle{
  background-color:#f5f8fa;
  background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.8)), to(rgba(255, 255, 255, 0)));
  background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.8), rgba(255, 255, 255, 0));
  -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
          box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
  color:#182026;
  border-radius:3px;
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 1px 1px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 1px 1px rgba(16, 22, 26, 0.2);
  cursor:pointer;
  height:16px;
  left:0;
  position:absolute;
  top:0;
  width:16px; }
  .bp3-slider-handle:hover{
    background-clip:padding-box;
    background-color:#ebf1f5;
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1); }
  .bp3-slider-handle:active, .bp3-slider-handle.bp3-active{
    background-color:#d8e1e8;
    background-image:none;
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
  .bp3-slider-handle:disabled, .bp3-slider-handle.bp3-disabled{
    background-color:rgba(206, 217, 224, 0.5);
    background-image:none;
    -webkit-box-shadow:none;
            box-shadow:none;
    color:rgba(92, 112, 128, 0.6);
    cursor:not-allowed;
    outline:none; }
    .bp3-slider-handle:disabled.bp3-active, .bp3-slider-handle:disabled.bp3-active:hover, .bp3-slider-handle.bp3-disabled.bp3-active, .bp3-slider-handle.bp3-disabled.bp3-active:hover{
      background:rgba(206, 217, 224, 0.7); }
  .bp3-slider-handle:focus{
    z-index:1; }
  .bp3-slider-handle:hover{
    background-clip:padding-box;
    background-color:#ebf1f5;
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 1px 1px rgba(16, 22, 26, 0.2);
    cursor:-webkit-grab;
    cursor:grab;
    z-index:2; }
  .bp3-slider-handle.bp3-active{
    background-color:#d8e1e8;
    background-image:none;
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2);
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 1px rgba(16, 22, 26, 0.1);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 1px rgba(16, 22, 26, 0.1);
    cursor:-webkit-grabbing;
    cursor:grabbing; }
  .bp3-disabled .bp3-slider-handle{
    background:#bfccd6;
    -webkit-box-shadow:none;
            box-shadow:none;
    pointer-events:none; }
  .bp3-dark .bp3-slider-handle{
    background-color:#394b59;
    background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.05)), to(rgba(255, 255, 255, 0)));
    background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.05), rgba(255, 255, 255, 0));
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
    color:#f5f8fa; }
    .bp3-dark .bp3-slider-handle:hover, .bp3-dark .bp3-slider-handle:active, .bp3-dark .bp3-slider-handle.bp3-active{
      color:#f5f8fa; }
    .bp3-dark .bp3-slider-handle:hover{
      background-color:#30404d;
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-slider-handle:active, .bp3-dark .bp3-slider-handle.bp3-active{
      background-color:#202b33;
      background-image:none;
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
    .bp3-dark .bp3-slider-handle:disabled, .bp3-dark .bp3-slider-handle.bp3-disabled{
      background-color:rgba(57, 75, 89, 0.5);
      background-image:none;
      -webkit-box-shadow:none;
              box-shadow:none;
      color:rgba(167, 182, 194, 0.6); }
      .bp3-dark .bp3-slider-handle:disabled.bp3-active, .bp3-dark .bp3-slider-handle.bp3-disabled.bp3-active{
        background:rgba(57, 75, 89, 0.7); }
    .bp3-dark .bp3-slider-handle .bp3-button-spinner .bp3-spinner-head{
      background:rgba(16, 22, 26, 0.5);
      stroke:#8a9ba8; }
    .bp3-dark .bp3-slider-handle, .bp3-dark .bp3-slider-handle:hover{
      background-color:#394b59; }
    .bp3-dark .bp3-slider-handle.bp3-active{
      background-color:#293742; }
  .bp3-dark .bp3-disabled .bp3-slider-handle{
    background:#5c7080;
    border-color:#5c7080;
    -webkit-box-shadow:none;
            box-shadow:none; }
  .bp3-slider-handle .bp3-slider-label{
    background:#394b59;
    border-radius:3px;
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
    color:#f5f8fa;
    margin-left:8px; }
    .bp3-dark .bp3-slider-handle .bp3-slider-label{
      background:#e1e8ed;
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4);
      color:#394b59; }
    .bp3-disabled .bp3-slider-handle .bp3-slider-label{
      -webkit-box-shadow:none;
              box-shadow:none; }
  .bp3-slider-handle.bp3-start, .bp3-slider-handle.bp3-end{
    width:8px; }
  .bp3-slider-handle.bp3-start{
    border-bottom-right-radius:0;
    border-top-right-radius:0; }
  .bp3-slider-handle.bp3-end{
    border-bottom-left-radius:0;
    border-top-left-radius:0;
    margin-left:8px; }
    .bp3-slider-handle.bp3-end .bp3-slider-label{
      margin-left:0; }

.bp3-slider-label{
  -webkit-transform:translate(-50%, 20px);
          transform:translate(-50%, 20px);
  display:inline-block;
  font-size:12px;
  line-height:1;
  padding:2px 5px;
  position:absolute;
  vertical-align:top; }

.bp3-slider.bp3-vertical{
  height:150px;
  min-width:40px;
  width:40px; }
  .bp3-slider.bp3-vertical .bp3-slider-track,
  .bp3-slider.bp3-vertical .bp3-slider-progress{
    bottom:0;
    height:auto;
    left:5px;
    top:0;
    width:6px; }
  .bp3-slider.bp3-vertical .bp3-slider-progress{
    top:auto; }
  .bp3-slider.bp3-vertical .bp3-slider-label{
    -webkit-transform:translate(20px, 50%);
            transform:translate(20px, 50%); }
  .bp3-slider.bp3-vertical .bp3-slider-handle{
    top:auto; }
    .bp3-slider.bp3-vertical .bp3-slider-handle .bp3-slider-label{
      margin-left:0;
      margin-top:-8px; }
    .bp3-slider.bp3-vertical .bp3-slider-handle.bp3-end, .bp3-slider.bp3-vertical .bp3-slider-handle.bp3-start{
      height:8px;
      margin-left:0;
      width:16px; }
    .bp3-slider.bp3-vertical .bp3-slider-handle.bp3-start{
      border-bottom-right-radius:3px;
      border-top-left-radius:0; }
      .bp3-slider.bp3-vertical .bp3-slider-handle.bp3-start .bp3-slider-label{
        -webkit-transform:translate(20px);
                transform:translate(20px); }
    .bp3-slider.bp3-vertical .bp3-slider-handle.bp3-end{
      border-bottom-left-radius:0;
      border-bottom-right-radius:0;
      border-top-left-radius:3px;
      margin-bottom:8px; }

@-webkit-keyframes pt-spinner-animation{
  from{
    -webkit-transform:rotate(0deg);
            transform:rotate(0deg); }
  to{
    -webkit-transform:rotate(360deg);
            transform:rotate(360deg); } }

@keyframes pt-spinner-animation{
  from{
    -webkit-transform:rotate(0deg);
            transform:rotate(0deg); }
  to{
    -webkit-transform:rotate(360deg);
            transform:rotate(360deg); } }

.bp3-spinner{
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-pack:center;
      -ms-flex-pack:center;
          justify-content:center;
  overflow:visible;
  vertical-align:middle; }
  .bp3-spinner svg{
    display:block; }
  .bp3-spinner path{
    fill-opacity:0; }
  .bp3-spinner .bp3-spinner-head{
    stroke:rgba(92, 112, 128, 0.8);
    stroke-linecap:round;
    -webkit-transform-origin:center;
            transform-origin:center;
    -webkit-transition:stroke-dashoffset 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
    transition:stroke-dashoffset 200ms cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-spinner .bp3-spinner-track{
    stroke:rgba(92, 112, 128, 0.2); }

.bp3-spinner-animation{
  -webkit-animation:pt-spinner-animation 500ms linear infinite;
          animation:pt-spinner-animation 500ms linear infinite; }
  .bp3-no-spin > .bp3-spinner-animation{
    -webkit-animation:none;
            animation:none; }

.bp3-dark .bp3-spinner .bp3-spinner-head{
  stroke:#8a9ba8; }

.bp3-dark .bp3-spinner .bp3-spinner-track{
  stroke:rgba(16, 22, 26, 0.5); }

.bp3-spinner.bp3-intent-primary .bp3-spinner-head{
  stroke:#137cbd; }

.bp3-spinner.bp3-intent-success .bp3-spinner-head{
  stroke:#0f9960; }

.bp3-spinner.bp3-intent-warning .bp3-spinner-head{
  stroke:#d9822b; }

.bp3-spinner.bp3-intent-danger .bp3-spinner-head{
  stroke:#db3737; }
.bp3-tabs.bp3-vertical{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex; }
  .bp3-tabs.bp3-vertical > .bp3-tab-list{
    -webkit-box-align:start;
        -ms-flex-align:start;
            align-items:flex-start;
    -webkit-box-orient:vertical;
    -webkit-box-direction:normal;
        -ms-flex-direction:column;
            flex-direction:column; }
    .bp3-tabs.bp3-vertical > .bp3-tab-list .bp3-tab{
      border-radius:3px;
      padding:0 10px;
      width:100%; }
      .bp3-tabs.bp3-vertical > .bp3-tab-list .bp3-tab[aria-selected="true"]{
        background-color:rgba(19, 124, 189, 0.2);
        -webkit-box-shadow:none;
                box-shadow:none; }
    .bp3-tabs.bp3-vertical > .bp3-tab-list .bp3-tab-indicator-wrapper .bp3-tab-indicator{
      background-color:rgba(19, 124, 189, 0.2);
      border-radius:3px;
      bottom:0;
      height:auto;
      left:0;
      right:0;
      top:0; }
  .bp3-tabs.bp3-vertical > .bp3-tab-panel{
    margin-top:0;
    padding-left:20px; }

.bp3-tab-list{
  -webkit-box-align:end;
      -ms-flex-align:end;
          align-items:flex-end;
  border:none;
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-flex:0;
      -ms-flex:0 0 auto;
          flex:0 0 auto;
  list-style:none;
  margin:0;
  padding:0;
  position:relative; }
  .bp3-tab-list > *:not(:last-child){
    margin-right:20px; }

.bp3-tab{
  overflow:hidden;
  text-overflow:ellipsis;
  white-space:nowrap;
  word-wrap:normal;
  color:#182026;
  cursor:pointer;
  -webkit-box-flex:0;
      -ms-flex:0 0 auto;
          flex:0 0 auto;
  font-size:14px;
  line-height:30px;
  max-width:100%;
  position:relative;
  vertical-align:top; }
  .bp3-tab a{
    color:inherit;
    display:block;
    text-decoration:none; }
  .bp3-tab-indicator-wrapper ~ .bp3-tab{
    background-color:transparent !important;
    -webkit-box-shadow:none !important;
            box-shadow:none !important; }
  .bp3-tab[aria-disabled="true"]{
    color:rgba(92, 112, 128, 0.6);
    cursor:not-allowed; }
  .bp3-tab[aria-selected="true"]{
    border-radius:0;
    -webkit-box-shadow:inset 0 -3px 0 #106ba3;
            box-shadow:inset 0 -3px 0 #106ba3; }
  .bp3-tab[aria-selected="true"], .bp3-tab:not([aria-disabled="true"]):hover{
    color:#106ba3; }
  .bp3-tab:focus{
    -moz-outline-radius:0; }
  .bp3-large > .bp3-tab{
    font-size:16px;
    line-height:40px; }

.bp3-tab-panel{
  margin-top:20px; }
  .bp3-tab-panel[aria-hidden="true"]{
    display:none; }

.bp3-tab-indicator-wrapper{
  left:0;
  pointer-events:none;
  position:absolute;
  top:0;
  -webkit-transform:translateX(0), translateY(0);
          transform:translateX(0), translateY(0);
  -webkit-transition:height, width, -webkit-transform;
  transition:height, width, -webkit-transform;
  transition:height, transform, width;
  transition:height, transform, width, -webkit-transform;
  -webkit-transition-duration:200ms;
          transition-duration:200ms;
  -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
          transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-tab-indicator-wrapper .bp3-tab-indicator{
    background-color:#106ba3;
    bottom:0;
    height:3px;
    left:0;
    position:absolute;
    right:0; }
  .bp3-tab-indicator-wrapper.bp3-no-animation{
    -webkit-transition:none;
    transition:none; }

.bp3-dark .bp3-tab{
  color:#f5f8fa; }
  .bp3-dark .bp3-tab[aria-disabled="true"]{
    color:rgba(167, 182, 194, 0.6); }
  .bp3-dark .bp3-tab[aria-selected="true"]{
    -webkit-box-shadow:inset 0 -3px 0 #48aff0;
            box-shadow:inset 0 -3px 0 #48aff0; }
  .bp3-dark .bp3-tab[aria-selected="true"], .bp3-dark .bp3-tab:not([aria-disabled="true"]):hover{
    color:#48aff0; }

.bp3-dark .bp3-tab-indicator{
  background-color:#48aff0; }

.bp3-flex-expander{
  -webkit-box-flex:1;
      -ms-flex:1 1;
          flex:1 1; }
.bp3-tag{
  display:-webkit-inline-box;
  display:-ms-inline-flexbox;
  display:inline-flex;
  -webkit-box-orient:horizontal;
  -webkit-box-direction:normal;
      -ms-flex-direction:row;
          flex-direction:row;
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  background-color:#5c7080;
  border:none;
  border-radius:3px;
  -webkit-box-shadow:none;
          box-shadow:none;
  color:#f5f8fa;
  font-size:12px;
  line-height:16px;
  max-width:100%;
  min-height:20px;
  min-width:20px;
  padding:2px 6px;
  position:relative; }
  .bp3-tag.bp3-interactive{
    cursor:pointer; }
    .bp3-tag.bp3-interactive:hover{
      background-color:rgba(92, 112, 128, 0.85); }
    .bp3-tag.bp3-interactive.bp3-active, .bp3-tag.bp3-interactive:active{
      background-color:rgba(92, 112, 128, 0.7); }
  .bp3-tag > *{
    -webkit-box-flex:0;
        -ms-flex-positive:0;
            flex-grow:0;
    -ms-flex-negative:0;
        flex-shrink:0; }
  .bp3-tag > .bp3-fill{
    -webkit-box-flex:1;
        -ms-flex-positive:1;
            flex-grow:1;
    -ms-flex-negative:1;
        flex-shrink:1; }
  .bp3-tag::before,
  .bp3-tag > *{
    margin-right:4px; }
  .bp3-tag:empty::before,
  .bp3-tag > :last-child{
    margin-right:0; }
  .bp3-tag:focus{
    outline:rgba(19, 124, 189, 0.6) auto 2px;
    outline-offset:0;
    -moz-outline-radius:6px; }
  .bp3-tag.bp3-round{
    border-radius:30px;
    padding-left:8px;
    padding-right:8px; }
  .bp3-dark .bp3-tag{
    background-color:#bfccd6;
    color:#182026; }
    .bp3-dark .bp3-tag.bp3-interactive{
      cursor:pointer; }
      .bp3-dark .bp3-tag.bp3-interactive:hover{
        background-color:rgba(191, 204, 214, 0.85); }
      .bp3-dark .bp3-tag.bp3-interactive.bp3-active, .bp3-dark .bp3-tag.bp3-interactive:active{
        background-color:rgba(191, 204, 214, 0.7); }
    .bp3-dark .bp3-tag > .bp3-icon, .bp3-dark .bp3-tag .bp3-icon-standard, .bp3-dark .bp3-tag .bp3-icon-large{
      fill:currentColor; }
  .bp3-tag > .bp3-icon, .bp3-tag .bp3-icon-standard, .bp3-tag .bp3-icon-large{
    fill:#ffffff; }
  .bp3-tag.bp3-large,
  .bp3-large .bp3-tag{
    font-size:14px;
    line-height:20px;
    min-height:30px;
    min-width:30px;
    padding:5px 10px; }
    .bp3-tag.bp3-large::before,
    .bp3-tag.bp3-large > *,
    .bp3-large .bp3-tag::before,
    .bp3-large .bp3-tag > *{
      margin-right:7px; }
    .bp3-tag.bp3-large:empty::before,
    .bp3-tag.bp3-large > :last-child,
    .bp3-large .bp3-tag:empty::before,
    .bp3-large .bp3-tag > :last-child{
      margin-right:0; }
    .bp3-tag.bp3-large.bp3-round,
    .bp3-large .bp3-tag.bp3-round{
      padding-left:12px;
      padding-right:12px; }
  .bp3-tag.bp3-intent-primary{
    background:#137cbd;
    color:#ffffff; }
    .bp3-tag.bp3-intent-primary.bp3-interactive{
      cursor:pointer; }
      .bp3-tag.bp3-intent-primary.bp3-interactive:hover{
        background-color:rgba(19, 124, 189, 0.85); }
      .bp3-tag.bp3-intent-primary.bp3-interactive.bp3-active, .bp3-tag.bp3-intent-primary.bp3-interactive:active{
        background-color:rgba(19, 124, 189, 0.7); }
  .bp3-tag.bp3-intent-success{
    background:#0f9960;
    color:#ffffff; }
    .bp3-tag.bp3-intent-success.bp3-interactive{
      cursor:pointer; }
      .bp3-tag.bp3-intent-success.bp3-interactive:hover{
        background-color:rgba(15, 153, 96, 0.85); }
      .bp3-tag.bp3-intent-success.bp3-interactive.bp3-active, .bp3-tag.bp3-intent-success.bp3-interactive:active{
        background-color:rgba(15, 153, 96, 0.7); }
  .bp3-tag.bp3-intent-warning{
    background:#d9822b;
    color:#ffffff; }
    .bp3-tag.bp3-intent-warning.bp3-interactive{
      cursor:pointer; }
      .bp3-tag.bp3-intent-warning.bp3-interactive:hover{
        background-color:rgba(217, 130, 43, 0.85); }
      .bp3-tag.bp3-intent-warning.bp3-interactive.bp3-active, .bp3-tag.bp3-intent-warning.bp3-interactive:active{
        background-color:rgba(217, 130, 43, 0.7); }
  .bp3-tag.bp3-intent-danger{
    background:#db3737;
    color:#ffffff; }
    .bp3-tag.bp3-intent-danger.bp3-interactive{
      cursor:pointer; }
      .bp3-tag.bp3-intent-danger.bp3-interactive:hover{
        background-color:rgba(219, 55, 55, 0.85); }
      .bp3-tag.bp3-intent-danger.bp3-interactive.bp3-active, .bp3-tag.bp3-intent-danger.bp3-interactive:active{
        background-color:rgba(219, 55, 55, 0.7); }
  .bp3-tag.bp3-fill{
    display:-webkit-box;
    display:-ms-flexbox;
    display:flex;
    width:100%; }
  .bp3-tag.bp3-minimal > .bp3-icon, .bp3-tag.bp3-minimal .bp3-icon-standard, .bp3-tag.bp3-minimal .bp3-icon-large{
    fill:#5c7080; }
  .bp3-tag.bp3-minimal:not([class*="bp3-intent-"]){
    background-color:rgba(138, 155, 168, 0.2);
    color:#182026; }
    .bp3-tag.bp3-minimal:not([class*="bp3-intent-"]).bp3-interactive{
      cursor:pointer; }
      .bp3-tag.bp3-minimal:not([class*="bp3-intent-"]).bp3-interactive:hover{
        background-color:rgba(92, 112, 128, 0.3); }
      .bp3-tag.bp3-minimal:not([class*="bp3-intent-"]).bp3-interactive.bp3-active, .bp3-tag.bp3-minimal:not([class*="bp3-intent-"]).bp3-interactive:active{
        background-color:rgba(92, 112, 128, 0.4); }
    .bp3-dark .bp3-tag.bp3-minimal:not([class*="bp3-intent-"]){
      color:#f5f8fa; }
      .bp3-dark .bp3-tag.bp3-minimal:not([class*="bp3-intent-"]).bp3-interactive{
        cursor:pointer; }
        .bp3-dark .bp3-tag.bp3-minimal:not([class*="bp3-intent-"]).bp3-interactive:hover{
          background-color:rgba(191, 204, 214, 0.3); }
        .bp3-dark .bp3-tag.bp3-minimal:not([class*="bp3-intent-"]).bp3-interactive.bp3-active, .bp3-dark .bp3-tag.bp3-minimal:not([class*="bp3-intent-"]).bp3-interactive:active{
          background-color:rgba(191, 204, 214, 0.4); }
      .bp3-dark .bp3-tag.bp3-minimal:not([class*="bp3-intent-"]) > .bp3-icon, .bp3-dark .bp3-tag.bp3-minimal:not([class*="bp3-intent-"]) .bp3-icon-standard, .bp3-dark .bp3-tag.bp3-minimal:not([class*="bp3-intent-"]) .bp3-icon-large{
        fill:#a7b6c2; }
  .bp3-tag.bp3-minimal.bp3-intent-primary{
    background-color:rgba(19, 124, 189, 0.15);
    color:#106ba3; }
    .bp3-tag.bp3-minimal.bp3-intent-primary.bp3-interactive{
      cursor:pointer; }
      .bp3-tag.bp3-minimal.bp3-intent-primary.bp3-interactive:hover{
        background-color:rgba(19, 124, 189, 0.25); }
      .bp3-tag.bp3-minimal.bp3-intent-primary.bp3-interactive.bp3-active, .bp3-tag.bp3-minimal.bp3-intent-primary.bp3-interactive:active{
        background-color:rgba(19, 124, 189, 0.35); }
    .bp3-tag.bp3-minimal.bp3-intent-primary > .bp3-icon, .bp3-tag.bp3-minimal.bp3-intent-primary .bp3-icon-standard, .bp3-tag.bp3-minimal.bp3-intent-primary .bp3-icon-large{
      fill:#137cbd; }
    .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-primary{
      background-color:rgba(19, 124, 189, 0.25);
      color:#48aff0; }
      .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-primary.bp3-interactive{
        cursor:pointer; }
        .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-primary.bp3-interactive:hover{
          background-color:rgba(19, 124, 189, 0.35); }
        .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-primary.bp3-interactive.bp3-active, .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-primary.bp3-interactive:active{
          background-color:rgba(19, 124, 189, 0.45); }
  .bp3-tag.bp3-minimal.bp3-intent-success{
    background-color:rgba(15, 153, 96, 0.15);
    color:#0d8050; }
    .bp3-tag.bp3-minimal.bp3-intent-success.bp3-interactive{
      cursor:pointer; }
      .bp3-tag.bp3-minimal.bp3-intent-success.bp3-interactive:hover{
        background-color:rgba(15, 153, 96, 0.25); }
      .bp3-tag.bp3-minimal.bp3-intent-success.bp3-interactive.bp3-active, .bp3-tag.bp3-minimal.bp3-intent-success.bp3-interactive:active{
        background-color:rgba(15, 153, 96, 0.35); }
    .bp3-tag.bp3-minimal.bp3-intent-success > .bp3-icon, .bp3-tag.bp3-minimal.bp3-intent-success .bp3-icon-standard, .bp3-tag.bp3-minimal.bp3-intent-success .bp3-icon-large{
      fill:#0f9960; }
    .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-success{
      background-color:rgba(15, 153, 96, 0.25);
      color:#3dcc91; }
      .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-success.bp3-interactive{
        cursor:pointer; }
        .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-success.bp3-interactive:hover{
          background-color:rgba(15, 153, 96, 0.35); }
        .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-success.bp3-interactive.bp3-active, .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-success.bp3-interactive:active{
          background-color:rgba(15, 153, 96, 0.45); }
  .bp3-tag.bp3-minimal.bp3-intent-warning{
    background-color:rgba(217, 130, 43, 0.15);
    color:#bf7326; }
    .bp3-tag.bp3-minimal.bp3-intent-warning.bp3-interactive{
      cursor:pointer; }
      .bp3-tag.bp3-minimal.bp3-intent-warning.bp3-interactive:hover{
        background-color:rgba(217, 130, 43, 0.25); }
      .bp3-tag.bp3-minimal.bp3-intent-warning.bp3-interactive.bp3-active, .bp3-tag.bp3-minimal.bp3-intent-warning.bp3-interactive:active{
        background-color:rgba(217, 130, 43, 0.35); }
    .bp3-tag.bp3-minimal.bp3-intent-warning > .bp3-icon, .bp3-tag.bp3-minimal.bp3-intent-warning .bp3-icon-standard, .bp3-tag.bp3-minimal.bp3-intent-warning .bp3-icon-large{
      fill:#d9822b; }
    .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-warning{
      background-color:rgba(217, 130, 43, 0.25);
      color:#ffb366; }
      .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-warning.bp3-interactive{
        cursor:pointer; }
        .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-warning.bp3-interactive:hover{
          background-color:rgba(217, 130, 43, 0.35); }
        .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-warning.bp3-interactive.bp3-active, .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-warning.bp3-interactive:active{
          background-color:rgba(217, 130, 43, 0.45); }
  .bp3-tag.bp3-minimal.bp3-intent-danger{
    background-color:rgba(219, 55, 55, 0.15);
    color:#c23030; }
    .bp3-tag.bp3-minimal.bp3-intent-danger.bp3-interactive{
      cursor:pointer; }
      .bp3-tag.bp3-minimal.bp3-intent-danger.bp3-interactive:hover{
        background-color:rgba(219, 55, 55, 0.25); }
      .bp3-tag.bp3-minimal.bp3-intent-danger.bp3-interactive.bp3-active, .bp3-tag.bp3-minimal.bp3-intent-danger.bp3-interactive:active{
        background-color:rgba(219, 55, 55, 0.35); }
    .bp3-tag.bp3-minimal.bp3-intent-danger > .bp3-icon, .bp3-tag.bp3-minimal.bp3-intent-danger .bp3-icon-standard, .bp3-tag.bp3-minimal.bp3-intent-danger .bp3-icon-large{
      fill:#db3737; }
    .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-danger{
      background-color:rgba(219, 55, 55, 0.25);
      color:#ff7373; }
      .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-danger.bp3-interactive{
        cursor:pointer; }
        .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-danger.bp3-interactive:hover{
          background-color:rgba(219, 55, 55, 0.35); }
        .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-danger.bp3-interactive.bp3-active, .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-danger.bp3-interactive:active{
          background-color:rgba(219, 55, 55, 0.45); }

.bp3-tag-remove{
  background:none;
  border:none;
  color:inherit;
  cursor:pointer;
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  margin-bottom:-2px;
  margin-right:-6px !important;
  margin-top:-2px;
  opacity:0.5;
  padding:2px;
  padding-left:0; }
  .bp3-tag-remove:hover{
    background:none;
    opacity:0.8;
    text-decoration:none; }
  .bp3-tag-remove:active{
    opacity:1; }
  .bp3-tag-remove:empty::before{
    font-family:"Icons16", sans-serif;
    font-size:16px;
    font-style:normal;
    font-weight:400;
    line-height:1;
    -moz-osx-font-smoothing:grayscale;
    -webkit-font-smoothing:antialiased;
    content:""; }
  .bp3-large .bp3-tag-remove{
    margin-right:-10px !important;
    padding:0 5px 0 0; }
    .bp3-large .bp3-tag-remove:empty::before{
      font-family:"Icons20", sans-serif;
      font-size:20px;
      font-style:normal;
      font-weight:400;
      line-height:1; }
.bp3-tag-input{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-orient:horizontal;
  -webkit-box-direction:normal;
      -ms-flex-direction:row;
          flex-direction:row;
  -webkit-box-align:start;
      -ms-flex-align:start;
          align-items:flex-start;
  cursor:text;
  height:auto;
  line-height:inherit;
  min-height:30px;
  padding-left:5px;
  padding-right:0; }
  .bp3-tag-input > *{
    -webkit-box-flex:0;
        -ms-flex-positive:0;
            flex-grow:0;
    -ms-flex-negative:0;
        flex-shrink:0; }
  .bp3-tag-input > .bp3-tag-input-values{
    -webkit-box-flex:1;
        -ms-flex-positive:1;
            flex-grow:1;
    -ms-flex-negative:1;
        flex-shrink:1; }
  .bp3-tag-input .bp3-tag-input-icon{
    color:#5c7080;
    margin-left:2px;
    margin-right:7px;
    margin-top:7px; }
  .bp3-tag-input .bp3-tag-input-values{
    display:-webkit-box;
    display:-ms-flexbox;
    display:flex;
    -webkit-box-orient:horizontal;
    -webkit-box-direction:normal;
        -ms-flex-direction:row;
            flex-direction:row;
    -webkit-box-align:center;
        -ms-flex-align:center;
            align-items:center;
    -ms-flex-item-align:stretch;
        align-self:stretch;
    -ms-flex-wrap:wrap;
        flex-wrap:wrap;
    margin-right:7px;
    margin-top:5px;
    min-width:0; }
    .bp3-tag-input .bp3-tag-input-values > *{
      -webkit-box-flex:0;
          -ms-flex-positive:0;
              flex-grow:0;
      -ms-flex-negative:0;
          flex-shrink:0; }
    .bp3-tag-input .bp3-tag-input-values > .bp3-fill{
      -webkit-box-flex:1;
          -ms-flex-positive:1;
              flex-grow:1;
      -ms-flex-negative:1;
          flex-shrink:1; }
    .bp3-tag-input .bp3-tag-input-values::before,
    .bp3-tag-input .bp3-tag-input-values > *{
      margin-right:5px; }
    .bp3-tag-input .bp3-tag-input-values:empty::before,
    .bp3-tag-input .bp3-tag-input-values > :last-child{
      margin-right:0; }
    .bp3-tag-input .bp3-tag-input-values:first-child .bp3-input-ghost:first-child{
      padding-left:5px; }
    .bp3-tag-input .bp3-tag-input-values > *{
      margin-bottom:5px; }
  .bp3-tag-input .bp3-tag{
    overflow-wrap:break-word; }
    .bp3-tag-input .bp3-tag.bp3-active{
      outline:rgba(19, 124, 189, 0.6) auto 2px;
      outline-offset:0;
      -moz-outline-radius:6px; }
  .bp3-tag-input .bp3-input-ghost{
    -webkit-box-flex:1;
        -ms-flex:1 1 auto;
            flex:1 1 auto;
    line-height:20px;
    width:80px; }
    .bp3-tag-input .bp3-input-ghost:disabled, .bp3-tag-input .bp3-input-ghost.bp3-disabled{
      cursor:not-allowed; }
  .bp3-tag-input .bp3-button,
  .bp3-tag-input .bp3-spinner{
    margin:3px;
    margin-left:0; }
  .bp3-tag-input .bp3-button{
    min-height:24px;
    min-width:24px;
    padding:0 7px; }
  .bp3-tag-input.bp3-large{
    height:auto;
    min-height:40px; }
    .bp3-tag-input.bp3-large::before,
    .bp3-tag-input.bp3-large > *{
      margin-right:10px; }
    .bp3-tag-input.bp3-large:empty::before,
    .bp3-tag-input.bp3-large > :last-child{
      margin-right:0; }
    .bp3-tag-input.bp3-large .bp3-tag-input-icon{
      margin-left:5px;
      margin-top:10px; }
    .bp3-tag-input.bp3-large .bp3-input-ghost{
      line-height:30px; }
    .bp3-tag-input.bp3-large .bp3-button{
      min-height:30px;
      min-width:30px;
      padding:5px 10px;
      margin:5px;
      margin-left:0; }
    .bp3-tag-input.bp3-large .bp3-spinner{
      margin:8px;
      margin-left:0; }
  .bp3-tag-input.bp3-active{
    background-color:#ffffff;
    -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-tag-input.bp3-active.bp3-intent-primary{
      -webkit-box-shadow:0 0 0 1px #106ba3, 0 0 0 3px rgba(16, 107, 163, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px #106ba3, 0 0 0 3px rgba(16, 107, 163, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-tag-input.bp3-active.bp3-intent-success{
      -webkit-box-shadow:0 0 0 1px #0d8050, 0 0 0 3px rgba(13, 128, 80, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px #0d8050, 0 0 0 3px rgba(13, 128, 80, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-tag-input.bp3-active.bp3-intent-warning{
      -webkit-box-shadow:0 0 0 1px #bf7326, 0 0 0 3px rgba(191, 115, 38, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px #bf7326, 0 0 0 3px rgba(191, 115, 38, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-tag-input.bp3-active.bp3-intent-danger{
      -webkit-box-shadow:0 0 0 1px #c23030, 0 0 0 3px rgba(194, 48, 48, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px #c23030, 0 0 0 3px rgba(194, 48, 48, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
  .bp3-dark .bp3-tag-input .bp3-tag-input-icon, .bp3-tag-input.bp3-dark .bp3-tag-input-icon{
    color:#a7b6c2; }
  .bp3-dark .bp3-tag-input .bp3-input-ghost, .bp3-tag-input.bp3-dark .bp3-input-ghost{
    color:#f5f8fa; }
    .bp3-dark .bp3-tag-input .bp3-input-ghost::-webkit-input-placeholder, .bp3-tag-input.bp3-dark .bp3-input-ghost::-webkit-input-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-tag-input .bp3-input-ghost::-moz-placeholder, .bp3-tag-input.bp3-dark .bp3-input-ghost::-moz-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-tag-input .bp3-input-ghost:-ms-input-placeholder, .bp3-tag-input.bp3-dark .bp3-input-ghost:-ms-input-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-tag-input .bp3-input-ghost::-ms-input-placeholder, .bp3-tag-input.bp3-dark .bp3-input-ghost::-ms-input-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-tag-input .bp3-input-ghost::placeholder, .bp3-tag-input.bp3-dark .bp3-input-ghost::placeholder{
      color:rgba(167, 182, 194, 0.6); }
  .bp3-dark .bp3-tag-input.bp3-active, .bp3-tag-input.bp3-dark.bp3-active{
    background-color:rgba(16, 22, 26, 0.3);
    -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px #137cbd, 0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-tag-input.bp3-active.bp3-intent-primary, .bp3-tag-input.bp3-dark.bp3-active.bp3-intent-primary{
      -webkit-box-shadow:0 0 0 1px #106ba3, 0 0 0 3px rgba(16, 107, 163, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px #106ba3, 0 0 0 3px rgba(16, 107, 163, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-tag-input.bp3-active.bp3-intent-success, .bp3-tag-input.bp3-dark.bp3-active.bp3-intent-success{
      -webkit-box-shadow:0 0 0 1px #0d8050, 0 0 0 3px rgba(13, 128, 80, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px #0d8050, 0 0 0 3px rgba(13, 128, 80, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-tag-input.bp3-active.bp3-intent-warning, .bp3-tag-input.bp3-dark.bp3-active.bp3-intent-warning{
      -webkit-box-shadow:0 0 0 1px #bf7326, 0 0 0 3px rgba(191, 115, 38, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px #bf7326, 0 0 0 3px rgba(191, 115, 38, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-tag-input.bp3-active.bp3-intent-danger, .bp3-tag-input.bp3-dark.bp3-active.bp3-intent-danger{
      -webkit-box-shadow:0 0 0 1px #c23030, 0 0 0 3px rgba(194, 48, 48, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px #c23030, 0 0 0 3px rgba(194, 48, 48, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }

.bp3-input-ghost{
  background:none;
  border:none;
  -webkit-box-shadow:none;
          box-shadow:none;
  padding:0; }
  .bp3-input-ghost::-webkit-input-placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-input-ghost::-moz-placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-input-ghost:-ms-input-placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-input-ghost::-ms-input-placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-input-ghost::placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-input-ghost:focus{
    outline:none !important; }
.bp3-toast{
  -webkit-box-align:start;
      -ms-flex-align:start;
          align-items:flex-start;
  background-color:#ffffff;
  border-radius:3px;
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  margin:20px 0 0;
  max-width:500px;
  min-width:300px;
  pointer-events:all;
  position:relative !important; }
  .bp3-toast.bp3-toast-enter, .bp3-toast.bp3-toast-appear{
    -webkit-transform:translateY(-40px);
            transform:translateY(-40px); }
  .bp3-toast.bp3-toast-enter-active, .bp3-toast.bp3-toast-appear-active{
    -webkit-transform:translateY(0);
            transform:translateY(0);
    -webkit-transition-delay:0;
            transition-delay:0;
    -webkit-transition-duration:300ms;
            transition-duration:300ms;
    -webkit-transition-property:-webkit-transform;
    transition-property:-webkit-transform;
    transition-property:transform;
    transition-property:transform, -webkit-transform;
    -webkit-transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11);
            transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11); }
  .bp3-toast.bp3-toast-enter ~ .bp3-toast, .bp3-toast.bp3-toast-appear ~ .bp3-toast{
    -webkit-transform:translateY(-40px);
            transform:translateY(-40px); }
  .bp3-toast.bp3-toast-enter-active ~ .bp3-toast, .bp3-toast.bp3-toast-appear-active ~ .bp3-toast{
    -webkit-transform:translateY(0);
            transform:translateY(0);
    -webkit-transition-delay:0;
            transition-delay:0;
    -webkit-transition-duration:300ms;
            transition-duration:300ms;
    -webkit-transition-property:-webkit-transform;
    transition-property:-webkit-transform;
    transition-property:transform;
    transition-property:transform, -webkit-transform;
    -webkit-transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11);
            transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11); }
  .bp3-toast.bp3-toast-exit{
    opacity:1;
    -webkit-filter:blur(0);
            filter:blur(0); }
  .bp3-toast.bp3-toast-exit-active{
    opacity:0;
    -webkit-filter:blur(10px);
            filter:blur(10px);
    -webkit-transition-delay:0;
            transition-delay:0;
    -webkit-transition-duration:300ms;
            transition-duration:300ms;
    -webkit-transition-property:opacity, -webkit-filter;
    transition-property:opacity, -webkit-filter;
    transition-property:opacity, filter;
    transition-property:opacity, filter, -webkit-filter;
    -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
            transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-toast.bp3-toast-exit ~ .bp3-toast{
    -webkit-transform:translateY(0);
            transform:translateY(0); }
  .bp3-toast.bp3-toast-exit-active ~ .bp3-toast{
    -webkit-transform:translateY(-40px);
            transform:translateY(-40px);
    -webkit-transition-delay:50ms;
            transition-delay:50ms;
    -webkit-transition-duration:100ms;
            transition-duration:100ms;
    -webkit-transition-property:-webkit-transform;
    transition-property:-webkit-transform;
    transition-property:transform;
    transition-property:transform, -webkit-transform;
    -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
            transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-toast .bp3-button-group{
    -webkit-box-flex:0;
        -ms-flex:0 0 auto;
            flex:0 0 auto;
    padding:5px;
    padding-left:0; }
  .bp3-toast > .bp3-icon{
    color:#5c7080;
    margin:12px;
    margin-right:0; }
  .bp3-toast.bp3-dark,
  .bp3-dark .bp3-toast{
    background-color:#394b59;
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4); }
    .bp3-toast.bp3-dark > .bp3-icon,
    .bp3-dark .bp3-toast > .bp3-icon{
      color:#a7b6c2; }
  .bp3-toast[class*="bp3-intent-"] a{
    color:rgba(255, 255, 255, 0.7); }
    .bp3-toast[class*="bp3-intent-"] a:hover{
      color:#ffffff; }
  .bp3-toast[class*="bp3-intent-"] > .bp3-icon{
    color:#ffffff; }
  .bp3-toast[class*="bp3-intent-"] .bp3-button, .bp3-toast[class*="bp3-intent-"] .bp3-button::before,
  .bp3-toast[class*="bp3-intent-"] .bp3-button .bp3-icon, .bp3-toast[class*="bp3-intent-"] .bp3-button:active{
    color:rgba(255, 255, 255, 0.7) !important; }
  .bp3-toast[class*="bp3-intent-"] .bp3-button:focus{
    outline-color:rgba(255, 255, 255, 0.5); }
  .bp3-toast[class*="bp3-intent-"] .bp3-button:hover{
    background-color:rgba(255, 255, 255, 0.15) !important;
    color:#ffffff !important; }
  .bp3-toast[class*="bp3-intent-"] .bp3-button:active{
    background-color:rgba(255, 255, 255, 0.3) !important;
    color:#ffffff !important; }
  .bp3-toast[class*="bp3-intent-"] .bp3-button::after{
    background:rgba(255, 255, 255, 0.3) !important; }
  .bp3-toast.bp3-intent-primary{
    background-color:#137cbd;
    color:#ffffff; }
  .bp3-toast.bp3-intent-success{
    background-color:#0f9960;
    color:#ffffff; }
  .bp3-toast.bp3-intent-warning{
    background-color:#d9822b;
    color:#ffffff; }
  .bp3-toast.bp3-intent-danger{
    background-color:#db3737;
    color:#ffffff; }

.bp3-toast-message{
  -webkit-box-flex:1;
      -ms-flex:1 1 auto;
          flex:1 1 auto;
  padding:11px;
  word-break:break-word; }

.bp3-toast-container{
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  display:-webkit-box !important;
  display:-ms-flexbox !important;
  display:flex !important;
  -webkit-box-orient:vertical;
  -webkit-box-direction:normal;
      -ms-flex-direction:column;
          flex-direction:column;
  left:0;
  overflow:hidden;
  padding:0 20px 20px;
  pointer-events:none;
  right:0;
  z-index:40; }
  .bp3-toast-container.bp3-toast-container-in-portal{
    position:fixed; }
  .bp3-toast-container.bp3-toast-container-inline{
    position:absolute; }
  .bp3-toast-container.bp3-toast-container-top{
    top:0; }
  .bp3-toast-container.bp3-toast-container-bottom{
    bottom:0;
    -webkit-box-orient:vertical;
    -webkit-box-direction:reverse;
        -ms-flex-direction:column-reverse;
            flex-direction:column-reverse;
    top:auto; }
  .bp3-toast-container.bp3-toast-container-left{
    -webkit-box-align:start;
        -ms-flex-align:start;
            align-items:flex-start; }
  .bp3-toast-container.bp3-toast-container-right{
    -webkit-box-align:end;
        -ms-flex-align:end;
            align-items:flex-end; }

.bp3-toast-container-bottom .bp3-toast.bp3-toast-enter:not(.bp3-toast-enter-active),
.bp3-toast-container-bottom .bp3-toast.bp3-toast-enter:not(.bp3-toast-enter-active) ~ .bp3-toast, .bp3-toast-container-bottom .bp3-toast.bp3-toast-appear:not(.bp3-toast-appear-active),
.bp3-toast-container-bottom .bp3-toast.bp3-toast-appear:not(.bp3-toast-appear-active) ~ .bp3-toast,
.bp3-toast-container-bottom .bp3-toast.bp3-toast-exit-active ~ .bp3-toast,
.bp3-toast-container-bottom .bp3-toast.bp3-toast-leave-active ~ .bp3-toast{
  -webkit-transform:translateY(60px);
          transform:translateY(60px); }
.bp3-tooltip{
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
  -webkit-transform:scale(1);
          transform:scale(1); }
  .bp3-tooltip .bp3-popover-arrow{
    height:22px;
    position:absolute;
    width:22px; }
    .bp3-tooltip .bp3-popover-arrow::before{
      height:14px;
      margin:4px;
      width:14px; }
  .bp3-tether-element-attached-bottom.bp3-tether-target-attached-top > .bp3-tooltip{
    margin-bottom:11px;
    margin-top:-11px; }
    .bp3-tether-element-attached-bottom.bp3-tether-target-attached-top > .bp3-tooltip > .bp3-popover-arrow{
      bottom:-8px; }
      .bp3-tether-element-attached-bottom.bp3-tether-target-attached-top > .bp3-tooltip > .bp3-popover-arrow svg{
        -webkit-transform:rotate(-90deg);
                transform:rotate(-90deg); }
  .bp3-tether-element-attached-left.bp3-tether-target-attached-right > .bp3-tooltip{
    margin-left:11px; }
    .bp3-tether-element-attached-left.bp3-tether-target-attached-right > .bp3-tooltip > .bp3-popover-arrow{
      left:-8px; }
      .bp3-tether-element-attached-left.bp3-tether-target-attached-right > .bp3-tooltip > .bp3-popover-arrow svg{
        -webkit-transform:rotate(0);
                transform:rotate(0); }
  .bp3-tether-element-attached-top.bp3-tether-target-attached-bottom > .bp3-tooltip{
    margin-top:11px; }
    .bp3-tether-element-attached-top.bp3-tether-target-attached-bottom > .bp3-tooltip > .bp3-popover-arrow{
      top:-8px; }
      .bp3-tether-element-attached-top.bp3-tether-target-attached-bottom > .bp3-tooltip > .bp3-popover-arrow svg{
        -webkit-transform:rotate(90deg);
                transform:rotate(90deg); }
  .bp3-tether-element-attached-right.bp3-tether-target-attached-left > .bp3-tooltip{
    margin-left:-11px;
    margin-right:11px; }
    .bp3-tether-element-attached-right.bp3-tether-target-attached-left > .bp3-tooltip > .bp3-popover-arrow{
      right:-8px; }
      .bp3-tether-element-attached-right.bp3-tether-target-attached-left > .bp3-tooltip > .bp3-popover-arrow svg{
        -webkit-transform:rotate(180deg);
                transform:rotate(180deg); }
  .bp3-tether-element-attached-middle > .bp3-tooltip > .bp3-popover-arrow{
    top:50%;
    -webkit-transform:translateY(-50%);
            transform:translateY(-50%); }
  .bp3-tether-element-attached-center > .bp3-tooltip > .bp3-popover-arrow{
    right:50%;
    -webkit-transform:translateX(50%);
            transform:translateX(50%); }
  .bp3-tether-element-attached-top.bp3-tether-target-attached-top > .bp3-tooltip > .bp3-popover-arrow{
    top:-0.22183px; }
  .bp3-tether-element-attached-right.bp3-tether-target-attached-right > .bp3-tooltip > .bp3-popover-arrow{
    right:-0.22183px; }
  .bp3-tether-element-attached-left.bp3-tether-target-attached-left > .bp3-tooltip > .bp3-popover-arrow{
    left:-0.22183px; }
  .bp3-tether-element-attached-bottom.bp3-tether-target-attached-bottom > .bp3-tooltip > .bp3-popover-arrow{
    bottom:-0.22183px; }
  .bp3-tether-element-attached-top.bp3-tether-element-attached-left > .bp3-tooltip{
    -webkit-transform-origin:top left;
            transform-origin:top left; }
  .bp3-tether-element-attached-top.bp3-tether-element-attached-center > .bp3-tooltip{
    -webkit-transform-origin:top center;
            transform-origin:top center; }
  .bp3-tether-element-attached-top.bp3-tether-element-attached-right > .bp3-tooltip{
    -webkit-transform-origin:top right;
            transform-origin:top right; }
  .bp3-tether-element-attached-middle.bp3-tether-element-attached-left > .bp3-tooltip{
    -webkit-transform-origin:center left;
            transform-origin:center left; }
  .bp3-tether-element-attached-middle.bp3-tether-element-attached-center > .bp3-tooltip{
    -webkit-transform-origin:center center;
            transform-origin:center center; }
  .bp3-tether-element-attached-middle.bp3-tether-element-attached-right > .bp3-tooltip{
    -webkit-transform-origin:center right;
            transform-origin:center right; }
  .bp3-tether-element-attached-bottom.bp3-tether-element-attached-left > .bp3-tooltip{
    -webkit-transform-origin:bottom left;
            transform-origin:bottom left; }
  .bp3-tether-element-attached-bottom.bp3-tether-element-attached-center > .bp3-tooltip{
    -webkit-transform-origin:bottom center;
            transform-origin:bottom center; }
  .bp3-tether-element-attached-bottom.bp3-tether-element-attached-right > .bp3-tooltip{
    -webkit-transform-origin:bottom right;
            transform-origin:bottom right; }
  .bp3-tooltip .bp3-popover-content{
    background:#394b59;
    color:#f5f8fa; }
  .bp3-tooltip .bp3-popover-arrow::before{
    -webkit-box-shadow:1px 1px 6px rgba(16, 22, 26, 0.2);
            box-shadow:1px 1px 6px rgba(16, 22, 26, 0.2); }
  .bp3-tooltip .bp3-popover-arrow-border{
    fill:#10161a;
    fill-opacity:0.1; }
  .bp3-tooltip .bp3-popover-arrow-fill{
    fill:#394b59; }
  .bp3-popover-enter > .bp3-tooltip, .bp3-popover-appear > .bp3-tooltip{
    -webkit-transform:scale(0.8);
            transform:scale(0.8); }
  .bp3-popover-enter-active > .bp3-tooltip, .bp3-popover-appear-active > .bp3-tooltip{
    -webkit-transform:scale(1);
            transform:scale(1);
    -webkit-transition-delay:0;
            transition-delay:0;
    -webkit-transition-duration:100ms;
            transition-duration:100ms;
    -webkit-transition-property:-webkit-transform;
    transition-property:-webkit-transform;
    transition-property:transform;
    transition-property:transform, -webkit-transform;
    -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
            transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-popover-exit > .bp3-tooltip{
    -webkit-transform:scale(1);
            transform:scale(1); }
  .bp3-popover-exit-active > .bp3-tooltip{
    -webkit-transform:scale(0.8);
            transform:scale(0.8);
    -webkit-transition-delay:0;
            transition-delay:0;
    -webkit-transition-duration:100ms;
            transition-duration:100ms;
    -webkit-transition-property:-webkit-transform;
    transition-property:-webkit-transform;
    transition-property:transform;
    transition-property:transform, -webkit-transform;
    -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
            transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-tooltip .bp3-popover-content{
    padding:10px 12px; }
  .bp3-tooltip.bp3-dark,
  .bp3-dark .bp3-tooltip{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4); }
    .bp3-tooltip.bp3-dark .bp3-popover-content,
    .bp3-dark .bp3-tooltip .bp3-popover-content{
      background:#e1e8ed;
      color:#394b59; }
    .bp3-tooltip.bp3-dark .bp3-popover-arrow::before,
    .bp3-dark .bp3-tooltip .bp3-popover-arrow::before{
      -webkit-box-shadow:1px 1px 6px rgba(16, 22, 26, 0.4);
              box-shadow:1px 1px 6px rgba(16, 22, 26, 0.4); }
    .bp3-tooltip.bp3-dark .bp3-popover-arrow-border,
    .bp3-dark .bp3-tooltip .bp3-popover-arrow-border{
      fill:#10161a;
      fill-opacity:0.2; }
    .bp3-tooltip.bp3-dark .bp3-popover-arrow-fill,
    .bp3-dark .bp3-tooltip .bp3-popover-arrow-fill{
      fill:#e1e8ed; }
  .bp3-tooltip.bp3-intent-primary .bp3-popover-content{
    background:#137cbd;
    color:#ffffff; }
  .bp3-tooltip.bp3-intent-primary .bp3-popover-arrow-fill{
    fill:#137cbd; }
  .bp3-tooltip.bp3-intent-success .bp3-popover-content{
    background:#0f9960;
    color:#ffffff; }
  .bp3-tooltip.bp3-intent-success .bp3-popover-arrow-fill{
    fill:#0f9960; }
  .bp3-tooltip.bp3-intent-warning .bp3-popover-content{
    background:#d9822b;
    color:#ffffff; }
  .bp3-tooltip.bp3-intent-warning .bp3-popover-arrow-fill{
    fill:#d9822b; }
  .bp3-tooltip.bp3-intent-danger .bp3-popover-content{
    background:#db3737;
    color:#ffffff; }
  .bp3-tooltip.bp3-intent-danger .bp3-popover-arrow-fill{
    fill:#db3737; }

.bp3-tooltip-indicator{
  border-bottom:dotted 1px;
  cursor:help; }
.bp3-tree .bp3-icon, .bp3-tree .bp3-icon-standard, .bp3-tree .bp3-icon-large{
  color:#5c7080; }
  .bp3-tree .bp3-icon.bp3-intent-primary, .bp3-tree .bp3-icon-standard.bp3-intent-primary, .bp3-tree .bp3-icon-large.bp3-intent-primary{
    color:#137cbd; }
  .bp3-tree .bp3-icon.bp3-intent-success, .bp3-tree .bp3-icon-standard.bp3-intent-success, .bp3-tree .bp3-icon-large.bp3-intent-success{
    color:#0f9960; }
  .bp3-tree .bp3-icon.bp3-intent-warning, .bp3-tree .bp3-icon-standard.bp3-intent-warning, .bp3-tree .bp3-icon-large.bp3-intent-warning{
    color:#d9822b; }
  .bp3-tree .bp3-icon.bp3-intent-danger, .bp3-tree .bp3-icon-standard.bp3-intent-danger, .bp3-tree .bp3-icon-large.bp3-intent-danger{
    color:#db3737; }

.bp3-tree-node-list{
  list-style:none;
  margin:0;
  padding-left:0; }

.bp3-tree-root{
  background-color:transparent;
  cursor:default;
  padding-left:0;
  position:relative; }

.bp3-tree-node-content-0{
  padding-left:0px; }

.bp3-tree-node-content-1{
  padding-left:23px; }

.bp3-tree-node-content-2{
  padding-left:46px; }

.bp3-tree-node-content-3{
  padding-left:69px; }

.bp3-tree-node-content-4{
  padding-left:92px; }

.bp3-tree-node-content-5{
  padding-left:115px; }

.bp3-tree-node-content-6{
  padding-left:138px; }

.bp3-tree-node-content-7{
  padding-left:161px; }

.bp3-tree-node-content-8{
  padding-left:184px; }

.bp3-tree-node-content-9{
  padding-left:207px; }

.bp3-tree-node-content-10{
  padding-left:230px; }

.bp3-tree-node-content-11{
  padding-left:253px; }

.bp3-tree-node-content-12{
  padding-left:276px; }

.bp3-tree-node-content-13{
  padding-left:299px; }

.bp3-tree-node-content-14{
  padding-left:322px; }

.bp3-tree-node-content-15{
  padding-left:345px; }

.bp3-tree-node-content-16{
  padding-left:368px; }

.bp3-tree-node-content-17{
  padding-left:391px; }

.bp3-tree-node-content-18{
  padding-left:414px; }

.bp3-tree-node-content-19{
  padding-left:437px; }

.bp3-tree-node-content-20{
  padding-left:460px; }

.bp3-tree-node-content{
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  height:30px;
  padding-right:5px;
  width:100%; }
  .bp3-tree-node-content:hover{
    background-color:rgba(191, 204, 214, 0.4); }

.bp3-tree-node-caret,
.bp3-tree-node-caret-none{
  min-width:30px; }

.bp3-tree-node-caret{
  color:#5c7080;
  cursor:pointer;
  padding:7px;
  -webkit-transform:rotate(0deg);
          transform:rotate(0deg);
  -webkit-transition:-webkit-transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
  transition:-webkit-transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
  transition:transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
  transition:transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-tree-node-caret:hover{
    color:#182026; }
  .bp3-dark .bp3-tree-node-caret{
    color:#a7b6c2; }
    .bp3-dark .bp3-tree-node-caret:hover{
      color:#f5f8fa; }
  .bp3-tree-node-caret.bp3-tree-node-caret-open{
    -webkit-transform:rotate(90deg);
            transform:rotate(90deg); }
  .bp3-tree-node-caret.bp3-icon-standard::before{
    content:""; }

.bp3-tree-node-icon{
  margin-right:7px;
  position:relative; }

.bp3-tree-node-label{
  overflow:hidden;
  text-overflow:ellipsis;
  white-space:nowrap;
  word-wrap:normal;
  -webkit-box-flex:1;
      -ms-flex:1 1 auto;
          flex:1 1 auto;
  position:relative;
  -webkit-user-select:none;
     -moz-user-select:none;
      -ms-user-select:none;
          user-select:none; }
  .bp3-tree-node-label span{
    display:inline; }

.bp3-tree-node-secondary-label{
  padding:0 5px;
  -webkit-user-select:none;
     -moz-user-select:none;
      -ms-user-select:none;
          user-select:none; }
  .bp3-tree-node-secondary-label .bp3-popover-wrapper,
  .bp3-tree-node-secondary-label .bp3-popover-target{
    -webkit-box-align:center;
        -ms-flex-align:center;
            align-items:center;
    display:-webkit-box;
    display:-ms-flexbox;
    display:flex; }

.bp3-tree-node.bp3-disabled .bp3-tree-node-content{
  background-color:inherit;
  color:rgba(92, 112, 128, 0.6);
  cursor:not-allowed; }

.bp3-tree-node.bp3-disabled .bp3-tree-node-caret,
.bp3-tree-node.bp3-disabled .bp3-tree-node-icon{
  color:rgba(92, 112, 128, 0.6);
  cursor:not-allowed; }

.bp3-tree-node.bp3-tree-node-selected > .bp3-tree-node-content{
  background-color:#137cbd; }
  .bp3-tree-node.bp3-tree-node-selected > .bp3-tree-node-content,
  .bp3-tree-node.bp3-tree-node-selected > .bp3-tree-node-content .bp3-icon, .bp3-tree-node.bp3-tree-node-selected > .bp3-tree-node-content .bp3-icon-standard, .bp3-tree-node.bp3-tree-node-selected > .bp3-tree-node-content .bp3-icon-large{
    color:#ffffff; }
  .bp3-tree-node.bp3-tree-node-selected > .bp3-tree-node-content .bp3-tree-node-caret::before{
    color:rgba(255, 255, 255, 0.7); }
  .bp3-tree-node.bp3-tree-node-selected > .bp3-tree-node-content .bp3-tree-node-caret:hover::before{
    color:#ffffff; }

.bp3-dark .bp3-tree-node-content:hover{
  background-color:rgba(92, 112, 128, 0.3); }

.bp3-dark .bp3-tree .bp3-icon, .bp3-dark .bp3-tree .bp3-icon-standard, .bp3-dark .bp3-tree .bp3-icon-large{
  color:#a7b6c2; }
  .bp3-dark .bp3-tree .bp3-icon.bp3-intent-primary, .bp3-dark .bp3-tree .bp3-icon-standard.bp3-intent-primary, .bp3-dark .bp3-tree .bp3-icon-large.bp3-intent-primary{
    color:#137cbd; }
  .bp3-dark .bp3-tree .bp3-icon.bp3-intent-success, .bp3-dark .bp3-tree .bp3-icon-standard.bp3-intent-success, .bp3-dark .bp3-tree .bp3-icon-large.bp3-intent-success{
    color:#0f9960; }
  .bp3-dark .bp3-tree .bp3-icon.bp3-intent-warning, .bp3-dark .bp3-tree .bp3-icon-standard.bp3-intent-warning, .bp3-dark .bp3-tree .bp3-icon-large.bp3-intent-warning{
    color:#d9822b; }
  .bp3-dark .bp3-tree .bp3-icon.bp3-intent-danger, .bp3-dark .bp3-tree .bp3-icon-standard.bp3-intent-danger, .bp3-dark .bp3-tree .bp3-icon-large.bp3-intent-danger{
    color:#db3737; }

.bp3-dark .bp3-tree-node.bp3-tree-node-selected > .bp3-tree-node-content{
  background-color:#137cbd; }
.bp3-omnibar{
  -webkit-filter:blur(0);
          filter:blur(0);
  opacity:1;
  background-color:#ffffff;
  border-radius:3px;
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 4px 8px rgba(16, 22, 26, 0.2), 0 18px 46px 6px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 4px 8px rgba(16, 22, 26, 0.2), 0 18px 46px 6px rgba(16, 22, 26, 0.2);
  left:calc(50% - 250px);
  top:20vh;
  width:500px;
  z-index:21; }
  .bp3-omnibar.bp3-overlay-enter, .bp3-omnibar.bp3-overlay-appear{
    -webkit-filter:blur(20px);
            filter:blur(20px);
    opacity:0.2; }
  .bp3-omnibar.bp3-overlay-enter-active, .bp3-omnibar.bp3-overlay-appear-active{
    -webkit-filter:blur(0);
            filter:blur(0);
    opacity:1;
    -webkit-transition-delay:0;
            transition-delay:0;
    -webkit-transition-duration:200ms;
            transition-duration:200ms;
    -webkit-transition-property:opacity, -webkit-filter;
    transition-property:opacity, -webkit-filter;
    transition-property:filter, opacity;
    transition-property:filter, opacity, -webkit-filter;
    -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
            transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-omnibar.bp3-overlay-exit{
    -webkit-filter:blur(0);
            filter:blur(0);
    opacity:1; }
  .bp3-omnibar.bp3-overlay-exit-active{
    -webkit-filter:blur(20px);
            filter:blur(20px);
    opacity:0.2;
    -webkit-transition-delay:0;
            transition-delay:0;
    -webkit-transition-duration:200ms;
            transition-duration:200ms;
    -webkit-transition-property:opacity, -webkit-filter;
    transition-property:opacity, -webkit-filter;
    transition-property:filter, opacity;
    transition-property:filter, opacity, -webkit-filter;
    -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
            transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-omnibar .bp3-input{
    background-color:transparent;
    border-radius:0; }
    .bp3-omnibar .bp3-input, .bp3-omnibar .bp3-input:focus{
      -webkit-box-shadow:none;
              box-shadow:none; }
  .bp3-omnibar .bp3-menu{
    background-color:transparent;
    border-radius:0;
    -webkit-box-shadow:inset 0 1px 0 rgba(16, 22, 26, 0.15);
            box-shadow:inset 0 1px 0 rgba(16, 22, 26, 0.15);
    max-height:calc(60vh - 40px);
    overflow:auto; }
    .bp3-omnibar .bp3-menu:empty{
      display:none; }
  .bp3-dark .bp3-omnibar, .bp3-omnibar.bp3-dark{
    background-color:#30404d;
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 4px 8px rgba(16, 22, 26, 0.4), 0 18px 46px 6px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 4px 8px rgba(16, 22, 26, 0.4), 0 18px 46px 6px rgba(16, 22, 26, 0.4); }

.bp3-omnibar-overlay .bp3-overlay-backdrop{
  background-color:rgba(16, 22, 26, 0.2); }

.bp3-select-popover .bp3-popover-content{
  padding:5px; }

.bp3-select-popover .bp3-input-group{
  margin-bottom:0; }

.bp3-select-popover .bp3-menu{
  max-height:300px;
  max-width:400px;
  overflow:auto;
  padding:0; }
  .bp3-select-popover .bp3-menu:not(:first-child){
    padding-top:5px; }

.bp3-multi-select{
  min-width:150px; }

.bp3-multi-select-popover .bp3-menu{
  max-height:300px;
  max-width:400px;
  overflow:auto; }

.bp3-select-popover .bp3-popover-content{
  padding:5px; }

.bp3-select-popover .bp3-input-group{
  margin-bottom:0; }

.bp3-select-popover .bp3-menu{
  max-height:300px;
  max-width:400px;
  overflow:auto;
  padding:0; }
  .bp3-select-popover .bp3-menu:not(:first-child){
    padding-top:5px; }
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
  --jp-icon-add: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTE5IDEzaC02djZoLTJ2LTZINXYtMmg2VjVoMnY2aDZ2MnoiLz4KICA8L2c+Cjwvc3ZnPgo=);
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
  --jp-icon-code: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjIiIGhlaWdodD0iMjIiIHZpZXdCb3g9IjAgMCAyOCAyOCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CgkJPHBhdGggZD0iTTExLjQgMTguNkw2LjggMTRMMTEuNCA5LjRMMTAgOEw0IDE0TDEwIDIwTDExLjQgMTguNlpNMTYuNiAxOC42TDIxLjIgMTRMMTYuNiA5LjRMMTggOEwyNCAxNEwxOCAyMEwxNi42IDE4LjZWMTguNloiLz4KCTwvZz4KPC9zdmc+Cg==);
  --jp-icon-console: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIwMCAyMDAiPgogIDxnIGNsYXNzPSJqcC1pY29uLWJyYW5kMSBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiMwMjg4RDEiPgogICAgPHBhdGggZD0iTTIwIDE5LjhoMTYwdjE1OS45SDIweiIvPgogIDwvZz4KICA8ZyBjbGFzcz0ianAtaWNvbi1zZWxlY3RhYmxlLWludmVyc2UiIGZpbGw9IiNmZmYiPgogICAgPHBhdGggZD0iTTEwNSAxMjcuM2g0MHYxMi44aC00MHpNNTEuMSA3N0w3NCA5OS45bC0yMy4zIDIzLjMgMTAuNSAxMC41IDIzLjMtMjMuM0w5NSA5OS45IDg0LjUgODkuNCA2MS42IDY2LjV6Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-copy: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMTggMTgiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTExLjksMUgzLjJDMi40LDEsMS43LDEuNywxLjcsMi41djEwLjJoMS41VjIuNWg4LjdWMXogTTE0LjEsMy45aC04Yy0wLjgsMC0xLjUsMC43LTEuNSwxLjV2MTAuMmMwLDAuOCwwLjcsMS41LDEuNSwxLjVoOCBjMC44LDAsMS41LTAuNywxLjUtMS41VjUuNEMxNS41LDQuNiwxNC45LDMuOSwxNC4xLDMuOXogTTE0LjEsMTUuNWgtOFY1LjRoOFYxNS41eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-copyright: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIGVuYWJsZS1iYWNrZ3JvdW5kPSJuZXcgMCAwIDI0IDI0IiBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCI+CiAgPGcgY2xhc3M9ImpwLWljb24zIiBmaWxsPSIjNjE2MTYxIj4KICAgIDxwYXRoIGQ9Ik0xMS44OCw5LjE0YzEuMjgsMC4wNiwxLjYxLDEuMTUsMS42MywxLjY2aDEuNzljLTAuMDgtMS45OC0xLjQ5LTMuMTktMy40NS0zLjE5QzkuNjQsNy42MSw4LDksOCwxMi4xNCBjMCwxLjk0LDAuOTMsNC4yNCwzLjg0LDQuMjRjMi4yMiwwLDMuNDEtMS42NSwzLjQ0LTIuOTVoLTEuNzljLTAuMDMsMC41OS0wLjQ1LDEuMzgtMS42MywxLjQ0QzEwLjU1LDE0LjgzLDEwLDEzLjgxLDEwLDEyLjE0IEMxMCw5LjI1LDExLjI4LDkuMTYsMTEuODgsOS4xNHogTTEyLDJDNi40OCwyLDIsNi40OCwyLDEyczQuNDgsMTAsMTAsMTBzMTAtNC40OCwxMC0xMFMxNy41MiwyLDEyLDJ6IE0xMiwyMGMtNC40MSwwLTgtMy41OS04LTggczMuNTktOCw4LThzOCwzLjU5LDgsOFMxNi40MSwyMCwxMiwyMHoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-cut: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTkuNjQgNy42NGMuMjMtLjUuMzYtMS4wNS4zNi0xLjY0IDAtMi4yMS0xLjc5LTQtNC00UzIgMy43OSAyIDZzMS43OSA0IDQgNGMuNTkgMCAxLjE0LS4xMyAxLjY0LS4zNkwxMCAxMmwtMi4zNiAyLjM2QzcuMTQgMTQuMTMgNi41OSAxNCA2IDE0Yy0yLjIxIDAtNCAxLjc5LTQgNHMxLjc5IDQgNCA0IDQtMS43OSA0LTRjMC0uNTktLjEzLTEuMTQtLjM2LTEuNjRMMTIgMTRsNyA3aDN2LTFMOS42NCA3LjY0ek02IDhjLTEuMSAwLTItLjg5LTItMnMuOS0yIDItMiAyIC44OSAyIDItLjkgMi0yIDJ6bTAgMTJjLTEuMSAwLTItLjg5LTItMnMuOS0yIDItMiAyIC44OSAyIDItLjkgMi0yIDJ6bTYtNy41Yy0uMjggMC0uNS0uMjItLjUtLjVzLjIyLS41LjUtLjUuNS4yMi41LjUtLjIyLjUtLjUuNXpNMTkgM2wtNiA2IDIgMiA3LTdWM3oiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-download: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTE5IDloLTRWM0g5djZINWw3IDcgNy03ek01IDE4djJoMTR2LTJINXoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-edit: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTMgMTcuMjVWMjFoMy43NUwxNy44MSA5Ljk0bC0zLjc1LTMuNzVMMyAxNy4yNXpNMjAuNzEgNy4wNGMuMzktLjM5LjM5LTEuMDIgMC0xLjQxbC0yLjM0LTIuMzRjLS4zOS0uMzktMS4wMi0uMzktMS40MSAwbC0xLjgzIDEuODMgMy43NSAzLjc1IDEuODMtMS44M3oiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-ellipses: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPGNpcmNsZSBjeD0iNSIgY3k9IjEyIiByPSIyIi8+CiAgICA8Y2lyY2xlIGN4PSIxMiIgY3k9IjEyIiByPSIyIi8+CiAgICA8Y2lyY2xlIGN4PSIxOSIgY3k9IjEyIiByPSIyIi8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-extension: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTIwLjUgMTFIMTlWN2MwLTEuMS0uOS0yLTItMmgtNFYzLjVDMTMgMi4xMiAxMS44OCAxIDEwLjUgMVM4IDIuMTIgOCAzLjVWNUg0Yy0xLjEgMC0xLjk5LjktMS45OSAydjMuOEgzLjVjMS40OSAwIDIuNyAxLjIxIDIuNyAyLjdzLTEuMjEgMi43LTIuNyAyLjdIMlYyMGMwIDEuMS45IDIgMiAyaDMuOHYtMS41YzAtMS40OSAxLjIxLTIuNyAyLjctMi43IDEuNDkgMCAyLjcgMS4yMSAyLjcgMi43VjIySDE3YzEuMSAwIDItLjkgMi0ydi00aDEuNWMxLjM4IDAgMi41LTEuMTIgMi41LTIuNVMyMS44OCAxMSAyMC41IDExeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-fast-forward: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTQgMThsOC41LTZMNCA2djEyem05LTEydjEybDguNS02TDEzIDZ6Ii8+CiAgICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-file-upload: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTkgMTZoNnYtNmg0bC03LTctNyA3aDR6bS00IDJoMTR2Mkg1eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-file: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMTkuMyA4LjJsLTUuNS01LjVjLS4zLS4zLS43LS41LTEuMi0uNUgzLjljLS44LjEtMS42LjktMS42IDEuOHYxNC4xYzAgLjkuNyAxLjYgMS42IDEuNmgxNC4yYy45IDAgMS42LS43IDEuNi0xLjZWOS40Yy4xLS41LS4xLS45LS40LTEuMnptLTUuOC0zLjNsMy40IDMuNmgtMy40VjQuOXptMy45IDEyLjdINC43Yy0uMSAwLS4yIDAtLjItLjJWNC43YzAtLjIuMS0uMy4yLS4zaDcuMnY0LjRzMCAuOC4zIDEuMWMuMy4zIDEuMS4zIDEuMS4zaDQuM3Y3LjJzLS4xLjItLjIuMnoiLz4KPC9zdmc+Cg==);
  --jp-icon-filter-list: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTEwIDE4aDR2LTJoLTR2MnpNMyA2djJoMThWNkgzem0zIDdoMTJ2LTJINnYyeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-folder: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMTAgNEg0Yy0xLjEgMC0xLjk5LjktMS45OSAyTDIgMThjMCAxLjEuOSAyIDIgMmgxNmMxLjEgMCAyLS45IDItMlY4YzAtMS4xLS45LTItMi0yaC04bC0yLTJ6Ii8+Cjwvc3ZnPgo=);
  --jp-icon-html5: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDUxMiA1MTIiPgogIDxwYXRoIGNsYXNzPSJqcC1pY29uMCBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiMwMDAiIGQ9Ik0xMDguNCAwaDIzdjIyLjhoMjEuMlYwaDIzdjY5aC0yM1Y0NmgtMjF2MjNoLTIzLjJNMjA2IDIzaC0yMC4zVjBoNjMuN3YyM0gyMjl2NDZoLTIzbTUzLjUtNjloMjQuMWwxNC44IDI0LjNMMzEzLjIgMGgyNC4xdjY5aC0yM1YzNC44bC0xNi4xIDI0LjgtMTYuMS0yNC44VjY5aC0yMi42bTg5LjItNjloMjN2NDYuMmgzMi42VjY5aC01NS42Ii8+CiAgPHBhdGggY2xhc3M9ImpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iI2U0NGQyNiIgZD0iTTEwNy42IDQ3MWwtMzMtMzcwLjRoMzYyLjhsLTMzIDM3MC4yTDI1NS43IDUxMiIvPgogIDxwYXRoIGNsYXNzPSJqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiNmMTY1MjkiIGQ9Ik0yNTYgNDgwLjVWMTMxaDE0OC4zTDM3NiA0NDciLz4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1zZWxlY3RhYmxlLWludmVyc2UiIGZpbGw9IiNlYmViZWIiIGQ9Ik0xNDIgMTc2LjNoMTE0djQ1LjRoLTY0LjJsNC4yIDQ2LjVoNjB2NDUuM0gxNTQuNG0yIDIyLjhIMjAybDMuMiAzNi4zIDUwLjggMTMuNnY0Ny40bC05My4yLTI2Ii8+CiAgPHBhdGggY2xhc3M9ImpwLWljb24tc2VsZWN0YWJsZS1pbnZlcnNlIiBmaWxsPSIjZmZmIiBkPSJNMzY5LjYgMTc2LjNIMjU1Ljh2NDUuNGgxMDkuNm0tNC4xIDQ2LjVIMjU1Ljh2NDUuNGg1NmwtNS4zIDU5LTUwLjcgMTMuNnY0Ny4ybDkzLTI1LjgiLz4KPC9zdmc+Cg==);
  --jp-icon-image: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1icmFuZDQganAtaWNvbi1zZWxlY3RhYmxlLWludmVyc2UiIGZpbGw9IiNGRkYiIGQ9Ik0yLjIgMi4yaDE3LjV2MTcuNUgyLjJ6Ii8+CiAgPHBhdGggY2xhc3M9ImpwLWljb24tYnJhbmQwIGpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iIzNGNTFCNSIgZD0iTTIuMiAyLjJ2MTcuNWgxNy41bC4xLTE3LjVIMi4yem0xMi4xIDIuMmMxLjIgMCAyLjIgMSAyLjIgMi4ycy0xIDIuMi0yLjIgMi4yLTIuMi0xLTIuMi0yLjIgMS0yLjIgMi4yLTIuMnpNNC40IDE3LjZsMy4zLTguOCAzLjMgNi42IDIuMi0zLjIgNC40IDUuNEg0LjR6Ii8+Cjwvc3ZnPgo=);
  --jp-icon-inspector: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMjAgNEg0Yy0xLjEgMC0xLjk5LjktMS45OSAyTDIgMThjMCAxLjEuOSAyIDIgMmgxNmMxLjEgMCAyLS45IDItMlY2YzAtMS4xLS45LTItMi0yem0tNSAxNEg0di00aDExdjR6bTAtNUg0VjloMTF2NHptNSA1aC00VjloNHY5eiIvPgo8L3N2Zz4K);
  --jp-icon-json: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8ZyBjbGFzcz0ianAtaWNvbi13YXJuMSBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiNGOUE4MjUiPgogICAgPHBhdGggZD0iTTIwLjIgMTEuOGMtMS42IDAtMS43LjUtMS43IDEgMCAuNC4xLjkuMSAxLjMuMS41LjEuOS4xIDEuMyAwIDEuNy0xLjQgMi4zLTMuNSAyLjNoLS45di0xLjloLjVjMS4xIDAgMS40IDAgMS40LS44IDAtLjMgMC0uNi0uMS0xIDAtLjQtLjEtLjgtLjEtMS4yIDAtMS4zIDAtMS44IDEuMy0yLTEuMy0uMi0xLjMtLjctMS4zLTIgMC0uNC4xLS44LjEtMS4yLjEtLjQuMS0uNy4xLTEgMC0uOC0uNC0uNy0xLjQtLjhoLS41VjQuMWguOWMyLjIgMCAzLjUuNyAzLjUgMi4zIDAgLjQtLjEuOS0uMSAxLjMtLjEuNS0uMS45LS4xIDEuMyAwIC41LjIgMSAxLjcgMXYxLjh6TTEuOCAxMC4xYzEuNiAwIDEuNy0uNSAxLjctMSAwLS40LS4xLS45LS4xLTEuMy0uMS0uNS0uMS0uOS0uMS0xLjMgMC0xLjYgMS40LTIuMyAzLjUtMi4zaC45djEuOWgtLjVjLTEgMC0xLjQgMC0xLjQuOCAwIC4zIDAgLjYuMSAxIDAgLjIuMS42LjEgMSAwIDEuMyAwIDEuOC0xLjMgMkM2IDExLjIgNiAxMS43IDYgMTNjMCAuNC0uMS44LS4xIDEuMi0uMS4zLS4xLjctLjEgMSAwIC44LjMuOCAxLjQuOGguNXYxLjloLS45Yy0yLjEgMC0zLjUtLjYtMy41LTIuMyAwLS40LjEtLjkuMS0xLjMuMS0uNS4xLS45LjEtMS4zIDAtLjUtLjItMS0xLjctMXYtMS45eiIvPgogICAgPGNpcmNsZSBjeD0iMTEiIGN5PSIxMy44IiByPSIyLjEiLz4KICAgIDxjaXJjbGUgY3g9IjExIiBjeT0iOC4yIiByPSIyLjEiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-julia: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDMyNSAzMDAiPgogIDxnIGNsYXNzPSJqcC1icmFuZDAganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjY2IzYzMzIj4KICAgIDxwYXRoIGQ9Ik0gMTUwLjg5ODQzOCAyMjUgQyAxNTAuODk4NDM4IDI2Ni40MjE4NzUgMTE3LjMyMDMxMiAzMDAgNzUuODk4NDM4IDMwMCBDIDM0LjQ3NjU2MiAzMDAgMC44OTg0MzggMjY2LjQyMTg3NSAwLjg5ODQzOCAyMjUgQyAwLjg5ODQzOCAxODMuNTc4MTI1IDM0LjQ3NjU2MiAxNTAgNzUuODk4NDM4IDE1MCBDIDExNy4zMjAzMTIgMTUwIDE1MC44OTg0MzggMTgzLjU3ODEyNSAxNTAuODk4NDM4IDIyNSIvPgogIDwvZz4KICA8ZyBjbGFzcz0ianAtYnJhbmQwIGpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iIzM4OTgyNiI+CiAgICA8cGF0aCBkPSJNIDIzNy41IDc1IEMgMjM3LjUgMTE2LjQyMTg3NSAyMDMuOTIxODc1IDE1MCAxNjIuNSAxNTAgQyAxMjEuMDc4MTI1IDE1MCA4Ny41IDExNi40MjE4NzUgODcuNSA3NSBDIDg3LjUgMzMuNTc4MTI1IDEyMS4wNzgxMjUgMCAxNjIuNSAwIEMgMjAzLjkyMTg3NSAwIDIzNy41IDMzLjU3ODEyNSAyMzcuNSA3NSIvPgogIDwvZz4KICA8ZyBjbGFzcz0ianAtYnJhbmQwIGpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iIzk1NThiMiI+CiAgICA8cGF0aCBkPSJNIDMyNC4xMDE1NjIgMjI1IEMgMzI0LjEwMTU2MiAyNjYuNDIxODc1IDI5MC41MjM0MzggMzAwIDI0OS4xMDE1NjIgMzAwIEMgMjA3LjY3OTY4OCAzMDAgMTc0LjEwMTU2MiAyNjYuNDIxODc1IDE3NC4xMDE1NjIgMjI1IEMgMTc0LjEwMTU2MiAxODMuNTc4MTI1IDIwNy42Nzk2ODggMTUwIDI0OS4xMDE1NjIgMTUwIEMgMjkwLjUyMzQzOCAxNTAgMzI0LjEwMTU2MiAxODMuNTc4MTI1IDMyNC4xMDE1NjIgMjI1Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-jupyter-favicon: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTUyIiBoZWlnaHQ9IjE2NSIgdmlld0JveD0iMCAwIDE1MiAxNjUiIHZlcnNpb249IjEuMSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbi13YXJuMCIgZmlsbD0iI0YzNzcyNiI+CiAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgwLjA3ODk0NywgMTEwLjU4MjkyNykiIGQ9Ik03NS45NDIyODQyLDI5LjU4MDQ1NjEgQzQzLjMwMjM5NDcsMjkuNTgwNDU2MSAxNC43OTY3ODMyLDE3LjY1MzQ2MzQgMCwwIEM1LjUxMDgzMjExLDE1Ljg0MDY4MjkgMTUuNzgxNTM4OSwyOS41NjY3NzMyIDI5LjM5MDQ5NDcsMzkuMjc4NDE3MSBDNDIuOTk5Nyw0OC45ODk4NTM3IDU5LjI3MzcsNTQuMjA2NzgwNSA3NS45NjA1Nzg5LDU0LjIwNjc4MDUgQzkyLjY0NzQ1NzksNTQuMjA2NzgwNSAxMDguOTIxNDU4LDQ4Ljk4OTg1MzcgMTIyLjUzMDY2MywzOS4yNzg0MTcxIEMxMzYuMTM5NDUzLDI5LjU2Njc3MzIgMTQ2LjQxMDI4NCwxNS44NDA2ODI5IDE1MS45MjExNTgsMCBDMTM3LjA4Nzg2OCwxNy42NTM0NjM0IDEwOC41ODI1ODksMjkuNTgwNDU2MSA3NS45NDIyODQyLDI5LjU4MDQ1NjEgTDc1Ljk0MjI4NDIsMjkuNTgwNDU2MSBaIiAvPgogICAgPHBhdGggdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMC4wMzczNjgsIDAuNzA0ODc4KSIgZD0iTTc1Ljk3ODQ1NzksMjQuNjI2NDA3MyBDMTA4LjYxODc2MywyNC42MjY0MDczIDEzNy4xMjQ0NTgsMzYuNTUzNDQxNSAxNTEuOTIxMTU4LDU0LjIwNjc4MDUgQzE0Ni40MTAyODQsMzguMzY2MjIyIDEzNi4xMzk0NTMsMjQuNjQwMTMxNyAxMjIuNTMwNjYzLDE0LjkyODQ4NzggQzEwOC45MjE0NTgsNS4yMTY4NDM5IDkyLjY0NzQ1NzksMCA3NS45NjA1Nzg5LDAgQzU5LjI3MzcsMCA0Mi45OTk3LDUuMjE2ODQzOSAyOS4zOTA0OTQ3LDE0LjkyODQ4NzggQzE1Ljc4MTUzODksMjQuNjQwMTMxNyA1LjUxMDgzMjExLDM4LjM2NjIyMiAwLDU0LjIwNjc4MDUgQzE0LjgzMzA4MTYsMzYuNTg5OTI5MyA0My4zMzg1Njg0LDI0LjYyNjQwNzMgNzUuOTc4NDU3OSwyNC42MjY0MDczIEw3NS45Nzg0NTc5LDI0LjYyNjQwNzMgWiIgLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-jupyter: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMzkiIGhlaWdodD0iNTEiIHZpZXdCb3g9IjAgMCAzOSA1MSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSgtMTYzOCAtMjI4MSkiPgogICAgPGcgY2xhc3M9ImpwLWljb24td2FybjAiIGZpbGw9IiNGMzc3MjYiPgogICAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxNjM5Ljc0IDIzMTEuOTgpIiBkPSJNIDE4LjI2NDYgNy4xMzQxMUMgMTAuNDE0NSA3LjEzNDExIDMuNTU4NzIgNC4yNTc2IDAgMEMgMS4zMjUzOSAzLjgyMDQgMy43OTU1NiA3LjEzMDgxIDcuMDY4NiA5LjQ3MzAzQyAxMC4zNDE3IDExLjgxNTIgMTQuMjU1NyAxMy4wNzM0IDE4LjI2OSAxMy4wNzM0QyAyMi4yODIzIDEzLjA3MzQgMjYuMTk2MyAxMS44MTUyIDI5LjQ2OTQgOS40NzMwM0MgMzIuNzQyNCA3LjEzMDgxIDM1LjIxMjYgMy44MjA0IDM2LjUzOCAwQyAzMi45NzA1IDQuMjU3NiAyNi4xMTQ4IDcuMTM0MTEgMTguMjY0NiA3LjEzNDExWiIvPgogICAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxNjM5LjczIDIyODUuNDgpIiBkPSJNIDE4LjI3MzMgNS45MzkzMUMgMjYuMTIzNSA1LjkzOTMxIDMyLjk3OTMgOC44MTU4MyAzNi41MzggMTMuMDczNEMgMzUuMjEyNiA5LjI1MzAzIDMyLjc0MjQgNS45NDI2MiAyOS40Njk0IDMuNjAwNEMgMjYuMTk2MyAxLjI1ODE4IDIyLjI4MjMgMCAxOC4yNjkgMEMgMTQuMjU1NyAwIDEwLjM0MTcgMS4yNTgxOCA3LjA2ODYgMy42MDA0QyAzLjc5NTU2IDUuOTQyNjIgMS4zMjUzOSA5LjI1MzAzIDAgMTMuMDczNEMgMy41Njc0NSA4LjgyNDYzIDEwLjQyMzIgNS45MzkzMSAxOC4yNzMzIDUuOTM5MzFaIi8+CiAgICA8L2c+CiAgICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxNjY5LjMgMjI4MS4zMSkiIGQ9Ik0gNS44OTM1MyAyLjg0NEMgNS45MTg4OSAzLjQzMTY1IDUuNzcwODUgNC4wMTM2NyA1LjQ2ODE1IDQuNTE2NDVDIDUuMTY1NDUgNS4wMTkyMiA0LjcyMTY4IDUuNDIwMTUgNC4xOTI5OSA1LjY2ODUxQyAzLjY2NDMgNS45MTY4OCAzLjA3NDQ0IDYuMDAxNTEgMi40OTgwNSA1LjkxMTcxQyAxLjkyMTY2IDUuODIxOSAxLjM4NDYzIDUuNTYxNyAwLjk1NDg5OCA1LjE2NDAxQyAwLjUyNTE3IDQuNzY2MzMgMC4yMjIwNTYgNC4yNDkwMyAwLjA4MzkwMzcgMy42Nzc1N0MgLTAuMDU0MjQ4MyAzLjEwNjExIC0wLjAyMTIzIDIuNTA2MTcgMC4xNzg3ODEgMS45NTM2NEMgMC4zNzg3OTMgMS40MDExIDAuNzM2ODA5IDAuOTIwODE3IDEuMjA3NTQgMC41NzM1MzhDIDEuNjc4MjYgMC4yMjYyNTkgMi4yNDA1NSAwLjAyNzU5MTkgMi44MjMyNiAwLjAwMjY3MjI5QyAzLjYwMzg5IC0wLjAzMDcxMTUgNC4zNjU3MyAwLjI0OTc4OSA0Ljk0MTQyIDAuNzgyNTUxQyA1LjUxNzExIDEuMzE1MzEgNS44NTk1NiAyLjA1Njc2IDUuODkzNTMgMi44NDRaIi8+CiAgICAgIDxwYXRoIHRyYW5zZm9ybT0idHJhbnNsYXRlKDE2MzkuOCAyMzIzLjgxKSIgZD0iTSA3LjQyNzg5IDMuNTgzMzhDIDcuNDYwMDggNC4zMjQzIDcuMjczNTUgNS4wNTgxOSA2Ljg5MTkzIDUuNjkyMTNDIDYuNTEwMzEgNi4zMjYwNyA1Ljk1MDc1IDYuODMxNTYgNS4yODQxMSA3LjE0NDZDIDQuNjE3NDcgNy40NTc2MyAzLjg3MzcxIDcuNTY0MTQgMy4xNDcwMiA3LjQ1MDYzQyAyLjQyMDMyIDcuMzM3MTIgMS43NDMzNiA3LjAwODcgMS4yMDE4NCA2LjUwNjk1QyAwLjY2MDMyOCA2LjAwNTIgMC4yNzg2MSA1LjM1MjY4IDAuMTA1MDE3IDQuNjMyMDJDIC0wLjA2ODU3NTcgMy45MTEzNSAtMC4wMjYyMzYxIDMuMTU0OTQgMC4yMjY2NzUgMi40NTg1NkMgMC40Nzk1ODcgMS43NjIxNyAwLjkzMTY5NyAxLjE1NzEzIDEuNTI1NzYgMC43MjAwMzNDIDIuMTE5ODMgMC4yODI5MzUgMi44MjkxNCAwLjAzMzQzOTUgMy41NjM4OSAwLjAwMzEzMzQ0QyA0LjU0NjY3IC0wLjAzNzQwMzMgNS41MDUyOSAwLjMxNjcwNiA2LjIyOTYxIDAuOTg3ODM1QyA2Ljk1MzkzIDEuNjU4OTYgNy4zODQ4NCAyLjU5MjM1IDcuNDI3ODkgMy41ODMzOEwgNy40Mjc4OSAzLjU4MzM4WiIvPgogICAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxNjM4LjM2IDIyODYuMDYpIiBkPSJNIDIuMjc0NzEgNC4zOTYyOUMgMS44NDM2MyA0LjQxNTA4IDEuNDE2NzEgNC4zMDQ0NSAxLjA0Nzk5IDQuMDc4NDNDIDAuNjc5MjY4IDMuODUyNCAwLjM4NTMyOCAzLjUyMTE0IDAuMjAzMzcxIDMuMTI2NTZDIDAuMDIxNDEzNiAyLjczMTk4IC0wLjA0MDM3OTggMi4yOTE4MyAwLjAyNTgxMTYgMS44NjE4MUMgMC4wOTIwMDMxIDEuNDMxOCAwLjI4MzIwNCAxLjAzMTI2IDAuNTc1MjEzIDAuNzEwODgzQyAwLjg2NzIyMiAwLjM5MDUxIDEuMjQ2OTEgMC4xNjQ3MDggMS42NjYyMiAwLjA2MjA1OTJDIDIuMDg1NTMgLTAuMDQwNTg5NyAyLjUyNTYxIC0wLjAxNTQ3MTQgMi45MzA3NiAwLjEzNDIzNUMgMy4zMzU5MSAwLjI4Mzk0MSAzLjY4NzkyIDAuNTUxNTA1IDMuOTQyMjIgMC45MDMwNkMgNC4xOTY1MiAxLjI1NDYyIDQuMzQxNjkgMS42NzQzNiA0LjM1OTM1IDIuMTA5MTZDIDQuMzgyOTkgMi42OTEwNyA0LjE3Njc4IDMuMjU4NjkgMy43ODU5NyAzLjY4NzQ2QyAzLjM5NTE2IDQuMTE2MjQgMi44NTE2NiA0LjM3MTE2IDIuMjc0NzEgNC4zOTYyOUwgMi4yNzQ3MSA0LjM5NjI5WiIvPgogICAgPC9nPgogIDwvZz4+Cjwvc3ZnPgo=);
  --jp-icon-jupyterlab-wordmark: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyMDAiIHZpZXdCb3g9IjAgMCAxODYwLjggNDc1Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjIiIGZpbGw9IiM0RTRFNEUiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDQ4MC4xMzY0MDEsIDY0LjI3MTQ5MykiPgogICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMC4wMDAwMDAsIDU4Ljg3NTU2NikiPgogICAgICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSgwLjA4NzYwMywgMC4xNDAyOTQpIj4KICAgICAgICA8cGF0aCBkPSJNLTQyNi45LDE2OS44YzAsNDguNy0zLjcsNjQuNy0xMy42LDc2LjRjLTEwLjgsMTAtMjUsMTUuNS0zOS43LDE1LjVsMy43LDI5IGMyMi44LDAuMyw0NC44LTcuOSw2MS45LTIzLjFjMTcuOC0xOC41LDI0LTQ0LjEsMjQtODMuM1YwSC00Mjd2MTcwLjFMLTQyNi45LDE2OS44TC00MjYuOSwxNjkuOHoiLz4KICAgICAgPC9nPgogICAgPC9nPgogICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMTU1LjA0NTI5NiwgNTYuODM3MTA0KSI+CiAgICAgIDxnIHRyYW5zZm9ybT0idHJhbnNsYXRlKDEuNTYyNDUzLCAxLjc5OTg0MikiPgogICAgICAgIDxwYXRoIGQ9Ik0tMzEyLDE0OGMwLDIxLDAsMzkuNSwxLjcsNTUuNGgtMzEuOGwtMi4xLTMzLjNoLTAuOGMtNi43LDExLjYtMTYuNCwyMS4zLTI4LDI3LjkgYy0xMS42LDYuNi0yNC44LDEwLTM4LjIsOS44Yy0zMS40LDAtNjktMTcuNy02OS04OVYwaDM2LjR2MTEyLjdjMCwzOC43LDExLjYsNjQuNyw0NC42LDY0LjdjMTAuMy0wLjIsMjAuNC0zLjUsMjguOS05LjQgYzguNS01LjksMTUuMS0xNC4zLDE4LjktMjMuOWMyLjItNi4xLDMuMy0xMi41LDMuMy0xOC45VjAuMmgzNi40VjE0OEgtMzEyTC0zMTIsMTQ4eiIvPgogICAgICA8L2c+CiAgICA8L2c+CiAgICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSgzOTAuMDEzMzIyLCA1My40Nzk2MzgpIj4KICAgICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMS43MDY0NTgsIDAuMjMxNDI1KSI+CiAgICAgICAgPHBhdGggZD0iTS00NzguNiw3MS40YzAtMjYtMC44LTQ3LTEuNy02Ni43aDMyLjdsMS43LDM0LjhoMC44YzcuMS0xMi41LDE3LjUtMjIuOCwzMC4xLTI5LjcgYzEyLjUtNywyNi43LTEwLjMsNDEtOS44YzQ4LjMsMCw4NC43LDQxLjcsODQuNywxMDMuM2MwLDczLjEtNDMuNywxMDkuMi05MSwxMDkuMmMtMTIuMSwwLjUtMjQuMi0yLjItMzUtNy44IGMtMTAuOC01LjYtMTkuOS0xMy45LTI2LjYtMjQuMmgtMC44VjI5MWgtMzZ2LTIyMEwtNDc4LjYsNzEuNEwtNDc4LjYsNzEuNHogTS00NDIuNiwxMjUuNmMwLjEsNS4xLDAuNiwxMC4xLDEuNywxNS4xIGMzLDEyLjMsOS45LDIzLjMsMTkuOCwzMS4xYzkuOSw3LjgsMjIuMSwxMi4xLDM0LjcsMTIuMWMzOC41LDAsNjAuNy0zMS45LDYwLjctNzguNWMwLTQwLjctMjEuMS03NS42LTU5LjUtNzUuNiBjLTEyLjksMC40LTI1LjMsNS4xLTM1LjMsMTMuNGMtOS45LDguMy0xNi45LDE5LjctMTkuNiwzMi40Yy0xLjUsNC45LTIuMywxMC0yLjUsMTUuMVYxMjUuNkwtNDQyLjYsMTI1LjZMLTQ0Mi42LDEyNS42eiIvPgogICAgICA8L2c+CiAgICA8L2c+CiAgICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSg2MDYuNzQwNzI2LCA1Ni44MzcxMDQpIj4KICAgICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMC43NTEyMjYsIDEuOTg5Mjk5KSI+CiAgICAgICAgPHBhdGggZD0iTS00NDAuOCwwbDQzLjcsMTIwLjFjNC41LDEzLjQsOS41LDI5LjQsMTIuOCw0MS43aDAuOGMzLjctMTIuMiw3LjktMjcuNywxMi44LTQyLjQgbDM5LjctMTE5LjJoMzguNUwtMzQ2LjksMTQ1Yy0yNiw2OS43LTQzLjcsMTA1LjQtNjguNiwxMjcuMmMtMTIuNSwxMS43LTI3LjksMjAtNDQuNiwyMy45bC05LjEtMzEuMSBjMTEuNy0zLjksMjIuNS0xMC4xLDMxLjgtMTguMWMxMy4yLTExLjEsMjMuNy0yNS4yLDMwLjYtNDEuMmMxLjUtMi44LDIuNS01LjcsMi45LTguOGMtMC4zLTMuMy0xLjItNi42LTIuNS05LjdMLTQ4MC4yLDAuMSBoMzkuN0wtNDQwLjgsMEwtNDQwLjgsMHoiLz4KICAgICAgPC9nPgogICAgPC9nPgogICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoODIyLjc0ODEwNCwgMC4wMDAwMDApIj4KICAgICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMS40NjQwNTAsIDAuMzc4OTE0KSI+CiAgICAgICAgPHBhdGggZD0iTS00MTMuNywwdjU4LjNoNTJ2MjguMmgtNTJWMTk2YzAsMjUsNywzOS41LDI3LjMsMzkuNWM3LjEsMC4xLDE0LjItMC43LDIxLjEtMi41IGwxLjcsMjcuN2MtMTAuMywzLjctMjEuMyw1LjQtMzIuMiw1Yy03LjMsMC40LTE0LjYtMC43LTIxLjMtMy40Yy02LjgtMi43LTEyLjktNi44LTE3LjktMTIuMWMtMTAuMy0xMC45LTE0LjEtMjktMTQuMS01Mi45IFY4Ni41aC0zMVY1OC4zaDMxVjkuNkwtNDEzLjcsMEwtNDEzLjcsMHoiLz4KICAgICAgPC9nPgogICAgPC9nPgogICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoOTc0LjQzMzI4NiwgNTMuNDc5NjM4KSI+CiAgICAgIDxnIHRyYW5zZm9ybT0idHJhbnNsYXRlKDAuOTkwMDM0LCAwLjYxMDMzOSkiPgogICAgICAgIDxwYXRoIGQ9Ik0tNDQ1LjgsMTEzYzAuOCw1MCwzMi4yLDcwLjYsNjguNiw3MC42YzE5LDAuNiwzNy45LTMsNTUuMy0xMC41bDYuMiwyNi40IGMtMjAuOSw4LjktNDMuNSwxMy4xLTY2LjIsMTIuNmMtNjEuNSwwLTk4LjMtNDEuMi05OC4zLTEwMi41Qy00ODAuMiw0OC4yLTQ0NC43LDAtMzg2LjUsMGM2NS4yLDAsODIuNyw1OC4zLDgyLjcsOTUuNyBjLTAuMSw1LjgtMC41LDExLjUtMS4yLDE3LjJoLTE0MC42SC00NDUuOEwtNDQ1LjgsMTEzeiBNLTMzOS4yLDg2LjZjMC40LTIzLjUtOS41LTYwLjEtNTAuNC02MC4xIGMtMzYuOCwwLTUyLjgsMzQuNC01NS43LDYwLjFILTMzOS4yTC0zMzkuMiw4Ni42TC0zMzkuMiw4Ni42eiIvPgogICAgICA8L2c+CiAgICA8L2c+CiAgICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxMjAxLjk2MTA1OCwgNTMuNDc5NjM4KSI+CiAgICAgIDxnIHRyYW5zZm9ybT0idHJhbnNsYXRlKDEuMTc5NjQwLCAwLjcwNTA2OCkiPgogICAgICAgIDxwYXRoIGQ9Ik0tNDc4LjYsNjhjMC0yMy45LTAuNC00NC41LTEuNy02My40aDMxLjhsMS4yLDM5LjloMS43YzkuMS0yNy4zLDMxLTQ0LjUsNTUuMy00NC41IGMzLjUtMC4xLDcsMC40LDEwLjMsMS4ydjM0LjhjLTQuMS0wLjktOC4yLTEuMy0xMi40LTEuMmMtMjUuNiwwLTQzLjcsMTkuNy00OC43LDQ3LjRjLTEsNS43LTEuNiwxMS41LTEuNywxNy4ydjEwOC4zaC0zNlY2OCBMLTQ3OC42LDY4eiIvPgogICAgICA8L2c+CiAgICA8L2c+CiAgPC9nPgoKICA8ZyBjbGFzcz0ianAtaWNvbi13YXJuMCIgZmlsbD0iI0YzNzcyNiI+CiAgICA8cGF0aCBkPSJNMTM1Mi4zLDMyNi4yaDM3VjI4aC0zN1YzMjYuMnogTTE2MDQuOCwzMjYuMmMtMi41LTEzLjktMy40LTMxLjEtMy40LTQ4Ljd2LTc2IGMwLTQwLjctMTUuMS04My4xLTc3LjMtODMuMWMtMjUuNiwwLTUwLDcuMS02Ni44LDE4LjFsOC40LDI0LjRjMTQuMy05LjIsMzQtMTUuMSw1My0xNS4xYzQxLjYsMCw0Ni4yLDMwLjIsNDYuMiw0N3Y0LjIgYy03OC42LTAuNC0xMjIuMywyNi41LTEyMi4zLDc1LjZjMCwyOS40LDIxLDU4LjQsNjIuMiw1OC40YzI5LDAsNTAuOS0xNC4zLDYyLjItMzAuMmgxLjNsMi45LDI1LjZIMTYwNC44eiBNMTU2NS43LDI1Ny43IGMwLDMuOC0wLjgsOC0yLjEsMTEuOGMtNS45LDE3LjItMjIuNywzNC00OS4yLDM0Yy0xOC45LDAtMzQuOS0xMS4zLTM0LjktMzUuM2MwLTM5LjUsNDUuOC00Ni42LDg2LjItNDUuOFYyNTcuN3ogTTE2OTguNSwzMjYuMiBsMS43LTMzLjZoMS4zYzE1LjEsMjYuOSwzOC43LDM4LjIsNjguMSwzOC4yYzQ1LjQsMCw5MS4yLTM2LjEsOTEuMi0xMDguOGMwLjQtNjEuNy0zNS4zLTEwMy43LTg1LjctMTAzLjcgYy0zMi44LDAtNTYuMywxNC43LTY5LjMsMzcuNGgtMC44VjI4aC0zNi42djI0NS43YzAsMTguMS0wLjgsMzguNi0xLjcsNTIuNUgxNjk4LjV6IE0xNzA0LjgsMjA4LjJjMC01LjksMS4zLTEwLjksMi4xLTE1LjEgYzcuNi0yOC4xLDMxLjEtNDUuNCw1Ni4zLTQ1LjRjMzkuNSwwLDYwLjUsMzQuOSw2MC41LDc1LjZjMCw0Ni42LTIzLjEsNzguMS02MS44LDc4LjFjLTI2LjksMC00OC4zLTE3LjYtNTUuNS00My4zIGMtMC44LTQuMi0xLjctOC44LTEuNy0xMy40VjIwOC4yeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-kernel: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiIgZmlsbD0iIzYxNjE2MSIgZD0iTTE1IDlIOXY2aDZWOXptLTIgNGgtMnYtMmgydjJ6bTgtMlY5aC0yVjdjMC0xLjEtLjktMi0yLTJoLTJWM2gtMnYyaC0yVjNIOXYySDdjLTEuMSAwLTIgLjktMiAydjJIM3YyaDJ2MkgzdjJoMnYyYzAgMS4xLjkgMiAyIDJoMnYyaDJ2LTJoMnYyaDJ2LTJoMmMxLjEgMCAyLS45IDItMnYtMmgydi0yaC0ydi0yaDJ6bS00IDZIN1Y3aDEwdjEweiIvPgo8L3N2Zz4K);
  --jp-icon-keyboard: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMjAgNUg0Yy0xLjEgMC0xLjk5LjktMS45OSAyTDIgMTdjMCAxLjEuOSAyIDIgMmgxNmMxLjEgMCAyLS45IDItMlY3YzAtMS4xLS45LTItMi0yem0tOSAzaDJ2MmgtMlY4em0wIDNoMnYyaC0ydi0yek04IDhoMnYySDhWOHptMCAzaDJ2Mkg4di0yem0tMSAySDV2LTJoMnYyem0wLTNINVY4aDJ2MnptOSA3SDh2LTJoOHYyem0wLTRoLTJ2LTJoMnYyem0wLTNoLTJWOGgydjJ6bTMgM2gtMnYtMmgydjJ6bTAtM2gtMlY4aDJ2MnoiLz4KPC9zdmc+Cg==);
  --jp-icon-launcher: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMTkgMTlINVY1aDdWM0g1YTIgMiAwIDAwLTIgMnYxNGEyIDIgMCAwMDIgMmgxNGMxLjEgMCAyLS45IDItMnYtN2gtMnY3ek0xNCAzdjJoMy41OWwtOS44MyA5LjgzIDEuNDEgMS40MUwxOSA2LjQxVjEwaDJWM2gtN3oiLz4KPC9zdmc+Cg==);
  --jp-icon-line-form: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxwYXRoIGZpbGw9IndoaXRlIiBkPSJNNS44OCA0LjEyTDEzLjc2IDEybC03Ljg4IDcuODhMOCAyMmwxMC0xMEw4IDJ6Ii8+Cjwvc3ZnPgo=);
  --jp-icon-link: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTMuOSAxMmMwLTEuNzEgMS4zOS0zLjEgMy4xLTMuMWg0VjdIN2MtMi43NiAwLTUgMi4yNC01IDVzMi4yNCA1IDUgNWg0di0xLjlIN2MtMS43MSAwLTMuMS0xLjM5LTMuMS0zLjF6TTggMTNoOHYtMkg4djJ6bTktNmgtNHYxLjloNGMxLjcxIDAgMy4xIDEuMzkgMy4xIDMuMXMtMS4zOSAzLjEtMy4xIDMuMWgtNFYxN2g0YzIuNzYgMCA1LTIuMjQgNS01cy0yLjI0LTUtNS01eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-list: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiM2MTYxNjEiIGQ9Ik0xOSA1djE0SDVWNWgxNG0xLjEtMkgzLjljLS41IDAtLjkuNC0uOS45djE2LjJjMCAuNC40LjkuOS45aDE2LjJjLjQgMCAuOS0uNS45LS45VjMuOWMwLS41LS41LS45LS45LS45ek0xMSA3aDZ2MmgtNlY3em0wIDRoNnYyaC02di0yem0wIDRoNnYyaC02ek03IDdoMnYySDd6bTAgNGgydjJIN3ptMCA0aDJ2Mkg3eiIvPgo8L3N2Zz4=);
  --jp-icon-listings-info: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCA1MC45NzggNTAuOTc4IiBzdHlsZT0iZW5hYmxlLWJhY2tncm91bmQ6bmV3IDAgMCA1MC45NzggNTAuOTc4OyIgeG1sOnNwYWNlPSJwcmVzZXJ2ZSI+Cgk8Zz4KCQk8cGF0aCBzdHlsZT0iZmlsbDojMDEwMDAyOyIgZD0iTTQzLjUyLDcuNDU4QzM4LjcxMSwyLjY0OCwzMi4zMDcsMCwyNS40ODksMEMxOC42NywwLDEyLjI2NiwyLjY0OCw3LjQ1OCw3LjQ1OAoJCQljLTkuOTQzLDkuOTQxLTkuOTQzLDI2LjExOSwwLDM2LjA2MmM0LjgwOSw0LjgwOSwxMS4yMTIsNy40NTYsMTguMDMxLDcuNDU4YzAsMCwwLjAwMSwwLDAuMDAyLDAKCQkJYzYuODE2LDAsMTMuMjIxLTIuNjQ4LDE4LjAyOS03LjQ1OGM0LjgwOS00LjgwOSw3LjQ1Ny0xMS4yMTIsNy40NTctMTguMDNDNTAuOTc3LDE4LjY3LDQ4LjMyOCwxMi4yNjYsNDMuNTIsNy40NTh6CgkJCSBNNDIuMTA2LDQyLjEwNWMtNC40MzIsNC40MzEtMTAuMzMyLDYuODcyLTE2LjYxNSw2Ljg3MmgtMC4wMDJjLTYuMjg1LTAuMDAxLTEyLjE4Ny0yLjQ0MS0xNi42MTctNi44NzIKCQkJYy05LjE2Mi05LjE2My05LjE2Mi0yNC4wNzEsMC0zMy4yMzNDMTMuMzAzLDQuNDQsMTkuMjA0LDIsMjUuNDg5LDJjNi4yODQsMCwxMi4xODYsMi40NCwxNi42MTcsNi44NzIKCQkJYzQuNDMxLDQuNDMxLDYuODcxLDEwLjMzMiw2Ljg3MSwxNi42MTdDNDguOTc3LDMxLjc3Miw0Ni41MzYsMzcuNjc1LDQyLjEwNiw0Mi4xMDV6Ii8+CgkJPHBhdGggc3R5bGU9ImZpbGw6IzAxMDAwMjsiIGQ9Ik0yMy41NzgsMzIuMjE4Yy0wLjAyMy0xLjczNCwwLjE0My0zLjA1OSwwLjQ5Ni0zLjk3MmMwLjM1My0wLjkxMywxLjExLTEuOTk3LDIuMjcyLTMuMjUzCgkJCWMwLjQ2OC0wLjUzNiwwLjkyMy0xLjA2MiwxLjM2Ny0xLjU3NWMwLjYyNi0wLjc1MywxLjEwNC0xLjQ3OCwxLjQzNi0yLjE3NWMwLjMzMS0wLjcwNywwLjQ5NS0xLjU0MSwwLjQ5NS0yLjUKCQkJYzAtMS4wOTYtMC4yNi0yLjA4OC0wLjc3OS0yLjk3OWMtMC41NjUtMC44NzktMS41MDEtMS4zMzYtMi44MDYtMS4zNjljLTEuODAyLDAuMDU3LTIuOTg1LDAuNjY3LTMuNTUsMS44MzIKCQkJYy0wLjMwMSwwLjUzNS0wLjUwMywxLjE0MS0wLjYwNywxLjgxNGMtMC4xMzksMC43MDctMC4yMDcsMS40MzItMC4yMDcsMi4xNzRoLTIuOTM3Yy0wLjA5MS0yLjIwOCwwLjQwNy00LjExNCwxLjQ5My01LjcxOQoJCQljMS4wNjItMS42NCwyLjg1NS0yLjQ4MSw1LjM3OC0yLjUyN2MyLjE2LDAuMDIzLDMuODc0LDAuNjA4LDUuMTQxLDEuNzU4YzEuMjc4LDEuMTYsMS45MjksMi43NjQsMS45NSw0LjgxMQoJCQljMCwxLjE0Mi0wLjEzNywyLjExMS0wLjQxLDIuOTExYy0wLjMwOSwwLjg0NS0wLjczMSwxLjU5My0xLjI2OCwyLjI0M2MtMC40OTIsMC42NS0xLjA2OCwxLjMxOC0xLjczLDIuMDAyCgkJCWMtMC42NSwwLjY5Ny0xLjMxMywxLjQ3OS0xLjk4NywyLjM0NmMtMC4yMzksMC4zNzctMC40MjksMC43NzctMC41NjUsMS4xOTljLTAuMTYsMC45NTktMC4yMTcsMS45NTEtMC4xNzEsMi45NzkKCQkJQzI2LjU4OSwzMi4yMTgsMjMuNTc4LDMyLjIxOCwyMy41NzgsMzIuMjE4eiBNMjMuNTc4LDM4LjIydi0zLjQ4NGgzLjA3NnYzLjQ4NEgyMy41Nzh6Ii8+Cgk8L2c+Cjwvc3ZnPgo=);
  --jp-icon-markdown: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1jb250cmFzdDAganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjN0IxRkEyIiBkPSJNNSAxNC45aDEybC02LjEgNnptOS40LTYuOGMwLTEuMy0uMS0yLjktLjEtNC41LS40IDEuNC0uOSAyLjktMS4zIDQuM2wtMS4zIDQuM2gtMkw4LjUgNy45Yy0uNC0xLjMtLjctMi45LTEtNC4zLS4xIDEuNi0uMSAzLjItLjIgNC42TDcgMTIuNEg0LjhsLjctMTFoMy4zTDEwIDVjLjQgMS4yLjcgMi43IDEgMy45LjMtMS4yLjctMi42IDEtMy45bDEuMi0zLjdoMy4zbC42IDExaC0yLjRsLS4zLTQuMnoiLz4KPC9zdmc+Cg==);
  --jp-icon-new-folder: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTIwIDZoLThsLTItMkg0Yy0xLjExIDAtMS45OS44OS0xLjk5IDJMMiAxOGMwIDEuMTEuODkgMiAyIDJoMTZjMS4xMSAwIDItLjg5IDItMlY4YzAtMS4xMS0uODktMi0yLTJ6bS0xIDhoLTN2M2gtMnYtM2gtM3YtMmgzVjloMnYzaDN2MnoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-not-trusted: url(data:image/svg+xml;base64,PHN2ZyBmaWxsPSJub25lIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI1IDI1Ij4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiIgc3Ryb2tlPSIjMzMzMzMzIiBzdHJva2Utd2lkdGg9IjIiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDMgMykiIGQ9Ik0xLjg2MDk0IDExLjQ0MDlDMC44MjY0NDggOC43NzAyNyAwLjg2Mzc3OSA2LjA1NzY0IDEuMjQ5MDcgNC4xOTkzMkMyLjQ4MjA2IDMuOTMzNDcgNC4wODA2OCAzLjQwMzQ3IDUuNjAxMDIgMi44NDQ5QzcuMjM1NDkgMi4yNDQ0IDguODU2NjYgMS41ODE1IDkuOTg3NiAxLjA5NTM5QzExLjA1OTcgMS41ODM0MSAxMi42MDk0IDIuMjQ0NCAxNC4yMTggMi44NDMzOUMxNS43NTAzIDMuNDEzOTQgMTcuMzk5NSAzLjk1MjU4IDE4Ljc1MzkgNC4yMTM4NUMxOS4xMzY0IDYuMDcxNzcgMTkuMTcwOSA4Ljc3NzIyIDE4LjEzOSAxMS40NDA5QzE3LjAzMDMgMTQuMzAzMiAxNC42NjY4IDE3LjE4NDQgOS45OTk5OSAxOC45MzU0QzUuMzMzMTkgMTcuMTg0NCAyLjk2OTY4IDE0LjMwMzIgMS44NjA5NCAxMS40NDA5WiIvPgogICAgPHBhdGggY2xhc3M9ImpwLWljb24yIiBzdHJva2U9IiMzMzMzMzMiIHN0cm9rZS13aWR0aD0iMiIgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoOS4zMTU5MiA5LjMyMDMxKSIgZD0iTTcuMzY4NDIgMEwwIDcuMzY0NzkiLz4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiIgc3Ryb2tlPSIjMzMzMzMzIiBzdHJva2Utd2lkdGg9IjIiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDkuMzE1OTIgMTYuNjgzNikgc2NhbGUoMSAtMSkiIGQ9Ik03LjM2ODQyIDBMMCA3LjM2NDc5Ii8+Cjwvc3ZnPgo=);
  --jp-icon-notebook: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8ZyBjbGFzcz0ianAtaWNvbi13YXJuMCBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiNFRjZDMDAiPgogICAgPHBhdGggZD0iTTE4LjcgMy4zdjE1LjRIMy4zVjMuM2gxNS40bTEuNS0xLjVIMS44djE4LjNoMTguM2wuMS0xOC4zeiIvPgogICAgPHBhdGggZD0iTTE2LjUgMTYuNWwtNS40LTQuMy01LjYgNC4zdi0xMWgxMXoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-numbering: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjIiIGhlaWdodD0iMjIiIHZpZXdCb3g9IjAgMCAyOCAyOCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CgkJPHBhdGggZD0iTTQgMTlINlYxOS41SDVWMjAuNUg2VjIxSDRWMjJIN1YxOEg0VjE5Wk01IDEwSDZWNkg0VjdINVYxMFpNNCAxM0g1LjhMNCAxNS4xVjE2SDdWMTVINS4yTDcgMTIuOVYxMkg0VjEzWk05IDdWOUgyM1Y3SDlaTTkgMjFIMjNWMTlIOVYyMVpNOSAxNUgyM1YxM0g5VjE1WiIvPgoJPC9nPgo8L3N2Zz4K);
  --jp-icon-offline-bolt: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgd2lkdGg9IjE2Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTEyIDIuMDJjLTUuNTEgMC05Ljk4IDQuNDctOS45OCA5Ljk4czQuNDcgOS45OCA5Ljk4IDkuOTggOS45OC00LjQ3IDkuOTgtOS45OFMxNy41MSAyLjAyIDEyIDIuMDJ6TTExLjQ4IDIwdi02LjI2SDhMMTMgNHY2LjI2aDMuMzVMMTEuNDggMjB6Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-palette: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTE4IDEzVjIwSDRWNkg5LjAyQzkuMDcgNS4yOSA5LjI0IDQuNjIgOS41IDRINEMyLjkgNCAyIDQuOSAyIDZWMjBDMiAyMS4xIDIuOSAyMiA0IDIySDE4QzE5LjEgMjIgMjAgMjEuMSAyMCAyMFYxNUwxOCAxM1pNMTkuMyA4Ljg5QzE5Ljc0IDguMTkgMjAgNy4zOCAyMCA2LjVDMjAgNC4wMSAxNy45OSAyIDE1LjUgMkMxMy4wMSAyIDExIDQuMDEgMTEgNi41QzExIDguOTkgMTMuMDEgMTEgMTUuNDkgMTFDMTYuMzcgMTEgMTcuMTkgMTAuNzQgMTcuODggMTAuM0wyMSAxMy40MkwyMi40MiAxMkwxOS4zIDguODlaTTE1LjUgOUMxNC4xMiA5IDEzIDcuODggMTMgNi41QzEzIDUuMTIgMTQuMTIgNCAxNS41IDRDMTYuODggNCAxOCA1LjEyIDE4IDYuNUMxOCA3Ljg4IDE2Ljg4IDkgMTUuNSA5WiIvPgogICAgPHBhdGggZmlsbC1ydWxlPSJldmVub2RkIiBjbGlwLXJ1bGU9ImV2ZW5vZGQiIGQ9Ik00IDZIOS4wMTg5NEM5LjAwNjM5IDYuMTY1MDIgOSA2LjMzMTc2IDkgNi41QzkgOC44MTU3NyAxMC4yMTEgMTAuODQ4NyAxMi4wMzQzIDEySDlWMTRIMTZWMTIuOTgxMUMxNi41NzAzIDEyLjkzNzcgMTcuMTIgMTIuODIwNyAxNy42Mzk2IDEyLjYzOTZMMTggMTNWMjBINFY2Wk04IDhINlYxMEg4VjhaTTYgMTJIOFYxNEg2VjEyWk04IDE2SDZWMThIOFYxNlpNOSAxNkgxNlYxOEg5VjE2WiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-paste: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTE5IDJoLTQuMThDMTQuNC44NCAxMy4zIDAgMTIgMGMtMS4zIDAtMi40Ljg0LTIuODIgMkg1Yy0xLjEgMC0yIC45LTIgMnYxNmMwIDEuMS45IDIgMiAyaDE0YzEuMSAwIDItLjkgMi0yVjRjMC0xLjEtLjktMi0yLTJ6bS03IDBjLjU1IDAgMSAuNDUgMSAxcy0uNDUgMS0xIDEtMS0uNDUtMS0xIC40NS0xIDEtMXptNyAxOEg1VjRoMnYzaDEwVjRoMnYxNnoiLz4KICAgIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-pdf: url(data:image/svg+xml;base64,PHN2ZwogICB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyMiAyMiIgd2lkdGg9IjE2Ij4KICAgIDxwYXRoIHRyYW5zZm9ybT0icm90YXRlKDQ1KSIgY2xhc3M9ImpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iI0ZGMkEyQSIKICAgICAgIGQ9Im0gMjIuMzQ0MzY5LC0zLjAxNjM2NDIgaCA1LjYzODYwNCB2IDEuNTc5MjQzMyBoIC0zLjU0OTIyNyB2IDEuNTA4NjkyOTkgaCAzLjMzNzU3NiBWIDEuNjUwODE1NCBoIC0zLjMzNzU3NiB2IDMuNDM1MjYxMyBoIC0yLjA4OTM3NyB6IG0gLTcuMTM2NDQ0LDEuNTc5MjQzMyB2IDQuOTQzOTU0MyBoIDAuNzQ4OTIgcSAxLjI4MDc2MSwwIDEuOTUzNzAzLC0wLjYzNDk1MzUgMC42NzgzNjksLTAuNjM0OTUzNSAwLjY3ODM2OSwtMS44NDUxNjQxIDAsLTEuMjA0NzgzNTUgLTAuNjcyOTQyLC0xLjgzNDMxMDExIC0wLjY3Mjk0MiwtMC42Mjk1MjY1OSAtMS45NTkxMywtMC42Mjk1MjY1OSB6IG0gLTIuMDg5Mzc3LC0xLjU3OTI0MzMgaCAyLjIwMzM0MyBxIDEuODQ1MTY0LDAgMi43NDYwMzksMC4yNjU5MjA3IDAuOTA2MzAxLDAuMjYwNDkzNyAxLjU1MjEwOCwwLjg5MDAyMDMgMC41Njk4MywwLjU0ODEyMjMgMC44NDY2MDUsMS4yNjQ0ODAwNiAwLjI3Njc3NCwwLjcxNjM1NzgxIDAuMjc2Nzc0LDEuNjIyNjU4OTQgMCwwLjkxNzE1NTEgLTAuMjc2Nzc0LDEuNjM4OTM5OSAtMC4yNzY3NzUsMC43MTYzNTc4IC0wLjg0NjYwNSwxLjI2NDQ4IC0wLjY1MTIzNCwwLjYyOTUyNjYgLTEuNTYyOTYyLDAuODk1NDQ3MyAtMC45MTE3MjgsMC4yNjA0OTM3IC0yLjczNTE4NSwwLjI2MDQ5MzcgaCAtMi4yMDMzNDMgeiBtIC04LjE0NTg1NjUsMCBoIDMuNDY3ODIzIHEgMS41NDY2ODE2LDAgMi4zNzE1Nzg1LDAuNjg5MjIzIDAuODMwMzI0LDAuNjgzNzk2MSAwLjgzMDMyNCwxLjk1MzcwMzE0IDAsMS4yNzUzMzM5NyAtMC44MzAzMjQsMS45NjQ1NTcwNiBRIDkuOTg3MTk2MSwyLjI3NDkxNSA4LjQ0MDUxNDUsMi4yNzQ5MTUgSCA3LjA2MjA2ODQgViA1LjA4NjA3NjcgSCA0Ljk3MjY5MTUgWiBtIDIuMDg5Mzc2OSwxLjUxNDExOTkgdiAyLjI2MzAzOTQzIGggMS4xNTU5NDEgcSAwLjYwNzgxODgsMCAwLjkzODg2MjksLTAuMjkzMDU1NDcgMC4zMzEwNDQxLC0wLjI5ODQ4MjQxIDAuMzMxMDQ0MSwtMC44NDExNzc3MiAwLC0wLjU0MjY5NTMxIC0wLjMzMTA0NDEsLTAuODM1NzUwNzQgLTAuMzMxMDQ0MSwtMC4yOTMwNTU1IC0wLjkzODg2MjksLTAuMjkzMDU1NSB6IgovPgo8L3N2Zz4K);
  --jp-icon-python: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8ZyBjbGFzcz0ianAtaWNvbi1icmFuZDAganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjMEQ0N0ExIj4KICAgIDxwYXRoIGQ9Ik0xMS4xIDYuOVY1LjhINi45YzAtLjUgMC0xLjMuMi0xLjYuNC0uNy44LTEuMSAxLjctMS40IDEuNy0uMyAyLjUtLjMgMy45LS4xIDEgLjEgMS45LjkgMS45IDEuOXY0LjJjMCAuNS0uOSAxLjYtMiAxLjZIOC44Yy0xLjUgMC0yLjQgMS40LTIuNCAyLjh2Mi4ySDQuN0MzLjUgMTUuMSAzIDE0IDMgMTMuMVY5Yy0uMS0xIC42LTIgMS44LTIgMS41LS4xIDYuMy0uMSA2LjMtLjF6Ii8+CiAgICA8cGF0aCBkPSJNMTAuOSAxNS4xdjEuMWg0LjJjMCAuNSAwIDEuMy0uMiAxLjYtLjQuNy0uOCAxLjEtMS43IDEuNC0xLjcuMy0yLjUuMy0zLjkuMS0xLS4xLTEuOS0uOS0xLjktMS45di00LjJjMC0uNS45LTEuNiAyLTEuNmgzLjhjMS41IDAgMi40LTEuNCAyLjQtMi44VjYuNmgxLjdDMTguNSA2LjkgMTkgOCAxOSA4LjlWMTNjMCAxLS43IDIuMS0xLjkgMi4xaC02LjJ6Ii8+CiAgPC9nPgo8L3N2Zz4K);
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
  --jp-icon-spreadsheet: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1jb250cmFzdDEganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNENBRjUwIiBkPSJNMi4yIDIuMnYxNy42aDE3LjZWMi4ySDIuMnptMTUuNCA3LjdoLTUuNVY0LjRoNS41djUuNXpNOS45IDQuNHY1LjVINC40VjQuNGg1LjV6bS01LjUgNy43aDUuNXY1LjVINC40di01LjV6bTcuNyA1LjV2LTUuNWg1LjV2NS41aC01LjV6Ii8+Cjwvc3ZnPgo=);
  --jp-icon-stop: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTAgMGgyNHYyNEgweiIgZmlsbD0ibm9uZSIvPgogICAgICAgIDxwYXRoIGQ9Ik02IDZoMTJ2MTJINnoiLz4KICAgIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-tab: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTIxIDNIM2MtMS4xIDAtMiAuOS0yIDJ2MTRjMCAxLjEuOSAyIDIgMmgxOGMxLjEgMCAyLS45IDItMlY1YzAtMS4xLS45LTItMi0yem0wIDE2SDNWNWgxMHY0aDh2MTB6Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-table-rows: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTAgMGgyNHYyNEgweiIgZmlsbD0ibm9uZSIvPgogICAgICAgIDxwYXRoIGQ9Ik0yMSw4SDNWNGgxOFY4eiBNMjEsMTBIM3Y0aDE4VjEweiBNMjEsMTZIM3Y0aDE4VjE2eiIvPgogICAgPC9nPgo8L3N2Zz4=);
  --jp-icon-tag: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjgiIGhlaWdodD0iMjgiIHZpZXdCb3g9IjAgMCA0MyAyOCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CgkJPHBhdGggZD0iTTI4LjgzMzIgMTIuMzM0TDMyLjk5OTggMTYuNTAwN0wzNy4xNjY1IDEyLjMzNEgyOC44MzMyWiIvPgoJCTxwYXRoIGQ9Ik0xNi4yMDk1IDIxLjYxMDRDMTUuNjg3MyAyMi4xMjk5IDE0Ljg0NDMgMjIuMTI5OSAxNC4zMjQ4IDIxLjYxMDRMNi45ODI5IDE0LjcyNDVDNi41NzI0IDE0LjMzOTQgNi4wODMxMyAxMy42MDk4IDYuMDQ3ODYgMTMuMDQ4MkM1Ljk1MzQ3IDExLjUyODggNi4wMjAwMiA4LjYxOTQ0IDYuMDY2MjEgNy4wNzY5NUM2LjA4MjgxIDYuNTE0NzcgNi41NTU0OCA2LjA0MzQ3IDcuMTE4MDQgNi4wMzA1NUM5LjA4ODYzIDUuOTg0NzMgMTMuMjYzOCA1LjkzNTc5IDEzLjY1MTggNi4zMjQyNUwyMS43MzY5IDEzLjYzOUMyMi4yNTYgMTQuMTU4NSAyMS43ODUxIDE1LjQ3MjQgMjEuMjYyIDE1Ljk5NDZMMTYuMjA5NSAyMS42MTA0Wk05Ljc3NTg1IDguMjY1QzkuMzM1NTEgNy44MjU2NiA4LjYyMzUxIDcuODI1NjYgOC4xODI4IDguMjY1QzcuNzQzNDYgOC43MDU3MSA3Ljc0MzQ2IDkuNDE3MzMgOC4xODI4IDkuODU2NjdDOC42MjM4MiAxMC4yOTY0IDkuMzM1ODIgMTAuMjk2NCA5Ljc3NTg1IDkuODU2NjdDMTAuMjE1NiA5LjQxNzMzIDEwLjIxNTYgOC43MDUzMyA5Ljc3NTg1IDguMjY1WiIvPgoJPC9nPgo8L3N2Zz4K);
  --jp-icon-terminal: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0IiA+CiAgICA8cmVjdCBjbGFzcz0ianAtaWNvbjIganAtaWNvbi1zZWxlY3RhYmxlIiB3aWR0aD0iMjAiIGhlaWdodD0iMjAiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDIgMikiIGZpbGw9IiMzMzMzMzMiLz4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uLWFjY2VudDIganAtaWNvbi1zZWxlY3RhYmxlLWludmVyc2UiIGQ9Ik01LjA1NjY0IDguNzYxNzJDNS4wNTY2NCA4LjU5NzY2IDUuMDMxMjUgOC40NTMxMiA0Ljk4MDQ3IDguMzI4MTJDNC45MzM1OSA4LjE5OTIyIDQuODU1NDcgOC4wODIwMyA0Ljc0NjA5IDcuOTc2NTZDNC42NDA2MiA3Ljg3MTA5IDQuNSA3Ljc3NTM5IDQuMzI0MjIgNy42ODk0NUM0LjE1MjM0IDcuNTk5NjEgMy45NDMzNiA3LjUxMTcyIDMuNjk3MjcgNy40MjU3OEMzLjMwMjczIDcuMjg1MTYgMi45NDMzNiA3LjEzNjcyIDIuNjE5MTQgNi45ODA0N0MyLjI5NDkyIDYuODI0MjIgMi4wMTc1OCA2LjY0MjU4IDEuNzg3MTEgNi40MzU1NUMxLjU2MDU1IDYuMjI4NTIgMS4zODQ3NyA1Ljk4ODI4IDEuMjU5NzcgNS43MTQ4NEMxLjEzNDc3IDUuNDM3NSAxLjA3MjI3IDUuMTA5MzggMS4wNzIyNyA0LjczMDQ3QzEuMDcyMjcgNC4zOTg0NCAxLjEyODkxIDQuMDk1NyAxLjI0MjE5IDMuODIyMjdDMS4zNTU0NyAzLjU0NDkyIDEuNTE1NjIgMy4zMDQ2OSAxLjcyMjY2IDMuMTAxNTZDMS45Mjk2OSAyLjg5ODQ0IDIuMTc5NjkgMi43MzQzNyAyLjQ3MjY2IDIuNjA5MzhDMi43NjU2MiAyLjQ4NDM4IDMuMDkxOCAyLjQwNDMgMy40NTExNyAyLjM2OTE0VjEuMTA5MzhINC4zODg2N1YyLjM4MDg2QzQuNzQwMjMgMi40Mjc3MyA1LjA1NjY0IDIuNTIzNDQgNS4zMzc4OSAyLjY2Nzk3QzUuNjE5MTQgMi44MTI1IDUuODU3NDIgMy4wMDE5NSA2LjA1MjczIDMuMjM2MzNDNi4yNTE5NSAzLjQ2NjggNi40MDQzIDMuNzQwMjMgNi41MDk3NyA0LjA1NjY0QzYuNjE5MTQgNC4zNjkxNCA2LjY3MzgzIDQuNzIwNyA2LjY3MzgzIDUuMTExMzNINS4wNDQ5MkM1LjA0NDkyIDQuNjM4NjcgNC45Mzc1IDQuMjgxMjUgNC43MjI2NiA0LjAzOTA2QzQuNTA3ODEgMy43OTI5NyA0LjIxNjggMy42Njk5MiAzLjg0OTYxIDMuNjY5OTJDMy42NTAzOSAzLjY2OTkyIDMuNDc2NTYgMy42OTcyNyAzLjMyODEyIDMuNzUxOTVDMy4xODM1OSAzLjgwMjczIDMuMDY0NDUgMy44NzY5NSAyLjk3MDcgMy45NzQ2MUMyLjg3Njk1IDQuMDY4MzYgMi44MDY2NCA0LjE3OTY5IDIuNzU5NzcgNC4zMDg1OUMyLjcxNjggNC40Mzc1IDIuNjk1MzEgNC41NzgxMiAyLjY5NTMxIDQuNzMwNDdDMi42OTUzMSA0Ljg4MjgxIDIuNzE2OCA1LjAxOTUzIDIuNzU5NzcgNS4xNDA2MkMyLjgwNjY0IDUuMjU3ODEgMi44ODI4MSA1LjM2NzE5IDIuOTg4MjggNS40Njg3NUMzLjA5NzY2IDUuNTcwMzEgMy4yNDAyMyA1LjY2Nzk3IDMuNDE2MDIgNS43NjE3MkMzLjU5MTggNS44NTE1NiAzLjgxMDU1IDUuOTQzMzYgNC4wNzIyNyA2LjAzNzExQzQuNDY2OCA2LjE4NTU1IDQuODI0MjIgNi4zMzk4NCA1LjE0NDUzIDYuNUM1LjQ2NDg0IDYuNjU2MjUgNS43MzgyOCA2LjgzOTg0IDUuOTY0ODQgNy4wNTA3OEM2LjE5NTMxIDcuMjU3ODEgNi4zNzEwOSA3LjUgNi40OTIxOSA3Ljc3NzM0QzYuNjE3MTkgOC4wNTA3OCA2LjY3OTY5IDguMzc1IDYuNjc5NjkgOC43NUM2LjY3OTY5IDkuMDkzNzUgNi42MjMwNSA5LjQwNDMgNi41MDk3NyA5LjY4MTY0QzYuMzk2NDggOS45NTUwOCA2LjIzNDM4IDEwLjE5MTQgNi4wMjM0NCAxMC4zOTA2QzUuODEyNSAxMC41ODk4IDUuNTU4NTkgMTAuNzUgNS4yNjE3MiAxMC44NzExQzQuOTY0ODQgMTAuOTg4MyA0LjYzMjgxIDExLjA2NDUgNC4yNjU2MiAxMS4wOTk2VjEyLjI0OEgzLjMzMzk4VjExLjA5OTZDMy4wMDE5NSAxMS4wNjg0IDIuNjc5NjkgMTAuOTk2MSAyLjM2NzE5IDEwLjg4MjhDMi4wNTQ2OSAxMC43NjU2IDEuNzc3MzQgMTAuNTk3NyAxLjUzNTE2IDEwLjM3ODlDMS4yOTY4OCAxMC4xNjAyIDEuMTA1NDcgOS44ODQ3NyAwLjk2MDkzOCA5LjU1MjczQzAuODE2NDA2IDkuMjE2OCAwLjc0NDE0MSA4LjgxNDQ1IDAuNzQ0MTQxIDguMzQ1N0gyLjM3ODkxQzIuMzc4OTEgOC42MjY5NSAyLjQxOTkyIDguODYzMjggMi41MDE5NSA5LjA1NDY5QzIuNTgzOTggOS4yNDIxOSAyLjY4OTQ1IDkuMzkyNTggMi44MTgzNiA5LjUwNTg2QzIuOTUxMTcgOS42MTUyMyAzLjEwMTU2IDkuNjkzMzYgMy4yNjk1MyA5Ljc0MDIzQzMuNDM3NSA5Ljc4NzExIDMuNjA5MzggOS44MTA1NSAzLjc4NTE2IDkuODEwNTVDNC4yMDMxMiA5LjgxMDU1IDQuNTE5NTMgOS43MTI4OSA0LjczNDM4IDkuNTE3NThDNC45NDkyMiA5LjMyMjI3IDUuMDU2NjQgOS4wNzAzMSA1LjA1NjY0IDguNzYxNzJaTTEzLjQxOCAxMi4yNzE1SDguMDc0MjJWMTFIMTMuNDE4VjEyLjI3MTVaIiB0cmFuc2Zvcm09InRyYW5zbGF0ZSgzLjk1MjY0IDYpIiBmaWxsPSJ3aGl0ZSIvPgo8L3N2Zz4K);
  --jp-icon-text-editor: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMTUgMTVIM3YyaDEydi0yem0wLThIM3YyaDEyVjd6TTMgMTNoMTh2LTJIM3Yyem0wIDhoMTh2LTJIM3Yyek0zIDN2MmgxOFYzSDN6Ii8+Cjwvc3ZnPgo=);
  --jp-icon-toc: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIj4KICAgIDxwYXRoIGQ9Ik03LDVIMjFWN0g3VjVNNywxM1YxMUgyMVYxM0g3TTQsNC41QTEuNSwxLjUgMCAwLDEgNS41LDZBMS41LDEuNSAwIDAsMSA0LDcuNUExLjUsMS41IDAgMCwxIDIuNSw2QTEuNSwxLjUgMCAwLDEgNCw0LjVNNCwxMC41QTEuNSwxLjUgMCAwLDEgNS41LDEyQTEuNSwxLjUgMCAwLDEgNCwxMy41QTEuNSwxLjUgMCAwLDEgMi41LDEyQTEuNSwxLjUgMCAwLDEgNCwxMC41TTcsMTlWMTdIMjFWMTlIN000LDE2LjVBMS41LDEuNSAwIDAsMSA1LjUsMThBMS41LDEuNSAwIDAsMSA0LDE5LjVBMS41LDEuNSAwIDAsMSAyLjUsMThBMS41LDEuNSAwIDAsMSA0LDE2LjVaIiAvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-tree-view: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTAgMGgyNHYyNEgweiIgZmlsbD0ibm9uZSIvPgogICAgICAgIDxwYXRoIGQ9Ik0yMiAxMVYzaC03djNIOVYzSDJ2OGg3VjhoMnYxMGg0djNoN3YtOGgtN3YzaC0yVjhoMnYzeiIvPgogICAgPC9nPgo8L3N2Zz4=);
  --jp-icon-trusted: url(data:image/svg+xml;base64,PHN2ZyBmaWxsPSJub25lIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI1Ij4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiIgc3Ryb2tlPSIjMzMzMzMzIiBzdHJva2Utd2lkdGg9IjIiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDIgMykiIGQ9Ik0xLjg2MDk0IDExLjQ0MDlDMC44MjY0NDggOC43NzAyNyAwLjg2Mzc3OSA2LjA1NzY0IDEuMjQ5MDcgNC4xOTkzMkMyLjQ4MjA2IDMuOTMzNDcgNC4wODA2OCAzLjQwMzQ3IDUuNjAxMDIgMi44NDQ5QzcuMjM1NDkgMi4yNDQ0IDguODU2NjYgMS41ODE1IDkuOTg3NiAxLjA5NTM5QzExLjA1OTcgMS41ODM0MSAxMi42MDk0IDIuMjQ0NCAxNC4yMTggMi44NDMzOUMxNS43NTAzIDMuNDEzOTQgMTcuMzk5NSAzLjk1MjU4IDE4Ljc1MzkgNC4yMTM4NUMxOS4xMzY0IDYuMDcxNzcgMTkuMTcwOSA4Ljc3NzIyIDE4LjEzOSAxMS40NDA5QzE3LjAzMDMgMTQuMzAzMiAxNC42NjY4IDE3LjE4NDQgOS45OTk5OSAxOC45MzU0QzUuMzMzMiAxNy4xODQ0IDIuOTY5NjggMTQuMzAzMiAxLjg2MDk0IDExLjQ0MDlaIi8+CiAgICA8cGF0aCBjbGFzcz0ianAtaWNvbjIiIGZpbGw9IiMzMzMzMzMiIHN0cm9rZT0iIzMzMzMzMyIgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoOCA5Ljg2NzE5KSIgZD0iTTIuODYwMTUgNC44NjUzNUwwLjcyNjU0OSAyLjk5OTU5TDAgMy42MzA0NUwyLjg2MDE1IDYuMTMxNTdMOCAwLjYzMDg3Mkw3LjI3ODU3IDBMMi44NjAxNSA0Ljg2NTM1WiIvPgo8L3N2Zz4K);
  --jp-icon-undo: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTEyLjUgOGMtMi42NSAwLTUuMDUuOTktNi45IDIuNkwyIDd2OWg5bC0zLjYyLTMuNjJjMS4zOS0xLjE2IDMuMTYtMS44OCA1LjEyLTEuODggMy41NCAwIDYuNTUgMi4zMSA3LjYgNS41bDIuMzctLjc4QzIxLjA4IDExLjAzIDE3LjE1IDggMTIuNSA4eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-vega: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8ZyBjbGFzcz0ianAtaWNvbjEganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjMjEyMTIxIj4KICAgIDxwYXRoIGQ9Ik0xMC42IDUuNGwyLjItMy4ySDIuMnY3LjNsNC02LjZ6Ii8+CiAgICA8cGF0aCBkPSJNMTUuOCAyLjJsLTQuNCA2LjZMNyA2LjNsLTQuOCA4djUuNWgxNy42VjIuMmgtNHptLTcgMTUuNEg1LjV2LTQuNGgzLjN2NC40em00LjQgMEg5LjhWOS44aDMuNHY3Ljh6bTQuNCAwaC0zLjRWNi41aDMuNHYxMS4xeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-yaml: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8ZyBjbGFzcz0ianAtaWNvbi1jb250cmFzdDIganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjRDgxQjYwIj4KICAgIDxwYXRoIGQ9Ik03LjIgMTguNnYtNS40TDMgNS42aDMuM2wxLjQgMy4xYy4zLjkuNiAxLjYgMSAyLjUuMy0uOC42LTEuNiAxLTIuNWwxLjQtMy4xaDMuNGwtNC40IDcuNnY1LjVsLTIuOS0uMXoiLz4KICAgIDxjaXJjbGUgY2xhc3M9InN0MCIgY3g9IjE3LjYiIGN5PSIxNi41IiByPSIyLjEiLz4KICAgIDxjaXJjbGUgY2xhc3M9InN0MCIgY3g9IjE3LjYiIGN5PSIxMSIgcj0iMi4xIi8+CiAgPC9nPgo8L3N2Zz4K);
}

/* Icon CSS class declarations */

.jp-AddIcon {
  background-image: var(--jp-icon-add);
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
.jp-CodeIcon {
  background-image: var(--jp-icon-code);
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
.jp-DownloadIcon {
  background-image: var(--jp-icon-download);
}
.jp-EditIcon {
  background-image: var(--jp-icon-edit);
}
.jp-EllipsesIcon {
  background-image: var(--jp-icon-ellipses);
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
.jp-FilterListIcon {
  background-image: var(--jp-icon-filter-list);
}
.jp-FolderIcon {
  background-image: var(--jp-icon-folder);
}
.jp-Html5Icon {
  background-image: var(--jp-icon-html5);
}
.jp-ImageIcon {
  background-image: var(--jp-icon-image);
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
.jp-ListingsInfoIcon {
  background-image: var(--jp-icon-listings-info);
}
.jp-MarkdownIcon {
  background-image: var(--jp-icon-markdown);
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
.jp-VegaIcon {
  background-image: var(--jp-icon-vega);
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

/* CSS for icons in selected items in the settings editor */
#setting-editor .jp-PluginList .jp-mod-selected .jp-icon-selectable[fill] {
  fill: #fff;
}
#setting-editor
  .jp-PluginList
  .jp-mod-selected
  .jp-icon-selectable-inverse[fill] {
  fill: var(--jp-brand-color1);
}

/* CSS for icons in selected filebrowser listing items */
.jp-DirListing-item.jp-mod-selected .jp-icon-selectable[fill] {
  fill: #fff;
}
.jp-DirListing-item.jp-mod-selected .jp-icon-selectable-inverse[fill] {
  fill: var(--jp-brand-color1);
}

/* CSS for icons in selected tabs in the sidebar tab manager */
#tab-manager .lm-TabBar-tab.jp-mod-active .jp-icon-selectable[fill] {
  fill: #fff;
}

#tab-manager .lm-TabBar-tab.jp-mod-active .jp-icon-selectable-inverse[fill] {
  fill: var(--jp-brand-color1);
}
#tab-manager
  .lm-TabBar-tab.jp-mod-active
  .jp-icon-hover
  :hover
  .jp-icon-selectable[fill] {
  fill: var(--jp-brand-color1);
}

#tab-manager
  .lm-TabBar-tab.jp-mod-active
  .jp-icon-hover
  :hover
  .jp-icon-selectable-inverse[fill] {
  fill: #fff;
}

/**
 * TODO: come up with non css-hack solution for showing the busy icon on top
 *  of the close icon
 * CSS for complex behavior of close icon of tabs in the sidebar tab manager
 */
#tab-manager
  .lm-TabBar-tab.jp-mod-dirty
  > .lm-TabBar-tabCloseIcon
  > :not(:hover)
  > .jp-icon3[fill] {
  fill: none;
}
#tab-manager
  .lm-TabBar-tab.jp-mod-dirty
  > .lm-TabBar-tabCloseIcon
  > :not(:hover)
  > .jp-icon-busy[fill] {
  fill: var(--jp-inverse-layout-color3);
}

#tab-manager
  .lm-TabBar-tab.jp-mod-dirty.jp-mod-active
  > .lm-TabBar-tabCloseIcon
  > :not(:hover)
  > .jp-icon-busy[fill] {
  fill: #fff;
}

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

.jp-icon-hoverShow:not(:hover) svg {
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
}

.jp-switch-track {
  cursor: pointer;
  background-color: var(--jp-border-color1);
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
  left: 0px;
  background-color: var(--jp-ui-inverse-font-color1);
  -webkit-transition: 0.4s;
  transition: 0.4s;
  border-radius: 50%;
}

.jp-switch[aria-checked='true'] .jp-switch-track {
  background-color: var(--jp-warn-color0);
}

.jp-switch[aria-checked='true'] .jp-switch-track::before {
  /* track width (35) - margins (3 + 3) - thumb width (10) */
  left: 19px;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/* Sibling imports */

/* Override Blueprint's _reset.scss styles */
html {
  box-sizing: unset;
}

*,
*::before,
*::after {
  box-sizing: unset;
}

body {
  color: unset;
  font-family: var(--jp-ui-font-family);
}

p {
  margin-top: unset;
  margin-bottom: unset;
}

small {
  font-size: unset;
}

strong {
  font-weight: unset;
}

/* Override Blueprint's _typography.scss styles */
a {
  text-decoration: unset;
  color: unset;
}
a:hover {
  text-decoration: unset;
  color: unset;
}

/* Override Blueprint's _accessibility.scss styles */
:focus {
  outline: unset;
  outline-offset: unset;
  -moz-outline-radius: unset;
}

/* Styles for ui-components */
.jp-Button {
  border-radius: var(--jp-border-radius);
  padding: 0px 12px;
  font-size: var(--jp-ui-font-size1);
}

/* Use our own theme for hover styles */
button.jp-Button.bp3-button.bp3-minimal:hover {
  background-color: var(--jp-layout-color2);
}
.jp-Button.minimal {
  color: unset !important;
}

.jp-Button.jp-ToolbarButtonComponent {
  text-transform: none;
}

.jp-InputGroup input {
  box-sizing: border-box;
  border-radius: 0;
  background-color: transparent;
  color: var(--jp-ui-font-color0);
  box-shadow: inset 0 0 0 var(--jp-border-width) var(--jp-input-border-color);
}

.jp-InputGroup input:focus {
  box-shadow: inset 0 0 0 var(--jp-border-width)
      var(--jp-input-active-box-shadow-color),
    inset 0 0 0 3px var(--jp-input-active-box-shadow-color);
}

.jp-InputGroup input::placeholder,
input::placeholder {
  color: var(--jp-ui-font-color3);
}

.jp-BPIcon {
  display: inline-block;
  vertical-align: middle;
  margin: auto;
}

/* Stop blueprint futzing with our icon fills */
.bp3-icon.jp-BPIcon > svg:not([fill]) {
  fill: var(--jp-inverse-layout-color3);
}

.jp-InputGroupAction {
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
  height: 24px;
  line-height: 14px;
  padding: 0 25px 0 10px;
  text-align: left;
  -moz-appearance: none;
  -webkit-appearance: none;
}

/* Use our own theme for hover and option styles */
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

.jp-Collapse {
  display: flex;
  flex-direction: column;
  align-items: stretch;
  border-top: 1px solid var(--jp-border-color2);
  border-bottom: 1px solid var(--jp-border-color2);
}

.jp-Collapse-header {
  padding: 1px 12px;
  color: var(--jp-ui-font-color1);
  background-color: var(--jp-layout-color1);
  font-size: var(--jp-ui-font-size2);
}

.jp-Collapse-header:hover {
  background-color: var(--jp-layout-color2);
}

.jp-Collapse-contents {
  padding: 0px 12px 0px 12px;
  background-color: var(--jp-layout-color1);
  color: var(--jp-ui-font-color1);
  overflow: auto;
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
  padding-bottom: 0px;
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
  padding: 0px 9px;
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
  padding: 5px 5px 1px 5px;
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
  margin-top: 0px;
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

.lm-CommandPalette-item.lm-mod-active .lm-CommandPalette-itemLabel > mark {
  color: var(--jp-ui-inverse-font-color0);
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

.lm-CommandPalette-content:empty:after {
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
  padding: 0px 8px;
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
  top: 0px;
  left: 0px;
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
  padding: 24px;
  padding-bottom: 12px;
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

.jp-Dialog-button {
  overflow: visible;
}

button.jp-Dialog-button:focus {
  outline: 1px solid var(--jp-brand-color1);
  outline-offset: 4px;
  -moz-outline-radius: 0px;
}

button.jp-Dialog-button:focus::-moz-focus-inner {
  border: 0;
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
  color: var(--jp-ui-font-color0);
}

.jp-Dialog-body {
  display: flex;
  flex-direction: column;
  flex: 1 1 auto;
  font-size: var(--jp-ui-font-size1);
  background: var(--jp-layout-color1);
  overflow: auto;
}

.jp-Dialog-footer {
  display: flex;
  flex-direction: row;
  justify-content: flex-end;
  flex: 0 0 auto;
  margin-left: -12px;
  margin-right: -12px;
  padding: 12px;
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
  padding: 0px 16px;
}

.jp-Dialog-body > label {
  line-height: 1.4;
  color: var(--jp-ui-font-color0);
}

.jp-Dialog-button.jp-mod-styled:not(:last-child) {
  margin-right: 12px;
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2014-2016, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-HoverBox {
  position: fixed;
}

.jp-HoverBox.jp-mod-outofview {
  display: none;
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
When drag events occur, `p-mod-override-cursor` is added to the body.
Because iframes steal all cursor events, the following two rules are necessary
to suppress pointer events while resize drags are occurring. There may be a
better solution to this problem.
*/
body.lm-mod-override-cursor .jp-IFrame {
  position: relative;
}

body.lm-mod-override-cursor .jp-IFrame:before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: transparent;
}

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
  --md-purple-A700: #aa00ff;

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
  --md-yellow-A200: #ffff00;
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
  --md-grey-200: #eeeeee;
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

.jp-SpinnerContent:before {
  width: 50%;
  height: 50%;
  background: #f37626;
  border-radius: 100% 0 0 0;
  position: absolute;
  top: 0;
  left: 0;
  content: '';
}

.jp-SpinnerContent:after {
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
  padding: 0px 12px;
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

.jp-FileDialog-Checkbox {
  margin-top: 35px;
  display: flex;
  flex-direction: row;
  align-items: end;
  width: 100%;
}

.jp-FileDialog-Checkbox > label {
  flex: 1 1 auto;
}

.jp-select-wrapper {
  display: flex;
  position: relative;
  flex-direction: column;
  padding: 1px;
  background-color: var(--jp-layout-color1);
  height: 28px;
  box-sizing: border-box;
  margin-bottom: 12px;
}

.jp-select-wrapper.jp-mod-focused select.jp-mod-styled {
  border: var(--jp-border-width) solid var(--jp-input-active-border-color);
  box-shadow: var(--jp-input-box-shadow);
  background-color: var(--jp-input-active-background);
}

select.jp-mod-styled:hover {
  background-color: var(--jp-layout-color1);
  cursor: pointer;
  color: var(--jp-ui-font-color0);
  background-color: var(--jp-input-hover-background);
  box-shadow: inset 0 0px 1px rgba(0, 0, 0, 0.5);
}

select.jp-mod-styled {
  flex: 1 1 auto;
  height: 32px;
  width: 100%;
  font-size: var(--jp-ui-font-size2);
  background: var(--jp-input-background);
  color: var(--jp-ui-font-color0);
  padding: 0 25px 0 8px;
  border: var(--jp-border-width) solid var(--jp-input-border-color);
  border-radius: 0px;
  outline: none;
  appearance: none;
  -webkit-appearance: none;
  -moz-appearance: none;
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
  z-index: 1;
  overflow-x: auto;
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
  padding: 0px;
  margin: 0px;
}

button.jp-ToolbarButtonComponent {
  background: var(--jp-layout-color1);
  border: none;
  box-sizing: border-box;
  outline: none;
  appearance: none;
  -webkit-appearance: none;
  -moz-appearance: none;
  padding: 0px 6px;
  margin: 0px;
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

button.jp-ToolbarButtonComponent span {
  padding: 0px;
  flex: 0 0 auto;
}

button.jp-ToolbarButtonComponent .jp-ToolbarButtonComponent-label {
  font-size: var(--jp-ui-font-size1);
  line-height: 100%;
  padding-left: 2px;
  color: var(--jp-ui-font-color1);
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

/*-----------------------------------------------------------------------------
| Copyright (c) 2014-2017, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/


/* <DEPRECATED> */ body.p-mod-override-cursor *, /* </DEPRECATED> */
body.lm-mod-override-cursor * {
  cursor: inherit !important;
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
  border-radius: 0px;
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

/* BASICS */

.CodeMirror {
  /* Set height, width, borders, and global font properties here */
  font-family: monospace;
  height: 300px;
  color: black;
  direction: ltr;
}

/* PADDING */

.CodeMirror-lines {
  padding: 4px 0; /* Vertical padding around content */
}
.CodeMirror pre.CodeMirror-line,
.CodeMirror pre.CodeMirror-line-like {
  padding: 0 4px; /* Horizontal padding of content */
}

.CodeMirror-scrollbar-filler, .CodeMirror-gutter-filler {
  background-color: white; /* The little square between H and V scrollbars */
}

/* GUTTER */

.CodeMirror-gutters {
  border-right: 1px solid #ddd;
  background-color: #f7f7f7;
  white-space: nowrap;
}
.CodeMirror-linenumbers {}
.CodeMirror-linenumber {
  padding: 0 3px 0 5px;
  min-width: 20px;
  text-align: right;
  color: #999;
  white-space: nowrap;
}

.CodeMirror-guttermarker { color: black; }
.CodeMirror-guttermarker-subtle { color: #999; }

/* CURSOR */

.CodeMirror-cursor {
  border-left: 1px solid black;
  border-right: none;
  width: 0;
}
/* Shown when moving in bi-directional text */
.CodeMirror div.CodeMirror-secondarycursor {
  border-left: 1px solid silver;
}
.cm-fat-cursor .CodeMirror-cursor {
  width: auto;
  border: 0 !important;
  background: #7e7;
}
.cm-fat-cursor div.CodeMirror-cursors {
  z-index: 1;
}
.cm-fat-cursor-mark {
  background-color: rgba(20, 255, 20, 0.5);
  -webkit-animation: blink 1.06s steps(1) infinite;
  -moz-animation: blink 1.06s steps(1) infinite;
  animation: blink 1.06s steps(1) infinite;
}
.cm-animate-fat-cursor {
  width: auto;
  border: 0;
  -webkit-animation: blink 1.06s steps(1) infinite;
  -moz-animation: blink 1.06s steps(1) infinite;
  animation: blink 1.06s steps(1) infinite;
  background-color: #7e7;
}
@-moz-keyframes blink {
  0% {}
  50% { background-color: transparent; }
  100% {}
}
@-webkit-keyframes blink {
  0% {}
  50% { background-color: transparent; }
  100% {}
}
@keyframes blink {
  0% {}
  50% { background-color: transparent; }
  100% {}
}

/* Can style cursor different in overwrite (non-insert) mode */
.CodeMirror-overwrite .CodeMirror-cursor {}

.cm-tab { display: inline-block; text-decoration: inherit; }

.CodeMirror-rulers {
  position: absolute;
  left: 0; right: 0; top: -50px; bottom: 0;
  overflow: hidden;
}
.CodeMirror-ruler {
  border-left: 1px solid #ccc;
  top: 0; bottom: 0;
  position: absolute;
}

/* DEFAULT THEME */

.cm-s-default .cm-header {color: blue;}
.cm-s-default .cm-quote {color: #090;}
.cm-negative {color: #d44;}
.cm-positive {color: #292;}
.cm-header, .cm-strong {font-weight: bold;}
.cm-em {font-style: italic;}
.cm-link {text-decoration: underline;}
.cm-strikethrough {text-decoration: line-through;}

.cm-s-default .cm-keyword {color: #708;}
.cm-s-default .cm-atom {color: #219;}
.cm-s-default .cm-number {color: #164;}
.cm-s-default .cm-def {color: #00f;}
.cm-s-default .cm-variable,
.cm-s-default .cm-punctuation,
.cm-s-default .cm-property,
.cm-s-default .cm-operator {}
.cm-s-default .cm-variable-2 {color: #05a;}
.cm-s-default .cm-variable-3, .cm-s-default .cm-type {color: #085;}
.cm-s-default .cm-comment {color: #a50;}
.cm-s-default .cm-string {color: #a11;}
.cm-s-default .cm-string-2 {color: #f50;}
.cm-s-default .cm-meta {color: #555;}
.cm-s-default .cm-qualifier {color: #555;}
.cm-s-default .cm-builtin {color: #30a;}
.cm-s-default .cm-bracket {color: #997;}
.cm-s-default .cm-tag {color: #170;}
.cm-s-default .cm-attribute {color: #00c;}
.cm-s-default .cm-hr {color: #999;}
.cm-s-default .cm-link {color: #00c;}

.cm-s-default .cm-error {color: #f00;}
.cm-invalidchar {color: #f00;}

.CodeMirror-composing { border-bottom: 2px solid; }

/* Default styles for common addons */

div.CodeMirror span.CodeMirror-matchingbracket {color: #0b0;}
div.CodeMirror span.CodeMirror-nonmatchingbracket {color: #a22;}
.CodeMirror-matchingtag { background: rgba(255, 150, 0, .3); }
.CodeMirror-activeline-background {background: #e8f2ff;}

/* STOP */

/* The rest of this file contains styles related to the mechanics of
   the editor. You probably shouldn't touch them. */

.CodeMirror {
  position: relative;
  overflow: hidden;
  background: white;
}

.CodeMirror-scroll {
  overflow: scroll !important; /* Things will break if this is overridden */
  /* 50px is the magic margin used to hide the element's real scrollbars */
  /* See overflow: hidden in .CodeMirror */
  margin-bottom: -50px; margin-right: -50px;
  padding-bottom: 50px;
  height: 100%;
  outline: none; /* Prevent dragging from highlighting the element */
  position: relative;
}
.CodeMirror-sizer {
  position: relative;
  border-right: 50px solid transparent;
}

/* The fake, visible scrollbars. Used to force redraw during scrolling
   before actual scrolling happens, thus preventing shaking and
   flickering artifacts. */
.CodeMirror-vscrollbar, .CodeMirror-hscrollbar, .CodeMirror-scrollbar-filler, .CodeMirror-gutter-filler {
  position: absolute;
  z-index: 6;
  display: none;
  outline: none;
}
.CodeMirror-vscrollbar {
  right: 0; top: 0;
  overflow-x: hidden;
  overflow-y: scroll;
}
.CodeMirror-hscrollbar {
  bottom: 0; left: 0;
  overflow-y: hidden;
  overflow-x: scroll;
}
.CodeMirror-scrollbar-filler {
  right: 0; bottom: 0;
}
.CodeMirror-gutter-filler {
  left: 0; bottom: 0;
}

.CodeMirror-gutters {
  position: absolute; left: 0; top: 0;
  min-height: 100%;
  z-index: 3;
}
.CodeMirror-gutter {
  white-space: normal;
  height: 100%;
  display: inline-block;
  vertical-align: top;
  margin-bottom: -50px;
}
.CodeMirror-gutter-wrapper {
  position: absolute;
  z-index: 4;
  background: none !important;
  border: none !important;
}
.CodeMirror-gutter-background {
  position: absolute;
  top: 0; bottom: 0;
  z-index: 4;
}
.CodeMirror-gutter-elt {
  position: absolute;
  cursor: default;
  z-index: 4;
}
.CodeMirror-gutter-wrapper ::selection { background-color: transparent }
.CodeMirror-gutter-wrapper ::-moz-selection { background-color: transparent }

.CodeMirror-lines {
  cursor: text;
  min-height: 1px; /* prevents collapsing before first draw */
}
.CodeMirror pre.CodeMirror-line,
.CodeMirror pre.CodeMirror-line-like {
  /* Reset some styles that the rest of the page might have set */
  -moz-border-radius: 0; -webkit-border-radius: 0; border-radius: 0;
  border-width: 0;
  background: transparent;
  font-family: inherit;
  font-size: inherit;
  margin: 0;
  white-space: pre;
  word-wrap: normal;
  line-height: inherit;
  color: inherit;
  z-index: 2;
  position: relative;
  overflow: visible;
  -webkit-tap-highlight-color: transparent;
  -webkit-font-variant-ligatures: contextual;
  font-variant-ligatures: contextual;
}
.CodeMirror-wrap pre.CodeMirror-line,
.CodeMirror-wrap pre.CodeMirror-line-like {
  word-wrap: break-word;
  white-space: pre-wrap;
  word-break: normal;
}

.CodeMirror-linebackground {
  position: absolute;
  left: 0; right: 0; top: 0; bottom: 0;
  z-index: 0;
}

.CodeMirror-linewidget {
  position: relative;
  z-index: 2;
  padding: 0.1px; /* Force widget margins to stay inside of the container */
}

.CodeMirror-widget {}

.CodeMirror-rtl pre { direction: rtl; }

.CodeMirror-code {
  outline: none;
}

/* Force content-box sizing for the elements where we expect it */
.CodeMirror-scroll,
.CodeMirror-sizer,
.CodeMirror-gutter,
.CodeMirror-gutters,
.CodeMirror-linenumber {
  -moz-box-sizing: content-box;
  box-sizing: content-box;
}

.CodeMirror-measure {
  position: absolute;
  width: 100%;
  height: 0;
  overflow: hidden;
  visibility: hidden;
}

.CodeMirror-cursor {
  position: absolute;
  pointer-events: none;
}
.CodeMirror-measure pre { position: static; }

div.CodeMirror-cursors {
  visibility: hidden;
  position: relative;
  z-index: 3;
}
div.CodeMirror-dragcursors {
  visibility: visible;
}

.CodeMirror-focused div.CodeMirror-cursors {
  visibility: visible;
}

.CodeMirror-selected { background: #d9d9d9; }
.CodeMirror-focused .CodeMirror-selected { background: #d7d4f0; }
.CodeMirror-crosshair { cursor: crosshair; }
.CodeMirror-line::selection, .CodeMirror-line > span::selection, .CodeMirror-line > span > span::selection { background: #d7d4f0; }
.CodeMirror-line::-moz-selection, .CodeMirror-line > span::-moz-selection, .CodeMirror-line > span > span::-moz-selection { background: #d7d4f0; }

.cm-searching {
  background-color: #ffa;
  background-color: rgba(255, 255, 0, .4);
}

/* Used to force a border model for a node */
.cm-force-border { padding-right: .1px; }

@media print {
  /* Hide the cursor when printing */
  .CodeMirror div.CodeMirror-cursors {
    visibility: hidden;
  }
}

/* See issue #2901 */
.cm-tab-wrap-hack:after { content: ''; }

/* Help users use markselection to safely style text background */
span.CodeMirror-selectedtext { background: none; }

.CodeMirror-dialog {
  position: absolute;
  left: 0; right: 0;
  background: inherit;
  z-index: 15;
  padding: .1em .8em;
  overflow: hidden;
  color: inherit;
}

.CodeMirror-dialog-top {
  border-bottom: 1px solid #eee;
  top: 0;
}

.CodeMirror-dialog-bottom {
  border-top: 1px solid #eee;
  bottom: 0;
}

.CodeMirror-dialog input {
  border: none;
  outline: none;
  background: transparent;
  width: 20em;
  color: inherit;
  font-family: monospace;
}

.CodeMirror-dialog button {
  font-size: 70%;
}

.CodeMirror-foldmarker {
  color: blue;
  text-shadow: #b9f 1px 1px 2px, #b9f -1px -1px 2px, #b9f 1px -1px 2px, #b9f -1px 1px 2px;
  font-family: arial;
  line-height: .3;
  cursor: pointer;
}
.CodeMirror-foldgutter {
  width: .7em;
}
.CodeMirror-foldgutter-open,
.CodeMirror-foldgutter-folded {
  cursor: pointer;
}
.CodeMirror-foldgutter-open:after {
  content: "\25BE";
}
.CodeMirror-foldgutter-folded:after {
  content: "\25B8";
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.CodeMirror {
  line-height: var(--jp-code-line-height);
  font-size: var(--jp-code-font-size);
  font-family: var(--jp-code-font-family);
  border: 0;
  border-radius: 0;
  height: auto;
  /* Changed to auto to autogrow */
}

.CodeMirror pre {
  padding: 0 var(--jp-code-padding);
}

.jp-CodeMirrorEditor[data-type='inline'] .CodeMirror-dialog {
  background-color: var(--jp-layout-color0);
  color: var(--jp-content-font-color1);
}

/* This causes https://github.com/jupyter/jupyterlab/issues/522 */
/* May not cause it not because we changed it! */
.CodeMirror-lines {
  padding: var(--jp-code-padding) 0;
}

.CodeMirror-linenumber {
  padding: 0 8px;
}

.jp-CodeMirrorEditor {
  cursor: text;
}

.jp-CodeMirrorEditor[data-type='inline'] .CodeMirror-cursor {
  border-left: var(--jp-code-cursor-width0) solid var(--jp-editor-cursor-color);
}

/* When zoomed out 67% and 33% on a screen of 1440 width x 900 height */
@media screen and (min-width: 2138px) and (max-width: 4319px) {
  .jp-CodeMirrorEditor[data-type='inline'] .CodeMirror-cursor {
    border-left: var(--jp-code-cursor-width1) solid
      var(--jp-editor-cursor-color);
  }
}

/* When zoomed out less than 33% */
@media screen and (min-width: 4320px) {
  .jp-CodeMirrorEditor[data-type='inline'] .CodeMirror-cursor {
    border-left: var(--jp-code-cursor-width2) solid
      var(--jp-editor-cursor-color);
  }
}

.CodeMirror.jp-mod-readOnly .CodeMirror-cursor {
  display: none;
}

.CodeMirror-gutters {
  border-right: 1px solid var(--jp-border-color2);
  background-color: var(--jp-layout-color0);
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

.CodeMirror-selectedtext.cm-searching {
  background-color: var(--jp-search-selected-match-background-color) !important;
  color: var(--jp-search-selected-match-color) !important;
}

.cm-searching {
  background-color: var(
    --jp-search-unselected-match-background-color
  ) !important;
  color: var(--jp-search-unselected-match-color) !important;
}

.CodeMirror-focused .CodeMirror-selected {
  background-color: var(--jp-editor-selected-focused-background);
}

.CodeMirror-selected {
  background-color: var(--jp-editor-selected-background);
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

/**
 * Here is our jupyter theme for CodeMirror syntax highlighting
 * This is used in our marked.js syntax highlighting and CodeMirror itself
 * The string "jupyter" is set in ../codemirror/widget.DEFAULT_CODEMIRROR_THEME
 * This came from the classic notebook, which came form highlight.js/GitHub
 */

/**
 * CodeMirror themes are handling the background/color in this way. This works
 * fine for CodeMirror editors outside the notebook, but the notebook styles
 * these things differently.
 */
.CodeMirror.cm-s-jupyter {
  background: var(--jp-layout-color0);
  color: var(--jp-content-font-color1);
}

/* In the notebook, we want this styling to be handled by its container */
.jp-CodeConsole .CodeMirror.cm-s-jupyter,
.jp-Notebook .CodeMirror.cm-s-jupyter {
  background: transparent;
}

.cm-s-jupyter .CodeMirror-cursor {
  border-left: var(--jp-code-cursor-width0) solid var(--jp-editor-cursor-color);
}
.cm-s-jupyter span.cm-keyword {
  color: var(--jp-mirror-editor-keyword-color);
  font-weight: bold;
}
.cm-s-jupyter span.cm-atom {
  color: var(--jp-mirror-editor-atom-color);
}
.cm-s-jupyter span.cm-number {
  color: var(--jp-mirror-editor-number-color);
}
.cm-s-jupyter span.cm-def {
  color: var(--jp-mirror-editor-def-color);
}
.cm-s-jupyter span.cm-variable {
  color: var(--jp-mirror-editor-variable-color);
}
.cm-s-jupyter span.cm-variable-2 {
  color: var(--jp-mirror-editor-variable-2-color);
}
.cm-s-jupyter span.cm-variable-3 {
  color: var(--jp-mirror-editor-variable-3-color);
}
.cm-s-jupyter span.cm-punctuation {
  color: var(--jp-mirror-editor-punctuation-color);
}
.cm-s-jupyter span.cm-property {
  color: var(--jp-mirror-editor-property-color);
}
.cm-s-jupyter span.cm-operator {
  color: var(--jp-mirror-editor-operator-color);
  font-weight: bold;
}
.cm-s-jupyter span.cm-comment {
  color: var(--jp-mirror-editor-comment-color);
  font-style: italic;
}
.cm-s-jupyter span.cm-string {
  color: var(--jp-mirror-editor-string-color);
}
.cm-s-jupyter span.cm-string-2 {
  color: var(--jp-mirror-editor-string-2-color);
}
.cm-s-jupyter span.cm-meta {
  color: var(--jp-mirror-editor-meta-color);
}
.cm-s-jupyter span.cm-qualifier {
  color: var(--jp-mirror-editor-qualifier-color);
}
.cm-s-jupyter span.cm-builtin {
  color: var(--jp-mirror-editor-builtin-color);
}
.cm-s-jupyter span.cm-bracket {
  color: var(--jp-mirror-editor-bracket-color);
}
.cm-s-jupyter span.cm-tag {
  color: var(--jp-mirror-editor-tag-color);
}
.cm-s-jupyter span.cm-attribute {
  color: var(--jp-mirror-editor-attribute-color);
}
.cm-s-jupyter span.cm-header {
  color: var(--jp-mirror-editor-header-color);
}
.cm-s-jupyter span.cm-quote {
  color: var(--jp-mirror-editor-quote-color);
}
.cm-s-jupyter span.cm-link {
  color: var(--jp-mirror-editor-link-color);
}
.cm-s-jupyter span.cm-error {
  color: var(--jp-mirror-editor-error-color);
}
.cm-s-jupyter span.cm-hr {
  color: #999;
}

.cm-s-jupyter span.cm-tab {
  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADAAAAAMCAYAAAAkuj5RAAAAAXNSR0IArs4c6QAAAGFJREFUSMft1LsRQFAQheHPowAKoACx3IgEKtaEHujDjORSgWTH/ZOdnZOcM/sgk/kFFWY0qV8foQwS4MKBCS3qR6ixBJvElOobYAtivseIE120FaowJPN75GMu8j/LfMwNjh4HUpwg4LUAAAAASUVORK5CYII=);
  background-position: right;
  background-repeat: no-repeat;
}

.cm-s-jupyter .CodeMirror-activeline-background,
.cm-s-jupyter .CodeMirror-gutter {
  background-color: var(--jp-layout-color2);
}

/* Styles for shared cursors (remote cursor locations and selected ranges) */
.jp-CodeMirrorEditor .remote-caret {
  position: relative;
  border-left: 2px solid black;
  margin-left: -1px;
  margin-right: -1px;
  box-sizing: border-box;
}

.jp-CodeMirrorEditor .remote-caret > div {
  white-space: nowrap;
  position: absolute;
  top: -1.15em;
  padding-bottom: 0.05em;
  left: -2px;
  font-size: 0.95em;
  background-color: rgb(250, 129, 0);
  font-family: var(--jp-ui-font-family);
  font-weight: bold;
  line-height: normal;
  user-select: none;
  color: white;
  padding-left: 2px;
  padding-right: 2px;
  z-index: 3;
  transition: opacity 0.3s ease-in-out;
}

.jp-CodeMirrorEditor .remote-caret.hide-name > div {
  transition-delay: 0.7s;
  opacity: 0;
}

.jp-CodeMirrorEditor .remote-caret:hover > div {
  opacity: 1;
  transition-delay: 0s;
}

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
  margin: 0px;
  padding: 0px;
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
  margin-bottom: 0em;
}

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
  font-size: 12px;
  table-layout: fixed;
  margin-left: auto;
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
  padding: 0.5em 0.5em;
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

.jp-RenderedHTMLCommon table {
  margin-bottom: 1em;
}

.jp-RenderedHTMLCommon p {
  text-align: left;
  margin: 0px;
}

.jp-RenderedHTMLCommon p {
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
/* ...or leave it untouched if they don't */
[data-jp-theme-light='false'] .jp-RenderedImage img.jp-needs-dark-background {
}
[data-jp-theme-light='true'] .jp-RenderedImage img.jp-needs-light-background {
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
  font-size: 0.8em;
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

.jp-FileBrowser {
  display: flex;
  flex-direction: column;
  color: var(--jp-ui-font-color1);
  background: var(--jp-layout-color1);
  /* This is needed so that all font sizing of children done in ems is
   * relative to this base size */
  font-size: var(--jp-ui-font-size1);
}

.jp-FileBrowser-toolbar.jp-Toolbar {
  border-bottom: none;
  height: auto;
  margin: var(--jp-toolbar-header-margin);
  box-shadow: none;
}

.jp-BreadCrumbs {
  flex: 0 0 auto;
  margin: 8px 12px 8px 12px;
}

.jp-BreadCrumbs-item {
  margin: 0px 2px;
  padding: 0px 2px;
  border-radius: var(--jp-border-radius);
  cursor: pointer;
}

.jp-BreadCrumbs-item:hover {
  background-color: var(--jp-layout-color2);
}

.jp-BreadCrumbs-item:first-child {
  margin-left: 0px;
}

.jp-BreadCrumbs-item.jp-mod-dropTarget {
  background-color: var(--jp-brand-color2);
  opacity: 0.7;
}

/*-----------------------------------------------------------------------------
| Buttons
|----------------------------------------------------------------------------*/

.jp-FileBrowser-toolbar.jp-Toolbar {
  padding: 0px;
  margin: 8px 12px 0px 12px;
}

.jp-FileBrowser-toolbar.jp-Toolbar {
  justify-content: flex-start;
}

.jp-FileBrowser-toolbar.jp-Toolbar .jp-Toolbar-item {
  flex: 0 0 auto;
  padding-left: 0px;
  padding-right: 2px;
}

.jp-FileBrowser-toolbar.jp-Toolbar .jp-ToolbarButtonComponent {
  width: 40px;
}

.jp-FileBrowser-toolbar.jp-Toolbar
  .jp-Toolbar-item:first-child
  .jp-ToolbarButtonComponent {
  width: 72px;
  background: var(--jp-brand-color1);
}

.jp-FileBrowser-toolbar.jp-Toolbar
  .jp-Toolbar-item:first-child
  .jp-ToolbarButtonComponent:focus-visible {
  background-color: var(--jp-brand-color0);
}

.jp-FileBrowser-toolbar.jp-Toolbar
  .jp-Toolbar-item:first-child
  .jp-ToolbarButtonComponent
  .jp-icon3 {
  fill: white;
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

.jp-FileBrowser-filterBox {
  padding: 0px;
  flex: 0 0 auto;
  margin: 8px 12px 0px 12px;
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

.jp-DirListing:focus-visible {
  border: 1px solid var(--jp-brand-color1);
}

.jp-DirListing-header {
  flex: 0 0 auto;
  display: flex;
  flex-direction: row;
  overflow: hidden;
  border-top: var(--jp-border-width) solid var(--jp-border-color2);
  border-bottom: var(--jp-border-width) solid var(--jp-border-color1);
  box-shadow: var(--jp-toolbar-box-shadow);
  z-index: 2;
}

.jp-DirListing-headerItem {
  padding: 4px 12px 2px 12px;
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

.jp-id-narrow {
  display: none;
  flex: 0 0 5px;
  padding: 4px 4px;
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
  padding: 4px 12px;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
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

.jp-DirListing-itemModified {
  flex: 0 0 125px;
  text-align: right;
}

.jp-DirListing-editor {
  flex: 1 0 64px;
  outline: none;
  border: none;
}

.jp-DirListing-item.jp-mod-running .jp-DirListing-itemIcon:before {
  color: var(--jp-success-color1);
  content: '\25CF';
  font-size: 8px;
  position: absolute;
  left: -8px;
}

.jp-DirListing-item.jp-mod-running.jp-mod-selected
  .jp-DirListing-itemIcon:before {
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
  border-radius: 0px;
  color: var(--jp-ui-font-color1);
  transform: translateX(-40%) translateY(-58%);
}

.jp-DirListing-deadSpace {
  flex: 1 1 auto;
  margin: 0;
  padding: 0;
  list-style-type: none;
  overflow: auto;
  background-color: var(--jp-layout-color1);
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
| Private CSS variables
|----------------------------------------------------------------------------*/

:root {
}

/*-----------------------------------------------------------------------------
| Main OutputArea
| OutputArea has a list of Outputs
|----------------------------------------------------------------------------*/

.jp-OutputArea {
  overflow-y: auto;
}

.jp-OutputArea-child {
  display: flex;
  flex-direction: row;
}

body[data-format='mobile'] .jp-OutputArea-child {
  flex-direction: column;
}

.jp-OutputPrompt {
  flex: 0 0 var(--jp-cell-prompt-width);
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

body[data-format='mobile'] .jp-OutputPrompt {
  flex: 0 0 auto;
  text-align: left;
}

.jp-OutputArea-output {
  height: auto;
  overflow: auto;
  user-select: text;
  -moz-user-select: text;
  -webkit-user-select: text;
  -ms-user-select: text;
}

.jp-OutputArea-child .jp-OutputArea-output {
  flex-grow: 1;
  flex-shrink: 1;
}

body[data-format='mobile'] .jp-OutputArea-child .jp-OutputArea-output {
  margin-left: var(--jp-notebook-padding);
}

/**
 * Isolated output.
 */
.jp-OutputArea-output.jp-mod-isolated {
  width: 100%;
  display: block;
}

/*
When drag events occur, `p-mod-override-cursor` is added to the body.
Because iframes steal all cursor events, the following two rules are necessary
to suppress pointer events while resize drags are occurring. There may be a
better solution to this problem.
*/
body.lm-mod-override-cursor .jp-OutputArea-output.jp-mod-isolated {
  position: relative;
}

body.lm-mod-override-cursor .jp-OutputArea-output.jp-mod-isolated:before {
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
  margin: 0px;
  padding: 0px;
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

/* Hide the gutter in case of
 *  - nested output areas (e.g. in the case of output widgets)
 *  - mirrored output areas
 */
.jp-OutputArea .jp-OutputArea .jp-OutputArea-prompt {
  display: none;
}

/*-----------------------------------------------------------------------------
| executeResult is added to any Output-result for the display of the object
| returned by a cell
|----------------------------------------------------------------------------*/

.jp-OutputArea-output.jp-OutputArea-executeResult {
  margin-left: 0px;
  flex: 1 1 auto;
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

.jp-OutputArea-stdin {
  line-height: var(--jp-code-line-height);
  padding-top: var(--jp-code-padding);
  display: flex;
}

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
  padding: 0em 0.25em;
  margin: 0em 0.25em;
  flex: 0 0 70%;
}

.jp-Stdin-input:focus {
  box-shadow: none;
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
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-Collapser {
  flex: 0 0 var(--jp-cell-collapser-width);
  padding: 0px;
  margin: 0px;
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
  top: 0px;
  bottom: 0px;
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
  height: 0px;
  width: 100%;
  padding: 0px;
  margin: 0px;
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
  display: flex;
  flex-direction: row;
  overflow: hidden;
}

body[data-format='mobile'] .jp-InputArea {
  flex-direction: column;
}

.jp-InputArea-editor {
  flex: 1 1 auto;
  overflow: hidden;
}

.jp-InputArea-editor {
  /* This is the non-active, default styling */
  border: var(--jp-border-width) solid var(--jp-cell-editor-border-color);
  border-radius: 0px;
  background: var(--jp-cell-editor-background);
}

body[data-format='mobile'] .jp-InputArea-editor {
  margin-left: var(--jp-notebook-padding);
}

.jp-InputPrompt {
  flex: 0 0 var(--jp-cell-prompt-width);
  color: var(--jp-cell-inprompt-font-color);
  font-family: var(--jp-cell-prompt-font-family);
  padding: var(--jp-code-padding);
  letter-spacing: var(--jp-cell-prompt-letter-spacing);
  opacity: var(--jp-cell-prompt-opacity);
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

body[data-format='mobile'] .jp-InputPrompt {
  flex: 0 0 auto;
  text-align: left;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Placeholder
|----------------------------------------------------------------------------*/

.jp-Placeholder {
  display: flex;
  flex-direction: row;
  flex: 1 1 auto;
}

.jp-Placeholder-prompt {
  box-sizing: border-box;
}

.jp-Placeholder-content {
  flex: 1 1 auto;
  border: none;
  background: transparent;
  height: 20px;
  box-sizing: border-box;
}

.jp-Placeholder-content .jp-MoreHorizIcon {
  width: 32px;
  height: 16px;
  border: 1px solid transparent;
  border-radius: var(--jp-border-radius);
}

.jp-Placeholder-content .jp-MoreHorizIcon:hover {
  border: 1px solid var(--jp-border-color1);
  box-shadow: 0px 0px 2px 0px rgba(0, 0, 0, 0.25);
  background-color: var(--jp-layout-color0);
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
  margin: 0px;
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
  padding: 0px;
  margin: 0px;
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
  max-height: 200px;
  box-shadow: inset 0 0 6px 2px rgba(0, 0, 0, 0.3);
  margin-left: var(--jp-private-cell-scrolling-output-offset);
}

.jp-CodeCell.jp-mod-outputsScrolled .jp-OutputArea-prompt {
  flex: 0 0
    calc(
      var(--jp-cell-prompt-width) -
        var(--jp-private-cell-scrolling-output-offset)
    );
}

/*-----------------------------------------------------------------------------
| CodeCell
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| MarkdownCell
|----------------------------------------------------------------------------*/

.jp-MarkdownOutput {
  flex: 1 1 auto;
  margin-top: 0;
  margin-bottom: 0;
  padding-left: var(--jp-code-padding);
}

.jp-MarkdownOutput.jp-RenderedHTMLCommon {
  overflow: auto;
}

.jp-showHiddenCellsButton {
  margin-left: calc(var(--jp-cell-prompt-width) + 2 * var(--jp-code-padding));
  margin-top: var(--jp-code-padding);
  border: 1px solid var(--jp-border-color2);
  background-color: var(--jp-border-color3) !important;
  color: var(--jp-content-font-color0) !important;
}

.jp-showHiddenCellsButton:hover {
  background-color: var(--jp-border-color2) !important;
}

.jp-collapseHeadingButton {
  display: none;
}

.jp-MarkdownCell:hover .jp-collapseHeadingButton {
  display: flex;
  min-height: var(--jp-cell-collapser-min-height);
  position: absolute;
  right: 0;
  top: 0;
  bottom: 0;
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

/*-----------------------------------------------------------------------------

/*-----------------------------------------------------------------------------
| Styles
|----------------------------------------------------------------------------*/

.jp-NotebookPanel-toolbar {
  padding: 2px;
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

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Private CSS variables
|----------------------------------------------------------------------------*/

:root {
  --jp-private-notebook-dragImage-width: 304px;
  --jp-private-notebook-dragImage-height: 36px;
  --jp-private-notebook-selected-color: var(--md-blue-400);
  --jp-private-notebook-active-color: var(--md-green-400);
}

/*-----------------------------------------------------------------------------
| Imports
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Notebook
|----------------------------------------------------------------------------*/

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

.jp-Notebook-render * {
  contain: none !important;
}

.jp-Notebook .jp-Cell {
  overflow: visible;
}

.jp-Notebook .jp-Cell .jp-InputPrompt {
  cursor: move;
  float: left;
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
.jp-Notebook .jp-Cell.jp-mod-dirty .jp-InputPrompt:before {
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
  box-shadow: 2px 2px 4px 0px rgba(0, 0, 0, 0.12);
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
  margin: 4px 4px 4px 0px;
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
  box-shadow: 2px 2px 4px 0px rgba(0, 0, 0, 0.12);
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

.jp-NotebookTools-tool {
  padding: 0px 12px 0 12px;
}

.jp-ActiveCellTool {
  padding: 12px;
  background-color: var(--jp-layout-color1);
  border-top: none !important;
}

.jp-ActiveCellTool .jp-InputArea-prompt {
  flex: 0 0 auto;
  padding-left: 0px;
}

.jp-ActiveCellTool .jp-InputArea-editor {
  flex: 1 1 auto;
  background: var(--jp-cell-editor-background);
  border-color: var(--jp-cell-editor-border-color);
}

.jp-ActiveCellTool .jp-InputArea-editor .CodeMirror {
  background: transparent;
}

.jp-MetadataEditorTool {
  flex-direction: column;
  padding: 12px 0px 12px 0px;
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
.jp-MetadataEditorTool label {
  line-height: 1.4;
}

.jp-NotebookTools .jp-select-wrapper {
  margin-top: 4px;
  margin-bottom: 0px;
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
  position: relative;
}

.jp-Cell-Placeholder-wrapper-body div {
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
  --jp-elevation-z1: 0px 2px 1px -1px var(--jp-shadow-umbra-color),
    0px 1px 1px 0px var(--jp-shadow-penumbra-color),
    0px 1px 3px 0px var(--jp-shadow-ambient-color);
  --jp-elevation-z2: 0px 3px 1px -2px var(--jp-shadow-umbra-color),
    0px 2px 2px 0px var(--jp-shadow-penumbra-color),
    0px 1px 5px 0px var(--jp-shadow-ambient-color);
  --jp-elevation-z4: 0px 2px 4px -1px var(--jp-shadow-umbra-color),
    0px 4px 5px 0px var(--jp-shadow-penumbra-color),
    0px 1px 10px 0px var(--jp-shadow-ambient-color);
  --jp-elevation-z6: 0px 3px 5px -1px var(--jp-shadow-umbra-color),
    0px 6px 10px 0px var(--jp-shadow-penumbra-color),
    0px 1px 18px 0px var(--jp-shadow-ambient-color);
  --jp-elevation-z8: 0px 5px 5px -3px var(--jp-shadow-umbra-color),
    0px 8px 10px 1px var(--jp-shadow-penumbra-color),
    0px 3px 14px 2px var(--jp-shadow-ambient-color);
  --jp-elevation-z12: 0px 7px 8px -4px var(--jp-shadow-umbra-color),
    0px 12px 17px 2px var(--jp-shadow-penumbra-color),
    0px 5px 22px 4px var(--jp-shadow-ambient-color);
  --jp-elevation-z16: 0px 8px 10px -5px var(--jp-shadow-umbra-color),
    0px 16px 24px 2px var(--jp-shadow-penumbra-color),
    0px 6px 30px 5px var(--jp-shadow-ambient-color);
  --jp-elevation-z20: 0px 10px 13px -6px var(--jp-shadow-umbra-color),
    0px 20px 31px 3px var(--jp-shadow-penumbra-color),
    0px 8px 38px 7px var(--jp-shadow-ambient-color);
  --jp-elevation-z24: 0px 11px 15px -7px var(--jp-shadow-umbra-color),
    0px 24px 38px 3px var(--jp-shadow-penumbra-color),
    0px 9px 46px 8px var(--jp-shadow-ambient-color);

  /* Borders
   *
   * The following variables, specify the visual styling of borders in JupyterLab.
   */

  --jp-border-width: 1px;
  --jp-border-color0: var(--md-grey-400);
  --jp-border-color1: var(--md-grey-400);
  --jp-border-color2: var(--md-grey-300);
  --jp-border-color3: var(--md-grey-200);
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

  --jp-ui-font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica,
    Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol';

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

  --jp-content-link-color: var(--md-blue-700);

  --jp-content-font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Helvetica, Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji',
    'Segoe UI Symbol';

  /*
   * Code Fonts
   *
   * Code font variables are used for typography of code and other monospaces content.
   */

  --jp-code-font-size: 13px;
  --jp-code-line-height: 1.3077; /* 17px for 13px base */
  --jp-code-padding: 5px; /* 5px for 13px base, codemirror highlighting needs integer px value */
  --jp-code-font-family-default: Menlo, Consolas, 'DejaVu Sans Mono', monospace;
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

  --jp-inverse-layout-color0: #111111;
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
  --jp-cell-prompt-letter-spacing: 0px;
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
  --jp-toolbar-box-shadow: 0px 0px 2px 0px rgba(0, 0, 0, 0.24);
  --jp-toolbar-header-margin: 4px 4px 0px 4px;
  --jp-toolbar-active-background: var(--md-grey-300);

  /* Statusbar specific styles */

  --jp-statusbar-height: 24px;

  /* Input field styles */

  --jp-input-box-shadow: inset 0 0 2px var(--md-blue-300);
  --jp-input-active-background: var(--jp-layout-color1);
  --jp-input-hover-background: var(--jp-layout-color1);
  --jp-input-background: var(--md-grey-100);
  --jp-input-border-color: var(--jp-border-color1);
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
  --jp-mirror-editor-variable-2-color: #05a;
  --jp-mirror-editor-variable-3-color: #085;
  --jp-mirror-editor-punctuation-color: #05a;
  --jp-mirror-editor-property-color: #05a;
  --jp-mirror-editor-operator-color: #aa22ff;
  --jp-mirror-editor-comment-color: #408080;
  --jp-mirror-editor-string-color: #ba2121;
  --jp-mirror-editor-string-2-color: #708;
  --jp-mirror-editor-meta-color: #aa22ff;
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
}
</style>

<style type="text/css">
/* Misc */
a.anchor-link {
  display: none;
}

.highlight  {
  margin: 0.4em;
}

/* Input area styling */
.jp-InputArea {
  overflow: hidden;
}

.jp-InputArea-editor {
  overflow: hidden;
}

.CodeMirror pre {
  margin: 0;
  padding: 0;
}

/* Using table instead of flexbox so that we can use break-inside property */
/* CSS rules under this comment should not be required anymore after we move to the JupyterLab 4.0 CSS */


.jp-CodeCell.jp-mod-outputsScrolled .jp-OutputArea-prompt {
  min-width: calc(
    var(--jp-cell-prompt-width) - var(--jp-private-cell-scrolling-output-offset)
  );
}

.jp-OutputArea-child {
  display: table;
  width: 100%;
}

.jp-OutputPrompt {
  display: table-cell;
  vertical-align: top;
  min-width: var(--jp-cell-prompt-width);
}

body[data-format='mobile'] .jp-OutputPrompt {
  display: table-row;
}

.jp-OutputArea-output {
  display: table-cell;
  width: 100%;
}

body[data-format='mobile'] .jp-OutputArea-child .jp-OutputArea-output {
  display: table-row;
}

.jp-OutputArea-output.jp-OutputArea-executeResult {
  width: 100%;
}

@media print {
  .jp-Collapser {
    display: none;
  }

  .jp-Cell-inputWrapper,
  .jp-Cell-outputWrapper {
    display: block;
  }

  .jp-OutputArea-child {
    break-inside: avoid-page;
  }
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
    <!-- End of mathjax configuration --></head>
<body class="jp-Notebook" data-jp-theme-light="true" data-jp-theme-name="JupyterLab Light">

<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput " data-mime-type="text/markdown">
<h1 id="Food-Nutrients-Analysis---Stat-196K">Food Nutrients Analysis - Stat 196K<a class="anchor-link" href="#Food-Nutrients-Analysis---Stat-196K">&#182;</a></h1><h2 id="Matthew-Caldwell,-May-2022">Matthew Caldwell, May 2022<a class="anchor-link" href="#Matthew-Caldwell,-May-2022">&#182;</a></h2><h1 id="Abstract">Abstract<a class="anchor-link" href="#Abstract">&#182;</a></h1><h3 id="Using-extracted-data-from-USDA's-BrandedFoods-database-and-supplementary-data-from-the-USDA's-SuperTracker-nutrient-and-dieting-tool/database,-I-explore-the-distribution-of-protein,-fat,-and-carbs-within-this-combined-food-data-and-examine-the-relationship-between-these-three-nutrients.">Using extracted data from USDA's BrandedFoods database and supplementary data from the USDA's SuperTracker nutrient and dieting tool/database, I explore the distribution of protein, fat, and carbs within this combined food data and examine the relationship between these three nutrients.<a class="anchor-link" href="#Using-extracted-data-from-USDA's-BrandedFoods-database-and-supplementary-data-from-the-USDA's-SuperTracker-nutrient-and-dieting-tool/database,-I-explore-the-distribution-of-protein,-fat,-and-carbs-within-this-combined-food-data-and-examine-the-relationship-between-these-three-nutrients.">&#182;</a></h3>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput " data-mime-type="text/markdown">
<h3 id="Imports">Imports<a class="anchor-link" href="#Imports">&#182;</a></h3>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs  ">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[1]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="kn">import</span> <span class="nn">json</span>
<span class="kn">import</span> <span class="nn">os</span>
<span class="kn">import</span> <span class="nn">multiprocessing</span>
<span class="kn">import</span> <span class="nn">itertools</span>
<span class="kn">import</span> <span class="nn">numpy</span> <span class="k">as</span> <span class="nn">np</span>
<span class="kn">import</span> <span class="nn">pandas</span> <span class="k">as</span> <span class="nn">pd</span>
<span class="kn">from</span> <span class="nn">sklearn</span> <span class="kn">import</span> <span class="n">preprocessing</span><span class="p">,</span> <span class="n">utils</span>
<span class="kn">from</span> <span class="nn">sklearn.model_selection</span> <span class="kn">import</span> <span class="n">train_test_split</span>
<span class="kn">from</span> <span class="nn">sklearn.linear_model</span> <span class="kn">import</span> <span class="n">LogisticRegression</span>
<span class="kn">from</span> <span class="nn">mpl_toolkits</span> <span class="kn">import</span> <span class="n">mplot3d</span>
<span class="kn">import</span> <span class="nn">matplotlib.pyplot</span> <span class="k">as</span> <span class="nn">plt</span>
<span class="o">%</span><span class="k">matplotlib</span> inline
</pre></div>

     </div>
</div>
</div>
</div>

</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput " data-mime-type="text/markdown">
<h3 id="Functions">Functions<a class="anchor-link" href="#Functions">&#182;</a></h3>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs  ">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[2]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1"># Extracts the numberical data from food_nutri and converts to a numpy array [Protein, Fat, Carbs].</span>
<span class="k">def</span> <span class="nf">prepare_dataset</span><span class="p">(</span><span class="n">food_nutri</span><span class="p">):</span>
    <span class="n">X</span> <span class="o">=</span> <span class="p">[]</span>
    <span class="k">for</span> <span class="n">f</span> <span class="ow">in</span> <span class="n">food_nutri</span><span class="p">:</span>
        <span class="n">X</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">f</span><span class="p">[</span><span class="mi">1</span><span class="p">:])</span>
    <span class="n">X</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">asarray</span><span class="p">(</span><span class="n">X</span><span class="p">)</span>
    <span class="c1"># Remove NaN Values and return</span>
    <span class="k">return</span> <span class="n">X</span><span class="p">[</span><span class="o">~</span><span class="n">np</span><span class="o">.</span><span class="n">isnan</span><span class="p">(</span><span class="n">X</span><span class="p">)</span><span class="o">.</span><span class="n">any</span><span class="p">(</span><span class="n">axis</span><span class="o">=</span><span class="mi">1</span><span class="p">)]</span>

<span class="c1"># Creates a full dataset with [Name, Protein, Fat, Carbs] from BrandedFoods and supertrackerfooddatabase combined.</span>
<span class="k">def</span> <span class="nf">prepare_food_nutri</span><span class="p">():</span>
    <span class="n">pwd</span> <span class="o">=</span> <span class="s2">&quot;/srv/data/food/BrandedFoods/&quot;</span>
    <span class="n">foodfiles</span> <span class="o">=</span> <span class="p">[</span><span class="n">pwd</span> <span class="o">+</span> <span class="n">f</span> <span class="k">for</span> <span class="n">f</span> <span class="ow">in</span> <span class="n">os</span><span class="o">.</span><span class="n">listdir</span><span class="p">(</span><span class="n">pwd</span><span class="p">)]</span>
    <span class="k">with</span> <span class="n">multiprocessing</span><span class="o">.</span><span class="n">Pool</span><span class="p">(</span><span class="mi">4</span><span class="p">)</span> <span class="k">as</span> <span class="n">p</span><span class="p">:</span>
        <span class="n">descriptions</span> <span class="o">=</span> <span class="n">p</span><span class="o">.</span><span class="n">map</span><span class="p">(</span><span class="n">extract_description</span><span class="p">,</span> <span class="n">foodfiles</span><span class="p">)</span>
        <span class="n">nutrients</span> <span class="o">=</span> <span class="n">p</span><span class="o">.</span><span class="n">map</span><span class="p">(</span><span class="n">extract_nutrients</span><span class="p">,</span> <span class="n">foodfiles</span><span class="p">)</span>
    <span class="n">food_nutri</span> <span class="o">=</span> <span class="n">build_food_nutri_list</span><span class="p">(</span><span class="nb">list</span><span class="p">(</span><span class="nb">zip</span><span class="p">(</span><span class="n">itertools</span><span class="o">.</span><span class="n">chain</span><span class="p">(</span><span class="o">*</span><span class="n">descriptions</span><span class="p">),</span> <span class="n">itertools</span><span class="o">.</span><span class="n">chain</span><span class="p">(</span><span class="o">*</span><span class="n">nutrients</span><span class="p">))))</span>
    <span class="n">food_nutri</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span><span class="n">extract_super_tracker</span><span class="p">(</span><span class="s2">&quot;supertrackerfooddatabase.xlsx&quot;</span><span class="p">))</span>
    <span class="k">return</span> <span class="n">food_nutri</span>

<span class="c1"># Returns all the descriptions for the foods inside jsonfile.</span>
<span class="k">def</span> <span class="nf">extract_description</span><span class="p">(</span><span class="n">jsonfile</span><span class="p">):</span>
    <span class="k">with</span> <span class="nb">open</span><span class="p">(</span><span class="n">jsonfile</span><span class="p">)</span> <span class="k">as</span> <span class="n">f</span><span class="p">:</span>
        <span class="n">d</span> <span class="o">=</span> <span class="n">json</span><span class="o">.</span><span class="n">load</span><span class="p">(</span><span class="n">f</span><span class="p">)</span>
    <span class="k">return</span> <span class="p">[</span><span class="n">x</span><span class="p">[</span><span class="s2">&quot;description&quot;</span><span class="p">]</span> <span class="k">for</span> <span class="n">x</span> <span class="ow">in</span> <span class="n">d</span><span class="p">]</span>

<span class="c1"># Returns all the food nutrients for the foods inside jsonfile.</span>
<span class="k">def</span> <span class="nf">extract_nutrients</span><span class="p">(</span><span class="n">jsonfile</span><span class="p">):</span>
    <span class="k">with</span> <span class="nb">open</span><span class="p">(</span><span class="n">jsonfile</span><span class="p">)</span> <span class="k">as</span> <span class="n">f</span><span class="p">:</span>
        <span class="n">d</span> <span class="o">=</span> <span class="n">json</span><span class="o">.</span><span class="n">load</span><span class="p">(</span><span class="n">f</span><span class="p">)</span>
    <span class="k">return</span> <span class="p">[</span><span class="n">x</span><span class="p">[</span><span class="s2">&quot;foodNutrients&quot;</span><span class="p">]</span> <span class="k">for</span> <span class="n">x</span> <span class="ow">in</span> <span class="n">d</span><span class="p">]</span>

<span class="c1"># Returns a list of Protein, Total Fat, and Carbs for the foods inside food_list from BrandedFoods.</span>
<span class="k">def</span> <span class="nf">build_food_nutri_list</span><span class="p">(</span><span class="n">food_list</span><span class="p">):</span>         
    <span class="n">food_nutri</span> <span class="o">=</span> <span class="p">[]</span> 
    <span class="k">for</span> <span class="n">item</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="nb">len</span><span class="p">(</span><span class="n">food_list</span><span class="p">)):</span>
        <span class="n">p</span><span class="p">,</span> <span class="n">f</span><span class="p">,</span> <span class="n">c</span> <span class="o">=</span> <span class="mi">0</span><span class="p">,</span> <span class="mi">0</span><span class="p">,</span> <span class="mi">0</span>
        <span class="k">for</span> <span class="n">n</span> <span class="ow">in</span> <span class="n">food_list</span><span class="p">[</span><span class="n">item</span><span class="p">][</span><span class="mi">1</span><span class="p">]:</span>
            <span class="k">try</span><span class="p">:</span>
                <span class="k">if</span> <span class="n">n</span><span class="p">[</span><span class="s2">&quot;nutrient&quot;</span><span class="p">][</span><span class="s2">&quot;name&quot;</span><span class="p">]</span> <span class="o">==</span> <span class="s2">&quot;Protein&quot;</span><span class="p">:</span>
                    <span class="n">p</span> <span class="o">=</span> <span class="n">n</span><span class="p">[</span><span class="s2">&quot;amount&quot;</span><span class="p">]</span>
                <span class="k">if</span> <span class="n">n</span><span class="p">[</span><span class="s2">&quot;nutrient&quot;</span><span class="p">][</span><span class="s2">&quot;name&quot;</span><span class="p">]</span> <span class="o">==</span> <span class="s2">&quot;Total lipid (fat)&quot;</span><span class="p">:</span>
                    <span class="n">f</span> <span class="o">=</span> <span class="n">n</span><span class="p">[</span><span class="s2">&quot;amount&quot;</span><span class="p">]</span>
                <span class="k">if</span> <span class="n">n</span><span class="p">[</span><span class="s2">&quot;nutrient&quot;</span><span class="p">][</span><span class="s2">&quot;name&quot;</span><span class="p">]</span> <span class="o">==</span> <span class="s2">&quot;Carbohydrate, by difference&quot;</span><span class="p">:</span>
                    <span class="n">c</span> <span class="o">=</span> <span class="n">n</span><span class="p">[</span><span class="s2">&quot;amount&quot;</span><span class="p">]</span>
            <span class="k">except</span> <span class="ne">KeyError</span><span class="p">:</span> 
                <span class="k">pass</span>
        <span class="k">if</span> <span class="n">p</span> <span class="o">!=</span> <span class="mi">0</span> <span class="ow">and</span> <span class="n">f</span> <span class="o">!=</span> <span class="mi">0</span> <span class="ow">and</span> <span class="n">c</span> <span class="o">!=</span> <span class="mi">0</span> <span class="ow">and</span> <span class="n">p</span> <span class="o">&lt;=</span> <span class="mi">500</span> <span class="ow">and</span> <span class="n">f</span> <span class="o">&lt;=</span> <span class="mi">500</span> <span class="ow">and</span> <span class="n">c</span> <span class="o">&lt;=</span> <span class="mi">500</span><span class="p">:</span>
            <span class="n">food_nutri</span><span class="o">.</span><span class="n">append</span><span class="p">((</span><span class="n">food_list</span><span class="p">[</span><span class="n">item</span><span class="p">][</span><span class="mi">0</span><span class="p">],</span> <span class="n">p</span><span class="p">,</span> <span class="n">f</span><span class="p">,</span> <span class="n">c</span><span class="p">))</span>
    <span class="k">return</span> <span class="n">food_nutri</span>

<span class="c1"># Returns a list of Protein, Total Fat, and Carbs for the foods inside supertrackerfooddatabase.</span>
<span class="k">def</span> <span class="nf">extract_super_tracker</span><span class="p">(</span><span class="n">super_tracker</span><span class="p">):</span>
    <span class="n">df</span> <span class="o">=</span> <span class="n">pd</span><span class="o">.</span><span class="n">read_excel</span><span class="p">(</span><span class="n">super_tracker</span><span class="p">,</span>
                       <span class="n">sheet_name</span><span class="o">=</span><span class="s2">&quot;Nutrients&quot;</span><span class="p">,</span>
                       <span class="n">usecols</span><span class="o">=</span><span class="p">[</span><span class="s2">&quot;foodname&quot;</span><span class="p">,</span> <span class="s2">&quot;_203 Protein (g)&quot;</span><span class="p">,</span> <span class="s2">&quot;_204 Total Fat (g)&quot;</span><span class="p">,</span> <span class="s2">&quot;_205 Carbohydrate (g)&quot;</span><span class="p">])</span>
    <span class="k">return</span> <span class="n">df</span><span class="o">.</span><span class="n">values</span><span class="o">.</span><span class="n">tolist</span><span class="p">()</span>

<span class="c1"># Converts data to int and reshapes to fit LogisticRegression model.</span>
<span class="k">def</span> <span class="nf">format_sample_data</span><span class="p">(</span><span class="n">data</span><span class="p">):</span>
    <span class="n">lab_enc</span> <span class="o">=</span> <span class="n">preprocessing</span><span class="o">.</span><span class="n">LabelEncoder</span><span class="p">()</span>
    <span class="n">data</span> <span class="o">=</span> <span class="n">lab_enc</span><span class="o">.</span><span class="n">fit_transform</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
    <span class="k">return</span> <span class="n">data</span><span class="o">.</span><span class="n">reshape</span><span class="p">(</span><span class="o">-</span><span class="mi">1</span><span class="p">,</span> <span class="mi">1</span><span class="p">)</span>
</pre></div>

     </div>
</div>
</div>
</div>

</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput " data-mime-type="text/markdown">
<h3 id="Build-Dataset,-Extract-Samples,-and-Prepare-for-Analysis">Build Dataset, Extract Samples, and Prepare for Analysis<a class="anchor-link" href="#Build-Dataset,-Extract-Samples,-and-Prepare-for-Analysis">&#182;</a></h3>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs  ">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[3]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1"># Custom dataset [Protein, Fat, Carbs] all ready to use!</span>
<span class="n">X</span> <span class="o">=</span> <span class="n">prepare_dataset</span><span class="p">(</span><span class="n">prepare_food_nutri</span><span class="p">())</span>

<span class="c1"># Setup LogisticRegression model with liblinear solver.</span>
<span class="n">Xtrain</span><span class="p">,</span> <span class="n">Xtest</span> <span class="o">=</span> <span class="n">train_test_split</span><span class="p">(</span><span class="n">X</span><span class="p">,</span> <span class="n">random_state</span><span class="o">=</span><span class="mi">27</span><span class="p">)</span>
<span class="n">model</span> <span class="o">=</span> <span class="n">LogisticRegression</span><span class="p">(</span><span class="n">solver</span><span class="o">=</span><span class="s2">&quot;liblinear&quot;</span><span class="p">,</span> <span class="n">max_iter</span><span class="o">=</span><span class="mi">1000</span><span class="p">)</span>

<span class="c1"># Break the data into their respective nutrients.</span>
<span class="n">Protein</span> <span class="o">=</span> <span class="n">Xtrain</span><span class="p">[:,</span> <span class="mi">0</span><span class="p">]</span>
<span class="n">Fat</span> <span class="o">=</span> <span class="n">Xtrain</span><span class="p">[:,</span> <span class="mi">1</span><span class="p">]</span>
<span class="n">Carbs</span> <span class="o">=</span> <span class="n">Xtrain</span><span class="p">[:,</span> <span class="mi">2</span><span class="p">]</span>

<span class="c1"># Prepare formatted samples of size 10000.</span>
<span class="n">P_Samp</span> <span class="o">=</span> <span class="n">format_sample_data</span><span class="p">(</span><span class="n">Protein</span><span class="p">[</span><span class="mi">0</span><span class="p">:</span><span class="mi">10000</span><span class="p">])</span>
<span class="n">F_Samp</span> <span class="o">=</span> <span class="n">format_sample_data</span><span class="p">(</span><span class="n">Fat</span><span class="p">[</span><span class="mi">0</span><span class="p">:</span><span class="mi">10000</span><span class="p">])</span>
<span class="n">C_Samp</span> <span class="o">=</span> <span class="n">format_sample_data</span><span class="p">(</span><span class="n">Carbs</span><span class="p">[</span><span class="mi">0</span><span class="p">:</span><span class="mi">10000</span><span class="p">])</span>
</pre></div>

     </div>
</div>
</div>
</div>

</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput " data-mime-type="text/markdown">
<h3 id="Predictions">Predictions<a class="anchor-link" href="#Predictions">&#182;</a></h3>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell   ">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[4]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1"># Predict Protein (g) from Fat (g)</span>
<span class="n">model</span><span class="o">.</span><span class="n">fit</span><span class="p">(</span><span class="n">F_Samp</span><span class="p">,</span> <span class="n">P_Samp</span><span class="o">.</span><span class="n">ravel</span><span class="p">())</span>
<span class="n">preds</span> <span class="o">=</span> <span class="n">model</span><span class="o">.</span><span class="n">predict_proba</span><span class="p">(</span><span class="n">F_Samp</span><span class="p">)[:,</span> <span class="mi">0</span><span class="p">]</span>
<span class="n">plt</span><span class="o">.</span><span class="n">scatter</span><span class="p">(</span><span class="n">F_Samp</span><span class="p">,</span> <span class="n">preds</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s2">&quot;Fat (g)&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s2">&quot;Probability of high protein content&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlim</span><span class="p">([</span><span class="mi">0</span><span class="p">,</span> <span class="mi">500</span><span class="p">]);</span>
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




<div class="jp-RenderedImage jp-OutputArea-output ">
<img src="data:image/png;base64,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
"
class="
jp-needs-light-background
"
>
</div>

</div>

</div>

</div>

</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell   ">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[5]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1"># Predict Protein (g) from Carbs (g) </span>
<span class="n">model</span><span class="o">.</span><span class="n">fit</span><span class="p">(</span><span class="n">C_Samp</span><span class="p">,</span> <span class="n">P_Samp</span><span class="o">.</span><span class="n">ravel</span><span class="p">())</span>
<span class="n">preds</span> <span class="o">=</span> <span class="n">model</span><span class="o">.</span><span class="n">predict_proba</span><span class="p">(</span><span class="n">C_Samp</span><span class="p">)[:,</span> <span class="mi">0</span><span class="p">]</span>
<span class="n">plt</span><span class="o">.</span><span class="n">scatter</span><span class="p">(</span><span class="n">C_Samp</span><span class="p">,</span> <span class="n">preds</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s2">&quot;Carbs (g)&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s2">&quot;Probability of high protein content&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlim</span><span class="p">([</span><span class="mi">0</span><span class="p">,</span> <span class="mi">500</span><span class="p">]);</span>
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




<div class="jp-RenderedImage jp-OutputArea-output ">
<img src="data:image/png;base64,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
"
class="
jp-needs-light-background
"
>
</div>

</div>

</div>

</div>

</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput " data-mime-type="text/markdown">
<h4 id="The-two-above-graphs-seem-to-slightly-show-that-high-fat-and-high-carb-foods-have-a-low-chance-of-having-high-protein.">The two above graphs seem to slightly show that high fat and high carb foods have a low chance of having high protein.<a class="anchor-link" href="#The-two-above-graphs-seem-to-slightly-show-that-high-fat-and-high-carb-foods-have-a-low-chance-of-having-high-protein.">&#182;</a></h4>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell   ">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[6]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1"># Predict Fat (g) from Carbs (g) </span>
<span class="n">model</span><span class="o">.</span><span class="n">fit</span><span class="p">(</span><span class="n">C_Samp</span><span class="p">,</span> <span class="n">F_Samp</span><span class="o">.</span><span class="n">ravel</span><span class="p">())</span>
<span class="n">preds</span> <span class="o">=</span> <span class="n">model</span><span class="o">.</span><span class="n">predict_proba</span><span class="p">(</span><span class="n">C_Samp</span><span class="p">)[:,</span> <span class="mi">1</span><span class="p">]</span>
<span class="n">plt</span><span class="o">.</span><span class="n">scatter</span><span class="p">(</span><span class="n">C_Samp</span><span class="p">,</span> <span class="n">preds</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s2">&quot;Carbs (g)&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s2">&quot;Probability of high fat content&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlim</span><span class="p">([</span><span class="mi">0</span><span class="p">,</span> <span class="mi">500</span><span class="p">]);</span>
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




<div class="jp-RenderedImage jp-OutputArea-output ">
<img src="data:image/png;base64,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
"
class="
jp-needs-light-background
"
>
</div>

</div>

</div>

</div>

</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell   ">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[7]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1"># Predict Fat (g) from Protein (g) </span>
<span class="n">model</span><span class="o">.</span><span class="n">fit</span><span class="p">(</span><span class="n">P_Samp</span><span class="p">,</span> <span class="n">F_Samp</span><span class="o">.</span><span class="n">ravel</span><span class="p">())</span>
<span class="n">preds</span> <span class="o">=</span> <span class="n">model</span><span class="o">.</span><span class="n">predict_proba</span><span class="p">(</span><span class="n">P_Samp</span><span class="p">)[:,</span> <span class="mi">1</span><span class="p">]</span>
<span class="n">plt</span><span class="o">.</span><span class="n">scatter</span><span class="p">(</span><span class="n">P_Samp</span><span class="p">,</span> <span class="n">preds</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s2">&quot;Protein (g)&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s2">&quot;Probability of high fat content&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlim</span><span class="p">([</span><span class="mi">0</span><span class="p">,</span> <span class="mi">500</span><span class="p">]);</span>
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




<div class="jp-RenderedImage jp-OutputArea-output ">
<img src="data:image/png;base64,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
"
class="
jp-needs-light-background
"
>
</div>

</div>

</div>

</div>

</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput " data-mime-type="text/markdown">
<h4 id="The-two-above-graphs-seem-to-show-that-high-protein-and-high-carb-foods-have-a-much-lower-chance-of-having-high-fat.">The two above graphs seem to show that high protein and high carb foods have a much lower chance of having high fat.<a class="anchor-link" href="#The-two-above-graphs-seem-to-show-that-high-protein-and-high-carb-foods-have-a-much-lower-chance-of-having-high-fat.">&#182;</a></h4>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell   ">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[8]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1"># Predict Carbs (g) from Protein (g) </span>
<span class="n">model</span><span class="o">.</span><span class="n">fit</span><span class="p">(</span><span class="n">P_Samp</span><span class="p">,</span> <span class="n">C_Samp</span><span class="o">.</span><span class="n">ravel</span><span class="p">())</span>
<span class="n">preds</span> <span class="o">=</span> <span class="n">model</span><span class="o">.</span><span class="n">predict_proba</span><span class="p">(</span><span class="n">P_Samp</span><span class="p">)[:,</span> <span class="mi">2</span><span class="p">]</span>
<span class="n">plt</span><span class="o">.</span><span class="n">scatter</span><span class="p">(</span><span class="n">P_Samp</span><span class="p">,</span> <span class="n">preds</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s2">&quot;Protein (g)&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s2">&quot;Probability of high carb content&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlim</span><span class="p">([</span><span class="mi">0</span><span class="p">,</span> <span class="mi">500</span><span class="p">]);</span>
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




<div class="jp-RenderedImage jp-OutputArea-output ">
<img src="data:image/png;base64,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
"
class="
jp-needs-light-background
"
>
</div>

</div>

</div>

</div>

</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell   ">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[9]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1"># Predict Carbs (g) from Fat (g)</span>
<span class="n">model</span><span class="o">.</span><span class="n">fit</span><span class="p">(</span><span class="n">F_Samp</span><span class="p">,</span> <span class="n">C_Samp</span><span class="o">.</span><span class="n">ravel</span><span class="p">())</span>
<span class="n">preds</span> <span class="o">=</span> <span class="n">model</span><span class="o">.</span><span class="n">predict_proba</span><span class="p">(</span><span class="n">F_Samp</span><span class="p">)[:,</span> <span class="mi">2</span><span class="p">]</span>
<span class="n">plt</span><span class="o">.</span><span class="n">scatter</span><span class="p">(</span><span class="n">F_Samp</span><span class="p">,</span> <span class="n">preds</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s2">&quot;Fat (g)&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s2">&quot;Probability of high carbs content&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlim</span><span class="p">([</span><span class="mi">0</span><span class="p">,</span> <span class="mi">500</span><span class="p">]);</span>
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




<div class="jp-RenderedImage jp-OutputArea-output ">
<img src="data:image/png;base64,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
"
class="
jp-needs-light-background
"
>
</div>

</div>

</div>

</div>

</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput " data-mime-type="text/markdown">
<h4 id="The-two-above-graphs-also-seem-to-show-that-high-protein-and-high-fat-foods-also-have-a-much-lower-chance-of-having-high-carbs.">The two above graphs also seem to show that high protein and high fat foods also have a much lower chance of having high carbs.<a class="anchor-link" href="#The-two-above-graphs-also-seem-to-show-that-high-protein-and-high-fat-foods-also-have-a-much-lower-chance-of-having-high-carbs.">&#182;</a></h4>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput " data-mime-type="text/markdown">
<h3 id="3D-and-2D-Nutrient-Distribution">3D and 2D Nutrient Distribution<a class="anchor-link" href="#3D-and-2D-Nutrient-Distribution">&#182;</a></h3>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell   ">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[10]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1"># Protein, Fat, and Carbs in 3D space, zoomed in on main data cluster to manually ignore outlires.</span>
<span class="n">fig</span> <span class="o">=</span> <span class="n">plt</span><span class="o">.</span><span class="n">figure</span><span class="p">(</span><span class="n">figsize</span><span class="o">=</span><span class="p">(</span><span class="mi">6</span><span class="p">,</span> <span class="mi">6</span><span class="p">))</span>
<span class="n">ax</span> <span class="o">=</span> <span class="n">plt</span><span class="o">.</span><span class="n">axes</span><span class="p">(</span><span class="n">projection</span><span class="o">=</span><span class="s1">&#39;3d&#39;</span><span class="p">)</span>
<span class="n">ax</span><span class="o">.</span><span class="n">scatter</span><span class="p">(</span><span class="n">Protein</span><span class="p">,</span> <span class="n">Fat</span><span class="p">,</span> <span class="n">Carbs</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s2">&quot;Protein (g)&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s2">&quot;Total Fat (g)&quot;</span><span class="p">)</span>
<span class="n">ax</span><span class="o">.</span><span class="n">set_zlabel</span><span class="p">(</span><span class="s2">&quot;Carbohydrate (g)&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlim</span><span class="p">([</span><span class="mi">0</span><span class="p">,</span> <span class="mi">100</span><span class="p">])</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylim</span><span class="p">([</span><span class="mi">0</span><span class="p">,</span> <span class="mi">100</span><span class="p">])</span>
<span class="n">ax</span><span class="o">.</span><span class="n">set_zlim</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="mi">500</span><span class="p">)</span>
<span class="n">ax</span><span class="o">.</span><span class="n">spines</span><span class="p">[</span><span class="s1">&#39;top&#39;</span><span class="p">]</span><span class="o">.</span><span class="n">set_visible</span><span class="p">(</span><span class="kc">False</span><span class="p">)</span>
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




<div class="jp-RenderedImage jp-OutputArea-output ">
<img src="data:image/png;base64,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LGPHjuXNN9/krrvu6tFWrSckSUKlUrF161b++c9/UlhYiE6n44orrmD06NGccsopPPnkk5SWlv6i9V6Oyk5cFEVGjRrFN998Q3p6OtOmTeOdd95h7NiedS6OdULFo6VLl/L555+TnJysaKKHWqhC3QVNTU24XC7i4uJITEzcr10sRHt7O0VFReTl5RER0X164IPNtfz1sz39+toGgki9gN0row06EhNn0hKm1wIyWhX4/QFEMYBBLaDRanCJKh5dMI5xqYefRgkhiiJ/eX8dX1f5EVBx/qQU7jxzZO+eK8lc+MomTDoVWrUKWZZpdQd4cG4uE9P7z1A4hCzLlJSUoFKpFNkJv9/PNddcw5QpU7jrrrsUsbji4mLGjRvXb2spKChQOlOGDRvG66+/jiRJLF68mOrqasVWLaRb3hs2btzI5Zdfzl133cXPP/+MLMtMnDiRG2+8EYBXX32VDz/8kHfeeacvDZwH1U78qATxn3/+mfvvv5+vvvoKgCVLlgBw991398XhBz2hnVBIEz06Opr58+czd+5cRSUupEfd3NyM3W4P7rKTkhSDgZaWFvbs2cPEiRMPWHWXJInzX9lEabMTtUpAliHapCU1Ws+2WvvResn9gk4tYNSqcftF/KLM+NQIwvQa2lw+ats8jEkOR5ZlfH4/VoeX80dqOXVMEklJSYSFhR3SrnxPs4Ofy1vRqSHR30huVqoyDHOofL6jiX+uquxwOYL89CjuPzf3iAW4DoYsy+zevRtZlsnNzVW093/7298yevRo/vKXv/RnG16/4PF4aGlpIS0tDVEUeemll7DZbNx9991YrVa+/vpr3nzzTc4//3wltfLqq69y/vnn92X/+aB6045KOqWuro6MjL06z+np6axfv/5onHpQIAgCY8eO5S9/+Qv33XcfpaWlLF26lIsvvhij0ci8efOYN28eSUlJJCYmKoqLdXV1ym2w1+tlypQpSidMT6hUKt76zWQeWFFCcZOD9Ggj9587ijs+LjpKr7b/MHYM+gQDj4zTJxKm16DTqDHq1LS5A8SYtKjUWoxGFadMG41JciqpqwM573SmoKadBz4rwS9JeNweYsMNvDDh8A11z8lLIjPWyJ5mJzEmLSeOiD0qAXzPnj1IksTo0aOV3fbNN99MTk7OMRnAAd59912+/vpr3n77bdRqNVFRUfzrX//isssuIzMz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iN4xtBM/SvTX4MQvFbfbzddff91FE33BggXMnDlT6WIpLi5WCqKdJXQPRQTq8+2N3P7RLiAYxENplvvOHskl09L7/HV1xuVysW3bti5aLpWVlVxyySW89tprTJ06tV/P3x/Y7XbltdhsNurq6oiNjeX555+nurqaBx98kLPPPpsJEybwyCOPkJOTAwyqQZ5ukWWZMrODVpefadmxg2onPhTEB4C+Hpz4pRPSRP/ggw/YuHEjM2fOJDY2llWrVvHFF1+g1WoVxcWmpiZ8Pl8XCd0DjWm7fSIzH1/VpdCpVQmsuu14IvswL77fed1uCgoKugTwmpoaFi9ezD//+c/+NPntN7xeL8899xzDhg2joqKCDRs28O677+JwOPjd737H3XffzdixY/n9739PWFgYDz/88GDvBweCAfzvX5fw6bYG1CqBH26fMxTEf+30xeDErxW/3899993H22+/TUxMDJMmTVI00UMBIRAIKBK6brdbEZXqSXFxT7OD697aRqvbT5RBw4uXTGBcavcytX1ByJCis555fX09F154Ic888wyzZs3qt3P3N7t372bKlCkkJCSwY8cOpUh777338tVXXzFr1ix27tzJsmXLiIiIOCa0UDZXWbn1vW2YdGpUgsDnt8waVAseCuJDHFO89dZbvPHGGyxfvhy9Xs/q1av54IMP+PHHH5k4caKiiR4qeoqiiMVioampCafTSVxcHElJSQPihwl7LeE6B/DGxkYuuOAC/v73v3PKKad0ebwkyQhC36v2ba6yUtrsICnSwOyRCaiOUFpAlmUkSUKtVnPbbbfxySefcPvttyu6Jx6Ph6VLl/Lzzz9z//33k5CQMOhTKCE+397Ao18UE64PpvGGgvgQQxwB27dvZ/jw4ftpoYiiyM8//6xooo8ZM4b58+d30UTf1w8zNjaWxMREoqOjj0pA93q9bN26tYslnNlsZtGiRSxZsoQzzjhDeawkyTz/Qykfbq0FBC6amsH1s4cdcbAF+PfPlbz8YzmiLKMSBE4encBD8/MO6z346aef0Gq1zJw5k02bNhEbG0tUVBSyLDNnzhwuvfRS7rnnHl5//XVOOeUUsrKygEHfB96F4kYb1/97MwaNCo1aNRTEhxiiv5EkiU2bNrF06VK++uorhg8fzrx58zj77LOV/LMkSVitVpqamrDZbERHR5OUlER0dHS/7A5D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XhISErqcPzRgse86BjNPPfUUr776KoIgMH78eF5//XVcLhcXXXQRlZWVZGdn8/777xMTEzPQSx1iiEHF0E68H9g3cIbSLieeeCLjx49Hqw1Owk2ePJl//etfvPzyy4wcORKv10t7eztXXXUVH330EStXrgRg/fr1TJ8+HYfDQW1tLVFRUTz11FO0t7fz0ksv7Xf+0B3Cb37zG9auXduPr7RvqKur45lnnmHTpk3s2LEDURR59913f9E6LkMM0VcMBfGjQCio7pu/vummmygoKODiiy9m/Pjx5OTksGDBAu68807+85//IMsyVquVkpISzjrrLDZu3EhsbCw33HAD6enp5OXlsW7dOqBrft7hcPDCCy8QHR3dxWxXFMVu8/iDgUAggNvtJhAI4HK5SE1NVUSbAK688ko+/vjjgV3kEEMMQoaC+FFk3x16aPw+MjIoxr9kyRJee+01DAYDxcXFCILA5s2blU6XzZs3K5KpEPTqXLx4sXLs0PHefvttCgoKuOmmm9DpdErgVqvV+11QBoOEblpaGrfffjuZmZmkpKQQFRXFGWecQVNTk9Kdk5KSotQChhhiiL0MBfEBpLPKYSio5uXl8cADD/Dwww8DEB8fz/nnn4/D4WD79u1KkGtpaaGmpoaTTz4ZCAbx0EXihRde4KyzzlKU5j744AMWLFjAtddey9atW5XH19fXc99991FfX3/UXnN3tLa2snz5cioqKqivr8fpdPLWW28N6JqGGOJYYSiIDxJCAViW5S4CWaeccgrXXXcdWq2Wyy+/XGlne+utt0hOTlZGuOUOsaG6ujoqKysV4aPPP/+cJ554gptuuolTTjmFW2+9lXvvvZfa2lpSU1MxGAysXr36KL/arnz77bfk5OQoKoCLFi1i7dq1hyTaNMQQv1aGgvggIzQ0FCKUCtHr9Zx22mnKAFF2djbXX3/9fo9bvnw5c+bMAYJ60qtWreK6667jtNNO49JLL8VqtRIREUFycjIAa9euHXDBoszMTNatW4fL5UKWZb777jvGjBnDvHnzePPNNwF48803mT9//oCuc4ghBiNDLYaDnM696J1bBvcNaKHA39zcrPSoazQampqa+P/27t+ltTMM4Pj3hZjsoYjFRGo8Ufw1RDAO/uCihGAGF20ICF6xQfwxOLikU5vJ/gEuDs6GKyIpBaMgCA5iFicPiIOojd0UxEGl8e2gTbX3xstt7D2e+HymnDfhnCcEHsJz3vM8vb29AOzt7dHd3U1TUxMOh4OzszNqamq+egfFf+vo6GBoaIi2tjYcDgeBQIDx8XGurq6IRqMsLi4W+rgIIZ6SJG4jj2+MFmu239XVxfb2Nnd3d1RXV3NyclLYW72ysoJSqlArN00Tt9vN9fX11/kCz0gmkySTySdrLpeLzc1NiyKyTiaTYWZmhnw+TzweJ5FIWB2SeMWknGJTxZ4WdTqdXFxcFN4fGRlheHiYeDzOxsYGHo8Hv98P3I/WcrvdlpdTxD/y+TzT09Osra1hmiZLS0uYpml1WOIVkyReZurr65mamgLuHxIKBoMcHBzQ0tJCa2srgUCAiooKjo+P2dnZoa+vrzCBRlgvm81iGAY+nw+n00ksFiOdTlsdlnjFpJxSZqqqqgo3LXO5HIlEgsvLS7xeL/39/YTDYW5ublhYWMAwDDo7Oy2OWDyWy+Xwer2FY4/Hw+7uroURiddO/omXscHBQba2tlheXiaZTDIxMQHA6uoqXq+X2dlZ4OMnSd+qsbExKisrn0xoPz8/JxQK4ff7CYVCT4YLz83NYRgGDQ0NrK+vv0gMn/ot7NL/RlhDkvgbUFdXV2i0pbUmGAwyOTlZ2GMuSeLe6OgomUzmyVqx/i2maZJKpdjf3yeTyTA1NfUiA7A9Hg+np6eF47/38wtRjCTxN0Yphc/nszqMV6mnp+ejUXTF+rek02lisRgul4va2loMwyCbzZYcQ3t7O4eHhxwdHXF7e0sqlWJgYKDk84ryJUlciGcU69/yqdp1Lpcr+XoOh4P5+XnC4TCNjY1Eo1Gam5tLPq8oX3JjU4j/4P+sXUciESKRyIucS5S/z027F+JNUUp9B/ymtW55OD4A3mmt/1BKfQtsaa0blFI/Amit5x4+tw78rLXesSh08UZJOUWI5/0KvH94/R5IP1qPKaVcSqlawA+UXhQX4gtJOUWIB0qpJeAd8I1S6nfgJ+AX4INS6gfgBPgeQGu9r5T6AJjAn8C01rr07SlCfCEppwghhI1JOUUIIWxMkrgQQtiYJHEhhLAxSeJCCGFjksSFEMLGJIkLIYSNSRIXQggbkyQuhBA29hcXUKoAC0uslAAAAABJRU5ErkJggg==
"
class="
jp-needs-light-background
"
>
</div>

</div>

</div>

</div>

</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell   ">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[11]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1"># Protein, Fat, and Carbs in 3D space, zoomed in even further.</span>
<span class="n">fig</span> <span class="o">=</span> <span class="n">plt</span><span class="o">.</span><span class="n">figure</span><span class="p">(</span><span class="n">figsize</span><span class="o">=</span><span class="p">(</span><span class="mi">6</span><span class="p">,</span> <span class="mi">6</span><span class="p">))</span>
<span class="n">ax</span> <span class="o">=</span> <span class="n">plt</span><span class="o">.</span><span class="n">axes</span><span class="p">(</span><span class="n">projection</span><span class="o">=</span><span class="s1">&#39;3d&#39;</span><span class="p">)</span>
<span class="n">ax</span><span class="o">.</span><span class="n">scatter</span><span class="p">(</span><span class="n">Protein</span><span class="p">,</span> <span class="n">Fat</span><span class="p">,</span> <span class="n">Carbs</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s2">&quot;Protein (g)&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s2">&quot;Total Fat (g)&quot;</span><span class="p">)</span>
<span class="n">ax</span><span class="o">.</span><span class="n">set_zlabel</span><span class="p">(</span><span class="s2">&quot;Carbohydrate (g)&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlim</span><span class="p">([</span><span class="mi">0</span><span class="p">,</span> <span class="mi">100</span><span class="p">])</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylim</span><span class="p">([</span><span class="mi">0</span><span class="p">,</span> <span class="mi">100</span><span class="p">])</span>
<span class="n">ax</span><span class="o">.</span><span class="n">set_zlim</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="mi">100</span><span class="p">)</span>
<span class="n">ax</span><span class="o">.</span><span class="n">spines</span><span class="p">[</span><span class="s1">&#39;top&#39;</span><span class="p">]</span><span class="o">.</span><span class="n">set_visible</span><span class="p">(</span><span class="kc">False</span><span class="p">)</span>
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




<div class="jp-RenderedImage jp-OutputArea-output ">
<img src="data:image/png;base64,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
"
class="
jp-needs-light-background
"
>
</div>

</div>

</div>

</div>

</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell   ">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[12]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1"># Protein and Carbs in 2D space</span>
<span class="n">plt</span><span class="o">.</span><span class="n">scatter</span><span class="p">(</span><span class="n">Protein</span><span class="p">,</span> <span class="n">Carbs</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s2">&quot;Protein (g)&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s2">&quot;Carbohydrate (g)&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlim</span><span class="p">([</span><span class="mi">0</span><span class="p">,</span> <span class="mi">100</span><span class="p">])</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylim</span><span class="p">([</span><span class="mi">0</span><span class="p">,</span> <span class="mi">100</span><span class="p">]);</span>
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




<div class="jp-RenderedImage jp-OutputArea-output ">
<img src="data:image/png;base64,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
"
class="
jp-needs-light-background
"
>
</div>

</div>

</div>

</div>

</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell   ">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[13]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1"># Protein and Fat in 2D space</span>
<span class="n">plt</span><span class="o">.</span><span class="n">scatter</span><span class="p">(</span><span class="n">Protein</span><span class="p">,</span> <span class="n">Fat</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s2">&quot;Protein (g)&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s2">&quot;Total Fat (g)&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlim</span><span class="p">([</span><span class="mi">0</span><span class="p">,</span> <span class="mi">100</span><span class="p">])</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylim</span><span class="p">([</span><span class="mi">0</span><span class="p">,</span> <span class="mi">100</span><span class="p">]);</span>
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




<div class="jp-RenderedImage jp-OutputArea-output ">
<img src="data:image/png;base64,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
"
class="
jp-needs-light-background
"
>
</div>

</div>

</div>

</div>

</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell   ">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[14]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1"># Carbs and Fat in 2D space</span>
<span class="n">plt</span><span class="o">.</span><span class="n">scatter</span><span class="p">(</span><span class="n">Carbs</span><span class="p">,</span> <span class="n">Fat</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s2">&quot;Carbohydrate (g)&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s2">&quot;Total Fat (g)&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlim</span><span class="p">([</span><span class="mi">0</span><span class="p">,</span> <span class="mi">100</span><span class="p">])</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylim</span><span class="p">([</span><span class="mi">0</span><span class="p">,</span> <span class="mi">100</span><span class="p">]);</span>
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




<div class="jp-RenderedImage jp-OutputArea-output ">
<img src="data:image/png;base64,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
"
class="
jp-needs-light-background
"
>
</div>

</div>

</div>

</div>

</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput " data-mime-type="text/markdown">
<h4 id="The-5-above-graphs-clearly-show-a-near-perfect-linear-correlation-in-3D-space-between-Protein,-Fat,-and-Carbs.">The 5 above graphs clearly show a near perfect linear correlation in 3D space between Protein, Fat, and Carbs.<a class="anchor-link" href="#The-5-above-graphs-clearly-show-a-near-perfect-linear-correlation-in-3D-space-between-Protein,-Fat,-and-Carbs.">&#182;</a></h4><h4 id="High-Protein-=-Low-Carbs-and-Fat,-High-Carbs-=-Low-Fat,-and-High-Fat-=-Low-Protein-and-Carbs.">High Protein = Low Carbs and Fat, High Carbs = Low Fat, and High Fat = Low Protein and Carbs.<a class="anchor-link" href="#High-Protein-=-Low-Carbs-and-Fat,-High-Carbs-=-Low-Fat,-and-High-Fat-=-Low-Protein-and-Carbs.">&#182;</a></h4>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput " data-mime-type="text/markdown">
<h1 id="Encountered-Problems">Encountered Problems<a class="anchor-link" href="#Encountered-Problems">&#182;</a></h1><ul>
<li>Lack of experience.</li>
<li>Time management with other classes/comitments.</li>
<li>Data munging and formatting takes a while.</li>
<li>LogisticRegression predictions may not be completly accurate.</li>
</ul>
<h1 id="Possible-Improvements">Possible Improvements<a class="anchor-link" href="#Possible-Improvements">&#182;</a></h1><ul>
<li>Start earlier! </li>
<li>Clean up the data better by normalizing and making sure more outlires are removed.</li>
<li>Study LogisticRegression further to fine tune predictions.</li>
</ul>
<h1 id="Final-Conclusions">Final Conclusions<a class="anchor-link" href="#Final-Conclusions">&#182;</a></h1><h3 id="As-shown-by-the-LogisticRegression-prediction-graphs-and-the-3D/2D-plots,-there-is-a-very-clear-relationship-between-Protein,-Fat,-and-Carbs-that-is-borderline-linear.">As shown by the LogisticRegression prediction graphs and the 3D/2D plots, there is a very clear relationship between Protein, Fat, and Carbs that is borderline linear.<a class="anchor-link" href="#As-shown-by-the-LogisticRegression-prediction-graphs-and-the-3D/2D-plots,-there-is-a-very-clear-relationship-between-Protein,-Fat,-and-Carbs-that-is-borderline-linear.">&#182;</a></h3><h3 id="The-higher-amount-of-protein,-the-lower-amount-of-carbs-and-fat.-The-higher-amount-of-carbs,-the-lower-amount-of-fat.-The-higher-amount-of-fat,-the-lower-amount-of-protein-and-carbs.">The higher amount of protein, the lower amount of carbs and fat. The higher amount of carbs, the lower amount of fat. The higher amount of fat, the lower amount of protein and carbs.<a class="anchor-link" href="#The-higher-amount-of-protein,-the-lower-amount-of-carbs-and-fat.-The-higher-amount-of-carbs,-the-lower-amount-of-fat.-The-higher-amount-of-fat,-the-lower-amount-of-protein-and-carbs.">&#182;</a></h3>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput " data-mime-type="text/markdown">
<h1 id="Sources">Sources<a class="anchor-link" href="#Sources">&#182;</a></h1><ul>
<li>Stat 196K Lectures/Examples provided by Professor Clark Fitzgerald</li>
<li><a href="https://www.usda.gov/">https://www.usda.gov/</a></li>
<li><a href="https://catalog.data.gov/dataset/supertracker-source-code-and-foods-database">https://catalog.data.gov/dataset/supertracker-source-code-and-foods-database</a></li>
<li><a href="https://stackoverflow.com/">https://stackoverflow.com/</a></li>
<li><a href="https://numpy.org/">https://numpy.org/</a></li>
<li><a href="https://scikit-learn.org/">https://scikit-learn.org/</a></li>
<li><a href="https://pandas.pydata.org/">https://pandas.pydata.org/</a></li>
<li><a href="https://www.youtube.com/">https://www.youtube.com/</a></li>
</ul>

</div>
</div>
</div>
</div>
</body>







</html>
