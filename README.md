<html><head><meta http-equiv="Content-Type" content="text/html; charset=utf-8"/><title>Every Linux Commands I know A-Z</title><style>
/* cspell:disable-file */
/* webkit printing magic: print all background colors */
html {
	-webkit-print-color-adjust: exact;
}
* {
	box-sizing: border-box;
	-webkit-print-color-adjust: exact;
}

html,
body {
	margin: 0;
	padding: 0;
}
@media only screen {
	body {
		margin: 2em auto;
		max-width: 900px;
		color: rgb(55, 53, 47);
	}
}

body {
	line-height: 1.5;
	white-space: pre-wrap;
}

a,
a.visited {
	color: inherit;
	text-decoration: underline;
}

.pdf-relative-link-path {
	font-size: 80%;
	color: #444;
}

h1,
h2,
h3 {
	letter-spacing: -0.01em;
	line-height: 1.2;
	font-weight: 600;
	margin-bottom: 0;
}

.page-title {
	font-size: 2.5rem;
	font-weight: 700;
	margin-top: 0;
	margin-bottom: 0.75em;
}

h1 {
	font-size: 1.875rem;
	margin-top: 1.875rem;
}

h2 {
	font-size: 1.5rem;
	margin-top: 1.5rem;
}

h3 {
	font-size: 1.25rem;
	margin-top: 1.25rem;
}

.source {
	border: 1px solid #ddd;
	border-radius: 3px;
	padding: 1.5em;
	word-break: break-all;
}

.callout {
	border-radius: 3px;
	padding: 1rem;
}

figure {
	margin: 1.25em 0;
	page-break-inside: avoid;
}

figcaption {
	opacity: 0.5;
	font-size: 85%;
	margin-top: 0.5em;
}

mark {
	background-color: transparent;
}

.indented {
	padding-left: 1.5em;
}

hr {
	background: transparent;
	display: block;
	width: 100%;
	height: 1px;
	visibility: visible;
	border: none;
	border-bottom: 1px solid rgba(55, 53, 47, 0.09);
}

img {
	max-width: 100%;
}

@media only print {
	img {
		max-height: 100vh;
		object-fit: contain;
	}
}

@page {
	margin: 1in;
}

.collection-content {
	font-size: 0.875rem;
}

.column-list {
	display: flex;
	justify-content: space-between;
}

.column {
	padding: 0 1em;
}

.column:first-child {
	padding-left: 0;
}

.column:last-child {
	padding-right: 0;
}

.table_of_contents-item {
	display: block;
	font-size: 0.875rem;
	line-height: 1.3;
	padding: 0.125rem;
}

.table_of_contents-indent-1 {
	margin-left: 1.5rem;
}

.table_of_contents-indent-2 {
	margin-left: 3rem;
}

.table_of_contents-indent-3 {
	margin-left: 4.5rem;
}

.table_of_contents-link {
	text-decoration: none;
	opacity: 0.7;
	border-bottom: 1px solid rgba(55, 53, 47, 0.18);
}

table,
th,
td {
	border: 1px solid rgba(55, 53, 47, 0.09);
	border-collapse: collapse;
}

table {
	border-left: none;
	border-right: none;
}

th,
td {
	font-weight: normal;
	padding: 0.25em 0.5em;
	line-height: 1.5;
	min-height: 1.5em;
	text-align: left;
}

th {
	color: rgba(55, 53, 47, 0.6);
}

ol,
ul {
	margin: 0;
	margin-block-start: 0.6em;
	margin-block-end: 0.6em;
}

li > ol:first-child,
li > ul:first-child {
	margin-block-start: 0.6em;
}

ul > li {
	list-style: disc;
}

ul.to-do-list {
	text-indent: -1.7em;
}

ul.to-do-list > li {
	list-style: none;
}

.to-do-children-checked {
	text-decoration: line-through;
	opacity: 0.375;
}

ul.toggle > li {
	list-style: none;
}

ul {
	padding-inline-start: 1.7em;
}

ul > li {
	padding-left: 0.1em;
}

ol {
	padding-inline-start: 1.6em;
}

ol > li {
	padding-left: 0.2em;
}

.mono ol {
	padding-inline-start: 2em;
}

.mono ol > li {
	text-indent: -0.4em;
}

.toggle {
	padding-inline-start: 0em;
	list-style-type: none;
}

/* Indent toggle children */
.toggle > li > details {
	padding-left: 1.7em;
}

.toggle > li > details > summary {
	margin-left: -1.1em;
}

.selected-value {
	display: inline-block;
	padding: 0 0.5em;
	background: rgba(206, 205, 202, 0.5);
	border-radius: 3px;
	margin-right: 0.5em;
	margin-top: 0.3em;
	margin-bottom: 0.3em;
	white-space: nowrap;
}

.collection-title {
	display: inline-block;
	margin-right: 1em;
}

.simple-table {
	margin-top: 1em;
	font-size: 0.875rem;
	empty-cells: show;
}
.simple-table td {
	height: 29px;
	min-width: 120px;
}

.simple-table th {
	height: 29px;
	min-width: 120px;
}

.simple-table-header-color {
	background: rgb(247, 246, 243);
	color: black;
}
.simple-table-header {
	font-weight: 500;
}

time {
	opacity: 0.5;
}

.icon {
	display: inline-block;
	max-width: 1.2em;
	max-height: 1.2em;
	text-decoration: none;
	vertical-align: text-bottom;
	margin-right: 0.5em;
}

img.icon {
	border-radius: 3px;
}

.user-icon {
	width: 1.5em;
	height: 1.5em;
	border-radius: 100%;
	margin-right: 0.5rem;
}

.user-icon-inner {
	font-size: 0.8em;
}

.text-icon {
	border: 1px solid #000;
	text-align: center;
}

.page-cover-image {
	display: block;
	object-fit: cover;
	width: 100%;
	max-height: 30vh;
}

.page-header-icon {
	font-size: 3rem;
	margin-bottom: 1rem;
}

.page-header-icon-with-cover {
	margin-top: -0.72em;
	margin-left: 0.07em;
}

.page-header-icon img {
	border-radius: 3px;
}

.link-to-page {
	margin: 1em 0;
	padding: 0;
	border: none;
	font-weight: 500;
}

p > .user {
	opacity: 0.5;
}

td > .user,
td > time {
	white-space: nowrap;
}

input[type="checkbox"] {
	transform: scale(1.5);
	margin-right: 0.6em;
	vertical-align: middle;
}

p {
	margin-top: 0.5em;
	margin-bottom: 0.5em;
}

.image {
	border: none;
	margin: 1.5em 0;
	padding: 0;
	border-radius: 0;
	text-align: center;
}

.code,
code {
	background: rgba(135, 131, 120, 0.15);
	border-radius: 3px;
	padding: 0.2em 0.4em;
	border-radius: 3px;
	font-size: 85%;
	tab-size: 2;
}

code {
	color: #eb5757;
}

.code {
	padding: 1.5em 1em;
}

.code-wrap {
	white-space: pre-wrap;
	word-break: break-all;
}

.code > code {
	background: none;
	padding: 0;
	font-size: 100%;
	color: inherit;
}

blockquote {
	font-size: 1.25em;
	margin: 1em 0;
	padding-left: 1em;
	border-left: 3px solid rgb(55, 53, 47);
}

.bookmark {
	text-decoration: none;
	max-height: 8em;
	padding: 0;
	display: flex;
	width: 100%;
	align-items: stretch;
}

.bookmark-title {
	font-size: 0.85em;
	overflow: hidden;
	text-overflow: ellipsis;
	height: 1.75em;
	white-space: nowrap;
}

.bookmark-text {
	display: flex;
	flex-direction: column;
}

.bookmark-info {
	flex: 4 1 180px;
	padding: 12px 14px 14px;
	display: flex;
	flex-direction: column;
	justify-content: space-between;
}

.bookmark-image {
	width: 33%;
	flex: 1 1 180px;
	display: block;
	position: relative;
	object-fit: cover;
	border-radius: 1px;
}

.bookmark-description {
	color: rgba(55, 53, 47, 0.6);
	font-size: 0.75em;
	overflow: hidden;
	max-height: 4.5em;
	word-break: break-word;
}

.bookmark-href {
	font-size: 0.75em;
	margin-top: 0.25em;
}

.sans { font-family: ui-sans-serif, -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, "Apple Color Emoji", Arial, sans-serif, "Segoe UI Emoji", "Segoe UI Symbol"; }
.code { font-family: "SFMono-Regular", Menlo, Consolas, "PT Mono", "Liberation Mono", Courier, monospace; }
.serif { font-family: Lyon-Text, Georgia, ui-serif, serif; }
.mono { font-family: iawriter-mono, Nitti, Menlo, Courier, monospace; }
.pdf .sans { font-family: Inter, ui-sans-serif, -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, "Apple Color Emoji", Arial, sans-serif, "Segoe UI Emoji", "Segoe UI Symbol", 'Twemoji', 'Noto Color Emoji', 'Noto Sans CJK JP'; }
.pdf:lang(zh-CN) .sans { font-family: Inter, ui-sans-serif, -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, "Apple Color Emoji", Arial, sans-serif, "Segoe UI Emoji", "Segoe UI Symbol", 'Twemoji', 'Noto Color Emoji', 'Noto Sans CJK SC'; }
.pdf:lang(zh-TW) .sans { font-family: Inter, ui-sans-serif, -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, "Apple Color Emoji", Arial, sans-serif, "Segoe UI Emoji", "Segoe UI Symbol", 'Twemoji', 'Noto Color Emoji', 'Noto Sans CJK TC'; }
.pdf:lang(ko-KR) .sans { font-family: Inter, ui-sans-serif, -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, "Apple Color Emoji", Arial, sans-serif, "Segoe UI Emoji", "Segoe UI Symbol", 'Twemoji', 'Noto Color Emoji', 'Noto Sans CJK KR'; }
.pdf .code { font-family: Source Code Pro, "SFMono-Regular", Menlo, Consolas, "PT Mono", "Liberation Mono", Courier, monospace, 'Twemoji', 'Noto Color Emoji', 'Noto Sans Mono CJK JP'; }
.pdf:lang(zh-CN) .code { font-family: Source Code Pro, "SFMono-Regular", Menlo, Consolas, "PT Mono", "Liberation Mono", Courier, monospace, 'Twemoji', 'Noto Color Emoji', 'Noto Sans Mono CJK SC'; }
.pdf:lang(zh-TW) .code { font-family: Source Code Pro, "SFMono-Regular", Menlo, Consolas, "PT Mono", "Liberation Mono", Courier, monospace, 'Twemoji', 'Noto Color Emoji', 'Noto Sans Mono CJK TC'; }
.pdf:lang(ko-KR) .code { font-family: Source Code Pro, "SFMono-Regular", Menlo, Consolas, "PT Mono", "Liberation Mono", Courier, monospace, 'Twemoji', 'Noto Color Emoji', 'Noto Sans Mono CJK KR'; }
.pdf .serif { font-family: PT Serif, Lyon-Text, Georgia, ui-serif, serif, 'Twemoji', 'Noto Color Emoji', 'Noto Serif CJK JP'; }
.pdf:lang(zh-CN) .serif { font-family: PT Serif, Lyon-Text, Georgia, ui-serif, serif, 'Twemoji', 'Noto Color Emoji', 'Noto Serif CJK SC'; }
.pdf:lang(zh-TW) .serif { font-family: PT Serif, Lyon-Text, Georgia, ui-serif, serif, 'Twemoji', 'Noto Color Emoji', 'Noto Serif CJK TC'; }
.pdf:lang(ko-KR) .serif { font-family: PT Serif, Lyon-Text, Georgia, ui-serif, serif, 'Twemoji', 'Noto Color Emoji', 'Noto Serif CJK KR'; }
.pdf .mono { font-family: PT Mono, iawriter-mono, Nitti, Menlo, Courier, monospace, 'Twemoji', 'Noto Color Emoji', 'Noto Sans Mono CJK JP'; }
.pdf:lang(zh-CN) .mono { font-family: PT Mono, iawriter-mono, Nitti, Menlo, Courier, monospace, 'Twemoji', 'Noto Color Emoji', 'Noto Sans Mono CJK SC'; }
.pdf:lang(zh-TW) .mono { font-family: PT Mono, iawriter-mono, Nitti, Menlo, Courier, monospace, 'Twemoji', 'Noto Color Emoji', 'Noto Sans Mono CJK TC'; }
.pdf:lang(ko-KR) .mono { font-family: PT Mono, iawriter-mono, Nitti, Menlo, Courier, monospace, 'Twemoji', 'Noto Color Emoji', 'Noto Sans Mono CJK KR'; }
.highlight-default {
	color: rgba(55, 53, 47, 1);
}
.highlight-gray {
	color: rgba(120, 119, 116, 1);
	fill: rgba(120, 119, 116, 1);
}
.highlight-brown {
	color: rgba(159, 107, 83, 1);
	fill: rgba(159, 107, 83, 1);
}
.highlight-orange {
	color: rgba(217, 115, 13, 1);
	fill: rgba(217, 115, 13, 1);
}
.highlight-yellow {
	color: rgba(203, 145, 47, 1);
	fill: rgba(203, 145, 47, 1);
}
.highlight-teal {
	color: rgba(68, 131, 97, 1);
	fill: rgba(68, 131, 97, 1);
}
.highlight-blue {
	color: rgba(51, 126, 169, 1);
	fill: rgba(51, 126, 169, 1);
}
.highlight-purple {
	color: rgba(144, 101, 176, 1);
	fill: rgba(144, 101, 176, 1);
}
.highlight-pink {
	color: rgba(193, 76, 138, 1);
	fill: rgba(193, 76, 138, 1);
}
.highlight-red {
	color: rgba(212, 76, 71, 1);
	fill: rgba(212, 76, 71, 1);
}
.highlight-gray_background {
	background: rgba(241, 241, 239, 1);
}
.highlight-brown_background {
	background: rgba(244, 238, 238, 1);
}
.highlight-orange_background {
	background: rgba(251, 236, 221, 1);
}
.highlight-yellow_background {
	background: rgba(251, 243, 219, 1);
}
.highlight-teal_background {
	background: rgba(237, 243, 236, 1);
}
.highlight-blue_background {
	background: rgba(231, 243, 248, 1);
}
.highlight-purple_background {
	background: rgba(244, 240, 247, 0.8);
}
.highlight-pink_background {
	background: rgba(249, 238, 243, 0.8);
}
.highlight-red_background {
	background: rgba(253, 235, 236, 1);
}
.block-color-default {
	color: inherit;
	fill: inherit;
}
.block-color-gray {
	color: rgba(120, 119, 116, 1);
	fill: rgba(120, 119, 116, 1);
}
.block-color-brown {
	color: rgba(159, 107, 83, 1);
	fill: rgba(159, 107, 83, 1);
}
.block-color-orange {
	color: rgba(217, 115, 13, 1);
	fill: rgba(217, 115, 13, 1);
}
.block-color-yellow {
	color: rgba(203, 145, 47, 1);
	fill: rgba(203, 145, 47, 1);
}
.block-color-teal {
	color: rgba(68, 131, 97, 1);
	fill: rgba(68, 131, 97, 1);
}
.block-color-blue {
	color: rgba(51, 126, 169, 1);
	fill: rgba(51, 126, 169, 1);
}
.block-color-purple {
	color: rgba(144, 101, 176, 1);
	fill: rgba(144, 101, 176, 1);
}
.block-color-pink {
	color: rgba(193, 76, 138, 1);
	fill: rgba(193, 76, 138, 1);
}
.block-color-red {
	color: rgba(212, 76, 71, 1);
	fill: rgba(212, 76, 71, 1);
}
.block-color-gray_background {
	background: rgba(241, 241, 239, 1);
}
.block-color-brown_background {
	background: rgba(244, 238, 238, 1);
}
.block-color-orange_background {
	background: rgba(251, 236, 221, 1);
}
.block-color-yellow_background {
	background: rgba(251, 243, 219, 1);
}
.block-color-teal_background {
	background: rgba(237, 243, 236, 1);
}
.block-color-blue_background {
	background: rgba(231, 243, 248, 1);
}
.block-color-purple_background {
	background: rgba(244, 240, 247, 0.8);
}
.block-color-pink_background {
	background: rgba(249, 238, 243, 0.8);
}
.block-color-red_background {
	background: rgba(253, 235, 236, 1);
}
.select-value-color-pink { background-color: rgba(245, 224, 233, 1); }
.select-value-color-purple { background-color: rgba(232, 222, 238, 1); }
.select-value-color-green { background-color: rgba(219, 237, 219, 1); }
.select-value-color-gray { background-color: rgba(227, 226, 224, 1); }
.select-value-color-opaquegray { background-color: rgba(255, 255, 255, 0.0375); }
.select-value-color-orange { background-color: rgba(250, 222, 201, 1); }
.select-value-color-brown { background-color: rgba(238, 224, 218, 1); }
.select-value-color-red { background-color: rgba(255, 226, 221, 1); }
.select-value-color-yellow { background-color: rgba(253, 236, 200, 1); }
.select-value-color-blue { background-color: rgba(211, 229, 239, 1); }

