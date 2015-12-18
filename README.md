# SVGS

Collection of reusable SVGs with easy integration with CSS.

## Getting Started

The easiest way to use the SVG images is to download the `.svg` files from within the `/svgs` directory. 

### Integrating with Sass

The recommended approach is to use the Sass partial in this project. The Sass partial contains a collection of Sass mixins that define an optimised inline SVG as a `background-image`. To install this project, run the command below.

	npm install moov2-svgs --save-dev --save-exact

The next step is to import the mixin partial from within the `node_modules/moov2-svgs/sass` directory as shown below. The example below assume `node_modules` is within a root directory that contains a directory that contains the Sass files.

	@import "../node_modules/moov2-svgs/sass/svg";
	
Importing this partial will make all the SVGs available to the Sass stylesheet. Below is an example of a selector that will display a black Twitter logo.

	.logo-twitter {
		@include svg-twitter-logo(#000);
		
		height: 32px;
		width: 32px;
	}
	
*Dimensions are never defined in the mixin and should be handled by you.*.
	
## Available SVGs

### Eventbrite

Logo for [Evenbrite](https://www.eventbrite.co.uk/).

#### Mixin

	@include svg-eventbrite-logo($fillColor);
	
#### Parameters

`$fillColor`: Colour of the logo.

### Facebook

Logo for [Facebook](https://facebook.com).

#### Mixin

	@include svg-facebook-logo($fillColor);
	
#### Parameters

`$fillColor`: Colour of the logo.

### Github

Logo for [Github](https://github.com/).

	@include svg-github-logo($fillColor);
	
#### Parameters

`$fillColor`: Colour of the logo.

### Twitter

Logo for [Twitter](https://twitter.com/).

	@include svg-twitter-logo($fillColor);
	
#### Parameters

`$fillColor`: Colour of the logo.
