# SCSS Mixins Cheat Sheet

> SCSS Custom Mixins

* Flexbox
* Position
* Grid

---

### Flexbox

```scss
@mixin flex($direction, $wrap, $justify, $align) {
  display: flex;
  flex-direction: $direction;
  flex-wrap: $wrap;
  justify-content: $justify;
  align-items: $align;
}

// @include flex(row, wrap, flex-start, center);
```
---

### Position

```scss
@mixin position($pos, $top, $right, $bottom, $left) {
  display: $pos;
  top: $top;
  right: $right;
  bottom: $bottom;
  left: $left;
}

// @include position(absolute, 0, null, 0, 0);
```

---

### Grid

```scss
@mixin grid($col, $colgap, $rowgap) {
  display: grid;
  grid-template-columns: $col;
  grid-template-rows: auto;
  grid-column-gap: $colgap;
  grid-row-gap: $rowgap;
}

// @include grid(1fr 1fr 1fr, 20px, 20px);
```
