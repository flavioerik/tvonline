<html lang="pt-BR"><head>
		<script type="module">import { injectIntoGlobalHook } from "/@react-refresh"
injectIntoGlobalHook(window);
window.$RefreshReg$ = () => {};
window.$RefreshSig$ = () => (type) => type;</script>

		<script type="module" src="/@vite/client"></script>

		<meta charset="UTF-8">
		<link rel="icon" type="image/svg+xml" href="/vite.svg">
		<meta name="generator" content="Hostinger Horizons">
		<meta name="viewport" content="width=device-width, initial-scale=1.0">
		<title>SharkTV - O Melhor IPTV do Brasil</title>
		<meta name="description" content="SharkTV oferece a melhor experiência de IPTV no Brasil com mais de 10.000 canais, qualidade 4K e suporte 24/7.">
		<style>
  #root[data-edit-mode-enabled="true"] [data-edit-id] {
    cursor: pointer; 
    outline: 1px dashed #357DF9; 
    outline-offset: 2px;
    min-height: 1em;
  }
  #root[data-edit-mode-enabled="true"] {
    cursor: pointer;
  }
  #root[data-edit-mode-enabled="true"] [data-edit-id]:hover {
    background-color: #357DF933;
    outline-color: #357DF9; 
  }

  @keyframes fadeInTooltip {
    from {
      opacity: 0;
      transform: translateY(5px);
    }
    to {
      opacity: 1;
      transform: translateY(0);
    }
  }

  #inline-editor-disabled-tooltip {
    display: none; 
    opacity: 0; 
    position: absolute;
    background-color: #1D1E20;
    color: white;
    padding: 4px 8px;
    border-radius: 8px;
    z-index: 10001;
    font-size: 14px;
    border: 1px solid #3B3D4A;
    max-width: 184px;
    text-align: center;
  }

  #inline-editor-disabled-tooltip.tooltip-active {
    display: block;
    animation: fadeInTooltip 0.2s ease-out forwards;
  }
</style>
		<script type="module">
window.onerror = (message, source, lineno, colno, errorObj) => {
	const errorDetails = errorObj ? JSON.stringify({
		name: errorObj.name,
		message: errorObj.message,
		stack: errorObj.stack,
		source,
		lineno,
		colno,
	}) : null;

	window.parent.postMessage({
		type: 'horizons-runtime-error',
		message,
		error: errorDetails
	}, '*');
};
</script>
		<script type="module">
const observer = new MutationObserver((mutations) => {
	for (const mutation of mutations) {
		for (const addedNode of mutation.addedNodes) {
			if (
				addedNode.nodeType === Node.ELEMENT_NODE &&
				(
					addedNode.tagName?.toLowerCase() === 'vite-error-overlay' ||
					addedNode.classList?.contains('backdrop')
				)
			) {
				handleViteOverlay(addedNode);
			}
		}
	}
});

observer.observe(document.documentElement, {
	childList: true,
	subtree: true
});

function handleViteOverlay(node) {
	if (!node.shadowRoot) {
		return;
	}

	const backdrop = node.shadowRoot.querySelector('.backdrop');

	if (backdrop) {
		const overlayHtml = backdrop.outerHTML;
		const parser = new DOMParser();
		const doc = parser.parseFromString(overlayHtml, 'text/html');
		const messageBodyElement = doc.querySelector('.message-body');
		const fileElement = doc.querySelector('.file');
		const messageText = messageBodyElement ? messageBodyElement.textContent.trim() : '';
		const fileText = fileElement ? fileElement.textContent.trim() : '';
		const error = messageText + (fileText ? ' File:' + fileText : '');

		window.parent.postMessage({
			type: 'horizons-vite-error',
			error,
		}, '*');
	}
}
</script>
		<script type="module">
const originalConsoleError = console.error;
console.error = function(...args) {
	originalConsoleError.apply(console, args);

	let errorString = '';

	for (let i = 0; i < args.length; i++) {
		const arg = args[i];
		if (arg instanceof Error) {
			errorString = arg.stack || `${arg.name}: ${arg.message}`;
			break;
		}
	}

	if (!errorString) {
		errorString = args.map(arg => typeof arg === 'object' ? JSON.stringify(arg) : String(arg)).join(' ');
	}

	window.parent.postMessage({
		type: 'horizons-console-error',
		error: errorString
	}, '*');
};
</script>
		<script type="module">
const originalFetch = window.fetch;