.checkbox {
	display: inline-flex;
	vertical-align: text-bottom;
	width: 16;
	height: 16;
	background-size: 16px;
	margin-left: 2px;
	margin-right: 5px;
}

.checkbox-on {
	background-image: url("data:image/svg+xml;charset=UTF-8,%3Csvg%20width%3D%2216%22%20height%3D%2216%22%20viewBox%3D%220%200%2016%2016%22%20fill%3D%22none%22%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%3E%0A%3Crect%20width%3D%2216%22%20height%3D%2216%22%20fill%3D%22%2358A9D7%22%2F%3E%0A%3Cpath%20d%3D%22M6.71429%2012.2852L14%204.9995L12.7143%203.71436L6.71429%209.71378L3.28571%206.2831L2%207.57092L6.71429%2012.2852Z%22%20fill%3D%22white%22%2F%3E%0A%3C%2Fsvg%3E");
}

.checkbox-off {
	background-image: url("data:image/svg+xml;charset=UTF-8,%3Csvg%20width%3D%2216%22%20height%3D%2216%22%20viewBox%3D%220%200%2016%2016%22%20fill%3D%22none%22%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%3E%0A%3Crect%20x%3D%220.75%22%20y%3D%220.75%22%20width%3D%2214.5%22%20height%3D%2214.5%22%20fill%3D%22white%22%20stroke%3D%22%2336352F%22%20stroke-width%3D%221.5%22%2F%3E%0A%3C%2Fsvg%3E");
}
	
