# CSS Utility Classes [![Build Status](https://travis-ci.org/LukeAskew/css-utils.svg?branch=master)](https://travis-ci.org/LukeAskew/css-utils)

A collection of CSS [utility classes](http://davidtheclark.com/on-utility-classes/) - based on [Emmet](http://emmet.io) shorthand conventions - to aid in [object-oriented](http://appendto.com/2014/04/oocss/) CSS development.


## The Classes

### Display

Selector | Responsibility
--- | ---
`.d-b`|display block
`.d-i`|display inline
`.d-ib`|display inline-block
`.d-tb`|display table
`.d-tbc`|display table-cell
`.d-tbr`|display table-row
`.vh`| visually hidden, but available for screen readers

### Floats

Selector | Responsibility
--- | ---
`.fl-l`|float left
`.fl-r`|float right
`.fl-n`|float none
`.cl-b`|clear both
`.cl-l`|clear left
`.cl-r`|clear right
`.cf`|clear fix (contain floats)

### Media

Selector | Responsibility
--- | ---
`.rwd-img`|responsive image (max-width: 100%)
`.rwd-img-st`|stretched responsive image (width: 100%)
`.intrinsic`|intrinsic ration wrapper; deafult 16:9 ratio

### Position

Selector | Responsibility
--- | ---
`.pos-r`|position relative
`.pos-s`|position static
`.pos-a`|position absolute
`.pos-f`|position fixed

### Spacing

Selector | Responsibility
--- | ---
`.{p/m}-0`|remove all padding/margin
`.{p/m}{t/r/b/l}-{xxs/xs/s/l/xl/xxl}`|apply padding/margin in a given direction (top/right/bottom/l) in a given increment.

Increment | Value
--- | ---
`xxs`|0.146em
`xs`|0.236em
`s`|0.618em
(none)|1em
`l`|1.618em
`xl`|4.236em
`xxl`|6.854em

Examples:

```markup
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



### Text

Selector | Responsibility
--- | ---
`.ta-l`|text align left
`.ta-c`|text align center
`.ta-r`|text align right
`.ta-j`|text align justify
`.c-i`|inherit ancestor text color
`.kern`|enable font kerning
`.whs-nw`|prevent wrapping on whitespace
`.truncate`|limit text to a single line, truncating with an ellipsis
`.fw-200`|font weight 200 (light)
`.fw-400`|font weight 400 (normal)
`.fw-700`|font weight 700 (bold)
`.fs-i`|italic
`.tt-u`|uppercase
`.wfsm`|font anti-aliasing

### Vertical Alignment

Selector | Responsibility
--- | ---
`.va-t`|align to top
`.va-m`|align to middle
`.va-b`|align to bottom

## License

The MIT License (MIT)

Copyright (c) 2014 Luke Askew

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