window.fetch = function(...args) {
	const url = args[0] instanceof Request ? args[0].url : args[0];

	// Skip WebSocket URLs
	if (url.startsWith('ws:') || url.startsWith('wss:')) {
		return originalFetch.apply(this, args);
	}

	return originalFetch.apply(this, args)
		.then(async response => {
			const contentType = response.headers.get('Content-Type') || '';

			// Exclude HTML document responses
			const isDocumentResponse =
				contentType.includes('text/html') ||
				contentType.includes('application/xhtml+xml');

			if (!response.ok && !isDocumentResponse) {
					const responseClone = response.clone();
					const errorFromRes = await responseClone.text();
					const requestUrl = response.url;
					console.error(`Fetch error from ${requestUrl}: ${errorFromRes}`);
			}

			return response;
		})
		.catch(error => {
			if (!url.match(/.html?$/i)) {
				console.error(error);
			}

			throw error;
		});
};
</script>
	<style type="text/css" data-vite-dev-id="/home/u126449404/websites/v4S4fTNJe/public_html/src/index.css">
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800;900&display=swap');
*, ::before, ::after{
  --tw-border-spacing-x: 0;
  --tw-border-spacing-y: 0;
  --tw-translate-x: 0;
  --tw-translate-y: 0;
  --tw-rotate: 0;
  --tw-skew-x: 0;
  --tw-skew-y: 0;
  --tw-scale-x: 1;
  --tw-scale-y: 1;
  --tw-pan-x:  ;
  --tw-pan-y:  ;
  --tw-pinch-zoom:  ;
  --tw-scroll-snap-strictness: proximity;
  --tw-gradient-from-position:  ;
  --tw-gradient-via-position:  ;
  --tw-gradient-to-position:  ;
  --tw-ordinal:  ;
  --tw-slashed-zero:  ;
  --tw-numeric-figure:  ;
  --tw-numeric-spacing:  ;
  --tw-numeric-fraction:  ;
  --tw-ring-inset:  ;
  --tw-ring-offset-width: 0px;
  --tw-ring-offset-color: #fff;
  --tw-ring-color: rgb(59 130 246 / 0.5);
  --tw-ring-offset-shadow: 0 0 #0000;
  --tw-ring-shadow: 0 0 #0000;
  --tw-shadow: 0 0 #0000;
  --tw-shadow-colored: 0 0 #0000;
  --tw-blur:  ;
  --tw-brightness:  ;
  --tw-contrast:  ;
  --tw-grayscale:  ;
  --tw-hue-rotate:  ;
  --tw-invert:  ;
  --tw-saturate:  ;
  --tw-sepia:  ;
  --tw-drop-shadow:  ;
  --tw-backdrop-blur:  ;
  --tw-backdrop-brightness:  ;
  --tw-backdrop-contrast:  ;
  --tw-backdrop-grayscale:  ;
  --tw-backdrop-hue-rotate:  ;
  --tw-backdrop-invert:  ;
  --tw-backdrop-opacity:  ;
  --tw-backdrop-saturate:  ;
  --tw-backdrop-sepia:  ;
  --tw-contain-size:  ;
  --tw-contain-layout:  ;
  --tw-contain-paint:  ;
  --tw-contain-style:  ;
}
::backdrop{
  --tw-border-spacing-x: 0;
  --tw-border-spacing-y: 0;
  --tw-translate-x: 0;
  --tw-translate-y: 0;
  --tw-rotate: 0;
  --tw-skew-x: 0;
  --tw-skew-y: 0;
  --tw-scale-x: 1;
  --tw-scale-y: 1;
  --tw-pan-x:  ;
  --tw-pan-y:  ;
  --tw-pinch-zoom:  ;
  --tw-scroll-snap-strictness: proximity;
  --tw-gradient-from-position:  ;
  --tw-gradient-via-position:  ;
  --tw-gradient-to-position:  ;
  --tw-ordinal:  ;
  --tw-slashed-zero:  ;
  --tw-numeric-figure:  ;
  --tw-numeric-spacing:  ;
  --tw-numeric-fraction:  ;
  --tw-ring-inset:  ;
  --tw-ring-offset-width: 0px;
  --tw-ring-offset-color: #fff;
  --tw-ring-color: rgb(59 130 246 / 0.5);
  --tw-ring-offset-shadow: 0 0 #0000;
  --tw-ring-shadow: 0 0 #0000;
  --tw-shadow: 0 0 #0000;
  --tw-shadow-colored: 0 0 #0000;
  --tw-blur:  ;
  --tw-brightness:  ;
  --tw-contrast:  ;
  --tw-grayscale:  ;
  --tw-hue-rotate:  ;
  --tw-invert:  ;
  --tw-saturate:  ;
  --tw-sepia:  ;
  --tw-drop-shadow:  ;
  --tw-backdrop-blur:  ;
  --tw-backdrop-brightness:  ;
  --tw-backdrop-contrast:  ;
  --tw-backdrop-grayscale:  ;
  --tw-backdrop-hue-rotate:  ;
  --tw-backdrop-invert:  ;
  --tw-backdrop-opacity:  ;
  --tw-backdrop-saturate:  ;
  --tw-backdrop-sepia:  ;
  --tw-contain-size:  ;
  --tw-contain-layout:  ;
  --tw-contain-paint:  ;
  --tw-contain-style:  ;
}
/*
! tailwindcss v3.4.17 | MIT License | https://tailwindcss.com
*/
/*
1. Prevent padding and border from affecting element width. (https://github.com/mozdevs/cssremedy/issues/4)
2. Allow adding a border to an element by just adding a border-width. (https://github.com/tailwindcss/tailwindcss/pull/116)
*/
*,
::before,
::after {
  box-sizing: border-box; /* 1 */
  border-width: 0; /* 2 */
  border-style: solid; /* 2 */
  border-color: #e5e7eb; /* 2 */
}
::before,
::after {
  --tw-content: '';
}
/*
1. Use a consistent sensible line-height in all browsers.
2. Prevent adjustments of font size after orientation changes in iOS.
3. Use a more readable tab size.
4. Use the user's configured `sans` font-family by default.
5. Use the user's configured `sans` font-feature-settings by default.
6. Use the user's configured `sans` font-variation-settings by default.
7. Disable tap highlights on iOS
*/
html,
:host {
  line-height: 1.5; /* 1 */
  -webkit-text-size-adjust: 100%; /* 2 */
  -moz-tab-size: 4; /* 3 */
  -o-tab-size: 4;
     tab-size: 4; /* 3 */
  font-family: ui-sans-serif, system-ui, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"; /* 4 */
  font-feature-settings: normal; /* 5 */
  font-variation-settings: normal; /* 6 */
  -webkit-tap-highlight-color: transparent; /* 7 */
}
/*
1. Remove the margin in all browsers.
2. Inherit line-height from `html` so users can set them as a class directly on the `html` element.
*/
body {
  margin: 0; /* 1 */
  line-height: inherit; /* 2 */
}
/*
1. Add the correct height in Firefox.
2. Correct the inheritance of border color in Firefox. (https://bugzilla.mozilla.org/show_bug.cgi?id=190655)
3. Ensure horizontal rules are visible by default.
*/
hr {
  height: 0; /* 1 */
  color: inherit; /* 2 */
  border-top-width: 1px; /* 3 */
}
/*
Add the correct text decoration in Chrome, Edge, and Safari.
*/
abbr:where([title]) {
  -webkit-text-decoration: underline dotted;
          text-decoration: underline dotted;
}
/*
Remove the default font size and weight for headings.
*/
h1,
h2,
h3,
h4,
h5,
h6 {
  font-size: inherit;
  font-weight: inherit;
}
/*
Reset links to optimize for opt-in styling instead of opt-out.
*/
a {
  color: inherit;
  text-decoration: inherit;
}
/*
Add the correct font weight in Edge and Safari.
*/
b,
strong {
  font-weight: bolder;
}
/*
1. Use the user's configured `mono` font-family by default.
2. Use the user's configured `mono` font-feature-settings by default.
3. Use the user's configured `mono` font-variation-settings by default.
4. Correct the odd `em` font sizing in all browsers.
*/
code,
kbd,
samp,
pre {
  font-family: ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, "Liberation Mono", "Courier New", monospace; /* 1 */
  font-feature-settings: normal; /* 2 */
  font-variation-settings: normal; /* 3 */
  font-size: 1em; /* 4 */
}
/*
Add the correct font size in all browsers.
*/
small {
  font-size: 80%;
}
/*
Prevent `sub` and `sup` elements from affecting the line height in all browsers.
*/
sub,
sup {
  font-size: 75%;
  line-height: 0;
  position: relative;
  vertical-align: baseline;
}
sub {
  bottom: -0.25em;
}
sup {
  top: -0.5em;
}
/*
1. Remove text indentation from table contents in Chrome and Safari. (https://bugs.chromium.org/p/chromium/issues/detail?id=999088, https://bugs.webkit.org/show_bug.cgi?id=201297)
2. Correct table border color inheritance in all Chrome and Safari. (https://bugs.chromium.org/p/chromium/issues/detail?id=935729, https://bugs.webkit.org/show_bug.cgi?id=195016)
3. Remove gaps between table borders by default.
*/
table {
  text-indent: 0; /* 1 */
  border-color: inherit; /* 2 */
  border-collapse: collapse; /* 3 */
}
/*
1. Change the font styles in all browsers.
2. Remove the margin in Firefox and Safari.
3. Remove default padding in all browsers.
*/
button,
input,
optgroup,
select,
textarea {
  font-family: inherit; /* 1 */
  font-feature-settings: inherit; /* 1 */
  font-variation-settings: inherit; /* 1 */
  font-size: 100%; /* 1 */
  font-weight: inherit; /* 1 */
  line-height: inherit; /* 1 */
  letter-spacing: inherit; /* 1 */
  color: inherit; /* 1 */
  margin: 0; /* 2 */
  padding: 0; /* 3 */
}
/*
Remove the inheritance of text transform in Edge and Firefox.
*/
button,
select {
  text-transform: none;
}
/*
1. Correct the inability to style clickable types in iOS and Safari.
2. Remove default button styles.
*/
button,
input:where([type='button']),
input:where([type='reset']),
input:where([type='submit']) {
  -webkit-appearance: button; /* 1 */
  background-color: transparent; /* 2 */
  background-image: none; /* 2 */
}
/*
Use the modern Firefox focus style for all focusable elements.
*/
:-moz-focusring {
  outline: auto;
}
/*
Remove the additional `:invalid` styles in Firefox. (https://github.com/mozilla/gecko-dev/blob/2f9eacd9d3d995c937b4251a5557d95d494c9be1/layout/style/res/forms.css#L728-L737)
*/
:-moz-ui-invalid {
  box-shadow: none;
}
/*
Add the correct vertical alignment in Chrome and Firefox.
*/
progress {
  vertical-align: baseline;
}
/*
Correct the cursor style of increment and decrement buttons in Safari.
*/
::-webkit-inner-spin-button,
::-webkit-outer-spin-button {
  height: auto;
}
/*
1. Correct the odd appearance in Chrome and Safari.
2. Correct the outline style in Safari.
*/
[type='search'] {
  -webkit-appearance: textfield; /* 1 */
  outline-offset: -2px; /* 2 */
}
/*
Remove the inner padding in Chrome and Safari on macOS.
*/
::-webkit-search-decoration {
  -webkit-appearance: none;
}
/*
1. Correct the inability to style clickable types in iOS and Safari.
2. Change font properties to `inherit` in Safari.
*/
::-webkit-file-upload-button {
  -webkit-appearance: button; /* 1 */
  font: inherit; /* 2 */
}
/*
Add the correct display in Chrome and Safari.
*/
summary {
  display: list-item;
}
/*
Removes the default spacing and border for appropriate elements.
*/
blockquote,
dl,
dd,
h1,
h2,
h3,
h4,
h5,
h6,
hr,
figure,
p,
pre {
  margin: 0;
}
fieldset {
  margin: 0;
  padding: 0;
}
legend {
  padding: 0;
}
ol,
ul,
menu {
  list-style: none;
  margin: 0;
  padding: 0;
}
/*
Reset default styling for dialogs.
*/
dialog {
  padding: 0;
}
/*
Prevent resizing textareas horizontally by default.
*/
textarea {
  resize: vertical;
}
/*
1. Reset the default placeholder opacity in Firefox. (https://github.com/tailwindlabs/tailwindcss/issues/3300)
2. Set the default placeholder color to the user's configured gray 400 color.
*/
input::-moz-placeholder, textarea::-moz-placeholder {
  opacity: 1; /* 1 */
  color: #9ca3af; /* 2 */
}
input::placeholder,
textarea::placeholder {
  opacity: 1; /* 1 */
  color: #9ca3af; /* 2 */
}
/*
Set the default cursor for buttons.
*/
button,
[role="button"] {
  cursor: pointer;
}
/*
Make sure disabled buttons don't get the pointer cursor.
*/
:disabled {
  cursor: default;
}
/*
1. Make replaced elements `display: block` by default. (https://github.com/mozdevs/cssremedy/issues/14)
2. Add `vertical-align: middle` to align replaced elements more sensibly by default. (https://github.com/jensimmons/cssremedy/issues/14#issuecomment-634934210)
   This can trigger a poorly considered lint error in some tools but is included by design.
*/
img,
svg,
video,
canvas,
audio,
iframe,
embed,
object {
  display: block; /* 1 */
  vertical-align: middle; /* 2 */
}
/*
Constrain images and videos to the parent width and preserve their intrinsic aspect ratio. (https://github.com/mozdevs/cssremedy/issues/14)
*/
img,
video {
  max-width: 100%;
  height: auto;
}
/* Make elements with the HTML hidden attribute stay hidden by default */
[hidden]:where(:not([hidden="until-found"])) {
  display: none;
}
.container{
  width: 100%;
  margin-right: auto;
  margin-left: auto;
  padding-right: 2rem;
  padding-left: 2rem;
}
@media (min-width: 1400px){
  .container{
    max-width: 1400px;
  }
}
.pointer-events-auto{
  pointer-events: auto;
}
.fixed{
  position: fixed;
}
.absolute{
  position: absolute;
}
.relative{
  position: relative;
}
.-top-4{
  top: -1rem;
}
.bottom-6{
  bottom: 1.5rem;
}
.left-1\/2{
  left: 50%;
}
.right-2{
  right: 0.5rem;
}
.right-6{
  right: 1.5rem;
}
.top-0{
  top: 0px;
}
.top-2{
  top: 0.5rem;
}
.z-50{
  z-index: 50;
}
.z-\[100\]{
  z-index: 100;
}
.mx-auto{
  margin-left: auto;
  margin-right: auto;
}
.mb-12{
  margin-bottom: 3rem;
}
.mb-16{
  margin-bottom: 4rem;
}
.mb-2{
  margin-bottom: 0.5rem;
}
.mb-3{
  margin-bottom: 0.75rem;
}
.mb-4{
  margin-bottom: 1rem;
}
.mb-6{
  margin-bottom: 1.5rem;
}
.mb-8{
  margin-bottom: 2rem;
}
.ml-2{
  margin-left: 0.5rem;
}
.mr-2{
  margin-right: 0.5rem;
}
.mr-3{
  margin-right: 0.75rem;
}
.mt-8{
  margin-top: 2rem;
}
.block{
  display: block;
}
.flex{
  display: flex;
}
.inline-flex{
  display: inline-flex;
}
.grid{
  display: grid;
}
.hidden{
  display: none;
}
.h-10{
  height: 2.5rem;
}
.h-11{
  height: 2.75rem;
}
.h-12{
  height: 3rem;
}
.h-16{
  height: 4rem;
}
.h-20{
  height: 5rem;
}
.h-3{
  height: 0.75rem;
}
.h-4{
  height: 1rem;
}
.h-5{
  height: 1.25rem;
}
.h-6{
  height: 1.5rem;
}
.h-8{
  height: 2rem;
}
.h-9{
  height: 2.25rem;
}
.max-h-screen{
  max-height: 100vh;
}
.min-h-screen{
  min-height: 100vh;
}
.w-10{
  width: 2.5rem;
}
.w-12{
  width: 3rem;
}
.w-16{
  width: 4rem;
}
.w-20{
  width: 5rem;
}
.w-3{
  width: 0.75rem;
}
.w-4{
  width: 1rem;
}
.w-5{
  width: 1.25rem;
}
.w-6{
  width: 1.5rem;
}
.w-8{
  width: 2rem;
}
.w-full{
  width: 100%;
}
.max-w-2xl{
  max-width: 42rem;
}
.max-w-3xl{
  max-width: 48rem;
}
.max-w-4xl{
  max-width: 56rem;
}
.max-w-6xl{
  max-width: 72rem;
}
.flex-shrink-0{
  flex-shrink: 0;
}
.shrink-0{
  flex-shrink: 0;
}
.-translate-x-1\/2{
  --tw-translate-x: -50%;
  transform: translate(var(--tw-translate-x), var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));
}
.transform{
  transform: translate(var(--tw-translate-x), var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));
}
.cursor-pointer{
  cursor: pointer;
}
.resize-none{
  resize: none;
}
.grid-cols-2{
  grid-template-columns: repeat(2, minmax(0, 1fr));
}
.flex-col{
  flex-direction: column;
}
.flex-col-reverse{
  flex-direction: column-reverse;
}
.items-center{
  align-items: center;
}
.justify-center{
  justify-content: center;
}
.justify-between{
  justify-content: space-between;
}
.gap-1{
  gap: 0.25rem;
}
.gap-12{
  gap: 3rem;
}
.gap-4{
  gap: 1rem;
}
.gap-8{
  gap: 2rem;
}
.space-x-2 > :not([hidden]) ~ :not([hidden]){
  --tw-space-x-reverse: 0;
  margin-right: calc(0.5rem * var(--tw-space-x-reverse));
  margin-left: calc(0.5rem * calc(1 - var(--tw-space-x-reverse)));
}
.space-x-4 > :not([hidden]) ~ :not([hidden]){
  --tw-space-x-reverse: 0;
  margin-right: calc(1rem * var(--tw-space-x-reverse));
  margin-left: calc(1rem * calc(1 - var(--tw-space-x-reverse)));
}
.space-x-8 > :not([hidden]) ~ :not([hidden]){
  --tw-space-x-reverse: 0;
  margin-right: calc(2rem * var(--tw-space-x-reverse));
  margin-left: calc(2rem * calc(1 - var(--tw-space-x-reverse)));
}
.space-y-2 > :not([hidden]) ~ :not([hidden]){
  --tw-space-y-reverse: 0;
  margin-top: calc(0.5rem * calc(1 - var(--tw-space-y-reverse)));
  margin-bottom: calc(0.5rem * var(--tw-space-y-reverse));
}
.space-y-3 > :not([hidden]) ~ :not([hidden]){
  --tw-space-y-reverse: 0;
  margin-top: calc(0.75rem * calc(1 - var(--tw-space-y-reverse)));
  margin-bottom: calc(0.75rem * var(--tw-space-y-reverse));
}
.space-y-4 > :not([hidden]) ~ :not([hidden]){
  --tw-space-y-reverse: 0;
  margin-top: calc(1rem * calc(1 - var(--tw-space-y-reverse)));
  margin-bottom: calc(1rem * var(--tw-space-y-reverse));
}
.space-y-8 > :not([hidden]) ~ :not([hidden]){
  --tw-space-y-reverse: 0;
  margin-top: calc(2rem * calc(1 - var(--tw-space-y-reverse)));
  margin-bottom: calc(2rem * var(--tw-space-y-reverse));
}
.overflow-hidden{
  overflow: hidden;
}
.rounded-2xl{
  border-radius: 1rem;
}
.rounded-3xl{
  border-radius: 1.5rem;
}
.rounded-full{
  border-radius: 9999px;
}
.rounded-lg{
  border-radius: var(--radius);
}
.rounded-md{
  border-radius: calc(var(--radius) - 2px);
}
.rounded-xl{
  border-radius: 0.75rem;
}
.border{
  border-width: 1px;
}
.border-t{
  border-top-width: 1px;
}
.border-cyan-400{
  --tw-border-opacity: 1;
  border-color: rgb(34 211 238 / var(--tw-border-opacity, 1));
}
.border-destructive{
  border-color: hsl(var(--destructive));
}
.border-input{
  border-color: hsl(var(--input));
}
.border-slate-700{
  --tw-border-opacity: 1;
  border-color: rgb(51 65 85 / var(--tw-border-opacity, 1));
}
.border-slate-800{
  --tw-border-opacity: 1;
  border-color: rgb(30 41 59 / var(--tw-border-opacity, 1));
}
.bg-background{
  background-color: hsl(var(--background));
}
.bg-blue-600{
  --tw-bg-opacity: 1;
  background-color: rgb(37 99 235 / var(--tw-bg-opacity, 1));
}
.bg-cyan-400{
  --tw-bg-opacity: 1;
  background-color: rgb(34 211 238 / var(--tw-bg-opacity, 1));
}
.bg-destructive{
  background-color: hsl(var(--destructive));
}
.bg-gray-600{
  --tw-bg-opacity: 1;
  background-color: rgb(75 85 99 / var(--tw-bg-opacity, 1));
}
.bg-green-500{
  --tw-bg-opacity: 1;
  background-color: rgb(34 197 94 / var(--tw-bg-opacity, 1));
}
.bg-pink-600{
  --tw-bg-opacity: 1;
  background-color: rgb(219 39 119 / var(--tw-bg-opacity, 1));
}
.bg-primary{
  background-color: hsl(var(--primary));
}
.bg-red-600{
  --tw-bg-opacity: 1;
  background-color: rgb(220 38 38 / var(--tw-bg-opacity, 1));
}
.bg-secondary{
  background-color: hsl(var(--secondary));
}
.bg-slate-800{
  --tw-bg-opacity: 1;
  background-color: rgb(30 41 59 / var(--tw-bg-opacity, 1));
}
.bg-slate-900{
  --tw-bg-opacity: 1;
  background-color: rgb(15 23 42 / var(--tw-bg-opacity, 1));
}
.bg-slate-900\/50{
  background-color: rgb(15 23 42 / 0.5);
}
.bg-slate-900\/95{
  background-color: rgb(15 23 42 / 0.95);
}
.bg-transparent{
  background-color: transparent;
}
.bg-gradient-to-br{
  background-image: linear-gradient(to bottom right, var(--tw-gradient-stops));
}
.bg-gradient-to-r{
  background-image: linear-gradient(to right, var(--tw-gradient-stops));
}
.from-blue-500{
  --tw-gradient-from: #3b82f6 var(--tw-gradient-from-position);
  --tw-gradient-to: rgb(59 130 246 / 0) var(--tw-gradient-to-position);
  --tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to);
}
.from-cyan-500{
  --tw-gradient-from: #06b6d4 var(--tw-gradient-from-position);
  --tw-gradient-to: rgb(6 182 212 / 0) var(--tw-gradient-to-position);
  --tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to);
}
.from-green-500{
  --tw-gradient-from: #22c55e var(--tw-gradient-from-position);
  --tw-gradient-to: rgb(34 197 94 / 0) var(--tw-gradient-to-position);
  --tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to);
}
.from-orange-500{
  --tw-gradient-from: #f97316 var(--tw-gradient-from-position);
  --tw-gradient-to: rgb(249 115 22 / 0) var(--tw-gradient-to-position);
  --tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to);
}
.from-purple-500{
  --tw-gradient-from: #a855f7 var(--tw-gradient-from-position);
  --tw-gradient-to: rgb(168 85 247 / 0) var(--tw-gradient-to-position);
  --tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to);
}
.from-red-500{
  --tw-gradient-from: #ef4444 var(--tw-gradient-from-position);
  --tw-gradient-to: rgb(239 68 68 / 0) var(--tw-gradient-to-position);
  --tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to);
}
.from-slate-900{
  --tw-gradient-from: #0f172a var(--tw-gradient-from-position);
  --tw-gradient-to: rgb(15 23 42 / 0) var(--tw-gradient-to-position);
  --tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to);
}
.via-blue-900{
  --tw-gradient-to: rgb(30 58 138 / 0)  var(--tw-gradient-to-position);
  --tw-gradient-stops: var(--tw-gradient-from), #1e3a8a var(--tw-gradient-via-position), var(--tw-gradient-to);
}
.to-blue-500{
  --tw-gradient-to: #3b82f6 var(--tw-gradient-to-position);
}
.to-blue-600{
  --tw-gradient-to: #2563eb var(--tw-gradient-to-position);
}
.to-cyan-500{
  --tw-gradient-to: #06b6d4 var(--tw-gradient-to-position);
}
.to-green-600{
  --tw-gradient-to: #16a34a var(--tw-gradient-to-position);
}
.to-pink-500{
  --tw-gradient-to: #ec4899 var(--tw-gradient-to-position);
}
.to-purple-600{
  --tw-gradient-to: #9333ea var(--tw-gradient-to-position);
}
.to-red-500{
  --tw-gradient-to: #ef4444 var(--tw-gradient-to-position);
}
.to-red-600{
  --tw-gradient-to: #dc2626 var(--tw-gradient-to-position);
}
.to-slate-900{
  --tw-gradient-to: #0f172a var(--tw-gradient-to-position);
}
.fill-current{
  fill: currentColor;
}
.p-1{
  padding: 0.25rem;
}
.p-4{
  padding: 1rem;
}
.p-6{
  padding: 1.5rem;
}
.p-8{
  padding: 2rem;
}
.px-3{
  padding-left: 0.75rem;
  padding-right: 0.75rem;
}
.px-4{
  padding-left: 1rem;
  padding-right: 1rem;
}
.px-6{
  padding-left: 1.5rem;
  padding-right: 1.5rem;
}
.px-8{
  padding-left: 2rem;
  padding-right: 2rem;
}
.py-12{
  padding-top: 3rem;
  padding-bottom: 3rem;
}
.py-16{
  padding-top: 4rem;
  padding-bottom: 4rem;
}
.py-2{
  padding-top: 0.5rem;
  padding-bottom: 0.5rem;
}
.py-3{
  padding-top: 0.75rem;
  padding-bottom: 0.75rem;
}
.py-4{
  padding-top: 1rem;
  padding-bottom: 1rem;
}
.pb-16{
  padding-bottom: 4rem;
}
.pr-8{
  padding-right: 2rem;
}
.pt-24{
  padding-top: 6rem;
}
.pt-8{
  padding-top: 2rem;
}
.text-center{
  text-align: center;
}
.text-2xl{
  font-size: 1.5rem;
  line-height: 2rem;
}
.text-3xl{
  font-size: 1.875rem;
  line-height: 2.25rem;
}
.text-4xl{
  font-size: 2.25rem;
  line-height: 2.5rem;
}
.text-5xl{
  font-size: 3rem;
  line-height: 1;
}
.text-lg{
  font-size: 1.125rem;
  line-height: 1.75rem;
}
.text-sm{
  font-size: 0.875rem;
  line-height: 1.25rem;
}
.text-xl{
  font-size: 1.25rem;
  line-height: 1.75rem;
}
.font-black{
  font-weight: 900;
}
.font-bold{
  font-weight: 700;
}
.font-medium{
  font-weight: 500;
}
.font-semibold{
  font-weight: 600;
}
.italic{
  font-style: italic;
}
.leading-relaxed{
  line-height: 1.625;
}
.text-cyan-400{
  --tw-text-opacity: 1;
  color: rgb(34 211 238 / var(--tw-text-opacity, 1));
}
.text-destructive-foreground{
  color: hsl(var(--destructive-foreground));
}
.text-foreground\/50{
  color: hsl(var(--foreground) / 0.5);
}
.text-gray-300{
  --tw-text-opacity: 1;
  color: rgb(209 213 219 / var(--tw-text-opacity, 1));
}
.text-gray-400{
  --tw-text-opacity: 1;
  color: rgb(156 163 175 / var(--tw-text-opacity, 1));
}
.text-green-400{
  --tw-text-opacity: 1;
  color: rgb(74 222 128 / var(--tw-text-opacity, 1));
}
.text-primary{
  color: hsl(var(--primary));
}
.text-primary-foreground{
  color: hsl(var(--primary-foreground));
}
.text-secondary-foreground{
  color: hsl(var(--secondary-foreground));
}
.text-white{
  --tw-text-opacity: 1;
  color: rgb(255 255 255 / var(--tw-text-opacity, 1));
}
.text-yellow-400{
  --tw-text-opacity: 1;
  color: rgb(250 204 21 / var(--tw-text-opacity, 1));
}
.underline-offset-4{
  text-underline-offset: 4px;
}
.placeholder-gray-400::-moz-placeholder{
  --tw-placeholder-opacity: 1;
  color: rgb(156 163 175 / var(--tw-placeholder-opacity, 1));
}
.placeholder-gray-400::placeholder{
  --tw-placeholder-opacity: 1;
  color: rgb(156 163 175 / var(--tw-placeholder-opacity, 1));
}
.opacity-0{
  opacity: 0;
}
.opacity-90{
  opacity: 0.9;
}
.shadow-lg{
  --tw-shadow: 0 10px 15px -3px rgb(0 0 0 / 0.1), 0 4px 6px -4px rgb(0 0 0 / 0.1);
  --tw-shadow-colored: 0 10px 15px -3px var(--tw-shadow-color), 0 4px 6px -4px var(--tw-shadow-color);
  box-shadow: var(--tw-ring-offset-shadow, 0 0 #0000), var(--tw-ring-shadow, 0 0 #0000), var(--tw-shadow);
}
.outline{
  outline-style: solid;
}
.ring-2{
  --tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);
  --tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(2px + var(--tw-ring-offset-width)) var(--tw-ring-color);
  box-shadow: var(--tw-ring-offset-shadow), var(--tw-ring-shadow), var(--tw-shadow, 0 0 #0000);
}
.ring-cyan-400{
  --tw-ring-opacity: 1;
  --tw-ring-color: rgb(34 211 238 / var(--tw-ring-opacity, 1));
}
.ring-offset-background{
  --tw-ring-offset-color: hsl(var(--background));
}
.filter{
  filter: var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) var(--tw-invert) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow);
}
.backdrop-blur-lg{
  --tw-backdrop-blur: blur(16px);
  -webkit-backdrop-filter: var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);
  backdrop-filter: var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);
}
.transition{
  transition-property: color, background-color, border-color, text-decoration-color, fill, stroke, opacity, box-shadow, transform, filter, -webkit-backdrop-filter;
  transition-property: color, background-color, border-color, text-decoration-color, fill, stroke, opacity, box-shadow, transform, filter, backdrop-filter;
  transition-property: color, background-color, border-color, text-decoration-color, fill, stroke, opacity, box-shadow, transform, filter, backdrop-filter, -webkit-backdrop-filter;
  transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1);
  transition-duration: 150ms;
}
.transition-all{
  transition-property: all;
  transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1);
  transition-duration: 150ms;
}
.transition-colors{
  transition-property: color, background-color, border-color, text-decoration-color, fill, stroke;
  transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1);
  transition-duration: 150ms;
}
.transition-opacity{
  transition-property: opacity;
  transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1);
  transition-duration: 150ms;
}
.duration-300{
  transition-duration: 300ms;
}
@keyframes enter{
  from{
    opacity: var(--tw-enter-opacity, 1);
    transform: translate3d(var(--tw-enter-translate-x, 0), var(--tw-enter-translate-y, 0), 0) scale3d(var(--tw-enter-scale, 1), var(--tw-enter-scale, 1), var(--tw-enter-scale, 1)) rotate(var(--tw-enter-rotate, 0));
  }
}
@keyframes exit{
  to{
    opacity: var(--tw-exit-opacity, 1);
    transform: translate3d(var(--tw-exit-translate-x, 0), var(--tw-exit-translate-y, 0), 0) scale3d(var(--tw-exit-scale, 1), var(--tw-exit-scale, 1), var(--tw-exit-scale, 1)) rotate(var(--tw-exit-rotate, 0));
  }
}
.duration-300{
  animation-duration: 300ms;
}
:root {
  --background: 220 13% 9%;
  --foreground: 220 9% 95%;
  --card: 220 13% 11%;
  --card-foreground: 220 9% 95%;
  --popover: 220 13% 11%;
  --popover-foreground: 220 9% 95%;
  --primary: 197 100% 50%;
  --primary-foreground: 220 13% 9%;
  --secondary: 220 13% 15%;
  --secondary-foreground: 220 9% 95%;
  --muted: 220 13% 15%;
  --muted-foreground: 220 9% 65%;
  --accent: 197 100% 50%;
  --accent-foreground: 220 13% 9%;
  --destructive: 0 84% 60%;
  --destructive-foreground: 220 9% 95%;
  --border: 220 13% 20%;
  --input: 220 13% 20%;
  --ring: 197 100% 50%;
  --radius: 0.5rem;
}
* {
  border-color: hsl(var(--border));
}
body {
  background-color: hsl(var(--background));
  color: hsl(var(--foreground));
  font-family: 'Inter', sans-serif;
}
.gradient-bg {
  background: linear-gradient(135deg, #0ea5e9 0%, #3b82f6 25%, #6366f1 50%, #8b5cf6 75%, #a855f7 100%);
}
.glass-effect {
  background: rgba(255, 255, 255, 0.1);
  -webkit-backdrop-filter: blur(10px);
          backdrop-filter: blur(10px);
  border: 1px solid rgba(255, 255, 255, 0.2);
}
.shark-glow {
  box-shadow: 0 0 30px rgba(14, 165, 233, 0.3);
}
.text-gradient {
  background: linear-gradient(135deg, #0ea5e9, #3b82f6, #6366f1);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}
.floating {
  animation: floating 3s ease-in-out infinite;
}
@keyframes floating {
  0%, 100% { transform: translateY(0px); }
  50% { transform: translateY(-10px); }
}
.pulse-glow {
  animation: pulse-glow 2s ease-in-out infinite;
}
@keyframes pulse-glow {
  0%, 100% { box-shadow: 0 0 20px rgba(14, 165, 233, 0.4); }
  50% { box-shadow: 0 0 40px rgba(14, 165, 233, 0.8); }
}
.channel-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(120px, 1fr));
  gap: 1rem;
}
.neon-border {
  border: 2px solid transparent;
  background: linear-gradient(135deg, #0ea5e9, #3b82f6) border-box;
  -webkit-mask: linear-gradient(#fff 0 0) padding-box, linear-gradient(#fff 0 0);
  -webkit-mask-composite: destination-out;
  -webkit-mask: linear-gradient(#fff 0 0) padding-box, linear-gradient(#fff 0 0);
          mask: linear-gradient(#fff 0 0) padding-box, linear-gradient(#fff 0 0);
  -webkit-mask-composite: xor;
          mask-composite: exclude;
}
.shark-pattern {
  background-image: 
    radial-gradient(circle at 25% 25%, rgba(14, 165, 233, 0.1) 0%, transparent 50%),
    radial-gradient(circle at 75% 75%, rgba(59, 130, 246, 0.1) 0%, transparent 50%);
}
.hover\:bg-accent:hover{
  background-color: hsl(var(--accent));
}
.hover\:bg-blue-700:hover{
  --tw-bg-opacity: 1;
  background-color: rgb(29 78 216 / var(--tw-bg-opacity, 1));
}
.hover\:bg-cyan-400:hover{
  --tw-bg-opacity: 1;
  background-color: rgb(34 211 238 / var(--tw-bg-opacity, 1));
}
.hover\:bg-destructive\/90:hover{
  background-color: hsl(var(--destructive) / 0.9);
}
.hover\:bg-green-600:hover{
  --tw-bg-opacity: 1;
  background-color: rgb(22 163 74 / var(--tw-bg-opacity, 1));
}
.hover\:bg-pink-700:hover{
  --tw-bg-opacity: 1;
  background-color: rgb(190 24 93 / var(--tw-bg-opacity, 1));
}
.hover\:bg-primary\/90:hover{
  background-color: hsl(var(--primary) / 0.9);
}
.hover\:bg-red-700:hover{
  --tw-bg-opacity: 1;
  background-color: rgb(185 28 28 / var(--tw-bg-opacity, 1));
}
.hover\:bg-secondary:hover{
  background-color: hsl(var(--secondary));
}
.hover\:bg-secondary\/80:hover{
  background-color: hsl(var(--secondary) / 0.8);
}
.hover\:from-cyan-600:hover{
  --tw-gradient-from: #0891b2 var(--tw-gradient-from-position);
  --tw-gradient-to: rgb(8 145 178 / 0) var(--tw-gradient-to-position);
  --tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to);
}
.hover\:to-blue-600:hover{
  --tw-gradient-to: #2563eb var(--tw-gradient-to-position);
}
.hover\:text-accent-foreground:hover{
  color: hsl(var(--accent-foreground));
}
.hover\:text-cyan-400:hover{
  --tw-text-opacity: 1;
  color: rgb(34 211 238 / var(--tw-text-opacity, 1));
}
.hover\:text-foreground:hover{
  color: hsl(var(--foreground));
}
.hover\:text-slate-900:hover{
  --tw-text-opacity: 1;
  color: rgb(15 23 42 / var(--tw-text-opacity, 1));
}
.hover\:underline:hover{
  text-decoration-line: underline;
}
.hover\:opacity-90:hover{
  opacity: 0.9;
}
.focus\:border-cyan-400:focus{
  --tw-border-opacity: 1;
  border-color: rgb(34 211 238 / var(--tw-border-opacity, 1));
}
.focus\:opacity-100:focus{
  opacity: 1;
}
.focus\:outline-none:focus{
  outline: 2px solid transparent;
  outline-offset: 2px;
}
.focus\:ring-2:focus{
  --tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);
  --tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(2px + var(--tw-ring-offset-width)) var(--tw-ring-color);
  box-shadow: var(--tw-ring-offset-shadow), var(--tw-ring-shadow), var(--tw-shadow, 0 0 #0000);
}
.focus\:ring-ring:focus{
  --tw-ring-color: hsl(var(--ring));
}
.focus\:ring-offset-2:focus{
  --tw-ring-offset-width: 2px;
}
.focus-visible\:outline-none:focus-visible{
  outline: 2px solid transparent;
  outline-offset: 2px;
}
.focus-visible\:ring-2:focus-visible{
  --tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);
  --tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(2px + var(--tw-ring-offset-width)) var(--tw-ring-color);
  box-shadow: var(--tw-ring-offset-shadow), var(--tw-ring-shadow), var(--tw-shadow, 0 0 #0000);
}
.focus-visible\:ring-ring:focus-visible{
  --tw-ring-color: hsl(var(--ring));
}
.focus-visible\:ring-offset-2:focus-visible{
  --tw-ring-offset-width: 2px;
}
.disabled\:pointer-events-none:disabled{
  pointer-events: none;
}
.disabled\:opacity-50:disabled{
  opacity: 0.5;
}
.group:hover .group-hover\:opacity-100{
  opacity: 1;
}
.group.destructive .group-\[\.destructive\]\:border-destructive\/30{
  border-color: hsl(var(--destructive) / 0.3);
}
.group.destructive .group-\[\.destructive\]\:text-red-300{
  --tw-text-opacity: 1;
  color: rgb(252 165 165 / var(--tw-text-opacity, 1));
}
.group.destructive .group-\[\.destructive\]\:hover\:border-destructive\/30:hover{
  border-color: hsl(var(--destructive) / 0.3);
}
.group.destructive .group-\[\.destructive\]\:hover\:bg-destructive:hover{
  background-color: hsl(var(--destructive));
}
.group.destructive .group-\[\.destructive\]\:hover\:text-destructive-foreground:hover{
  color: hsl(var(--destructive-foreground));
}
.group.destructive .group-\[\.destructive\]\:hover\:text-red-50:hover{
  --tw-text-opacity: 1;
  color: rgb(254 242 242 / var(--tw-text-opacity, 1));
}
.group.destructive .group-\[\.destructive\]\:focus\:ring-destructive:focus{
  --tw-ring-color: hsl(var(--destructive));
}
.group.destructive .group-\[\.destructive\]\:focus\:ring-red-400:focus{
  --tw-ring-opacity: 1;
  --tw-ring-color: rgb(248 113 113 / var(--tw-ring-opacity, 1));
}
.group.destructive .group-\[\.destructive\]\:focus\:ring-offset-red-600:focus{
  --tw-ring-offset-color: #dc2626;
}
.data-\[swipe\=cancel\]\:translate-x-0[data-swipe="cancel"]{
  --tw-translate-x: 0px;
  transform: translate(var(--tw-translate-x), var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));
}
.data-\[swipe\=end\]\:translate-x-\[var\(--radix-toast-swipe-end-x\)\][data-swipe="end"]{
  --tw-translate-x: var(--radix-toast-swipe-end-x);
  transform: translate(var(--tw-translate-x), var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));
}
.data-\[swipe\=move\]\:translate-x-\[var\(--radix-toast-swipe-move-x\)\][data-swipe="move"]{
  --tw-translate-x: var(--radix-toast-swipe-move-x);
  transform: translate(var(--tw-translate-x), var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));
}
.data-\[swipe\=move\]\:transition-none[data-swipe="move"]{
  transition-property: none;
}
.data-\[state\=open\]\:animate-in[data-state="open"]{
  animation-name: enter;
  animation-duration: 150ms;
  --tw-enter-opacity: initial;
  --tw-enter-scale: initial;
  --tw-enter-rotate: initial;
  --tw-enter-translate-x: initial;
  --tw-enter-translate-y: initial;
}
.data-\[state\=closed\]\:animate-out[data-state="closed"]{
  animation-name: exit;
  animation-duration: 150ms;
  --tw-exit-opacity: initial;
  --tw-exit-scale: initial;
  --tw-exit-rotate: initial;
  --tw-exit-translate-x: initial;
  --tw-exit-translate-y: initial;
}
.data-\[swipe\=end\]\:animate-out[data-swipe="end"]{
  animation-name: exit;
  animation-duration: 150ms;
  --tw-exit-opacity: initial;
  --tw-exit-scale: initial;
  --tw-exit-rotate: initial;
  --tw-exit-translate-x: initial;
  --tw-exit-translate-y: initial;
}
.data-\[state\=closed\]\:fade-out-80[data-state="closed"]{
  --tw-exit-opacity: 0.8;
}
.data-\[state\=closed\]\:slide-out-to-right-full[data-state="closed"]{
  --tw-exit-translate-x: 100%;
}
.data-\[state\=open\]\:slide-in-from-top-full[data-state="open"]{
  --tw-enter-translate-y: -100%;
}
@media (min-width: 640px){
  .sm\:bottom-0{
    bottom: 0px;
  }
  .sm\:right-0{
    right: 0px;
  }
  .sm\:top-auto{
    top: auto;
  }
  .sm\:flex-row{
    flex-direction: row;
  }
  .sm\:flex-col{
    flex-direction: column;
  }
  .data-\[state\=open\]\:sm\:slide-in-from-bottom-full[data-state="open"]{
    --tw-enter-translate-y: 100%;
  }
}
@media (min-width: 768px){
  .md\:flex{
    display: flex;
  }
  .md\:hidden{
    display: none;
  }
  .md\:max-w-\[420px\]{
    max-width: 420px;
  }
  .md\:grid-cols-2{
    grid-template-columns: repeat(2, minmax(0, 1fr));
  }
  .md\:grid-cols-3{
    grid-template-columns: repeat(3, minmax(0, 1fr));
  }
  .md\:grid-cols-4{
    grid-template-columns: repeat(4, minmax(0, 1fr));
  }
  .md\:text-2xl{
    font-size: 1.5rem;
    line-height: 2rem;
  }
  .md\:text-5xl{
    font-size: 3rem;
    line-height: 1;
  }
  .md\:text-7xl{
    font-size: 4.5rem;
    line-height: 1;
  }
}
@media (min-width: 1024px){
  .lg\:grid-cols-3{
    grid-template-columns: repeat(3, minmax(0, 1fr));
  }
  .lg\:grid-cols-6{
    grid-template-columns: repeat(6, minmax(0, 1fr));
  }
}
</style></head>
	<body>
		<div id="root"><div class="min-h-screen bg-gradient-to-br from-slate-900 via-blue-900 to-slate-900 shark-pattern"><div role="region" aria-label="Notifications (F8)" tabindex="-1" style="pointer-events: none;"><ol tabindex="-1" class="fixed top-0 z-[100] flex max-h-screen w-full flex-col-reverse p-4 sm:bottom-0 sm:right-0 sm:top-auto sm:flex-col md:max-w-[420px]"></ol></div><header class="fixed top-0 w-full z-50 glass-effect" style="transform: none;"><nav class="container mx-auto px-4 py-4 flex items-center justify-between"><div class="flex items-center space-x-2"><div class="w-10 h-10 bg-gradient-to-r from-blue-500 to-cyan-500 rounded-lg flex items-center justify-center"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-6 h-6 text-white"><rect width="20" height="15" x="2" y="7" rx="2" ry="2"></rect><polyline points="17 2 12 7 7 2"></polyline></svg></div><span class="text-2xl font-bold text-gradient" data-edit-id="src/App.jsx:152:13">SharkTV</span></div><div class="hidden md:flex items-center space-x-8"><button class="text-white hover:text-cyan-400 transition-colors" data-edit-id="src/App.jsx:157:13">Início</button><button class="text-white hover:text-cyan-400 transition-colors" data-edit-id="src/App.jsx:160:13">Planos</button><button class="text-white hover:text-cyan-400 transition-colors" data-edit-id="src/App.jsx:163:13">Canais</button><button class="text-white hover:text-cyan-400 transition-colors" data-edit-id="src/App.jsx:166:13">Depoimentos</button><button class="text-white hover:text-cyan-400 transition-colors" data-edit-id="src/App.jsx:169:13">Contato</button><button class="inline-flex items-center justify-center rounded-md text-sm font-medium ring-offset-background transition-colors focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:pointer-events-none disabled:opacity-50 bg-primary text-primary-foreground hover:bg-primary/90 h-10 px-4 py-2 bg-gradient-to-r from-cyan-500 to-blue-500 hover:from-cyan-600 hover:to-blue-600 pulse-glow" data-edit-id="src/App.jsx:172:13">Assinar Agora</button></div><button class="md:hidden text-white" data-edit-disabled="true"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-6 h-6"><line x1="4" x2="20" y1="12" y2="12"></line><line x1="4" x2="20" y1="6" y2="6"></line><line x1="4" x2="20" y1="18" y2="18"></line></svg></button></nav></header><section id="home" class="pt-24 pb-16 px-4"><div class="container mx-auto text-center"><div class="max-w-4xl mx-auto" style="opacity: 1; transform: none;"><h1 class="text-5xl md:text-7xl font-black mb-6" data-edit-disabled="true"><span class="text-gradient">SHARK</span><span class="text-white">TV</span></h1><p class="text-xl md:text-2xl text-gray-300 mb-8 leading-relaxed" data-edit-disabled="true">O <span class="text-cyan-400 font-bold">melhor IPTV do Brasil</span> com mais de<span class="text-cyan-400 font-bold"> 15.000 canais</span> em qualidade 4K</p><div class="flex flex-col sm:flex-row gap-4 justify-center items-center mb-12"><button class="inline-flex items-center justify-center font-medium ring-offset-background transition-colors focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:pointer-events-none disabled:opacity-50 bg-primary text-primary-foreground hover:bg-primary/90 h-11 rounded-md bg-gradient-to-r from-cyan-500 to-blue-500 hover:from-cyan-600 hover:to-blue-600 text-lg px-8 py-4 pulse-glow" data-edit-disabled="true"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-5 h-5 mr-2"><polygon points="5 3 19 12 5 21 5 3"></polygon></svg>Começar Agora</button><button class="inline-flex items-center justify-center font-medium ring-offset-background transition-colors focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:pointer-events-none disabled:opacity-50 border bg-background h-11 rounded-md border-cyan-400 text-cyan-400 hover:bg-cyan-400 hover:text-slate-900 text-lg px-8 py-4" data-edit-disabled="true">Ver Canais<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-5 h-5 ml-2"><path d="M5 12h14"></path><path d="m12 5 7 7-7 7"></path></svg></button></div><div class="grid grid-cols-2 md:grid-cols-4 gap-8 max-w-3xl mx-auto"><div class="text-center"><div class="text-3xl font-bold text-cyan-400">15K+</div><div class="text-gray-400">Canais</div></div><div class="text-center"><div class="text-3xl font-bold text-cyan-400">4K</div><div class="text-gray-400">Qualidade</div></div><div class="text-center"><div class="text-3xl font-bold text-cyan-400">24/7</div><div class="text-gray-400">Suporte</div></div><div class="text-center"><div class="text-3xl font-bold text-cyan-400">99%</div><div class="text-gray-400">Uptime</div></div></div></div></div></section><section class="py-16 px-4"><div class="container mx-auto"><div class="text-center mb-16" style="opacity: 1; transform: none;"><h2 class="text-4xl md:text-5xl font-bold text-white mb-4" data-edit-disabled="true">Por que escolher a <span class="text-gradient">SharkTV</span>?</h2><p class="text-xl text-gray-300 max-w-2xl mx-auto" data-edit-id="src/App.jsx:304:13">Tecnologia de ponta e qualidade incomparável para sua diversão</p></div><div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8"><div class="glass-effect rounded-2xl p-6 text-center hover:shark-glow transition-all duration-300" style="opacity: 1; transform: none;"><div class="w-16 h-16 bg-gradient-to-r from-cyan-500 to-blue-500 rounded-full flex items-center justify-center mx-auto mb-4 text-white"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-8 h-8"><polygon points="13 2 3 14 12 14 11 22 21 10 12 10 13 2"></polygon></svg></div><h3 class="text-xl font-bold text-white mb-3" data-edit-disabled="true">Velocidade Extrema</h3><p class="text-gray-300" data-edit-disabled="true">Streaming sem travamentos com nossa infraestrutura de alta performance</p></div><div class="glass-effect rounded-2xl p-6 text-center hover:shark-glow transition-all duration-300" style="opacity: 1; transform: none;"><div class="w-16 h-16 bg-gradient-to-r from-cyan-500 to-blue-500 rounded-full flex items-center justify-center mx-auto mb-4 text-white"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-8 h-8"><path d="M12 22s8-4 8-10V5l-8-3-8 3v7c0 6 8 10 8 10"></path></svg></div><h3 class="text-xl font-bold text-white mb-3" data-edit-disabled="true">100% Seguro</h3><p class="text-gray-300" data-edit-disabled="true">Conexão criptografada e dados protegidos para sua tranquilidade</p></div><div class="glass-effect rounded-2xl p-6 text-center hover:shark-glow transition-all duration-300" style="opacity: 1; transform: none;"><div class="w-16 h-16 bg-gradient-to-r from-cyan-500 to-blue-500 rounded-full flex items-center justify-center mx-auto mb-4 text-white"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-8 h-8"><rect width="20" height="14" x="2" y="3" rx="2"></rect><line x1="8" x2="16" y1="21" y2="21"></line><line x1="12" x2="12" y1="17" y2="21"></line></svg></div><h3 class="text-xl font-bold text-white mb-3" data-edit-disabled="true">Qualidade 4K/8K</h3><p class="text-gray-300" data-edit-disabled="true">Imagem cristalina em ultra alta definição para todos os dispositivos</p></div><div class="glass-effect rounded-2xl p-6 text-center hover:shark-glow transition-all duration-300" style="opacity: 1; transform: none;"><div class="w-16 h-16 bg-gradient-to-r from-cyan-500 to-blue-500 rounded-full flex items-center justify-center mx-auto mb-4 text-white"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-8 h-8"><rect width="14" height="20" x="5" y="2" rx="2" ry="2"></rect><path d="M12 18h.01"></path></svg></div><h3 class="text-xl font-bold text-white mb-3" data-edit-disabled="true">Multi-Dispositivos</h3><p class="text-gray-300" data-edit-disabled="true">Assista em TV, celular, tablet, computador - onde quiser!</p></div><div class="glass-effect rounded-2xl p-6 text-center hover:shark-glow transition-all duration-300" style="opacity: 1; transform: none;"><div class="w-16 h-16 bg-gradient-to-r from-cyan-500 to-blue-500 rounded-full flex items-center justify-center mx-auto mb-4 text-white"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-8 h-8"><circle cx="12" cy="12" r="10"></circle><polyline points="12 6 12 12 16 14"></polyline></svg></div><h3 class="text-xl font-bold text-white mb-3" data-edit-disabled="true">Suporte 24/7</h3><p class="text-gray-300" data-edit-disabled="true">Atendimento especializado disponível todos os dias, a qualquer hora</p></div><div class="glass-effect rounded-2xl p-6 text-center hover:shark-glow transition-all duration-300" style="opacity: 1; transform: none;"><div class="w-16 h-16 bg-gradient-to-r from-cyan-500 to-blue-500 rounded-full flex items-center justify-center mx-auto mb-4 text-white"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-8 h-8"><path d="M5 13a10 10 0 0 1 14 0"></path><path d="M8.5 16.5a5 5 0 0 1 7 0"></path><path d="M2 8.82a15 15 0 0 1 20 0"></path><line x1="12" x2="12.01" y1="20" y2="20"></line></svg></div><h3 class="text-xl font-bold text-white mb-3" data-edit-disabled="true">Fácil Instalação</h3><p class="text-gray-300" data-edit-disabled="true">Configure em minutos com nosso guia passo a passo simplificado</p></div></div></div></section><section id="plans" class="py-16 px-4 bg-slate-900/50"><div class="container mx-auto"><div class="text-center mb-16" style="opacity: 1; transform: none;"><h2 class="text-4xl md:text-5xl font-bold text-white mb-4" data-edit-disabled="true">Escolha seu <span class="text-gradient">Plano</span></h2><p class="text-xl text-gray-300 max-w-2xl mx-auto" data-edit-id="src/App.jsx:374:13">Planos flexíveis para todos os perfis e orçamentos</p></div><div class="grid md:grid-cols-3 gap-8 max-w-6xl mx-auto"><div class="relative glass-effect rounded-3xl p-8 text-center " style="opacity: 1; transform: none;"><div class="w-20 h-20 bg-gradient-to-r from-blue-500 to-cyan-500 rounded-full flex items-center justify-center mx-auto mb-6"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-10 h-10 text-white"><rect width="20" height="15" x="2" y="7" rx="2" ry="2"></rect><polyline points="17 2 12 7 7 2"></polyline></svg></div><h3 class="text-2xl font-bold text-white mb-2" data-edit-disabled="true">Plano Básico</h3><div class="mb-6"><span class="text-4xl font-black text-cyan-400" data-edit-disabled="true">R$ 29,90</span><span class="text-gray-400" data-edit-disabled="true">/mês</span></div><ul class="space-y-3 mb-8"><li class="flex items-center text-gray-300"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-5 h-5 text-green-400 mr-3 flex-shrink-0"><path d="M22 11.08V12a10 10 0 1 1-5.93-9.14"></path><polyline points="22 4 12 14.01 9 11.01"></polyline></svg>5.000+ Canais HD</li><li class="flex items-center text-gray-300"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-5 h-5 text-green-400 mr-3 flex-shrink-0"><path d="M22 11.08V12a10 10 0 1 1-5.93-9.14"></path><polyline points="22 4 12 14.01 9 11.01"></polyline></svg>Filmes e Séries</li><li class="flex items-center text-gray-300"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-5 h-5 text-green-400 mr-3 flex-shrink-0"><path d="M22 11.08V12a10 10 0 1 1-5.93-9.14"></path><polyline points="22 4 12 14.01 9 11.01"></polyline></svg>2 Dispositivos</li><li class="flex items-center text-gray-300"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-5 h-5 text-green-400 mr-3 flex-shrink-0"><path d="M22 11.08V12a10 10 0 1 1-5.93-9.14"></path><polyline points="22 4 12 14.01 9 11.01"></polyline></svg>Suporte 24/7</li><li class="flex items-center text-gray-300"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-5 h-5 text-green-400 mr-3 flex-shrink-0"><path d="M22 11.08V12a10 10 0 1 1-5.93-9.14"></path><polyline points="22 4 12 14.01 9 11.01"></polyline></svg>Qualidade HD</li></ul><button class="inline-flex items-center justify-center rounded-md text-sm ring-offset-background transition-colors focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:pointer-events-none disabled:opacity-50 bg-primary hover:bg-primary/90 h-10 px-4 w-full bg-gradient-to-r from-blue-500 to-cyan-500 hover:opacity-90 text-white font-bold py-3" data-edit-id="src/App.jsx:419:17">Escolher Plano</button></div><div class="relative glass-effect rounded-3xl p-8 text-center ring-2 ring-cyan-400 shark-glow" style="opacity: 1; transform: none;"><div class="absolute -top-4 left-1/2 transform -translate-x-1/2"><span class="bg-gradient-to-r from-cyan-500 to-blue-500 text-white px-6 py-2 rounded-full text-sm font-bold" data-edit-id="src/App.jsx:394:21">MAIS POPULAR</span></div><div class="w-20 h-20 bg-gradient-to-r from-purple-500 to-pink-500 rounded-full flex items-center justify-center mx-auto mb-6"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-10 h-10 text-white"><rect width="20" height="15" x="2" y="7" rx="2" ry="2"></rect><polyline points="17 2 12 7 7 2"></polyline></svg></div><h3 class="text-2xl font-bold text-white mb-2" data-edit-disabled="true">Plano Premium</h3><div class="mb-6"><span class="text-4xl font-black text-cyan-400" data-edit-disabled="true">R$ 49,90</span><span class="text-gray-400" data-edit-disabled="true">/mês</span></div><ul class="space-y-3 mb-8"><li class="flex items-center text-gray-300"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-5 h-5 text-green-400 mr-3 flex-shrink-0"><path d="M22 11.08V12a10 10 0 1 1-5.93-9.14"></path><polyline points="22 4 12 14.01 9 11.01"></polyline></svg>10.000+ Canais 4K</li><li class="flex items-center text-gray-300"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-5 h-5 text-green-400 mr-3 flex-shrink-0"><path d="M22 11.08V12a10 10 0 1 1-5.93-9.14"></path><polyline points="22 4 12 14.01 9 11.01"></polyline></svg>Netflix + Prime Video</li><li class="flex items-center text-gray-300"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-5 h-5 text-green-400 mr-3 flex-shrink-0"><path d="M22 11.08V12a10 10 0 1 1-5.93-9.14"></path><polyline points="22 4 12 14.01 9 11.01"></polyline></svg>4 Dispositivos</li><li class="flex items-center text-gray-300"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-5 h-5 text-green-400 mr-3 flex-shrink-0"><path d="M22 11.08V12a10 10 0 1 1-5.93-9.14"></path><polyline points="22 4 12 14.01 9 11.01"></polyline></svg>Suporte Prioritário</li><li class="flex items-center text-gray-300"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-5 h-5 text-green-400 mr-3 flex-shrink-0"><path d="M22 11.08V12a10 10 0 1 1-5.93-9.14"></path><polyline points="22 4 12 14.01 9 11.01"></polyline></svg>Qualidade 4K Ultra HD</li><li class="flex items-center text-gray-300"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-5 h-5 text-green-400 mr-3 flex-shrink-0"><path d="M22 11.08V12a10 10 0 1 1-5.93-9.14"></path><polyline points="22 4 12 14.01 9 11.01"></polyline></svg>Canais Adultos</li></ul><button class="inline-flex items-center justify-center rounded-md text-sm ring-offset-background transition-colors focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:pointer-events-none disabled:opacity-50 bg-primary hover:bg-primary/90 h-10 px-4 w-full bg-gradient-to-r from-purple-500 to-pink-500 hover:opacity-90 text-white font-bold py-3" data-edit-id="src/App.jsx:419:17">Escolher Plano</button></div><div class="relative glass-effect rounded-3xl p-8 text-center " style="opacity: 0; transform: translateY(50px) translateZ(0px);"><div class="w-20 h-20 bg-gradient-to-r from-orange-500 to-red-500 rounded-full flex items-center justify-center mx-auto mb-6"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-10 h-10 text-white"><rect width="20" height="15" x="2" y="7" rx="2" ry="2"></rect><polyline points="17 2 12 7 7 2"></polyline></svg></div><h3 class="text-2xl font-bold text-white mb-2" data-edit-disabled="true">Plano Família</h3><div class="mb-6"><span class="text-4xl font-black text-cyan-400" data-edit-disabled="true">R$ 79,90</span><span class="text-gray-400" data-edit-disabled="true">/mês</span></div><ul class="space-y-3 mb-8"><li class="flex items-center text-gray-300"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-5 h-5 text-green-400 mr-3 flex-shrink-0"><path d="M22 11.08V12a10 10 0 1 1-5.93-9.14"></path><polyline points="22 4 12 14.01 9 11.01"></polyline></svg>15.000+ Canais 4K</li><li class="flex items-center text-gray-300"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-5 h-5 text-green-400 mr-3 flex-shrink-0"><path d="M22 11.08V12a10 10 0 1 1-5.93-9.14"></path><polyline points="22 4 12 14.01 9 11.01"></polyline></svg>Todas as Plataformas</li><li class="flex items-center text-gray-300"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-5 h-5 text-green-400 mr-3 flex-shrink-0"><path d="M22 11.08V12a10 10 0 1 1-5.93-9.14"></path><polyline points="22 4 12 14.01 9 11.01"></polyline></svg>Dispositivos Ilimitados</li><li class="flex items-center text-gray-300"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-5 h-5 text-green-400 mr-3 flex-shrink-0"><path d="M22 11.08V12a10 10 0 1 1-5.93-9.14"></path><polyline points="22 4 12 14.01 9 11.01"></polyline></svg>Suporte VIP</li><li class="flex items-center text-gray-300"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-5 h-5 text-green-400 mr-3 flex-shrink-0"><path d="M22 11.08V12a10 10 0 1 1-5.93-9.14"></path><polyline points="22 4 12 14.01 9 11.01"></polyline></svg>Qualidade 8K</li><li class="flex items-center text-gray-300"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-5 h-5 text-green-400 mr-3 flex-shrink-0"><path d="M22 11.08V12a10 10 0 1 1-5.93-9.14"></path><polyline points="22 4 12 14.01 9 11.01"></polyline></svg>Canais Internacionais</li><li class="flex items-center text-gray-300"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-5 h-5 text-green-400 mr-3 flex-shrink-0"><path d="M22 11.08V12a10 10 0 1 1-5.93-9.14"></path><polyline points="22 4 12 14.01 9 11.01"></polyline></svg>PPV Incluído</li></ul><button class="inline-flex items-center justify-center rounded-md text-sm ring-offset-background transition-colors focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:pointer-events-none disabled:opacity-50 bg-primary hover:bg-primary/90 h-10 px-4 w-full bg-gradient-to-r from-orange-500 to-red-500 hover:opacity-90 text-white font-bold py-3" data-edit-id="src/App.jsx:419:17">Escolher Plano</button></div></div></div></section><section id="channels" class="py-16 px-4"><div class="container mx-auto"><div class="text-center mb-16" style="opacity: 0; transform: translateY(50px) translateZ(0px);"><h2 class="text-4xl md:text-5xl font-bold text-white mb-4" data-edit-disabled="true"><span class="text-gradient">Canais</span> Disponíveis</h2><p class="text-xl text-gray-300 max-w-2xl mx-auto" data-edit-id="src/App.jsx:443:13">Os melhores canais do Brasil e do mundo na palma da sua mão</p></div><div class="grid grid-cols-2 md:grid-cols-4 lg:grid-cols-6 gap-4 mb-12"><div class="glass-effect rounded-xl p-4 text-center hover:shark-glow transition-all duration-300" style="opacity: 0; transform: scale(0.8) translateZ(0px);"><div class="w-12 h-12 bg-gradient-to-r from-cyan-500 to-blue-500 rounded-lg flex items-center justify-center mx-auto mb-2"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-6 h-6 text-white"><rect width="20" height="15" x="2" y="7" rx="2" ry="2"></rect><polyline points="17 2 12 7 7 2"></polyline></svg></div><span class="text-white font-medium text-sm" data-edit-disabled="true">Globo</span></div><div class="glass-effect rounded-xl p-4 text-center hover:shark-glow transition-all duration-300" style="opacity: 0; transform: scale(0.8) translateZ(0px);"><div class="w-12 h-12 bg-gradient-to-r from-cyan-500 to-blue-500 rounded-lg flex items-center justify-center mx-auto mb-2"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-6 h-6 text-white"><rect width="20" height="15" x="2" y="7" rx="2" ry="2"></rect><polyline points="17 2 12 7 7 2"></polyline></svg></div><span class="text-white font-medium text-sm" data-edit-disabled="true">SBT</span></div><div class="glass-effect rounded-xl p-4 text-center hover:shark-glow transition-all duration-300" style="opacity: 0; transform: scale(0.8) translateZ(0px);"><div class="w-12 h-12 bg-gradient-to-r from-cyan-500 to-blue-500 rounded-lg flex items-center justify-center mx-auto mb-2"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-6 h-6 text-white"><rect width="20" height="15" x="2" y="7" rx="2" ry="2"></rect><polyline points="17 2 12 7 7 2"></polyline></svg></div><span class="text-white font-medium text-sm" data-edit-disabled="true">Record</span></div><div class="glass-effect rounded-xl p-4 text-center hover:shark-glow transition-all duration-300" style="opacity: 0; transform: scale(0.8) translateZ(0px);"><div class="w-12 h-12 bg-gradient-to-r from-cyan-500 to-blue-500 rounded-lg flex items-center justify-center mx-auto mb-2"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-6 h-6 text-white"><rect width="20" height="15" x="2" y="7" rx="2" ry="2"></rect><polyline points="17 2 12 7 7 2"></polyline></svg></div><span class="text-white font-medium text-sm" data-edit-disabled="true">Band</span></div><div class="glass-effect rounded-xl p-4 text-center hover:shark-glow transition-all duration-300" style="opacity: 0; transform: scale(0.8) translateZ(0px);"><div class="w-12 h-12 bg-gradient-to-r from-cyan-500 to-blue-500 rounded-lg flex items-center justify-center mx-auto mb-2"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-6 h-6 text-white"><rect width="20" height="15" x="2" y="7" rx="2" ry="2"></rect><polyline points="17 2 12 7 7 2"></polyline></svg></div><span class="text-white font-medium text-sm" data-edit-disabled="true">RedeTV</span></div><div class="glass-effect rounded-xl p-4 text-center hover:shark-glow transition-all duration-300" style="opacity: 0; transform: scale(0.8) translateZ(0px);"><div class="w-12 h-12 bg-gradient-to-r from-cyan-500 to-blue-500 rounded-lg flex items-center justify-center mx-auto mb-2"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-6 h-6 text-white"><rect width="20" height="15" x="2" y="7" rx="2" ry="2"></rect><polyline points="17 2 12 7 7 2"></polyline></svg></div><span class="text-white font-medium text-sm" data-edit-disabled="true">ESPN</span></div><div class="glass-effect rounded-xl p-4 text-center hover:shark-glow transition-all duration-300" style="opacity: 0; transform: scale(0.8) translateZ(0px);"><div class="w-12 h-12 bg-gradient-to-r from-cyan-500 to-blue-500 rounded-lg flex items-center justify-center mx-auto mb-2"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-6 h-6 text-white"><rect width="20" height="15" x="2" y="7" rx="2" ry="2"></rect><polyline points="17 2 12 7 7 2"></polyline></svg></div><span class="text-white font-medium text-sm" data-edit-disabled="true">Fox Sports</span></div><div class="glass-effect rounded-xl p-4 text-center hover:shark-glow transition-all duration-300" style="opacity: 0; transform: scale(0.8) translateZ(0px);"><div class="w-12 h-12 bg-gradient-to-r from-cyan-500 to-blue-500 rounded-lg flex items-center justify-center mx-auto mb-2"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-6 h-6 text-white"><rect width="20" height="15" x="2" y="7" rx="2" ry="2"></rect><polyline points="17 2 12 7 7 2"></polyline></svg></div><span class="text-white font-medium text-sm" data-edit-disabled="true">Sportv</span></div><div class="glass-effect rounded-xl p-4 text-center hover:shark-glow transition-all duration-300" style="opacity: 0; transform: scale(0.8) translateZ(0px);"><div class="w-12 h-12 bg-gradient-to-r from-cyan-500 to-blue-500 rounded-lg flex items-center justify-center mx-auto mb-2"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-6 h-6 text-white"><rect width="20" height="15" x="2" y="7" rx="2" ry="2"></rect><polyline points="17 2 12 7 7 2"></polyline></svg></div><span class="text-white font-medium text-sm" data-edit-disabled="true">Premiere</span></div><div class="glass-effect rounded-xl p-4 text-center hover:shark-glow transition-all duration-300" style="opacity: 0; transform: scale(0.8) translateZ(0px);"><div class="w-12 h-12 bg-gradient-to-r from-cyan-500 to-blue-500 rounded-lg flex items-center justify-center mx-auto mb-2"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-6 h-6 text-white"><rect width="20" height="15" x="2" y="7" rx="2" ry="2"></rect><polyline points="17 2 12 7 7 2"></polyline></svg></div><span class="text-white font-medium text-sm" data-edit-disabled="true">Multishow</span></div><div class="glass-effect rounded-xl p-4 text-center hover:shark-glow transition-all duration-300" style="opacity: 0; transform: scale(0.8) translateZ(0px);"><div class="w-12 h-12 bg-gradient-to-r from-cyan-500 to-blue-500 rounded-lg flex items-center justify-center mx-auto mb-2"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-6 h-6 text-white"><rect width="20" height="15" x="2" y="7" rx="2" ry="2"></rect><polyline points="17 2 12 7 7 2"></polyline></svg></div><span class="text-white font-medium text-sm" data-edit-disabled="true">GNT</span></div><div class="glass-effect rounded-xl p-4 text-center hover:shark-glow transition-all duration-300" style="opacity: 0; transform: scale(0.8) translateZ(0px);"><div class="w-12 h-12 bg-gradient-to-r from-cyan-500 to-blue-500 rounded-lg flex items-center justify-center mx-auto mb-2"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-6 h-6 text-white"><rect width="20" height="15" x="2" y="7" rx="2" ry="2"></rect><polyline points="17 2 12 7 7 2"></polyline></svg></div><span class="text-white font-medium text-sm" data-edit-disabled="true">Discovery</span></div><div class="glass-effect rounded-xl p-4 text-center hover:shark-glow transition-all duration-300" style="opacity: 0; transform: scale(0.8) translateZ(0px);"><div class="w-12 h-12 bg-gradient-to-r from-cyan-500 to-blue-500 rounded-lg flex items-center justify-center mx-auto mb-2"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-6 h-6 text-white"><rect width="20" height="15" x="2" y="7" rx="2" ry="2"></rect><polyline points="17 2 12 7 7 2"></polyline></svg></div><span class="text-white font-medium text-sm" data-edit-disabled="true">History</span></div><div class="glass-effect rounded-xl p-4 text-center hover:shark-glow transition-all duration-300" style="opacity: 0; transform: scale(0.8) translateZ(0px);"><div class="w-12 h-12 bg-gradient-to-r from-cyan-500 to-blue-500 rounded-lg flex items-center justify-center mx-auto mb-2"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-6 h-6 text-white"><rect width="20" height="15" x="2" y="7" rx="2" ry="2"></rect><polyline points="17 2 12 7 7 2"></polyline></svg></div><span class="text-white font-medium text-sm" data-edit-disabled="true">National Geographic</span></div><div class="glass-effect rounded-xl p-4 text-center hover:shark-glow transition-all duration-300" style="opacity: 0; transform: scale(0.8) translateZ(0px);"><div class="w-12 h-12 bg-gradient-to-r from-cyan-500 to-blue-500 rounded-lg flex items-center justify-center mx-auto mb-2"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-6 h-6 text-white"><rect width="20" height="15" x="2" y="7" rx="2" ry="2"></rect><polyline points="17 2 12 7 7 2"></polyline></svg></div><span class="text-white font-medium text-sm" data-edit-disabled="true">Animal Planet</span></div><div class="glass-effect rounded-xl p-4 text-center hover:shark-glow transition-all duration-300" style="opacity: 0; transform: scale(0.8) translateZ(0px);"><div class="w-12 h-12 bg-gradient-to-r from-cyan-500 to-blue-500 rounded-lg flex items-center justify-center mx-auto mb-2"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-6 h-6 text-white"><rect width="20" height="15" x="2" y="7" rx="2" ry="2"></rect><polyline points="17 2 12 7 7 2"></polyline></svg></div><span class="text-white font-medium text-sm" data-edit-disabled="true">Cartoon Network</span></div><div class="glass-effect rounded-xl p-4 text-center hover:shark-glow transition-all duration-300" style="opacity: 0; transform: scale(0.8) translateZ(0px);"><div class="w-12 h-12 bg-gradient-to-r from-cyan-500 to-blue-500 rounded-lg flex items-center justify-center mx-auto mb-2"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-6 h-6 text-white"><rect width="20" height="15" x="2" y="7" rx="2" ry="2"></rect><polyline points="17 2 12 7 7 2"></polyline></svg></div><span class="text-white font-medium text-sm" data-edit-disabled="true">Disney</span></div></div><div class="text-center"><p class="text-2xl text-cyan-400 font-bold mb-4" data-edit-id="src/App.jsx:468:13">+ Milhares de outros canais!</p><p class="text-gray-300 mb-8" data-edit-id="src/App.jsx:469:13">Esportes, filmes, séries, documentários, infantil, notícias e muito mais</p><button class="inline-flex items-center justify-center text-sm font-medium ring-offset-background transition-colors focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:pointer-events-none disabled:opacity-50 bg-primary text-primary-foreground hover:bg-primary/90 h-11 rounded-md px-8 bg-gradient-to-r from-cyan-500 to-blue-500 hover:from-cyan-600 hover:to-blue-600" data-edit-id="src/App.jsx:472:13">Ver Lista Completa</button></div></div></section><section id="testimonials" class="py-16 px-4 bg-slate-900/50"><div class="container mx-auto"><div class="text-center mb-16" style="opacity: 0; transform: translateY(50px) translateZ(0px);"><h2 class="text-4xl md:text-5xl font-bold text-white mb-4" data-edit-disabled="true">O que nossos <span class="text-gradient">clientes</span> dizem</h2><p class="text-xl text-gray-300 max-w-2xl mx-auto" data-edit-id="src/App.jsx:495:13">Mais de 50.000 clientes satisfeitos em todo o Brasil</p></div><div class="max-w-4xl mx-auto"><div class="glass-effect rounded-3xl p-8 text-center" style="opacity: 1; transform: none;"><div class="flex justify-center mb-4"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-6 h-6 text-yellow-400 fill-current"><polygon points="12 2 15.09 8.26 22 9.27 17 14.14 18.18 21.02 12 17.77 5.82 21.02 7 14.14 2 9.27 8.91 8.26 12 2"></polygon></svg><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-6 h-6 text-yellow-400 fill-current"><polygon points="12 2 15.09 8.26 22 9.27 17 14.14 18.18 21.02 12 17.77 5.82 21.02 7 14.14 2 9.27 8.91 8.26 12 2"></polygon></svg><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-6 h-6 text-yellow-400 fill-current"><polygon points="12 2 15.09 8.26 22 9.27 17 14.14 18.18 21.02 12 17.77 5.82 21.02 7 14.14 2 9.27 8.91 8.26 12 2"></polygon></svg><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-6 h-6 text-yellow-400 fill-current"><polygon points="12 2 15.09 8.26 22 9.27 17 14.14 18.18 21.02 12 17.77 5.82 21.02 7 14.14 2 9.27 8.91 8.26 12 2"></polygon></svg><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-6 h-6 text-yellow-400 fill-current"><polygon points="12 2 15.09 8.26 22 9.27 17 14.14 18.18 21.02 12 17.77 5.82 21.02 7 14.14 2 9.27 8.91 8.26 12 2"></polygon></svg></div><p class="text-xl text-gray-300 mb-6 italic" data-edit-disabled="true">"Canais em 4K são perfeitos! Parece que estou no cinema em casa."</p><div class="flex items-center justify-center space-x-4"><div class="w-12 h-12 bg-gradient-to-r from-cyan-500 to-blue-500 rounded-full flex items-center justify-center"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-6 h-6 text-white"><path d="M16 21v-2a4 4 0 0 0-4-4H6a4 4 0 0 0-4 4v2"></path><circle cx="9" cy="7" r="4"></circle><path d="M22 21v-2a4 4 0 0 0-3-3.87"></path><path d="M16 3.13a4 4 0 0 1 0 7.75"></path></svg></div><div><p class="text-white font-bold" data-edit-disabled="true">João Oliveira</p><p class="text-gray-400" data-edit-disabled="true">Belo Horizonte, MG</p></div></div></div><div class="flex justify-center mt-8 space-x-2"><button class="w-3 h-3 rounded-full transition-colors bg-gray-600" data-edit-id="src/App.jsx:531:17"></button><button class="w-3 h-3 rounded-full transition-colors bg-gray-600" data-edit-id="src/App.jsx:531:17"></button><button class="w-3 h-3 rounded-full transition-colors bg-cyan-400" data-edit-id="src/App.jsx:531:17"></button></div></div></div></section><section id="contact" class="py-16 px-4"><div class="container mx-auto"><div class="text-center mb-16" style="opacity: 0; transform: translateY(50px) translateZ(0px);"><h2 class="text-4xl md:text-5xl font-bold text-white mb-4" data-edit-disabled="true">Entre em <span class="text-gradient">Contato</span></h2><p class="text-xl text-gray-300 max-w-2xl mx-auto" data-edit-id="src/App.jsx:556:13">Nossa equipe está pronta para te ajudar a escolher o melhor plano</p></div><div class="grid md:grid-cols-2 gap-12 max-w-6xl mx-auto"><div class="space-y-8" style="opacity: 0; transform: translateX(-50px) translateZ(0px);"><div class="flex items-center space-x-4"><div class="w-12 h-12 bg-gradient-to-r from-green-500 to-green-600 rounded-full flex items-center justify-center"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-6 h-6 text-white"><path d="m3 21 1.9-5.7a8.5 8.5 0 1 1 3.8 3.8z"></path></svg></div><div><h3 class="text-xl font-bold text-white" data-edit-id="src/App.jsx:573:19">WhatsApp</h3><p class="text-gray-300" data-edit-id="src/App.jsx:574:19">(11) 99999-9999</p></div></div><div class="flex items-center space-x-4"><div class="w-12 h-12 bg-gradient-to-r from-blue-500 to-blue-600 rounded-full flex items-center justify-center"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-6 h-6 text-white"><path d="M22 16.92v3a2 2 0 0 1-2.18 2 19.79 19.79 0 0 1-8.63-3.07 19.5 19.5 0 0 1-6-6 19.79 19.79 0 0 1-3.07-8.67A2 2 0 0 1 4.11 2h3a2 2 0 0 1 2 1.72 12.84 12.84 0 0 0 .7 2.81 2 2 0 0 1-.45 2.11L8.09 9.91a16 16 0 0 0 6 6l1.27-1.27a2 2 0 0 1 2.11-.45 12.84 12.84 0 0 0 2.81.7A2 2 0 0 1 22 16.92z"></path></svg></div><div><h3 class="text-xl font-bold text-white" data-edit-id="src/App.jsx:583:19">Telefone</h3><p class="text-gray-300" data-edit-id="src/App.jsx:584:19">(11) 3333-4444</p></div></div><div class="flex items-center space-x-4"><div class="w-12 h-12 bg-gradient-to-r from-purple-500 to-purple-600 rounded-full flex items-center justify-center"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-6 h-6 text-white"><rect width="20" height="16" x="2" y="4" rx="2"></rect><path d="m22 7-8.97 5.7a1.94 1.94 0 0 1-2.06 0L2 7"></path></svg></div><div><h3 class="text-xl font-bold text-white" data-edit-id="src/App.jsx:593:19">E-mail</h3><p class="text-gray-300" data-edit-id="src/App.jsx:594:19">contato@sharktv.com.br</p></div></div><div class="flex items-center space-x-4"><div class="w-12 h-12 bg-gradient-to-r from-red-500 to-red-600 rounded-full flex items-center justify-center"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-6 h-6 text-white"><path d="M20 10c0 6-8 12-8 12s-8-6-8-12a8 8 0 0 1 16 0Z"></path><circle cx="12" cy="10" r="3"></circle></svg></div><div><h3 class="text-xl font-bold text-white" data-edit-id="src/App.jsx:603:19">Endereço</h3><p class="text-gray-300" data-edit-id="src/App.jsx:604:19">São Paulo, SP - Brasil</p></div></div></div><div class="glass-effect rounded-3xl p-8" style="opacity: 0; transform: translateX(50px) translateZ(0px);"><h3 class="text-2xl font-bold text-white mb-6" data-edit-id="src/App.jsx:615:15">Solicite seu Teste Grátis</h3><div class="space-y-4"><input type="text" placeholder="Seu nome" class="w-full bg-slate-800 border border-slate-700 rounded-lg px-4 py-3 text-white placeholder-gray-400 focus:border-cyan-400 focus:outline-none"><input type="email" placeholder="Seu e-mail" class="w-full bg-slate-800 border border-slate-700 rounded-lg px-4 py-3 text-white placeholder-gray-400 focus:border-cyan-400 focus:outline-none"><input type="tel" placeholder="Seu WhatsApp" class="w-full bg-slate-800 border border-slate-700 rounded-lg px-4 py-3 text-white placeholder-gray-400 focus:border-cyan-400 focus:outline-none"><textarea placeholder="Mensagem (opcional)" rows="4" class="w-full bg-slate-800 border border-slate-700 rounded-lg px-4 py-3 text-white placeholder-gray-400 focus:border-cyan-400 focus:outline-none resize-none"></textarea><button class="inline-flex items-center justify-center rounded-md font-medium ring-offset-background transition-colors focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:pointer-events-none disabled:opacity-50 bg-primary text-primary-foreground hover:bg-primary/90 h-10 px-4 w-full bg-gradient-to-r from-cyan-500 to-blue-500 hover:from-cyan-600 hover:to-blue-600 text-lg py-3" data-edit-id="src/App.jsx:637:17">Enviar Mensagem</button></div></div></div></div></section><footer class="bg-slate-900 py-12 px-4"><div class="container mx-auto"><div class="grid md:grid-cols-4 gap-8 mb-8"><div><div class="flex items-center space-x-2 mb-4"><div class="w-10 h-10 bg-gradient-to-r from-blue-500 to-cyan-500 rounded-lg flex items-center justify-center"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-6 h-6 text-white"><rect width="20" height="15" x="2" y="7" rx="2" ry="2"></rect><polyline points="17 2 12 7 7 2"></polyline></svg></div><span class="text-2xl font-bold text-gradient" data-edit-id="src/App.jsx:661:17">SharkTV</span></div><p class="text-gray-400 mb-4" data-edit-id="src/App.jsx:663:15">O melhor IPTV do Brasil com qualidade incomparável e suporte 24/7.</p><div class="flex space-x-4"><div class="w-10 h-10 bg-blue-600 rounded-full flex items-center justify-center hover:bg-blue-700 transition-colors cursor-pointer"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-5 h-5 text-white"><path d="M18 2h-3a5 5 0 0 0-5 5v3H7v4h3v8h4v-8h3l1-4h-4V7a1 1 0 0 1 1-1h3z"></path></svg></div><div class="w-10 h-10 bg-pink-600 rounded-full flex items-center justify-center hover:bg-pink-700 transition-colors cursor-pointer"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-5 h-5 text-white"><rect width="20" height="20" x="2" y="2" rx="5" ry="5"></rect><path d="M16 11.37A4 4 0 1 1 12.63 8 4 4 0 0 1 16 11.37z"></path><line x1="17.5" x2="17.51" y1="6.5" y2="6.5"></line></svg></div><div class="w-10 h-10 bg-red-600 rounded-full flex items-center justify-center hover:bg-red-700 transition-colors cursor-pointer"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-5 h-5 text-white"><path d="M2.5 17a24.12 24.12 0 0 1 0-10 2 2 0 0 1 1.4-1.4 49.56 49.56 0 0 1 16.2 0A2 2 0 0 1 21.5 7a24.12 24.12 0 0 1 0 10 2 2 0 0 1-1.4 1.4 49.55 49.55 0 0 1-16.2 0A2 2 0 0 1 2.5 17"></path><path d="m10 15 5-3-5-3z"></path></svg></div></div></div><div><h3 class="text-white font-bold mb-4" data-edit-id="src/App.jsx:680:15">Planos</h3><ul class="space-y-2 text-gray-400"><li>Plano Básico</li><li>Plano Premium</li><li>Plano Família</li><li>Teste Grátis</li></ul></div><div><h3 class="text-white font-bold mb-4" data-edit-id="src/App.jsx:690:15">Suporte</h3><ul class="space-y-2 text-gray-400"><li>Central de Ajuda</li><li>Como Instalar</li><li>Configuração</li><li>Contato</li></ul></div><div><h3 class="text-white font-bold mb-4" data-edit-id="src/App.jsx:700:15">Empresa</h3><ul class="space-y-2 text-gray-400"><li>Sobre Nós</li><li>Termos de Uso</li><li>Política de Privacidade</li><li>Trabalhe Conosco</li></ul></div></div><div class="border-t border-slate-800 pt-8 text-center"><p class="text-gray-400" data-edit-id="src/App.jsx:711:13">© 2024 SharkTV. Todos os direitos reservados. O melhor IPTV do Brasil.</p></div></div></footer><div class="fixed bottom-6 right-6 z-50" style="transform: none;"><button class="w-16 h-16 bg-green-500 rounded-full flex items-center justify-center shadow-lg hover:bg-green-600 transition-colors floating" data-edit-disabled="true" tabindex="0"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-8 h-8 text-white"><path d="m3 21 1.9-5.7a8.5 8.5 0 1 1 3.8 3.8z"></path></svg></button></div></div></div>
		<script type="module" src="/src/main.jsx"></script>
		<script type="module">import { POPUP_STYLES, getPopupHTMLTemplate } from './plugins/visual-editor/visual-editor-config.js';

const PLUGIN_APPLY_EDIT_API_URL = '/api/apply-edit';

let popupElement = null;
let popupTextarea = null;
let popupSaveButton = null;
let popupCancelButton = null;
let currentEditingInfo = null;
let disabledTooltipElement = null;

let translations = {
  cancel: 'Cancel',
  save: 'Save',
  addText: 'Add text',
  disabledTooltipText: "This text can be changed only through chat."
};

let areStylesInjected = false;

let globalEventHandlers = null;

function injectPopupStyles() {
  if (areStylesInjected) return;

  const styleElement = document.createElement('style');
  styleElement.id = 'inline-editor-styles';
  styleElement.textContent = POPUP_STYLES;
  document.head.appendChild(styleElement);
  areStylesInjected = true;
}

function createPopup() {
  if (popupElement) return;

  injectPopupStyles();

  popupElement = document.createElement('div');
  popupElement.id = 'inline-editor-popup';
 
  popupElement.innerHTML = getPopupHTMLTemplate(translations.save, translations.cancel);
  document.body.appendChild(popupElement);
 
  popupTextarea = popupElement.querySelector('textarea');
  popupSaveButton = popupElement.querySelector('.save-button');
  popupCancelButton = popupElement.querySelector('.cancel-button');

  popupTextarea.placeholder = `${translations.addText}...`;
 
  popupSaveButton.addEventListener('click', handlePopupSave);
  popupCancelButton.addEventListener('click', handlePopupCancel);
}

function showPopup(targetElement, editId, currentText) {
  if (!popupElement) createPopup();

  currentEditingInfo = { editId, targetElement };

  popupSaveButton.textContent = translations.save;
  popupCancelButton.textContent = translations.cancel;

  popupTextarea.style.display = 'block';
  popupTextarea.value = currentText;
  popupTextarea.disabled = false;
  popupSaveButton.style.display = 'inline-block';

  popupElement.classList.add('is-active');
  popupTextarea.focus();
}

function hidePopup() {
  if (popupElement) {
    popupElement.classList.remove('is-active');
    popupElement.classList.remove('is-disabled-view');
   
    if(popupTextarea) popupTextarea.style.display = 'none';
    if(popupSaveButton) popupSaveButton.style.display = 'none';
  }
  currentEditingInfo = null;
}

function handleGlobalEvent(event) {
  if (!document.getElementById('root')?.getAttribute('data-edit-mode-enabled')) {
    return;
  }

  if (event.target.closest('#inline-editor-popup')) {
    return;
  }

  const editableElement = event.target.closest('[data-edit-id]');

  if (editableElement) {
    event.preventDefault();
    event.stopPropagation();
    event.stopImmediatePropagation();

    if (event.type === 'click') {
      if (currentEditingInfo) {
        hidePopup();
      }

      const editId = editableElement.getAttribute('data-edit-id');
      if (!editId) {
        console.warn('[INLINE EDITOR] Clicked element missing data-edit-id');
        return;
      }

      const currentText = editableElement.textContent || '';
      showPopup(editableElement, editId, currentText);
    }
  } else {
    event.preventDefault();
    event.stopPropagation();
    event.stopImmediatePropagation();
  }
}

function getParentOrigin() {
  if (window.location.ancestorOrigins && window.location.ancestorOrigins.length > 0) {
    return window.location.ancestorOrigins[0];
  }
  
  if (document.referrer) {
    try {
      return new URL(document.referrer).origin;
    } catch (e) {
      console.warn('Invalid referrer URL:', document.referrer);
    }
  }
  
  return null;
}

async function handlePopupSave() {
  if (!currentEditingInfo) return;
  
  const newText = popupTextarea.value;
  const { editId } = currentEditingInfo;

  try {
    const response = await fetch(PLUGIN_APPLY_EDIT_API_URL, {
      method: 'POST',
      headers: {
        'Content-Type': 'application/json',
      },
      body: JSON.stringify({
        editId: editId,
        newFullText: newText
      }),
    });

    const result = await response.json();
    if (result.success) {
      const ALLOWED_PARENT_ORIGINS = [
        'https://horizons.hostinger.com',
        'https://horizons.hostinger.dev',
        'https://horizons-frontend-local.hostinger.dev',
      ];

      const parentOrigin = getParentOrigin();
      if (parentOrigin && ALLOWED_PARENT_ORIGINS.includes(parentOrigin)) {
        window.parent.postMessage({
          type: 'editApplied',
          payload: {
            editId: editId,
            fileContent: result.newFileContent,
          }
        }, parentOrigin);
      } else {
        console.error('Unauthorized parent origin:', parentOrigin);
      }
    } else {
      console.error(`[vite][visual-editor] Error saving changes: ${result.error}`);
    }
  } catch (error) {
    console.error(`[vite][visual-editor] Error during fetch for ${editId}:`, error);
  }

  hidePopup();
}

function handlePopupCancel() {
  hidePopup();
}

function createDisabledTooltip() {
  if (disabledTooltipElement) return;

  disabledTooltipElement = document.createElement('div');
  disabledTooltipElement.id = 'inline-editor-disabled-tooltip';
  document.body.appendChild(disabledTooltipElement);
}

function showDisabledTooltip(targetElement) {
  if (!disabledTooltipElement) createDisabledTooltip();

  disabledTooltipElement.textContent = translations.disabledTooltipText;
  
  if (!disabledTooltipElement.isConnected) {
    document.body.appendChild(disabledTooltipElement);
  }
  disabledTooltipElement.classList.add('tooltip-active');

  const tooltipWidth = disabledTooltipElement.offsetWidth;
  const tooltipHeight = disabledTooltipElement.offsetHeight;
  const rect = targetElement.getBoundingClientRect();

  // Ensures that tooltip is not off the screen with 5px margin
  let newLeft = rect.left + window.scrollX + (rect.width / 2) - (tooltipWidth / 2);
  let newTop = rect.bottom + window.scrollY + 5;

  if (newLeft < window.scrollX) {
    newLeft = window.scrollX + 5; 
  }
  if (newLeft + tooltipWidth > window.innerWidth + window.scrollX) {
    newLeft = window.innerWidth + window.scrollX - tooltipWidth - 5; 
  }
  if (newTop + tooltipHeight > window.innerHeight + window.scrollY) {
    newTop = rect.top + window.scrollY - tooltipHeight - 5; 
  }
  if (newTop < window.scrollY) {
    newTop = window.scrollY + 5; 
  }

  disabledTooltipElement.style.left = `${newLeft}px`;
  disabledTooltipElement.style.top = `${newTop}px`;
}

function hideDisabledTooltip() {
  if (disabledTooltipElement) {
    disabledTooltipElement.classList.remove('tooltip-active');
  }
}

function handleDisabledElementHover(event) {
  showDisabledTooltip(event.currentTarget);
}

function handleDisabledElementLeave() {
  hideDisabledTooltip();
}

function enableEditMode() {
  document.getElementById('root')?.setAttribute('data-edit-mode-enabled', 'true');
  
  injectPopupStyles(); 
  
  if (!globalEventHandlers) {
    globalEventHandlers = {
      mousedown: handleGlobalEvent,
      pointerdown: handleGlobalEvent,
      click: handleGlobalEvent
    };
    
    Object.entries(globalEventHandlers).forEach(([eventType, handler]) => {
      document.addEventListener(eventType, handler, true);
    });
  }
  
  document.querySelectorAll('[data-edit-disabled]').forEach(el => {
    el.removeEventListener('mouseenter', handleDisabledElementHover);
    el.addEventListener('mouseenter', handleDisabledElementHover);
    el.removeEventListener('mouseleave', handleDisabledElementLeave);
    el.addEventListener('mouseleave', handleDisabledElementLeave);
  });
}

function disableEditMode() {
  document.getElementById('root')?.removeAttribute('data-edit-mode-enabled');

  hidePopup();
  hideDisabledTooltip();

  if (globalEventHandlers) {
    Object.entries(globalEventHandlers).forEach(([eventType, handler]) => {
      document.removeEventListener(eventType, handler, true);
    });
    globalEventHandlers = null;
  }
  
  document.querySelectorAll('[data-edit-disabled]').forEach(el => {
    el.removeEventListener('mouseenter', handleDisabledElementHover);
    el.removeEventListener('mouseleave', handleDisabledElementLeave);
  });
}

window.addEventListener("message", function(event) {
  if (event.data?.type === "enable-edit-mode") {
    if (event.data?.translations) {
        translations = { ...translations, ...event.data.translations };
    }
    enableEditMode();
  }
  if (event.data?.type === "disable-edit-mode") {
    disableEditMode();
  }
}); </script>
	

</body></html>