</style></head><body><article id="677fa7a2-11e5-4eb1-bbac-79ffd6d5373e" class="page sans"><header><img class="page-cover-image" src="https://images.unsplash.com/photo-1550745165-9bc0b252726f?ixlib=rb-1.2.1&amp;q=80&amp;cs=tinysrgb&amp;fm=jpg&amp;crop=entropy" style="object-position:center 50%"/><div class="page-header-icon page-header-icon-with-cover"><span class="icon">🐧</span></div><h1 class="page-title">Every Linux Commands I know A-Z</h1></header><div class="page-body"><figure class="block-color-gray_background callout" style="white-space:pre-wrap;display:flex" id="dae7f874-da73-4be4-97f1-db070114a55a"><div style="font-size:1.5em"><span class="icon">💡</span></div><div style="width:100%">Follow me on twitter: twitter.com/xtremepentest</div></figure><p id="a2b2bd5b-41d2-423c-a30f-72735201621c" class="">
</p><div id="b79c651b-9dc5-4e28-a6dd-737dbd6c54f4" class="collection-content"><h4 class="collection-title"></h4><table class="collection-content"><thead><tr><th><span class="icon property-icon"><svg viewBox="0 0 14 14" style="width:14px;height:14px;display:block;fill:rgba(55, 53, 47, 0.45);flex-shrink:0;-webkit-backface-visibility:hidden" class="typesTitle"><path d="M7.73943662,8.6971831 C7.77640845,8.7834507 7.81338028,8.8943662 7.81338028,9.00528169 C7.81338028,9.49823944 7.40669014,9.89260563 6.91373239,9.89260563 C6.53169014,9.89260563 6.19894366,9.64612676 6.08802817,9.30105634 L5.75528169,8.33978873 L2.05809859,8.33978873 L1.72535211,9.30105634 C1.61443662,9.64612676 1.2693662,9.89260563 0.887323944,9.89260563 C0.394366197,9.89260563 0,9.49823944 0,9.00528169 C0,8.8943662 0.0246478873,8.7834507 0.0616197183,8.6971831 L2.46478873,2.48591549 C2.68661972,1.90669014 3.24119718,1.5 3.90669014,1.5 C4.55985915,1.5 5.12676056,1.90669014 5.34859155,2.48591549 L7.73943662,8.6971831 Z M2.60035211,6.82394366 L5.21302817,6.82394366 L3.90669014,3.10211268 L2.60035211,6.82394366 Z M11.3996479,3.70598592 C12.7552817,3.70598592 14,4.24823944 14,5.96126761 L14,9.07922535 C14,9.52288732 13.6549296,9.89260563 13.2112676,9.89260563 C12.8169014,9.89260563 12.471831,9.59683099 12.4225352,9.19014085 C12.028169,9.6584507 11.3257042,9.95422535 10.5492958,9.95422535 C9.60035211,9.95422535 8.47887324,9.31338028 8.47887324,7.98239437 C8.47887324,6.58978873 9.60035211,6.08450704 10.5492958,6.08450704 C11.3380282,6.08450704 12.040493,6.33098592 12.4348592,6.81161972 L12.4348592,5.98591549 C12.4348592,5.38204225 11.9172535,4.98767606 11.1285211,4.98767606 C10.6602113,4.98767606 10.2411972,5.11091549 9.80985915,5.38204225 C9.72359155,5.43133803 9.61267606,5.46830986 9.50176056,5.46830986 C9.18133803,5.46830986 8.91021127,5.1971831 8.91021127,4.86443662 C8.91021127,4.64260563 9.0334507,4.44542254 9.19366197,4.34683099 C9.87147887,3.90316901 10.6232394,3.70598592 11.3996479,3.70598592 Z M11.1778169,8.8943662 C11.6830986,8.8943662 12.1760563,8.72183099 12.4348592,8.37676056 L12.4348592,7.63732394 C12.1760563,7.29225352 11.6830986,7.11971831 11.1778169,7.11971831 C10.5616197,7.11971831 10.056338,7.45246479 10.056338,8.0193662 C10.056338,8.57394366 10.5616197,8.8943662 11.1778169,8.8943662 Z M0.65625,11.125 L13.34375,11.125 C13.7061869,11.125 14,11.4188131 14,11.78125 C14,12.1436869 13.7061869,12.4375 13.34375,12.4375 L0.65625,12.4375 C0.293813133,12.4375 4.43857149e-17,12.1436869 0,11.78125 C-4.43857149e-17,11.4188131 0.293813133,11.125 0.65625,11.125 Z"></path></svg></span>A</th><th><span class="icon property-icon"><svg viewBox="0 0 14 14" style="width:14px;height:14px;display:block;fill:rgba(55, 53, 47, 0.45);flex-shrink:0;-webkit-backface-visibility:hidden" class="typesText"><path d="M7,4.56818 C7,4.29204 6.77614,4.06818 6.5,4.06818 L0.5,4.06818 C0.223858,4.06818 0,4.29204 0,4.56818 L0,5.61364 C0,5.88978 0.223858,6.11364 0.5,6.11364 L6.5,6.11364 C6.77614,6.11364 7,5.88978 7,5.61364 L7,4.56818 Z M0.5,1 C0.223858,1 0,1.223858 0,1.5 L0,2.54545 C0,2.8216 0.223858,3.04545 0.5,3.04545 L12.5,3.04545 C12.7761,3.04545 13,2.8216 13,2.54545 L13,1.5 C13,1.223858 12.7761,1 12.5,1 L0.5,1 Z M0,8.68182 C0,8.95796 0.223858,9.18182 0.5,9.18182 L11.5,9.18182 C11.7761,9.18182 12,8.95796 12,8.68182 L12,7.63636 C12,7.36022 11.7761,7.13636 11.5,7.13636 L0.5,7.13636 C0.223858,7.13636 0,7.36022 0,7.63636 L0,8.68182 Z M0,11.75 C0,12.0261 0.223858,12.25 0.5,12.25 L9.5,12.25 C9.77614,12.25 10,12.0261 10,11.75 L10,10.70455 C10,10.4284 9.77614,10.20455 9.5,10.20455 L0.5,10.20455 C0.223858,10.20455 0,10.4284 0,10.70455 L0,11.75 Z"></path></svg></span>Command</th><th><span class="icon property-icon"><svg viewBox="0 0 14 14" style="width:14px;height:14px;display:block;fill:rgba(55, 53, 47, 0.45);flex-shrink:0;-webkit-backface-visibility:hidden" class="typesText"><path d="M7,4.56818 C7,4.29204 6.77614,4.06818 6.5,4.06818 L0.5,4.06818 C0.223858,4.06818 0,4.29204 0,4.56818 L0,5.61364 C0,5.88978 0.223858,6.11364 0.5,6.11364 L6.5,6.11364 C6.77614,6.11364 7,5.88978 7,5.61364 L7,4.56818 Z M0.5,1 C0.223858,1 0,1.223858 0,1.5 L0,2.54545 C0,2.8216 0.223858,3.04545 0.5,3.04545 L12.5,3.04545 C12.7761,3.04545 13,2.8216 13,2.54545 L13,1.5 C13,1.223858 12.7761,1 12.5,1 L0.5,1 Z M0,8.68182 C0,8.95796 0.223858,9.18182 0.5,9.18182 L11.5,9.18182 C11.7761,9.18182 12,8.95796 12,8.68182 L12,7.63636 C12,7.36022 11.7761,7.13636 11.5,7.13636 L0.5,7.13636 C0.223858,7.13636 0,7.36022 0,7.63636 L0,8.68182 Z M0,11.75 C0,12.0261 0.223858,12.25 0.5,12.25 L9.5,12.25 C9.77614,12.25 10,12.0261 10,11.75 L10,10.70455 C10,10.4284 9.77614,10.20455 9.5,10.20455 L0.5,10.20455 C0.223858,10.20455 0,10.4284 0,10.70455 L0,11.75 Z"></path></svg></span>Command Description</th></tr></thead><tbody><tr id="40ba77ae-2a04-4d0c-b910-2869081de90b"><td class="cell-title"><a href="https://www.notion.so/40ba77ae2a044d0cb9102869081de90b">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/bg.html">&amp;</a></td><td class="cell-yrFK">Start a new process in the background</td></tr><tr id="ec52d5bf-dfad-47c6-a4f7-53f38c29cf99"><td class="cell-title"><a href="https://www.notion.so/ec52d5bfdfad47c6a4f753f38c29cf99">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/alias.html">alias</a></td><td class="cell-yrFK">Create an alias •</td></tr><tr id="79e4d412-a971-4a69-86d0-3df9628f4ff6"><td class="cell-title"><a href="https://www.notion.so/79e4d412a9714a6986d03df9628f4ff6">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/apropos.html">apropos</a></td><td class="cell-yrFK">Search Help manual pages (man -k)</td></tr><tr id="398d6736-d2e7-4cc7-954c-63de172fbf7b"><td class="cell-title"><a href="https://www.notion.so/398d6736d2e74cc7954c63de172fbf7b">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/apt.html">apt</a></td><td class="cell-yrFK">Search for and install software packages (Debian/Ubuntu)</td></tr><tr id="af110b2a-7621-4ea1-9660-58f124fbf93a"><td class="cell-title"><a href="https://www.notion.so/af110b2a76214ea1966058f124fbf93a">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/apt-get.html">apt-get</a></td><td class="cell-yrFK">Search for and install software packages (Debian/Ubuntu)</td></tr><tr id="9306ad63-0ddf-4310-be91-fd31837d7d2a"><td class="cell-title"><a href="https://www.notion.so/9306ad630ddf4310be91fd31837d7d2a">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/aptitude.html">aptitude</a></td><td class="cell-yrFK">Search for and install software packages (Debian/Ubuntu)</td></tr><tr id="df8fa215-d4bb-4369-b8d9-00fb76106905"><td class="cell-title"><a href="https://www.notion.so/df8fa215d4bb4369b8d900fb76106905">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/aspell.html">aspell</a></td><td class="cell-yrFK">Spell Checker</td></tr><tr id="34041712-234e-457e-aec5-0489b04df20c"><td class="cell-title"><a href="https://www.notion.so/34041712234e457eaec50489b04df20c">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/at.html">at</a></td><td class="cell-yrFK">Schedule a command to run once at a particular time</td></tr><tr id="e3be2692-400e-4a6d-85ce-c20a83dc9ce0"><td class="cell-title"><a href="https://www.notion.so/e3be2692400e4a6d85cec20a83dc9ce0">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/awk.html">awk</a></td><td class="cell-yrFK">Find and Replace text, database sort/validate/index</td></tr><tr id="f13c280c-32c3-4021-ba46-436ccb2f9ad6"><td class="cell-title"><a href="https://www.notion.so/B-f13c280c32c34021ba46436ccb2f9ad6">B</a></td><td class="cell-RMJm"></td><td class="cell-yrFK"></td></tr><tr id="dbb40f4b-4641-4950-be18-69fb3aaac981"><td class="cell-title"><a href="https://www.notion.so/dbb40f4b46414950be1869fb3aaac981">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/basename.html">basename</a></td><td class="cell-yrFK">Strip directory and suffix from filenames</td></tr><tr id="c7c29b34-d7e3-470f-9718-e1de95a5a7d8"><td class="cell-title"><a href="https://www.notion.so/c7c29b34d7e3470f9718e1de95a5a7d8">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/base32.html">base32</a></td><td class="cell-yrFK">Base32 encode/decode data and print to standard output</td></tr><tr id="9bcff2c2-7fc3-4008-a260-b91b4a2404c5"><td class="cell-title"><a href="https://www.notion.so/9bcff2c27fc34008a260b91b4a2404c5">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/base64.html">base64</a></td><td class="cell-yrFK">Base64 encode/decode data and print to standard output</td></tr><tr id="dbb6ef13-5c6d-454b-94b2-a1335da08e36"><td class="cell-title"><a href="https://www.notion.so/dbb6ef135c6d454b94b2a1335da08e36">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/bash.html">bash</a></td><td class="cell-yrFK">GNU Bourne-Again SHell</td></tr><tr id="a7f86e47-6e6b-410e-a8e0-ef0555d5cffd"><td class="cell-title"><a href="https://www.notion.so/a7f86e476e6b410ea8e0ef0555d5cffd">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/bc.html">bc</a></td><td class="cell-yrFK">Arbitrary precision calculator language</td></tr><tr id="24a67b37-5106-476f-9216-3860d3ff3a8a"><td class="cell-title"><a href="https://www.notion.so/24a67b375106476f92163860d3ff3a8a">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/bg.html">bg</a></td><td class="cell-yrFK">Send to background</td></tr><tr id="068c3f30-8e05-46fb-ac72-ecad49250aba"><td class="cell-title"><a href="https://www.notion.so/068c3f308e0546fbac72ecad49250aba">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/bind.html">bind</a></td><td class="cell-yrFK">Set or display readline key and function bindings •</td></tr><tr id="c8bfefed-3e93-409c-a152-8836f9043d8e"><td class="cell-title"><a href="https://www.notion.so/c8bfefed3e93409ca1528836f9043d8e">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/break.html">break</a></td><td class="cell-yrFK">Exit from a loop •</td></tr><tr id="75d7663c-21b9-424d-80ed-84139eaa63fb"><td class="cell-title"><a href="https://www.notion.so/75d7663c21b9424d80ed84139eaa63fb">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/builtin.html">builtin</a></td><td class="cell-yrFK">Run a shell builtin</td></tr><tr id="fc0ef1ff-2575-43ca-a749-508b7b100ea2"><td class="cell-title"><a href="https://www.notion.so/fc0ef1ff257543caa749508b7b100ea2">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/bzip2.html">bzip2</a></td><td class="cell-yrFK">Compress or decompress named file(s)</td></tr><tr id="e3b935e0-da6e-44e6-8eb9-7c802fd4f943"><td class="cell-title"><a href="https://www.notion.so/C-e3b935e0da6e44e68eb97c802fd4f943">C</a></td><td class="cell-RMJm"></td><td class="cell-yrFK"></td></tr><tr id="c33cb1c4-4289-4dd9-a792-3ead09cc1d9a"><td class="cell-title"><a href="https://www.notion.so/c33cb1c442894dd9a7923ead09cc1d9a">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/cal.html">cal</a></td><td class="cell-yrFK">Display a calendar</td></tr><tr id="f16e802d-8eb5-4371-a2bb-2bf43b9f2fc6"><td class="cell-title"><a href="https://www.notion.so/f16e802d8eb54371a2bb2bf43b9f2fc6">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/caller.html">caller</a></td><td class="cell-yrFK">Return the context of any active subroutine call •</td></tr><tr id="ffc7cd78-e246-4eb3-8a9f-b2e58b019e30"><td class="cell-title"><a href="https://www.notion.so/ffc7cd78e2464eb38a9fb2e58b019e30">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/case.html">case</a></td><td class="cell-yrFK">Conditionally perform a command</td></tr><tr id="600d3126-f544-4be1-ad9e-a2750af846f2"><td class="cell-title"><a href="https://www.notion.so/600d3126f5444be1ad9ea2750af846f2">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/cat.html">cat</a></td><td class="cell-yrFK">Concatenate and print (display) the content of files</td></tr><tr id="73d31b59-2492-43c5-9778-c7efa199aa72"><td class="cell-title"><a href="https://www.notion.so/73d31b59249243c59778c7efa199aa72">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/cd.html">cd</a></td><td class="cell-yrFK">Change Directory</td></tr><tr id="cb3cbfa6-3ca6-4f50-b02d-adfccffc582f"><td class="cell-title"><a href="https://www.notion.so/cb3cbfa63ca64f50b02dadfccffc582f">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/cfdisk.html">cfdisk</a></td><td class="cell-yrFK">Partition table manipulator for Linux</td></tr><tr id="ef377cc4-208c-4d9c-8945-91950f43e280"><td class="cell-title"><a href="https://www.notion.so/ef377cc4208c4d9c894591950f43e280">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/chattr.html">chattr</a></td><td class="cell-yrFK">Change file attributes on a Linux file system</td></tr><tr id="eb755a35-caa3-4ec4-9920-bfe38fa4fc01"><td class="cell-title"><a href="https://www.notion.so/eb755a35caa34ec49920bfe38fa4fc01">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/chgrp.html">chgrp</a></td><td class="cell-yrFK">Change group ownership</td></tr><tr id="0ba5c2b4-fdd0-484e-bb1c-3b9553a68a77"><td class="cell-title"><a href="https://www.notion.so/0ba5c2b4fdd0484ebb1c3b9553a68a77">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/chmod.html">chmod</a></td><td class="cell-yrFK">Change access permissions</td></tr><tr id="3c32108d-eb68-4601-8d20-982ba5dc1d05"><td class="cell-title"><a href="https://www.notion.so/3c32108deb6846018d20982ba5dc1d05">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/chown.html">chown</a></td><td class="cell-yrFK">Change file owner and group</td></tr><tr id="16015028-6a74-4be8-a3e6-b0f9549ea309"><td class="cell-title"><a href="https://www.notion.so/160150286a744be8a3e6b0f9549ea309">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/chpasswd.html">chpasswd</a></td><td class="cell-yrFK">Update passwords in batch mode</td></tr><tr id="c127ccbf-4ea9-4b77-9fc6-be2b76f9bb13"><td class="cell-title"><a href="https://www.notion.so/c127ccbf4ea94b779fc6be2b76f9bb13">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/chroot.html">chroot</a></td><td class="cell-yrFK">Run a command with a different root directory</td></tr><tr id="4e469a59-de37-4c4b-ae98-e7655b6f29ff"><td class="cell-title"><a href="https://www.notion.so/4e469a59de374c4bae98e7655b6f29ff">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/chkconfig.html">chkconfig</a></td><td class="cell-yrFK">System services (runlevel)</td></tr><tr id="64bdb417-56f5-409f-90b0-12540cb924c3"><td class="cell-title"><a href="https://www.notion.so/64bdb41756f5409f90b012540cb924c3">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/cksum.html">cksum</a></td><td class="cell-yrFK">Print CRC checksum and byte counts</td></tr><tr id="8c383c71-a65b-414e-9590-796991bb129e"><td class="cell-title"><a href="https://www.notion.so/8c383c71a65b414e9590796991bb129e">Untitled</a></td><td class="cell-RMJm">clear</td><td class="cell-yrFK">Clear terminal screen</td></tr><tr id="35750b26-c2ea-4d61-9bf9-46d87723e1ee"><td class="cell-title"><a href="https://www.notion.so/35750b26c2ea4d619bf946d87723e1ee">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/cmp.html">cmp</a></td><td class="cell-yrFK">Compare two files</td></tr><tr id="ddc74fb2-cf18-479c-881d-22ce3ee0f424"><td class="cell-title"><a href="https://www.notion.so/ddc74fb2cf18479c881d22ce3ee0f424">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/comm.html">comm</a></td><td class="cell-yrFK">Compare two sorted files line by line</td></tr><tr id="38fb42f5-c610-434f-a652-d21bcc8b7429"><td class="cell-title"><a href="https://www.notion.so/38fb42f5c610434fa652d21bcc8b7429">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/command.html">command</a></td><td class="cell-yrFK">Run a command - ignoring shell functions •</td></tr><tr id="d75cd835-28e7-4140-9b92-9071b1288188"><td class="cell-title"><a href="https://www.notion.so/d75cd83528e741409b929071b1288188">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/continue.html">continue</a></td><td class="cell-yrFK">Resume the next iteration of a loop •</td></tr><tr id="d24fe233-59cd-4dd3-bb93-037b4b446182"><td class="cell-title"><a href="https://www.notion.so/d24fe23359cd4dd3bb93037b4b446182">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/cp.html">cp</a></td><td class="cell-yrFK">Copy one or more files to another location</td></tr><tr id="e64f8629-ef1f-4eb2-8713-35f7ca64cffd"><td class="cell-title"><a href="https://www.notion.so/e64f8629ef1f4eb2871335f7ca64cffd">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/cpio.html">cpio</a></td><td class="cell-yrFK">Copy files to and from archives</td></tr><tr id="5a095528-8d2d-4f34-a993-ae5cd544d257"><td class="cell-title"><a href="https://www.notion.so/5a0955288d2d4f34a993ae5cd544d257">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/cron.html">cron</a></td><td class="cell-yrFK">Daemon to execute scheduled commands</td></tr><tr id="7f4055da-bc82-4b6c-af3e-f51fa8c05def"><td class="cell-title"><a href="https://www.notion.so/7f4055dabc824b6caf3ef51fa8c05def">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/crontab.html">crontab</a></td><td class="cell-yrFK">Schedule a command to run at a later time</td></tr><tr id="ff5b056c-c4f1-4ee2-a334-297d7a9886b6"><td class="cell-title"><a href="https://www.notion.so/ff5b056cc4f14ee2a334297d7a9886b6">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/csplit.html">csplit</a></td><td class="cell-yrFK">Split a file into context-determined pieces</td></tr><tr id="bce15df9-0c9f-4abd-9fdd-50945e28c53c"><td class="cell-title"><a href="https://www.notion.so/bce15df90c9f4abd9fdd50945e28c53c">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/curl.html">curl</a></td><td class="cell-yrFK">Transfer data from or to a server</td></tr><tr id="006fcb99-480c-4880-b7ba-8c43ca1badf2"><td class="cell-title"><a href="https://www.notion.so/006fcb99480c4880b7ba8c43ca1badf2">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/cut.html">cut</a></td><td class="cell-yrFK">Divide a file into several parts</td></tr><tr id="8b387013-f538-46f8-80dc-c99946ef579c"><td class="cell-title"><a href="https://www.notion.so/D-8b387013f53846f880dcc99946ef579c">D</a></td><td class="cell-RMJm"></td><td class="cell-yrFK"></td></tr><tr id="ca59f238-01bb-45f7-9f22-2a3f62876138"><td class="cell-title"><a href="https://www.notion.so/ca59f23801bb45f79f222a3f62876138">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/date.html">date</a></td><td class="cell-yrFK">Display or change the date &amp; time</td></tr><tr id="2e40f8cc-3888-4c4a-8c1c-aea51d873b78"><td class="cell-title"><a href="https://www.notion.so/2e40f8cc38884c4a8c1caea51d873b78">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/dc.html">dc</a></td><td class="cell-yrFK">Desk Calculator</td></tr><tr id="0e891d08-6edd-4a46-ad30-a3eb6aa35a99"><td class="cell-title"><a href="https://www.notion.so/0e891d086edd4a46ad30a3eb6aa35a99">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/dd.html">dd</a></td><td class="cell-yrFK">Data Duplicator - convert and copy a file, write disk headers, boot records</td></tr><tr id="865f4d50-a908-42e3-9154-8dc086bd5894"><td class="cell-title"><a href="https://www.notion.so/865f4d50a90842e391548dc086bd5894">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/ddrescue.html">ddrescue</a></td><td class="cell-yrFK">Data recovery tool</td></tr><tr id="52424d6a-32e9-4cb3-b857-58816de12dda"><td class="cell-title"><a href="https://www.notion.so/52424d6a32e94cb3b85758816de12dda">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/declare.html">declare</a></td><td class="cell-yrFK">Declare variables and give them attributes •</td></tr><tr id="93077ee3-b514-4c1f-9e05-df0450c454ca"><td class="cell-title"><a href="https://www.notion.so/93077ee3b5144c1f9e05df0450c454ca">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/df.html">df</a></td><td class="cell-yrFK">Display free disk space</td></tr><tr id="14bead31-a91a-4f38-8461-b8a63c2e0fe3"><td class="cell-title"><a href="https://www.notion.so/14bead31a91a4f388461b8a63c2e0fe3">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/diff.html">diff</a></td><td class="cell-yrFK">Display the differences between two files</td></tr><tr id="dec22a4a-b757-4204-b823-baf00ea4b2de"><td class="cell-title"><a href="https://www.notion.so/dec22a4ab7574204b823baf00ea4b2de">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/diff3.html">diff3</a></td><td class="cell-yrFK">Show differences among three files</td></tr><tr id="29df6792-8281-4528-a4b8-0f76803674be"><td class="cell-title"><a href="https://www.notion.so/29df679282814528a4b80f76803674be">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/dig.html">dig</a></td><td class="cell-yrFK">DNS lookup</td></tr><tr id="12c977dd-911b-477f-90f4-38cc275699be"><td class="cell-title"><a href="https://www.notion.so/12c977dd911b477f90f438cc275699be">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/dir.html">dir</a></td><td class="cell-yrFK">Briefly list directory contents</td></tr><tr id="d0e3a5e7-56a9-4115-a1b0-f274e1601e2d"><td class="cell-title"><a href="https://www.notion.so/d0e3a5e756a94115a1b0f274e1601e2d">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/dircolors.html">dircolors</a></td><td class="cell-yrFK">Colour setup for &#x27;ls&#x27;</td></tr><tr id="a5545cad-2bac-4c08-86b1-0ab0f4b6ef8a"><td class="cell-title"><a href="https://www.notion.so/a5545cad2bac4c0886b10ab0f4b6ef8a">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/dirname.html">dirname</a></td><td class="cell-yrFK">Convert a full pathname to just a path</td></tr><tr id="e5dad9f2-f12f-402e-be46-8f8ded7013f7"><td class="cell-title"><a href="https://www.notion.so/e5dad9f2f12f402ebe468f8ded7013f7">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/dirs.html">dirs</a></td><td class="cell-yrFK">Display list of remembered directories</td></tr><tr id="93a17145-75a3-4c4d-a483-afe51cd9f4f0"><td class="cell-title"><a href="https://www.notion.so/93a1714575a34c4da483afe51cd9f4f0">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/dos2unix.html">dos2unix</a></td><td class="cell-yrFK">Windows/MAC to UNIX text file format converter</td></tr><tr id="c0f7eb38-bf35-4587-824f-2e94ba09cf95"><td class="cell-title"><a href="https://www.notion.so/c0f7eb38bf354587824f2e94ba09cf95">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/dmesg.html">dmesg</a></td><td class="cell-yrFK">Print kernel &amp; driver messages</td></tr><tr id="5e9e3943-a4b6-491e-898f-34566ead8ae1"><td class="cell-title"><a href="https://www.notion.so/5e9e3943a4b6491e898f34566ead8ae1">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/dpkg.html">dpkg</a></td><td class="cell-yrFK">Package manager (Debian/Ubuntu).</td></tr><tr id="f6f8b01d-b43a-479d-89a5-da445d8016d8"><td class="cell-title"><a href="https://www.notion.so/f6f8b01db43a479d89a5da445d8016d8">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/du.html">du</a></td><td class="cell-yrFK">Estimate file space usage</td></tr><tr id="f6516799-4dd9-42d7-8977-8bab2cd82487"><td class="cell-title"><a href="https://www.notion.so/E-f65167994dd942d789778bab2cd82487">E</a></td><td class="cell-RMJm"></td><td class="cell-yrFK"></td></tr><tr id="41eb512a-fbbe-4e8a-b46e-c8ac1963db89"><td class="cell-title"><a href="https://www.notion.so/41eb512afbbe4e8ab46ec8ac1963db89">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/echo.html">echo</a></td><td class="cell-yrFK">Display message on screen •</td></tr><tr id="c9078f34-95a2-4d41-96bd-b0dcef9cc3c3"><td class="cell-title"><a href="https://www.notion.so/c9078f3495a24d4196bdb0dcef9cc3c3">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/egrep.html">egrep</a></td><td class="cell-yrFK">Search file(s) for lines that match an extended expression</td></tr><tr id="11378d63-0cde-4609-b480-46f59a5185d3"><td class="cell-title"><a href="https://www.notion.so/11378d630cde4609b48046f59a5185d3">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/eject.html">eject</a></td><td class="cell-yrFK">Eject removable media</td></tr><tr id="24cab878-0ebc-4902-af48-f276de21d879"><td class="cell-title"><a href="https://www.notion.so/24cab8780ebc4902af48f276de21d879">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/enable.html">enable</a></td><td class="cell-yrFK">Enable and disable builtin shell commands •</td></tr><tr id="4026d5df-58a8-4733-b782-a59d20d58535"><td class="cell-title"><a href="https://www.notion.so/4026d5df58a84733b782a59d20d58535">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/env.html">env</a></td><td class="cell-yrFK">Environment variables</td></tr><tr id="4a96bb4c-b6fb-49ac-b4eb-f35051cfc735"><td class="cell-title"><a href="https://www.notion.so/4a96bb4cb6fb49acb4ebf35051cfc735">Untitled</a></td><td class="cell-RMJm">ethtool</td><td class="cell-yrFK">Ethernet card settings</td></tr><tr id="943567e5-c8a0-4cc1-97aa-b7cd2e84548d"><td class="cell-title"><a href="https://www.notion.so/943567e5c8a04cc197aab7cd2e84548d">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/eval.html">eval</a></td><td class="cell-yrFK">Evaluate several commands/arguments</td></tr><tr id="c5bec20a-a35a-4204-a3a8-46284a85a7fe"><td class="cell-title"><a href="https://www.notion.so/c5bec20aa35a4204a3a846284a85a7fe">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/exec.html">exec</a></td><td class="cell-yrFK">Execute a command</td></tr><tr id="80eb5bca-18ba-44ce-aa1a-6b983a2618fa"><td class="cell-title"><a href="https://www.notion.so/80eb5bca18ba44ceaa1a6b983a2618fa">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/exit.html">exit</a></td><td class="cell-yrFK">Exit the shell</td></tr><tr id="9db4a049-a65c-48f3-ab90-211d87c46983"><td class="cell-title"><a href="https://www.notion.so/9db4a049a65c48f3ab90211d87c46983">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/expand.html">expand</a></td><td class="cell-yrFK">Convert tabs to spaces</td></tr><tr id="896a40a2-77fc-4731-b81d-c6e360996946"><td class="cell-title"><a href="https://www.notion.so/896a40a277fc4731b81dc6e360996946">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/export.html">export</a></td><td class="cell-yrFK">Set an environment variable</td></tr><tr id="5131d54d-0bad-4925-9ff9-8b0b4ba44d9c"><td class="cell-title"><a href="https://www.notion.so/5131d54d0bad49259ff98b0b4ba44d9c">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/expr.html">expr</a></td><td class="cell-yrFK">Evaluate expressions</td></tr><tr id="caab9711-3f90-4888-8258-5a001f7d18ee"><td class="cell-title"><a href="https://www.notion.so/F-caab97113f90488882585a001f7d18ee">F</a></td><td class="cell-RMJm"></td><td class="cell-yrFK"></td></tr><tr id="749a76e3-efd0-4c75-9ae8-21cb9428dd12"><td class="cell-title"><a href="https://www.notion.so/749a76e3efd04c759ae821cb9428dd12">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/false.html">false</a></td><td class="cell-yrFK">Do nothing, unsuccessfully</td></tr><tr id="9048c924-52c9-4e78-b526-5f9560bd27fc"><td class="cell-title"><a href="https://www.notion.so/9048c92452c94e78b5265f9560bd27fc">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/fdformat.html">fdformat</a></td><td class="cell-yrFK">Low-level format a floppy disk</td></tr><tr id="f42031a6-587d-4549-b629-1f0eae1f55c7"><td class="cell-title"><a href="https://www.notion.so/f42031a6587d4549b6291f0eae1f55c7">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/fdisk.html">fdisk</a></td><td class="cell-yrFK">Partition table manipulator for Linux</td></tr><tr id="79c690ce-52a0-461e-9de5-7206b29049e3"><td class="cell-title"><a href="https://www.notion.so/79c690ce52a0461e9de57206b29049e3">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/fg.html">fg</a></td><td class="cell-yrFK">Send job to foreground</td></tr><tr id="a2035c1a-02b9-4890-85c4-18f324dbadeb"><td class="cell-title"><a href="https://www.notion.so/a2035c1a02b9489085c418f324dbadeb">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/fgrep.html">fgrep</a></td><td class="cell-yrFK">Search file(s) for lines that match a fixed string</td></tr><tr id="d578ca72-112f-4d72-8253-daa65377f4cf"><td class="cell-title"><a href="https://www.notion.so/d578ca72112f4d728253daa65377f4cf">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/file.html">file</a></td><td class="cell-yrFK">Determine file type</td></tr><tr id="6121aae0-eeb1-46fb-aa27-23f2bf5dbd34"><td class="cell-title"><a href="https://www.notion.so/6121aae0eeb146fbaa2723f2bf5dbd34">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/find.html">find</a></td><td class="cell-yrFK">Search for files that meet a desired criteria</td></tr><tr id="c6cccdd5-dd0d-49c8-a86c-df0a56c3a12a"><td class="cell-title"><a href="https://www.notion.so/c6cccdd5dd0d49c8a86cdf0a56c3a12a">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/fmt.html">fmt</a></td><td class="cell-yrFK">Reformat paragraph text</td></tr><tr id="671baa5f-1f07-45c0-8199-fc8632be861c"><td class="cell-title"><a href="https://www.notion.so/671baa5f1f0745c08199fc8632be861c">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/fold.html">fold</a></td><td class="cell-yrFK">Wrap text to fit a specified width</td></tr><tr id="27620043-a6bd-4190-a742-8637dd82d319"><td class="cell-title"><a href="https://www.notion.so/27620043a6bd4190a7428637dd82d319">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/for.html">for</a></td><td class="cell-yrFK">Expand <em>words</em>, and execute <em>commands</em></td></tr><tr id="1894475e-9ee6-485e-a907-235eef5ca43a"><td class="cell-title"><a href="https://www.notion.so/1894475e9ee6485ea907235eef5ca43a">Untitled</a></td><td class="cell-RMJm">format</td><td class="cell-yrFK">Format disks or tapes</td></tr><tr id="cf3f60f1-3387-4745-988c-fb15cfded568"><td class="cell-title"><a href="https://www.notion.so/cf3f60f133874745988cfb15cfded568">Untitled</a></td><td class="cell-RMJm">free</td><td class="cell-yrFK">Display memory usage</td></tr><tr id="28c0ed90-ee2d-4e3f-b80f-124fa6543574"><td class="cell-title"><a href="https://www.notion.so/28c0ed90ee2d4e3fb80f124fa6543574">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/fsck.html">fsck</a></td><td class="cell-yrFK">File system consistency check and repair</td></tr><tr id="7f375282-083c-4493-989b-b55926b0c449"><td class="cell-title"><a href="https://www.notion.so/7f375282083c4493989bb55926b0c449">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/ftp.html">ftp</a></td><td class="cell-yrFK">File Transfer Protocol</td></tr><tr id="0e75ffae-5d5f-4ef3-937a-d386c1f095d1"><td class="cell-title"><a href="https://www.notion.so/0e75ffae5d5f4ef3937ad386c1f095d1">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/function.html">function</a></td><td class="cell-yrFK">Define Function Macros</td></tr><tr id="f0407b7c-f04b-4651-9cc7-d4a120489064"><td class="cell-title"><a href="https://www.notion.so/f0407b7cf04b46519cc7d4a120489064">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/fuser.html">fuser</a></td><td class="cell-yrFK">Identify/kill the process that is accessing a file</td></tr><tr id="7beb15ec-16a7-43b5-ba0f-7364921e1f84"><td class="cell-title"><a href="https://www.notion.so/G-7beb15ec16a743b5ba0f7364921e1f84">G</a></td><td class="cell-RMJm"></td><td class="cell-yrFK"></td></tr><tr id="da8b4f32-7a50-4b05-8807-2037d39b86af"><td class="cell-title"><a href="https://www.notion.so/da8b4f327a504b0588072037d39b86af">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/awk.html">gawk</a></td><td class="cell-yrFK">Find and Replace text within file(s)</td></tr><tr id="68355712-6e4a-44b7-b5a0-c06a4d140457"><td class="cell-title"><a href="https://www.notion.so/683557126e4a44b7b5a0c06a4d140457">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/getopts.html">getopts</a></td><td class="cell-yrFK">Parse positional parameters</td></tr><tr id="795c06a0-57af-43dd-b7ab-be4c3a578995"><td class="cell-title"><a href="https://www.notion.so/795c06a057af43ddb7abbe4c3a578995">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/grep.html">grep</a></td><td class="cell-yrFK">Search file(s) for lines that match a given pattern</td></tr><tr id="c581d5c3-2ac2-4a0b-815a-24bea48251fb"><td class="cell-title"><a href="https://www.notion.so/c581d5c32ac24a0b815a24bea48251fb">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/groupadd.html">groupadd</a></td><td class="cell-yrFK">Add a user security group</td></tr><tr id="e19c4fff-f468-4a26-8e42-2d51d15b2f07"><td class="cell-title"><a href="https://www.notion.so/e19c4ffff4684a268e422d51d15b2f07">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/groupdel.html">groupdel</a></td><td class="cell-yrFK">Delete a group</td></tr><tr id="bc9c3bc3-96a4-4c7f-b568-33cceab734fb"><td class="cell-title"><a href="https://www.notion.so/bc9c3bc396a44c7fb56833cceab734fb">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/groupmod.html">groupmod</a></td><td class="cell-yrFK">Modify a group</td></tr><tr id="6c3ffbb3-7285-448b-85dd-bd592a7f77c3"><td class="cell-title"><a href="https://www.notion.so/6c3ffbb37285448b85ddbd592a7f77c3">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/groups.html">groups</a></td><td class="cell-yrFK">Print group names a user is in</td></tr><tr id="c2a7c3a5-e23c-48fb-adc9-b3c07be34755"><td class="cell-title"><a href="https://www.notion.so/c2a7c3a5e23c48fbadc9b3c07be34755">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/gzip.html">gzip</a></td><td class="cell-yrFK">Compress or decompress named file(s)</td></tr><tr id="36070d62-8540-4a08-89ca-76152bea24b6"><td class="cell-title"><a href="https://www.notion.so/H-36070d6285404a0889ca76152bea24b6">H</a></td><td class="cell-RMJm"></td><td class="cell-yrFK"></td></tr><tr id="e37e9794-f131-495c-b9bf-a1aafa5972bb"><td class="cell-title"><a href="https://www.notion.so/e37e9794f131495cb9bfa1aafa5972bb">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/hash.html">hash</a></td><td class="cell-yrFK">Remember the full pathname of a name argument</td></tr><tr id="94d5cd5e-b723-49b6-97ac-41361abf8f69"><td class="cell-title"><a href="https://www.notion.so/94d5cd5eb72349b697ac41361abf8f69">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/head.html">head</a></td><td class="cell-yrFK">Output the first part of file(s)</td></tr><tr id="8ce62a4a-7ae1-4ad3-8afa-7e7752e35f4a"><td class="cell-title"><a href="https://www.notion.so/8ce62a4a7ae14ad38afa7e7752e35f4a">Untitled</a></td><td class="cell-RMJm">help</td><td class="cell-yrFK">Display help for a built-in command •</td></tr><tr id="2fe3f426-ed18-4b76-8892-cf5137824a1b"><td class="cell-title"><a href="https://www.notion.so/2fe3f426ed184b768892cf5137824a1b">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/history.html">history</a></td><td class="cell-yrFK">Command History</td></tr><tr id="49a8ea38-9d07-4ffb-a5ea-d3379397fbe5"><td class="cell-title"><a href="https://www.notion.so/49a8ea389d074ffba5ead3379397fbe5">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/hostname.html">hostname</a></td><td class="cell-yrFK">Print or set system name</td></tr><tr id="fd3195cd-29b3-435e-8b10-adb39766d7a7"><td class="cell-title"><a href="https://www.notion.so/fd3195cd29b3435e8b10adb39766d7a7">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/htop.html">htop</a></td><td class="cell-yrFK">Interactive process viewer</td></tr><tr id="d538db72-5083-4fae-b8d4-fde29247d9bc"><td class="cell-title"><a href="https://www.notion.so/I-d538db7250834faeb8d4fde29247d9bc">I</a></td><td class="cell-RMJm"></td><td class="cell-yrFK"></td></tr><tr id="b8cf3830-284b-4a37-b7a7-6ccda7f6b4c5"><td class="cell-title"><a href="https://www.notion.so/b8cf3830284b4a37b7a76ccda7f6b4c5">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/iconv.html">iconv</a></td><td class="cell-yrFK">Convert the character set of a file</td></tr><tr id="e029fbe3-092a-48c4-ad37-713e3eb22f68"><td class="cell-title"><a href="https://www.notion.so/e029fbe3092a48c4ad37713e3eb22f68">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/id.html">id</a></td><td class="cell-yrFK">Print user and group id&#x27;s</td></tr><tr id="c5cf71df-ca78-4175-b8f9-3b0ad9696677"><td class="cell-title"><a href="https://www.notion.so/c5cf71dfca784175b8f93b0ad9696677">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/if.html">if</a></td><td class="cell-yrFK">Conditionally perform a command</td></tr><tr id="9057e281-c9cf-4a01-aad5-363643174ffd"><td class="cell-title"><a href="https://www.notion.so/9057e281c9cf4a01aad5363643174ffd">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/ifconfig.html">ifconfig</a></td><td class="cell-yrFK">Configure a network interface</td></tr><tr id="d07d7235-cc29-413a-b5b1-6ada47555910"><td class="cell-title"><a href="https://www.notion.so/d07d7235cc29413ab5b16ada47555910">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/ifup.html">ifdown</a></td><td class="cell-yrFK">Stop a network interface</td></tr><tr id="c3f90069-8f29-4b1b-9029-64120ffbab9c"><td class="cell-title"><a href="https://www.notion.so/c3f900698f294b1b902964120ffbab9c">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/ifup.html">ifup</a></td><td class="cell-yrFK">Start a network interface up</td></tr><tr id="e9dec262-fa03-4783-ac8e-a7bd606865a4"><td class="cell-title"><a href="https://www.notion.so/e9dec262fa034783ac8ea7bd606865a4">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/import.html">import</a></td><td class="cell-yrFK">Capture an X server screen and save the image to file</td></tr><tr id="c4e8761c-eb8d-47e0-8e85-0c28ebbd732e"><td class="cell-title"><a href="https://www.notion.so/c4e8761ceb8d47e08e850c28ebbd732e">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/install.html">install</a></td><td class="cell-yrFK">Copy files and set attributes</td></tr><tr id="6e5fe2f5-a684-4a7e-8f4f-9643c171bd81"><td class="cell-title"><a href="https://www.notion.so/6e5fe2f5a6844a7e8f4f9643c171bd81">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/iostat.html">iostat</a></td><td class="cell-yrFK">Report CPU and i/o statistics</td></tr><tr id="83da63e1-d9ec-47c7-b686-bd0689a724f0"><td class="cell-title"><a href="https://www.notion.so/83da63e1d9ec47c7b686bd0689a724f0">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/ip.html">ip</a></td><td class="cell-yrFK">Routing, devices and tunnels</td></tr><tr id="015e8f9d-6e24-4b0d-8496-32d066175374"><td class="cell-title"><a href="https://www.notion.so/J-015e8f9d6e244b0d849632d066175374">J</a></td><td class="cell-RMJm"></td><td class="cell-yrFK"></td></tr><tr id="68acafc0-7c4b-4df8-8653-ce88228feff1"><td class="cell-title"><a href="https://www.notion.so/68acafc07c4b4df88653ce88228feff1">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/jobs.html">jobs</a></td><td class="cell-yrFK">List active jobs •</td></tr><tr id="54edd590-67cc-41a7-8058-a5363657d771"><td class="cell-title"><a href="https://www.notion.so/54edd59067cc41a78058a5363657d771">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/join.html">join</a></td><td class="cell-yrFK">Join lines on a common field</td></tr><tr id="914d7cf5-5c00-4276-8ee1-66cf02b18e60"><td class="cell-title"><a href="https://www.notion.so/K-914d7cf55c0042768ee166cf02b18e60">K</a></td><td class="cell-RMJm"></td><td class="cell-yrFK"></td></tr><tr id="4643406c-b2f5-434b-99ed-b74f291c7b6a"><td class="cell-title"><a href="https://www.notion.so/4643406cb2f5434b99edb74f291c7b6a">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/kill.html">kill</a></td><td class="cell-yrFK">Kill a process by specifying its PID</td></tr><tr id="739e8fe6-d325-4971-8a4e-84fb66963942"><td class="cell-title"><a href="https://www.notion.so/739e8fe6d32549718a4e84fb66963942">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/killall.html">killall</a></td><td class="cell-yrFK">Kill processes by name</td></tr><tr id="ec024704-2378-40ae-aa4f-b9f496d0575d"><td class="cell-title"><a href="https://www.notion.so/L-ec024704237840aeaa4fb9f496d0575d">L</a></td><td class="cell-RMJm"></td><td class="cell-yrFK"></td></tr><tr id="e96edd72-3b14-47f0-9f06-2744f0d45461"><td class="cell-title"><a href="https://www.notion.so/e96edd723b1447f09f062744f0d45461">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/less.html">less</a></td><td class="cell-yrFK">Display output one screen at a time</td></tr><tr id="a209c18d-fcde-4272-9f05-079ffef3cf91"><td class="cell-title"><a href="https://www.notion.so/a209c18dfcde42729f05079ffef3cf91">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/let.html">let</a></td><td class="cell-yrFK">Perform arithmetic on shell variables •</td></tr><tr id="853aca94-f210-4666-91df-703925a1cfff"><td class="cell-title"><a href="https://www.notion.so/853aca94f210466691df703925a1cfff">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/link.html">link</a></td><td class="cell-yrFK">Create a link to a file</td></tr><tr id="f311fe53-2ce6-4b26-8e8f-f1dd0c259ed8"><td class="cell-title"><a href="https://www.notion.so/f311fe532ce64b268e8ff1dd0c259ed8">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/ln.html">ln</a></td><td class="cell-yrFK">Create a symbolic link to a file</td></tr><tr id="49723633-3fbd-4b83-a95d-e3de54f5908e"><td class="cell-title"><a href="https://www.notion.so/497236333fbd4b83a95de3de54f5908e">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/local.html">local</a></td><td class="cell-yrFK">Create a function variable •</td></tr><tr id="adf8f273-3d4f-411e-989f-b2ebdb5d9de2"><td class="cell-title"><a href="https://www.notion.so/adf8f2733d4f411e989fb2ebdb5d9de2">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/locate.html">locate</a></td><td class="cell-yrFK">Find files</td></tr><tr id="21f24337-c68a-4b9a-9adc-45bbe28c66a3"><td class="cell-title"><a href="https://www.notion.so/21f24337c68a4b9a9adc45bbe28c66a3">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/logname.html">logname</a></td><td class="cell-yrFK">Print current login name</td></tr><tr id="22cd01d8-879d-4dc0-9af1-758d61b7c654"><td class="cell-title"><a href="https://www.notion.so/22cd01d8879d4dc09af1758d61b7c654">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/logout.html">logout</a></td><td class="cell-yrFK">Exit a login shell •</td></tr><tr id="119e38e8-a128-4c3e-a4d4-95ace6b7d78a"><td class="cell-title"><a href="https://www.notion.so/119e38e8a1284c3ea4d495ace6b7d78a">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/look.html">look</a></td><td class="cell-yrFK">Display lines beginning with a given string</td></tr><tr id="e9fb28fc-dee5-4645-b982-077fbda3c943"><td class="cell-title"><a href="https://www.notion.so/e9fb28fcdee54645b982077fbda3c943">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/lpc.html">lpc</a></td><td class="cell-yrFK">Line printer control program</td></tr><tr id="1a779fd7-6bf9-487d-930d-7186f7066d59"><td class="cell-title"><a href="https://www.notion.so/1a779fd76bf9487d930d7186f7066d59">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/lpr.html">lpr</a></td><td class="cell-yrFK">Print files</td></tr><tr id="4a0a89b2-193e-44e0-978d-f5a6d5f18952"><td class="cell-title"><a href="https://www.notion.so/4a0a89b2193e44e0978df5a6d5f18952">Untitled</a></td><td class="cell-RMJm">lprint</td><td class="cell-yrFK">Print a file</td></tr><tr id="4764a628-14f2-40e0-91cc-0b8f602bed97"><td class="cell-title"><a href="https://www.notion.so/4764a62814f240e091cc0b8f602bed97">Untitled</a></td><td class="cell-RMJm">lprintd</td><td class="cell-yrFK">Delete a print job</td></tr><tr id="fb7c0c0e-c3f2-42ab-bf03-b2265fbf03a4"><td class="cell-title"><a href="https://www.notion.so/fb7c0c0ec3f242abbf03b2265fbf03a4">Untitled</a></td><td class="cell-RMJm">lprintq</td><td class="cell-yrFK">List the print queue</td></tr><tr id="4a521bcb-0d4c-4ee9-b80f-354b9fd4a75e"><td class="cell-title"><a href="https://www.notion.so/4a521bcb0d4c4ee9b80f354b9fd4a75e">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/lprm.html">lprm</a></td><td class="cell-yrFK">Remove jobs from the print queue</td></tr><tr id="fe35ef3f-7f50-40f7-b12a-abbfc3ed3132"><td class="cell-title"><a href="https://www.notion.so/fe35ef3f7f5040f7b12aabbfc3ed3132">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/lsattr.html">lsattr</a></td><td class="cell-yrFK">List file attributes on a Linux second extended file system</td></tr><tr id="fdf7f6af-1be0-4b8a-b69c-d0c56669936c"><td class="cell-title"><a href="https://www.notion.so/fdf7f6af1be04b8ab69cd0c56669936c">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/lsblk.html">lsblk</a></td><td class="cell-yrFK">List block devices</td></tr><tr id="a80230c7-f6a2-4f95-a038-543a9f60de6f"><td class="cell-title"><a href="https://www.notion.so/a80230c7f6a24f95a038543a9f60de6f">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/ls.html">ls</a></td><td class="cell-yrFK">List information about file(s)</td></tr><tr id="16d3da9d-06dd-4d7f-be03-f2976de20275"><td class="cell-title"><a href="https://www.notion.so/16d3da9d06dd4d7fbe03f2976de20275">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/lsof.html">lsof</a></td><td class="cell-yrFK">List open files</td></tr><tr id="be523382-76ab-40eb-823f-70262dd3786c"><td class="cell-title"><a href="https://www.notion.so/be52338276ab40eb823f70262dd3786c">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/lspci.html">lspci</a></td><td class="cell-yrFK">List all PCI devices</td></tr><tr id="bc52596a-c91f-4d9e-8124-c55fdeb8f454"><td class="cell-title"><a href="https://www.notion.so/M-bc52596ac91f4d9e8124c55fdeb8f454">M</a></td><td class="cell-RMJm"></td><td class="cell-yrFK"></td></tr><tr id="d1bf79fc-8660-4f7a-a543-e2cd57735314"><td class="cell-title"><a href="https://www.notion.so/d1bf79fc86604f7aa543e2cd57735314">Untitled</a></td><td class="cell-RMJm">make</td><td class="cell-yrFK">Recompile a group of programs</td></tr><tr id="33b721be-94d6-409d-9671-fac09f693944"><td class="cell-title"><a href="https://www.notion.so/33b721be94d6409d9671fac09f693944">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/man.html">man</a></td><td class="cell-yrFK">Help manual</td></tr><tr id="31a44b03-81a4-4121-abf3-61a64b32b295"><td class="cell-title"><a href="https://www.notion.so/31a44b0381a44121abf361a64b32b295">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/mapfile.html">mapfile</a></td><td class="cell-yrFK">Read lines from standard input into an indexed array variable •</td></tr><tr id="07052f97-f165-4bbc-9f11-3b9676816fbf"><td class="cell-title"><a href="https://www.notion.so/07052f97f1654bbc9f113b9676816fbf">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/mkdir.html">mkdir</a></td><td class="cell-yrFK">Create new folder(s)</td></tr><tr id="c160e3a6-63b6-44aa-ad50-ce79edf4c7fd"><td class="cell-title"><a href="https://www.notion.so/c160e3a663b644aaad50ce79edf4c7fd">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/mkfifo.html">mkfifo</a></td><td class="cell-yrFK">Make FIFOs (named pipes)</td></tr><tr id="81fa6735-d9c3-4317-942c-09bd95f191de"><td class="cell-title"><a href="https://www.notion.so/81fa6735d9c34317942c09bd95f191de">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/mkfile.html">mkfile</a></td><td class="cell-yrFK">Make a file</td></tr><tr id="c2f2f0a4-aaef-4218-93e5-d59c6eeeb029"><td class="cell-title"><a href="https://www.notion.so/c2f2f0a4aaef421893e5d59c6eeeb029">Untitled</a></td><td class="cell-RMJm">mkisofs</td><td class="cell-yrFK">Create a hybrid ISO9660/JOLIET/HFS filesystem</td></tr><tr id="00cf48b1-1b59-492a-99d4-6f20f3be8a76"><td class="cell-title"><a href="https://www.notion.so/00cf48b11b59492a99d46f20f3be8a76">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/mknod.html">mknod</a></td><td class="cell-yrFK">Make block or character special files</td></tr><tr id="a6de533e-a28c-489a-aa89-91551c61ab9d"><td class="cell-title"><a href="https://www.notion.so/a6de533ea28c489aaa8991551c61ab9d">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/mktemp.html">mktemp</a></td><td class="cell-yrFK">Make a temporary file</td></tr><tr id="6d06093e-0324-4b46-a463-ef4350d1a4c5"><td class="cell-title"><a href="https://www.notion.so/6d06093e03244b46a463ef4350d1a4c5">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/more.html">more</a></td><td class="cell-yrFK">Display output one screen at a time</td></tr><tr id="e709c086-1009-47ae-ad7e-42a4189e4f8e"><td class="cell-title"><a href="https://www.notion.so/e709c086100947aead7e42a4189e4f8e">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/most.html">most</a></td><td class="cell-yrFK">Browse or page through a text file</td></tr><tr id="b93c00d6-7cdc-45d7-95ce-771799d65bfd"><td class="cell-title"><a href="https://www.notion.so/b93c00d67cdc45d795ce771799d65bfd">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/mount.html">mount</a></td><td class="cell-yrFK">Mount a file system</td></tr><tr id="07253bb4-9dcc-4b98-8b39-4c5593132add"><td class="cell-title"><a href="https://www.notion.so/07253bb49dcc4b988b394c5593132add">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/mtools.html">mtools</a></td><td class="cell-yrFK">Manipulate MS-DOS files</td></tr><tr id="bf805994-ec6f-4a6d-928c-f0819bfe5c54"><td class="cell-title"><a href="https://www.notion.so/bf805994ec6f4a6d928cf0819bfe5c54">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/mtr.html">mtr</a></td><td class="cell-yrFK">Network diagnostics (traceroute/ping)</td></tr><tr id="c27a10f4-0385-4ded-ac71-4fed82312a62"><td class="cell-title"><a href="https://www.notion.so/c27a10f403854dedac714fed82312a62">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/mv.html">mv</a></td><td class="cell-yrFK">Move or rename files or directories</td></tr><tr id="db2e05ac-d48b-4c99-81b2-e7e002ac7f17"><td class="cell-title"><a href="https://www.notion.so/db2e05acd48b4c9981b2e7e002ac7f17">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/mmv.html">mmv</a></td><td class="cell-yrFK">Mass Move and rename (files)</td></tr><tr id="8ecb8e05-56d3-4047-a8d4-926a4e82b233"><td class="cell-title"><a href="https://www.notion.so/N-8ecb8e0556d34047a8d4926a4e82b233">N</a></td><td class="cell-RMJm"></td><td class="cell-yrFK"></td></tr><tr id="e78350b6-41dd-45f3-8370-2a61f0f79aa7"><td class="cell-title"><a href="https://www.notion.so/e78350b641dd45f383702a61f0f79aa7">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/nc.html">nc</a></td><td class="cell-yrFK">Netcat, read and write data across networks</td></tr><tr id="6276713e-29e6-4728-806a-a74ff519161e"><td class="cell-title"><a href="https://www.notion.so/6276713e29e64728806aa74ff519161e">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/netstat.html">netstat</a></td><td class="cell-yrFK">Networking connections/stats</td></tr><tr id="b02643de-7394-43c2-93ea-7cd6c78aab88"><td class="cell-title"><a href="https://www.notion.so/b02643de739443c293ea7cd6c78aab88">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/nft.html">nft</a></td><td class="cell-yrFK">nftables for packet filtering and classification</td></tr><tr id="0c4bbfbc-cf8e-4742-a649-0bc7d976f0d7"><td class="cell-title"><a href="https://www.notion.so/0c4bbfbccf8e4742a6490bc7d976f0d7">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/nice.html">nice</a></td><td class="cell-yrFK">Set the priority of a command or job</td></tr><tr id="fbab0562-28ef-4efd-a79b-25521287a57d"><td class="cell-title"><a href="https://www.notion.so/fbab056228ef4efda79b25521287a57d">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/nl.html">nl</a></td><td class="cell-yrFK">Number lines and write files</td></tr><tr id="221140f5-7228-4fc5-8a3e-2db755dd5af7"><td class="cell-title"><a href="https://www.notion.so/221140f572284fc58a3e2db755dd5af7">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/nohup.html">nohup</a></td><td class="cell-yrFK">Run a command immune to hangups</td></tr><tr id="b73cf05a-cf6d-4013-8571-6d77e10efb48"><td class="cell-title"><a href="https://www.notion.so/b73cf05acf6d401385716d77e10efb48">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/notify-send.html">notify-send</a></td><td class="cell-yrFK">Send desktop notifications</td></tr><tr id="ee2e031e-6c73-49e2-aa66-64750c2086e1"><td class="cell-title"><a href="https://www.notion.so/ee2e031e6c7349e2aa6664750c2086e1">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/nslookup.html">nslookup</a></td><td class="cell-yrFK">Query Internet name servers interactively</td></tr><tr id="c4012518-3a79-4f0b-acc4-030cabaf641f"><td class="cell-title"><a href="https://www.notion.so/O-c40125183a794f0bacc4030cabaf641f">O</a></td><td class="cell-RMJm"></td><td class="cell-yrFK"></td></tr><tr id="0e5079b2-5a3c-4a3e-92cf-d6c9e8a4ec76"><td class="cell-title"><a href="https://www.notion.so/0e5079b25a3c4a3e92cfd6c9e8a4ec76">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/open.html">open</a></td><td class="cell-yrFK">Open a file in its default application</td></tr><tr id="3f5cd3da-2be7-4b4b-8f9d-82d36ba2c9cd"><td class="cell-title"><a href="https://www.notion.so/3f5cd3da2be74b4b8f9d82d36ba2c9cd">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/op.html">op</a></td><td class="cell-yrFK">Operator access</td></tr><tr id="2172b11e-9e4e-4703-85a5-a2a089ff3321"><td class="cell-title"><a href="https://www.notion.so/P-2172b11e9e4e470385a5a2a089ff3321">P</a></td><td class="cell-RMJm"></td><td class="cell-yrFK"></td></tr><tr id="c23e3e00-ca2f-438f-8d4f-d0fb42bad443"><td class="cell-title"><a href="https://www.notion.so/c23e3e00ca2f438f8d4fd0fb42bad443">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/passwd.html">passwd</a></td><td class="cell-yrFK">Modify a user password</td></tr><tr id="4772e799-9272-4e65-980a-6fce10bc6054"><td class="cell-title"><a href="https://www.notion.so/4772e79992724e65980a6fce10bc6054">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/paste.html">paste</a></td><td class="cell-yrFK">Merge lines of files</td></tr><tr id="248b60db-2bfb-4542-b922-df92e0f0fce5"><td class="cell-title"><a href="https://www.notion.so/248b60db2bfb4542b922df92e0f0fce5">Untitled</a></td><td class="cell-RMJm">pathchk</td><td class="cell-yrFK">Check file name portability</td></tr><tr id="b3892222-af10-4148-b9c8-2854acd9c958"><td class="cell-title"><a href="https://www.notion.so/b3892222af104148b9c82854acd9c958">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/perf.html">Perf</a></td><td class="cell-yrFK">Performance analysis tools for Linux</td></tr><tr id="bbe0fcf1-ce9f-43ba-a4a2-8a1e19996286"><td class="cell-title"><a href="https://www.notion.so/bbe0fcf1ce9f43baa4a28a1e19996286">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/ping.html">ping</a></td><td class="cell-yrFK">Test a network connection</td></tr><tr id="df154214-c6d0-49fd-b29b-09fe0af82b99"><td class="cell-title"><a href="https://www.notion.so/df154214c6d049fdb29b09fe0af82b99">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/pkill.html">pgrep</a></td><td class="cell-yrFK">List processes by name</td></tr><tr id="97809b09-79e2-4719-a7f0-e5f046f01753"><td class="cell-title"><a href="https://www.notion.so/97809b0979e24719a7f0e5f046f01753">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/pkill.html">pkill</a></td><td class="cell-yrFK">Kill processes by name</td></tr><tr id="a9d2fa0f-7ad8-4816-a219-4b0e13f94937"><td class="cell-title"><a href="https://www.notion.so/a9d2fa0f7ad84816a2194b0e13f94937">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/popd.html">popd</a></td><td class="cell-yrFK">Restore the previous value of the current directory</td></tr><tr id="c99e1e07-4ecc-4e00-819c-4817a02602c5"><td class="cell-title"><a href="https://www.notion.so/c99e1e074ecc4e00819c4817a02602c5">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/pr.html">pr</a></td><td class="cell-yrFK">Prepare files for printing</td></tr><tr id="eb36a4cc-c200-4335-82af-11c0ad36d4e3"><td class="cell-title"><a href="https://www.notion.so/eb36a4ccc200433582af11c0ad36d4e3">Untitled</a></td><td class="cell-RMJm">printcap</td><td class="cell-yrFK">Printer capability database</td></tr><tr id="6d60b63c-2a46-46ba-9133-4fdb18584dc0"><td class="cell-title"><a href="https://www.notion.so/6d60b63c2a4646ba91334fdb18584dc0">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/printenv.html">printenv</a></td><td class="cell-yrFK">Print environment variables</td></tr><tr id="e2b806f7-7689-47fc-93ad-39dc92b9ea89"><td class="cell-title"><a href="https://www.notion.so/e2b806f7768947fc93ad39dc92b9ea89">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/printf.html">printf</a></td><td class="cell-yrFK">Format and print data •</td></tr><tr id="a171f5fa-efa3-42e3-88c9-a8c289bbe891"><td class="cell-title"><a href="https://www.notion.so/a171f5faefa342e388c9a8c289bbe891">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/ps.html">ps</a></td><td class="cell-yrFK">Process status</td></tr><tr id="e8f66357-5ef4-4172-9aa7-b49932916970"><td class="cell-title"><a href="https://www.notion.so/e8f663575ef441729aa7b49932916970">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/pushd.html">pushd</a></td><td class="cell-yrFK">Save and then change the current directory</td></tr><tr id="a5b47ec6-4819-4867-b566-b0f998f8a71f"><td class="cell-title"><a href="https://www.notion.so/a5b47ec648194867b566b0f998f8a71f">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/pv.html">pv</a></td><td class="cell-yrFK">Monitor the progress of data through a pipe</td></tr><tr id="828cd6c8-52f8-4cfa-a393-7e1b4de14564"><td class="cell-title"><a href="https://www.notion.so/828cd6c852f84cfaa3937e1b4de14564">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/pwd.html">pwd</a></td><td class="cell-yrFK">Print Working Directory</td></tr><tr id="5e0e5f00-51d9-47c3-bacf-e9cc1c2c72d0"><td class="cell-title"><a href="https://www.notion.so/Q-5e0e5f0051d947c3bacfe9cc1c2c72d0">Q</a></td><td class="cell-RMJm"></td><td class="cell-yrFK"></td></tr><tr id="373825ae-4ef3-487e-8fbc-bac7f2b3be7c"><td class="cell-title"><a href="https://www.notion.so/373825ae4ef3487e8fbcbac7f2b3be7c">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/quota.html">quota</a></td><td class="cell-yrFK">Display disk usage and limits</td></tr><tr id="6e074729-a9c7-4ceb-acaf-379f3f831962"><td class="cell-title"><a href="https://www.notion.so/6e074729a9c74cebacaf379f3f831962">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/quotacheck.html">quotacheck</a></td><td class="cell-yrFK">Scan a file system for disk usage</td></tr><tr id="6bf79a4e-1f4c-4068-bbc1-2053fed5f246"><td class="cell-title"><a href="https://www.notion.so/R-6bf79a4e1f4c4068bbc12053fed5f246">R</a></td><td class="cell-RMJm"></td><td class="cell-yrFK"></td></tr><tr id="5370ab62-5331-431f-a071-a2298c858fe1"><td class="cell-title"><a href="https://www.notion.so/5370ab625331431fa071a2298c858fe1">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/ram.html">ram</a></td><td class="cell-yrFK">ram disk device</td></tr><tr id="ccd3336a-2b9c-4428-91d7-29e76c9695b7"><td class="cell-title"><a href="https://www.notion.so/ccd3336a2b9c442891d729e76c9695b7">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/rar.html">rar</a></td><td class="cell-yrFK">Archive files with compression</td></tr><tr id="a94bc661-b830-49c9-9f8b-9f4e29a2d8c5"><td class="cell-title"><a href="https://www.notion.so/a94bc661b83049c99f8b9f4e29a2d8c5">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/rcp.html">rcp</a></td><td class="cell-yrFK">Copy files between two machines</td></tr><tr id="60766220-e4af-438d-aafb-030ea3bf791d"><td class="cell-title"><a href="https://www.notion.so/60766220e4af438daafb030ea3bf791d">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/read.html">read</a></td><td class="cell-yrFK">Read a line from standard input •</td></tr><tr id="eee2ba31-6821-4b42-bf5c-a5bc1b1b0e89"><td class="cell-title"><a href="https://www.notion.so/eee2ba3168214b42bf5ca5bc1b1b0e89">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/mapfile.html">readarray</a></td><td class="cell-yrFK">Read from stdin into an array variable •</td></tr><tr id="17e548ed-ca66-4391-b457-e853560edda9"><td class="cell-title"><a href="https://www.notion.so/17e548edca664391b457e853560edda9">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/readonly.html">readonly</a></td><td class="cell-yrFK">Mark variables/functions as readonly</td></tr><tr id="3ab3b497-136a-4277-aa16-c1ff9f7240b0"><td class="cell-title"><a href="https://www.notion.so/3ab3b497136a4277aa16c1ff9f7240b0">Untitled</a></td><td class="cell-RMJm">reboot</td><td class="cell-yrFK">Reboot the system</td></tr><tr id="396732a8-9224-4337-b52b-b6b0c879f001"><td class="cell-title"><a href="https://www.notion.so/396732a892244337b52bb6b0c879f001">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/rename.html">rename</a></td><td class="cell-yrFK">Rename files</td></tr><tr id="47b98f78-baa3-4079-9f60-8ea9f6bbea1b"><td class="cell-title"><a href="https://www.notion.so/47b98f78baa340799f608ea9f6bbea1b">Untitled</a></td><td class="cell-RMJm">renice</td><td class="cell-yrFK">Alter priority of running processes</td></tr><tr id="d71e1985-0f8c-43d8-b54d-cba00b27c864"><td class="cell-title"><a href="https://www.notion.so/d71e19850f8c43d8b54dcba00b27c864">Untitled</a></td><td class="cell-RMJm">remsync</td><td class="cell-yrFK">Synchronize remote files via email</td></tr><tr id="7bae5a54-539e-4094-9ad4-eaaec965958d"><td class="cell-title"><a href="https://www.notion.so/7bae5a54539e40949ad4eaaec965958d">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/return.html">return</a></td><td class="cell-yrFK">Exit a shell function</td></tr><tr id="bc61f242-cb8f-47e9-8759-09367b2fdb55"><td class="cell-title"><a href="https://www.notion.so/bc61f242cb8f47e9875909367b2fdb55">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/rev.html">rev</a></td><td class="cell-yrFK">Reverse lines of a file</td></tr><tr id="0b39f543-2fb2-4373-9c3f-1a41adb08411"><td class="cell-title"><a href="https://www.notion.so/0b39f5432fb243739c3f1a41adb08411">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/rm.html">rm</a></td><td class="cell-yrFK">Remove files</td></tr><tr id="c6dcaff1-d7db-4f56-a592-e00fb4816a5e"><td class="cell-title"><a href="https://www.notion.so/c6dcaff1d7db4f56a592e00fb4816a5e">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/rmdir.html">rmdir</a></td><td class="cell-yrFK">Remove folder(s)</td></tr><tr id="3d25cbdc-9bbe-4079-b5fd-1d8e488d0a3d"><td class="cell-title"><a href="https://www.notion.so/3d25cbdc9bbe4079b5fd1d8e488d0a3d">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/rsync.html">rsync</a></td><td class="cell-yrFK">Remote file copy (Synchronize file trees)</td></tr><tr id="a8575453-a487-4882-b202-85056addaad8"><td class="cell-title"><a href="https://www.notion.so/S-a8575453a4874882b20285056addaad8">S</a></td><td class="cell-RMJm"></td><td class="cell-yrFK"></td></tr><tr id="9d801d29-dfd7-4c35-90a0-9238f794ae11"><td class="cell-title"><a href="https://www.notion.so/9d801d29dfd74c3590a09238f794ae11">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/screen.html">screen</a></td><td class="cell-yrFK">Multiplex terminal, run remote shells via ssh</td></tr><tr id="cca1a3f7-f7ac-4bb3-9405-d75cbdc9829f"><td class="cell-title"><a href="https://www.notion.so/cca1a3f7f7ac4bb39405d75cbdc9829f">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/scp.html">scp</a></td><td class="cell-yrFK">Secure copy (remote file copy)</td></tr><tr id="4dab5dce-f05a-40cc-90ff-478787537a8a"><td class="cell-title"><a href="https://www.notion.so/4dab5dcef05a40cc90ff478787537a8a">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/sdiff.html">sdiff</a></td><td class="cell-yrFK">Merge two files interactively</td></tr><tr id="b47a23df-4274-4d92-a9e6-021eb8b187ec"><td class="cell-title"><a href="https://www.notion.so/b47a23df42744d92a9e6021eb8b187ec">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/sed.html">sed</a></td><td class="cell-yrFK">Stream Editor</td></tr><tr id="efab80d5-823d-45e1-a434-0e0999397842"><td class="cell-title"><a href="https://www.notion.so/efab80d5823d45e1a4340e0999397842">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/select.html">select</a></td><td class="cell-yrFK">Accept user choices via keyboard input</td></tr><tr id="1d2614f8-4216-40af-a173-fab73b4d09b6"><td class="cell-title"><a href="https://www.notion.so/1d2614f8421640afa173fab73b4d09b6">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/seq.html">seq</a></td><td class="cell-yrFK">Print numeric sequences</td></tr><tr id="5e6003cf-fb93-44b5-a6fe-89d58cb8b6de"><td class="cell-title"><a href="https://www.notion.so/5e6003cffb9344b5a6fe89d58cb8b6de">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/set.html">set</a></td><td class="cell-yrFK">Manipulate shell variables and functions</td></tr><tr id="7411f8ce-213e-428a-ad27-ce1af5fe9c34"><td class="cell-title"><a href="https://www.notion.so/7411f8ce213e428aad27ce1af5fe9c34">Untitled</a></td><td class="cell-RMJm">sftp</td><td class="cell-yrFK">Secure File Transfer Program</td></tr><tr id="3ac8b7c8-6714-4e79-861a-bd04ee0d9302"><td class="cell-title"><a href="https://www.notion.so/3ac8b7c867144e79861abd04ee0d9302">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/shift.html">shift</a></td><td class="cell-yrFK">Shift positional parameters</td></tr><tr id="0bab4e4a-2e43-4985-9dec-ac8d7f3a17a7"><td class="cell-title"><a href="https://www.notion.so/0bab4e4a2e4349859decac8d7f3a17a7">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/shopt.html">shopt</a></td><td class="cell-yrFK">Shell Options</td></tr><tr id="16ab02d4-5dcf-4e6d-8406-403e06026594"><td class="cell-title"><a href="https://www.notion.so/16ab02d45dcf4e6d8406403e06026594">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/shuf.html">shuf</a></td><td class="cell-yrFK">Generate random permutations</td></tr><tr id="acbb2545-3313-4759-9f8f-8281a9bb8493"><td class="cell-title"><a href="https://www.notion.so/acbb2545331347599f8f8281a9bb8493">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/shutdown.html">shutdown</a></td><td class="cell-yrFK">Shutdown or restart linux</td></tr><tr id="ba211fdd-ef0f-44a0-99ff-9b1e69ac132d"><td class="cell-title"><a href="https://www.notion.so/ba211fddef0f44a099ff9b1e69ac132d">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/sleep.html">sleep</a></td><td class="cell-yrFK">Delay for a specified time</td></tr><tr id="a085c681-e009-485f-a781-0ab727d28a6d"><td class="cell-title"><a href="https://www.notion.so/a085c681e009485fa7810ab727d28a6d">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/slocate.html">slocate</a></td><td class="cell-yrFK">Find files</td></tr><tr id="603c52e4-fd9b-4cfb-bf51-dd94c6bc370e"><td class="cell-title"><a href="https://www.notion.so/603c52e4fd9b4cfbbf51dd94c6bc370e">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/sort.html">sort</a></td><td class="cell-yrFK">Sort text files</td></tr><tr id="65deeef6-9fcc-4c8c-ac44-fc4d0b0693a6"><td class="cell-title"><a href="https://www.notion.so/65deeef69fcc4c8cac44fc4d0b0693a6">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/source.html">source</a></td><td class="cell-yrFK">Run commands from a file &#x27;.&#x27;  •</td></tr><tr id="9fb999a6-de71-4b68-bb34-6a12265480d9"><td class="cell-title"><a href="https://www.notion.so/9fb999a6de714b68bb346a12265480d9">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/split.html">split</a></td><td class="cell-yrFK">Split a file into fixed-size pieces</td></tr><tr id="0de15b36-2f4b-4a96-9d4f-ff7b8322c6f2"><td class="cell-title"><a href="https://www.notion.so/0de15b362f4b4a969d4fff7b8322c6f2">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/ss.html">ss</a></td><td class="cell-yrFK">Socket Statistics</td></tr><tr id="2d289006-3ae9-45bd-b146-e0798d491a48"><td class="cell-title"><a href="https://www.notion.so/2d2890063ae945bdb146e0798d491a48">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/ssh.html">ssh</a></td><td class="cell-yrFK">Secure Shell client (remote login program)</td></tr><tr id="d94e63a3-a6eb-4456-a989-9c613c6411b3"><td class="cell-title"><a href="https://www.notion.so/d94e63a3a6eb4456a9899c613c6411b3">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/stat.html">stat</a></td><td class="cell-yrFK">Display file or file system status</td></tr><tr id="8b46bdd3-d483-47c2-9b81-2b85ef806b86"><td class="cell-title"><a href="https://www.notion.so/8b46bdd3d48347c29b812b85ef806b86">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/strace.html">strace</a></td><td class="cell-yrFK">Trace system calls and signals</td></tr><tr id="fed167e9-bfdd-4f8d-ad52-e3204a25b029"><td class="cell-title"><a href="https://www.notion.so/fed167e9bfdd4f8dad52e3204a25b029">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/su.html">su</a></td><td class="cell-yrFK">Substitute user identity</td></tr><tr id="48e89f5e-6917-430a-b67b-c7fd1c7c2ba0"><td class="cell-title"><a href="https://www.notion.so/48e89f5e6917430ab67bc7fd1c7c2ba0">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/sudo.html">sudo</a></td><td class="cell-yrFK">Execute a command as another user</td></tr><tr id="3e52e77f-7995-49e4-8138-edd5a5428180"><td class="cell-title"><a href="https://www.notion.so/3e52e77f799549e48138edd5a5428180">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/sum.html">sum</a></td><td class="cell-yrFK">Print a checksum for a file</td></tr><tr id="d7357aa5-81fc-41fa-91a0-fa0047d7b922"><td class="cell-title"><a href="https://www.notion.so/d7357aa581fc41fa91a0fa0047d7b922">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/suspend.html">suspend</a></td><td class="cell-yrFK">Suspend execution of this shell •</td></tr><tr id="51746cfd-2165-4db4-b7d4-a5463f8a7a67"><td class="cell-title"><a href="https://www.notion.so/51746cfd21654db4b7d4a5463f8a7a67">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/sync.html">sync</a></td><td class="cell-yrFK">Synchronize data on disk with memory</td></tr><tr id="16b8ac41-a74c-4379-b886-1d24f91c6adc"><td class="cell-title"><a href="https://www.notion.so/T-16b8ac41a74c4379b8861d24f91c6adc">T</a></td><td class="cell-RMJm"></td><td class="cell-yrFK"></td></tr><tr id="6399633f-4f97-4def-b7b3-7b716e9b8aa7"><td class="cell-title"><a href="https://www.notion.so/6399633f4f974defb7b37b716e9b8aa7">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/tail.html">tail</a></td><td class="cell-yrFK">Output the last part of a file</td></tr><tr id="5ca30f62-69b9-4e21-97a5-0db582ebd8fd"><td class="cell-title"><a href="https://www.notion.so/5ca30f6269b94e2197a50db582ebd8fd">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/tar.html">tar</a></td><td class="cell-yrFK">Store, list or extract files in an archive</td></tr><tr id="5041436d-98f1-4633-9e7c-5d26ab249415"><td class="cell-title"><a href="https://www.notion.so/5041436d98f146339e7c5d26ab249415">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/tee.html">tee</a></td><td class="cell-yrFK">Redirect output to multiple files</td></tr><tr id="707e2ba0-d23c-44dd-83c7-02a48d98a85a"><td class="cell-title"><a href="https://www.notion.so/707e2ba0d23c44dd83c702a48d98a85a">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/test.html">test</a></td><td class="cell-yrFK">Evaluate a conditional expression</td></tr><tr id="5620be6f-c01b-4848-bbf6-c77dcae8f1ed"><td class="cell-title"><a href="https://www.notion.so/5620be6fc01b4848bbf6c77dcae8f1ed">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/time.html">time</a></td><td class="cell-yrFK">Measure Program running time</td></tr><tr id="a1fcd33b-36f5-4ae8-b44c-24e741b1aa17"><td class="cell-title"><a href="https://www.notion.so/a1fcd33b36f54ae8b44c24e741b1aa17">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/timeout.html">timeout</a></td><td class="cell-yrFK">Run a command with a time limit</td></tr><tr id="19f20f91-ea01-47a0-8c96-6b9e39c43052"><td class="cell-title"><a href="https://www.notion.so/19f20f91ea0147a08c966b9e39c43052">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/times.html">times</a></td><td class="cell-yrFK">User and system times</td></tr><tr id="c73dfa1d-19d9-41f7-8f56-3facb3677521"><td class="cell-title"><a href="https://www.notion.so/c73dfa1d19d941f78f563facb3677521">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/tmux.html">tmux</a></td><td class="cell-yrFK">Terminal multiplexer</td></tr><tr id="3fc5f04e-e83c-47e6-a704-7a959f6e1ec6"><td class="cell-title"><a href="https://www.notion.so/3fc5f04ee83c47e6a7047a959f6e1ec6">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/touch.html">touch</a></td><td class="cell-yrFK">Change file timestamps</td></tr><tr id="20f9e893-7339-4fda-8364-fd60763f97e0"><td class="cell-title"><a href="https://www.notion.so/20f9e89373394fda8364fd60763f97e0">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/top.html">top</a></td><td class="cell-yrFK">List processes running on the system</td></tr><tr id="727f3a12-da03-4441-9a29-61f9cadf2d03"><td class="cell-title"><a href="https://www.notion.so/727f3a12da0344419a2961f9cadf2d03">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/tput.html">tput</a></td><td class="cell-yrFK">Set terminal-dependent capabilities, color, position</td></tr><tr id="82aefbb8-d3bf-4a1e-8b85-a396dffed516"><td class="cell-title"><a href="https://www.notion.so/82aefbb8d3bf4a1e8b85a396dffed516">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/traceroute.html">traceroute</a></td><td class="cell-yrFK">Trace Route to Host</td></tr><tr id="a451816e-a0de-4222-b361-b353c1eb6d83"><td class="cell-title"><a href="https://www.notion.so/a451816ea0de4222b361b353c1eb6d83">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/trap.html">trap</a></td><td class="cell-yrFK">Execute a command when the shell receives a signal •</td></tr><tr id="01f14ca2-3951-4299-8ac8-d72c3dcaab62"><td class="cell-title"><a href="https://www.notion.so/01f14ca2395142998ac8d72c3dcaab62">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/tr.html">tr</a></td><td class="cell-yrFK">Translate, squeeze, and/or delete characters</td></tr><tr id="d95b0a24-bcae-4788-9bd5-2a2c0523df14"><td class="cell-title"><a href="https://www.notion.so/d95b0a24bcae47889bd52a2c0523df14">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/true.html">true</a></td><td class="cell-yrFK">Do nothing, successfully</td></tr><tr id="85b32aa8-5ee1-4f6d-ab8b-1777c2f4b5a6"><td class="cell-title"><a href="https://www.notion.so/85b32aa85ee14f6dab8b1777c2f4b5a6">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/tsort.html">tsort</a></td><td class="cell-yrFK">Topological sort</td></tr><tr id="f4ad2cf1-49eb-4178-96a9-fd1c5c398fdc"><td class="cell-title"><a href="https://www.notion.so/f4ad2cf149eb417896a9fd1c5c398fdc">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/tty.html">tty</a></td><td class="cell-yrFK">Print filename of terminal on stdin</td></tr><tr id="55f7a04a-ac0d-47e4-8755-ed14908a2266"><td class="cell-title"><a href="https://www.notion.so/55f7a04aac0d47e48755ed14908a2266">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/type.html">type</a></td><td class="cell-yrFK">Describe a command •</td></tr><tr id="c1a02a1a-f96c-49bf-9057-a888286c2a58"><td class="cell-title"><a href="https://www.notion.so/U-c1a02a1af96c49bf9057a888286c2a58">U</a></td><td class="cell-RMJm"></td><td class="cell-yrFK"></td></tr><tr id="587d00f5-0979-4be6-876a-8a6a63878f2a"><td class="cell-title"><a href="https://www.notion.so/587d00f509794be6876a8a6a63878f2a">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/ulimit.html">ulimit</a></td><td class="cell-yrFK">Limit user resources •</td></tr><tr id="0d3da2a8-dc92-4007-a970-d2308b5ba394"><td class="cell-title"><a href="https://www.notion.so/0d3da2a8dc924007a970d2308b5ba394">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/umask.html">umask</a></td><td class="cell-yrFK">Users file creation mask</td></tr><tr id="772ef31d-1aee-4646-985b-7b297799a661"><td class="cell-title"><a href="https://www.notion.so/772ef31d1aee4646985b7b297799a661">Untitled</a></td><td class="cell-RMJm">umount</td><td class="cell-yrFK">Unmount a device</td></tr><tr id="808e65f9-2c0c-4ee4-a348-18b85d7d7759"><td class="cell-title"><a href="https://www.notion.so/808e65f92c0c4ee4a34818b85d7d7759">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/alias.html">unalias</a></td><td class="cell-yrFK">Remove an alias •</td></tr><tr id="c922298d-5397-44b9-90fc-e463c3ff7106"><td class="cell-title"><a href="https://www.notion.so/c922298d539744b990fce463c3ff7106">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/uname.html">uname</a></td><td class="cell-yrFK">Print system information</td></tr><tr id="9a8a9b29-aaef-4b88-93b2-b8be8c961f78"><td class="cell-title"><a href="https://www.notion.so/9a8a9b29aaef4b8893b2b8be8c961f78">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/unexpand.html">unexpand</a></td><td class="cell-yrFK">Convert spaces to tabs</td></tr><tr id="65ab1166-92f2-4c00-82db-025c518d01a4"><td class="cell-title"><a href="https://www.notion.so/65ab116692f24c0082db025c518d01a4">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/uniq.html">uniq</a></td><td class="cell-yrFK">Uniquify files</td></tr><tr id="c98fa921-e6e2-4690-ae28-785aa4838795"><td class="cell-title"><a href="https://www.notion.so/c98fa921e6e24690ae28785aa4838795">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/units.html">units</a></td><td class="cell-yrFK">Convert units from one scale to another</td></tr><tr id="1ec6111e-ed77-4e48-b780-d8d23ede0270"><td class="cell-title"><a href="https://www.notion.so/1ec6111eed774e48b780d8d23ede0270">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/unix2dos.html">unix2dos</a></td><td class="cell-yrFK">UNIX to Windows or MAC text file format converter</td></tr><tr id="4a83329e-7d8a-4879-acfb-fd2429136464"><td class="cell-title"><a href="https://www.notion.so/4a83329e7d8a4879acfbfd2429136464">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/unrar.html">unrar</a></td><td class="cell-yrFK">Extract files from a rar archive</td></tr><tr id="b274a9d4-8315-4095-8e1f-01e8972c0373"><td class="cell-title"><a href="https://www.notion.so/b274a9d4831540958e1f01e8972c0373">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/unset.html">unset</a></td><td class="cell-yrFK">Remove variable or function names</td></tr><tr id="d3d14559-b38c-46c8-a3e8-49a34fb79110"><td class="cell-title"><a href="https://www.notion.so/d3d14559b38c46c8a3e849a34fb79110">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/unshar.html">unshar</a></td><td class="cell-yrFK">Unpack shell archive scripts</td></tr><tr id="399b85e6-8cdb-49aa-8ab7-52685c577ce5"><td class="cell-title"><a href="https://www.notion.so/399b85e68cdb49aa8ab752685c577ce5">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/until.html">until</a></td><td class="cell-yrFK">Execute commands (until error)</td></tr><tr id="047f153c-667f-486f-927e-9a98ea53d350"><td class="cell-title"><a href="https://www.notion.so/047f153c667f486f927e9a98ea53d350">Untitled</a></td><td class="cell-RMJm">uptime</td><td class="cell-yrFK">Show uptime</td></tr><tr id="4620056e-d4c5-4cba-a8c3-152f86065d8a"><td class="cell-title"><a href="https://www.notion.so/4620056ed4c54cbaa8c3152f86065d8a">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/useradd.html">useradd</a></td><td class="cell-yrFK">Create new user account</td></tr><tr id="028ee7c0-d0e8-47aa-8729-edff82166b2f"><td class="cell-title"><a href="https://www.notion.so/028ee7c0d0e847aa8729edff82166b2f">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/userdel.html">userdel</a></td><td class="cell-yrFK">Delete a user account</td></tr><tr id="e9d44761-5e8b-4c77-b4ce-427cffd8dd2b"><td class="cell-title"><a href="https://www.notion.so/e9d447615e8b4c77b4ce427cffd8dd2b">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/usermod.html">usermod</a></td><td class="cell-yrFK">Modify user account</td></tr><tr id="229e6ee8-0233-454d-84fa-378f5d77b538"><td class="cell-title"><a href="https://www.notion.so/229e6ee80233454d84fa378f5d77b538">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/users.html">users</a></td><td class="cell-yrFK">List users currently logged in</td></tr><tr id="eb6634ec-61ee-4e7c-a228-98edf2c2d4f2"><td class="cell-title"><a href="https://www.notion.so/eb6634ec61ee4e7ca22898edf2c2d4f2">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/uuencode.html">uuencode</a></td><td class="cell-yrFK">Encode a binary file</td></tr><tr id="38f3dbaf-766d-4e40-933d-042b98a9d561"><td class="cell-title"><a href="https://www.notion.so/38f3dbaf766d4e40933d042b98a9d561">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/uuencode.html">uudecode</a></td><td class="cell-yrFK">Decode a file created by uuencode</td></tr><tr id="546f0be8-01a3-4630-bf71-7628807349e2"><td class="cell-title"><a href="https://www.notion.so/V-546f0be801a34630bf717628807349e2">V</a></td><td class="cell-RMJm"></td><td class="cell-yrFK"></td></tr><tr id="11e7b384-0560-43bb-9f69-c644c0eba013"><td class="cell-title"><a href="https://www.notion.so/11e7b384056043bb9f69c644c0eba013">Untitled</a></td><td class="cell-RMJm">v</td><td class="cell-yrFK">Verbosely list directory contents (&#x27;ls -l -b&#x27;)</td></tr><tr id="b9308c03-72d9-4451-812a-b9508c2cb9f9"><td class="cell-title"><a href="https://www.notion.so/b9308c0372d94451812ab9508c2cb9f9">Untitled</a></td><td class="cell-RMJm">vdir</td><td class="cell-yrFK">Verbosely list directory contents (&#x27;ls -l -b&#x27;)</td></tr><tr id="9084cbc9-17c3-4b6c-9468-30fc25087deb"><td class="cell-title"><a href="https://www.notion.so/9084cbc917c34b6c946830fc25087deb">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/vi.html">vi</a></td><td class="cell-yrFK">Text Editor</td></tr><tr id="f4980e8d-9117-474b-a205-632b75e76391"><td class="cell-title"><a href="https://www.notion.so/f4980e8d9117474ba205632b75e76391">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/vmstat.html">vmstat</a></td><td class="cell-yrFK">Report virtual memory statistics</td></tr><tr id="59d9b955-dbb5-4767-a697-c9279eebce8e"><td class="cell-title"><a href="https://www.notion.so/W-59d9b955dbb54767a697c9279eebce8e">W</a></td><td class="cell-RMJm"></td><td class="cell-yrFK"></td></tr><tr id="f7533503-adb7-45be-82e4-d091ff3e5696"><td class="cell-title"><a href="https://www.notion.so/f7533503adb745be82e4d091ff3e5696">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/w.html">w</a></td><td class="cell-yrFK">Show who is logged on and what they are doing</td></tr><tr id="3816c526-3d00-4cb1-8a71-72704fb58f12"><td class="cell-title"><a href="https://www.notion.so/3816c5263d004cb18a7172704fb58f12">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/wait.html">wait</a></td><td class="cell-yrFK">Wait for a process to complete •</td></tr><tr id="806190c4-02f0-4d62-9cf9-979880630612"><td class="cell-title"><a href="https://www.notion.so/806190c402f04d629cf9979880630612">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/watch.html">watch</a></td><td class="cell-yrFK">Execute/display a program periodically</td></tr><tr id="71a83484-299e-4f30-b9a5-abc1e4f48e78"><td class="cell-title"><a href="https://www.notion.so/71a83484299e4f30b9a5abc1e4f48e78">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/wc.html">wc</a></td><td class="cell-yrFK">Print byte, word, and line counts</td></tr><tr id="25ca390b-99dc-4960-bf7c-158d5c0d0142"><td class="cell-title"><a href="https://www.notion.so/25ca390b99dc4960bf7c158d5c0d0142">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/whereis.html">whereis</a></td><td class="cell-yrFK">Search the user&#x27;s $path, man pages and source files for a program</td></tr><tr id="15e315a0-02e3-4394-9721-2c57e7607951"><td class="cell-title"><a href="https://www.notion.so/15e315a002e3439497212c57e7607951">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/which.html">which</a></td><td class="cell-yrFK">Search the user&#x27;s $path for a program file</td></tr><tr id="d01e15fa-71a0-44e4-a91d-57a9caacd869"><td class="cell-title"><a href="https://www.notion.so/d01e15fa71a044e4a91d57a9caacd869">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/while.html">while</a></td><td class="cell-yrFK">Execute commands</td></tr><tr id="efab26ec-eefc-4d29-9d56-80fca426a97f"><td class="cell-title"><a href="https://www.notion.so/efab26eceefc4d299d5680fca426a97f">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/who.html">who</a></td><td class="cell-yrFK">Print all usernames currently logged in</td></tr><tr id="e211057b-3db2-4d9a-a5f3-9a5b449e32bc"><td class="cell-title"><a href="https://www.notion.so/e211057b3db24d9aa5f39a5b449e32bc">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/whoami.html">whoami</a></td><td class="cell-yrFK">Print the current user id and name (&#x27;id -un&#x27;)</td></tr><tr id="feef6ef7-933b-4d42-8029-c2cb36f90968"><td class="cell-title"><a href="https://www.notion.so/feef6ef7933b4d428029c2cb36f90968">Untitled</a></td><td class="cell-RMJm">wget</td><td class="cell-yrFK">Retrieve web pages or files via HTTP, HTTPS or FTP</td></tr><tr id="20a35e23-ac36-4113-a481-de8528cbed20"><td class="cell-title"><a href="https://www.notion.so/20a35e23ac364113a481de8528cbed20">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/write.html">write</a></td><td class="cell-yrFK">Send a message to another user</td></tr><tr id="11262f73-aa5a-4657-a912-c017b6752b4e"><td class="cell-title"><a href="https://www.notion.so/X-11262f73aa5a4657a912c017b6752b4e">X</a></td><td class="cell-RMJm"></td><td class="cell-yrFK"></td></tr><tr id="e23717bb-b719-4d25-ba13-4206080f52d1"><td class="cell-title"><a href="https://www.notion.so/e23717bbb7194d25ba134206080f52d1">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/xargs.html">xargs</a></td><td class="cell-yrFK">Execute utility, passing constructed argument list(s)</td></tr><tr id="7bdc0032-fab3-4a15-90dd-ab8a33b66de3"><td class="cell-title"><a href="https://www.notion.so/7bdc0032fab34a1590ddab8a33b66de3">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/xdg-open.html">xdg-open</a></td><td class="cell-yrFK">Open a file or URL in the user&#x27;s preferred application.</td></tr><tr id="772be068-f5c9-4d63-996a-a3b21ef011b4"><td class="cell-title"><a href="https://www.notion.so/772be068f5c94d63996aa3b21ef011b4">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/xxd.html">xxd</a></td><td class="cell-yrFK">Make a hexdump or do the reverse</td></tr><tr id="d7648c9f-66f9-46cb-a808-7cb7ea1c9766"><td class="cell-title"><a href="https://www.notion.so/d7648c9f66f946cba8087cb7ea1c9766">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/xz.html">xz</a></td><td class="cell-yrFK">Compress or decompress .xz and .lzma files</td></tr><tr id="41c33fd2-da68-421d-9687-5ee7c599a146"><td class="cell-title"><a href="https://www.notion.so/41c33fd2da68421d96875ee7c599a146">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/yes.html">yes</a></td><td class="cell-yrFK">Print a string until interrupted</td></tr><tr id="a4664bb0-c2b3-46df-a695-3557662f4364"><td class="cell-title"><a href="https://www.notion.so/a4664bb0c2b346dfa6953557662f4364">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/zip.html">zip</a></td><td class="cell-yrFK">Package and compress (archive) files</td></tr><tr id="f5e6a39e-e598-404f-8aec-40faaaf18a84"><td class="cell-title"><a href="https://www.notion.so/f5e6a39ee598404f8aec40faaaf18a84">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/source.html">.</a></td><td class="cell-yrFK"><a href="https://ss64.com/bash/source.html">Run</a> a command script in the current shell</td></tr><tr id="daaaab95-2a84-47a0-b4dc-5bdcfe6b7fcf"><td class="cell-title"><a href="https://www.notion.so/daaaab952a8447a0b4dc5bdcfe6b7fcf">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/bang.html">!!</a></td><td class="cell-yrFK">Run the <a href="https://ss64.com/bash/bang.html">last</a> command again</td></tr><tr id="140b4389-2ad6-43d5-8b00-c8422f8d38cc"><td class="cell-title"><a href="https://www.notion.so/140b43892ad643d58b00c8422f8d38cc">Untitled</a></td><td class="cell-RMJm"><a href="https://ss64.com/bash/rem.html">###</a></td><td class="cell-yrFK">Comment / <a href="https://ss64.com/bash/rem.html">Rem</a>ark</td></tr></tbody></table></div></div></article></body></html>
