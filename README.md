# Native LazyLoad with Fade in
 Uses javascript to implement a CSS animated fade-in effect for native lazy-loaded images.

# Usage
 - make sure all your image tags have `loading="lazy"`
		<img src="./picture/of/wood.jpg" loading="lazy" alt="This is a picture of some wood">
 - add this to your html header:
		<script src="lazy-load.js" charset="utf-8" async></script>`
 - add the css below
		.no-js img[loading='lazy'] {
			opacity: 1;
		}
		img[loading='lazy'] {
			opacity: 0;
			transition: 400ms ease-out;
		}
		img[loading='lazy'].loaded {
			opacity: 1;
			transition: 400ms ease-out;
		}

 - and you're done!
