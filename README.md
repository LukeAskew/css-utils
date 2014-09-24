# CSS Utility Classes
---

> A library of stylesheet utility classes, based on Emmet short-hand

## Overview

OOCSSS. Faster.
Single responsiblity princple

## The Classes

### Display

Selector | Responsibility
--- | ---
`.d` `.d-b`|display block
`.d-i`|display inline
`.d-ib`|display inline-block
`.d-tb`|display table
`.d-tbc`|display table-cell
`.d-tbr`|display table-row
`.vh`| visually hidden, but available for screen readers

### Floats

Selector | Responsibility
--- | ---
`.fl` `.fl-l`|float left
`.fl-r`|float right
`.fl-n`|float none
`.cl` `.cl-b`|clear both
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
`.pos` `.pos-r`|position relative
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
`.ta` `.ta-l`|text align left
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
`.va` `.va-t`|align to top
`.va-m`|align to middle
`.va-b`|align to bottom

## License
