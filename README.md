# CSS Utility Classes [![Build Status](https://travis-ci.org/LukeAskew/css-utils.svg?branch=master)](https://travis-ci.org/LukeAskew/css-utils)

A collection of CSS [utility classes](http://davidtheclark.com/on-utility-classes/) - based on [Emmet](http://docs.emmet.io/cheat-sheet/) shorthand conventions - to aid in [object-oriented](http://appendto.com/2014/04/oocss/) CSS development.

## Usage

Terse OOCSS classes can be a powerful tool for rapid and scalable development. They can be used independently, or to augment existing objects.

```html
<div class="card">
	<div class="card__photo ta-c">
		<h3>Business Name</h3>
		<div class="fz-s">Some City, America</div>
	</div>
	<div class="card__cell">
		<h3 class="mt-xs mb-xxs">John Doe</h3>
		<div class="fz-s"><span class="fw-b">Member number:</span> 081425</div>
		<div class="mt mb-l">
			123 Main St.<br />
			Columbus, OH 43215
		</div>
		<a href="#" class="button">Select Account</a>
	</div>
</div>
```

## Install

You can [download the repo](https://github.com/LukeAskew/css-utils/archive/master.zip), or install via [Bower](http://bower.io/):

```bash
$ bower install css-utils --save-dev
```

## The Classes

### Display

Selector | Responsibility
--- | ---
`.d-b` | display block
`.d-i` | display inline
`.d-ib` | display inline-block
`.d-tb` | display table
`.d-tbc` | display table-cell
`.d-tbr` | display table-row
`.vh` | visually hidden, but available for screen readers

### Floats

Selector | Responsibility
--- | ---
`.fl-l` | float left
`.fl-r` | float right
`.fl-n` | float none
`.cl-b` | clear both
`.cl-l` | clear left
`.cl-r` | clear right
`.cf` | clear fix (contain floats)

### Media

Selector | Responsibility
--- | ---
`.rwd-img` | responsive image (max-width: 100%)
`.rwd-img-st` | stretched responsive image (width: 100%)
`.intrinsic` | intrinsic ratio wrapper; default 16:9 ratio
`.ir` | image replacement (@mixin included)

### Position

Selector | Responsibility
--- | ---
`.pos-r` | position relative
`.pos-s` | position static
`.pos-a` | position absolute
`.pos-f` | position fixed

### Spacing

Selector | Responsibility
--- | ---
`.{p/m}{t/r/b/l}-{xxs/xs/s/l/xl/xxl}` | apply padding/margin in a given direction (top/right/bottom/left) in a given increment.
`.{p/m}-0` | remove all padding/margin
`.m{r/l}-a` | margin left/right auto (centering)

Increment | Value*
--- | ---
`xxs` | 0.146em
`xs` | 0.236em
`s` | 0.618em
(none) | 1em
`l` | 1.618em
`xl`| 4.236em
`xxl` | 6.854em

*values derived from [golden ratio](http://modularscale.com/scale/?px1=16&px2=&ra1=1.618&ra2=0)

Examples:

```html
<div class="mt-xl">
	<!-- 4.236em top margin -->
</div>

<div class="pl-s">
	<!-- 0.618em left padding -->
</div>

<div class="mb">
	<!-- 1em bottom margin -->
</div>
```

The spacing scale and step progression are configurable. Set these values in your own Sass, before including the css-utils lib:

```sass
// default values
$util-ratio: 1.618;
$util-base: 1em;
$util-spacing: (
	xxs: -4,
	xs: -3,
	s: -1,
	base: 0,
	l: 1,
	xl: 3,
	xxl: 4
);
```

### Text

Selector | Responsibility
--- | ---
`.ta-l` | text align left
`.ta-c` | text align center
`.ta-r` | text align right
`.ta-j` | text align justify
`.c-i` | inherit ancestor text color
`.kern` | enable font kerning
`.whs-nw` | prevent wrapping on whitespace
`.truncate` | limit text to a single line, truncating with an ellipsis
`.fw-l` | font weight light (200)
`.fw-n` | font weight normal (400)
`.fw-b` | font weight bold (700)
`.fs-i` | italic
`.tt-u` | uppercase
`.wfsm` | font anti-aliasing

### Vertical Alignment

Selector | Responsibility
--- | ---
`.va-t`|align to top
`.va-m`|align to middle
`.va-b`|align to bottom

## License

[The MIT License (MIT)](http://opensource.org/licenses/mit-license.php)
