# SCSS Columns

> SCSS Column Layout Classes

* Global `col-`
* XL `xl-`
* LG `lg-`
* MD `md-`
* SM `sm-`
* XS `xs-`

* Hide At
* Show At

* Hide On
* Show On

---

```scss
// Screens
$xs: 560px;
$sm: 768px;
$md: 1024px;
$lg: 1280px;
$xl: 1400px;

// Global
.col-1-1, .col-12-12 { width: 100%; }
.col-1-2, .col-6-12 { width: 50%; }
.col-1-3, .col-4-12 { width: 33.3333%; }
.col-1-4, .col-3-12 { width: 25%; }
.col-1-5 { width: 20%; }
.col-1-6, .col-2-12 { width: 16.667%; }
.col-1-7 { width: 14.28%; }
.col-1-8 { width: 12.5%; }
.col-1-9 { width: 11.1%; }
.col-1-10 { width: 10%; }
.col-1-11 { width: 9.09%; }
.col-1-12 { width: 8.33%; }
.col-2-3, .col-8-12 { width: 66.66%; }
.col-5-12 { width: 41.66%; }
.col-7-12 { width: 58.33%; }
.col-9-12, .col-3-4 { width: 75%; }
.col-4-5 { width: 80%; }
.col-10-12 { width: 83.333%; }
.col-11-12 { width: 91.66%; }

// hide-at-X
@media screen and (max-width: $xl) {
  .hide-at-xl { display: none !important; }
}
@media screen and (max-width: $lg) {
  .hide-at-lg { display: none !important; }
}
@media screen and (max-width: $md) {
  .hide-at-md { display: none !important; }
}
@media screen and (max-width: $sm) {
  .hide-at-sm { display: none !important; }
}
@media screen and (max-width: $xs) {
  .hide-at-xs { display: none !important; }
}

// show-at-X
@media screen and (min-width: $xl + 1) {
  .show-at-xl { display: none !important; }
}
@media screen and (min-width: $lg + 1) {
  .show-at-lg { display: none !important; }
}
@media screen and (min-width: $md + 1) {
  .show-at-md { display: none !important; }
}
@media screen and (min-width: $sm + 1) {
  .show-at-sm { display: none !important; }
}
@media screen and (min-width: $xs + 1) {
  .show-at-xs { display: none !important; }
}

// $xl +
// hide-on-X
// show-on-X
@media screen and (min-width: $xl + 1) {
  .max-1-1, .max-12-12 { width: 100%; }
  .max-1-2, .max-6-12 { width: 50%; }
  .max-1-3, .max-4-12 { width: 33.3333%; }
  .max-1-4, .max-3-12 { width: 25%; }
  .max-1-5 { width: 20%; }
  .max-1-6, .max-2-12 { width: 16.667%; }
  .max-1-7 { width: 14.28%; }
  .max-1-8 { width: 12.5%; }
  .max-1-9 { width: 11.1%; }
  .max-1-10 { width: 10%; }
  .max-1-11 { width: 9.09%; }
  .max-1-12 { width: 8.33%; }
  .max-2-3, .max-8-12 { width: 66.66%; }
  .max-5-12 { width: 41.66%; }
  .max-7-12 { width: 58.33%; }
  .max-9-12, .max-3-4 { width: 75%; }
  .max-4-5 { width: 80%; }
  .max-10-12 { width: 83.333%; }
  .max-11-12 { width: 91.66%; }

  .hide-on-max { display: none !important; }
  .show-on-xl { display: none !important; }
  .show-on-lg { display: none !important; }
  .show-on-md { display: none !important; }
  .show-on-sm { display: none !important; }
  .show-on-xs { display: none !important; }
}

// $lg -> $xl
// hide-on-X
// show-on-X
@media screen and (min-width: $lg + 1) and (max-width: $xl) {
  .xl-1-1, .xl-12-12 { width: 100%; }
  .xl-1-2, .xl-6-12 { width: 50%; }
  .xl-1-3, .xl-4-12 { width: 33.3333%; }
  .xl-1-4, .xl-3-12 { width: 25%; }
  .xl-1-5 { width: 20%; }
  .xl-1-6, .xl-2-12 { width: 16.667%; }
  .xl-1-7 { width: 14.28%; }
  .xl-1-8 { width: 12.5%; }
  .xl-1-9 { width: 11.1%; }
  .xl-1-10 { width: 10%; }
  .xl-1-11 { width: 9.09%; }
  .xl-1-12 { width: 8.33%; }
  .xl-2-3, .xl-8-12 { width: 66.66%; }
  .xl-5-12 { width: 41.66%; }
  .xl-7-12 { width: 58.33%; }
  .xl-9-12, .xl-3-4 { width: 75%; }
  .xl-4-5 { width: 80%; }
  .xl-10-12 { width: 83.333%; }
  .xl-11-12 { width: 91.66%; }

  .show-on-max { display: none !important; }
  .hide-on-xl { display: none !important; }
  .show-on-lg { display: none !important; }
  .show-on-md { display: none !important; }
  .show-on-sm { display: none !important; }
  .show-on-xs { display: none !important; }
}

// $md -> $lg
// hide-on-X
// show-on-X
@media screen and (min-width: $md + 1) and (max-width: $lg) {
  .lg-1-1, .lg-12-12 { width: 100%; }
  .lg-1-2, .lg-6-12 { width: 50%; }
  .lg-1-3, .lg-4-12 { width: 33.3333%; }
  .lg-1-4, .lg-3-12 { width: 25%; }
  .lg-1-5 { width: 20%; }
  .lg-1-6, .lg-2-12 { width: 16.667%; }
  .lg-1-7 { width: 14.28%; }
  .lg-1-8 { width: 12.5%; }
  .lg-1-9 { width: 11.1%; }
  .lg-1-10 { width: 10%; }
  .lg-1-11 { width: 9.09%; }
  .lg-1-12 { width: 8.33%; }
  .lg-2-3, .lg-8-12 { width: 66.66%; }
  .lg-5-12 { width: 41.66%; }
  .lg-7-12 { width: 58.33%; }
  .lg-9-12, .lg-3-4 { width: 75%; }
  .lg-4-5 { width: 80%; }
  .lg-10-12 { width: 83.333%; }
  .lg-11-12 { width: 91.66%; }

  .show-on-max { display: none !important; }
  .show-on-xl { display: none !important; }
  .hide-on-lg { display: none !important; }
  .show-on-md { display: none !important; }
  .show-on-sm { display: none !important; }
  .show-on-xs { display: none !important; }
}

// $sm -> $md
// hide-on-X
// show-on-X
@media screen and (min-width: $sm + 1) and (max-width: $md) {
  .md-1-1, .md-12-12 { width: 100%; }
  .md-1-2, .md-6-12 { width: 50%; }
  .md-1-3, .md-4-12 { width: 33.3333%; }
  .md-1-4, .md-3-12 { width: 25%; }
  .md-1-5 { width: 20%; }
  .md-1-6, .md-2-12 { width: 16.667%; }
  .md-1-7 { width: 14.28%; }
  .md-1-8 { width: 12.5%; }
  .md-1-9 { width: 11.1%; }
  .md-1-10 { width: 10%; }
  .md-1-11 { width: 9.09%; }
  .md-1-12 { width: 8.33%; }
  .md-2-3, .md-8-12 { width: 66.66%; }
  .md-5-12 { width: 41.66%; }
  .md-7-12 { width: 58.33%; }
  .md-9-12, .md-3-4 { width: 75%; }
  .md-4-5 { width: 80%; }
  .md-10-12 { width: 83.333%; }
  .md-11-12 { width: 91.66%; }

  .show-on-max { display: none !important; }
  .show-on-xl { display: none !important; }
  .show-on-lg { display: none !important; }
  .hide-on-md { display: none !important; }
  .show-on-sm { display: none !important; }
  .show-on-xs { display: none !important; }
}

// $xs -> $sm
// hide-on-X
// show-on-X
@media screen and (min-width: $xs + 1) and (max-width: $sm) {
  .sm-1-1, .sm-12-12 { width: 100%; }
  .sm-1-2, .sm-6-12 { width: 50%; }
  .sm-1-3, .sm-4-12 { width: 33.3333%; }
  .sm-1-4, .sm-3-12 { width: 25%; }
  .sm-1-5 { width: 20%; }
  .sm-1-6, .sm-2-12 { width: 16.667%; }
  .sm-1-7 { width: 14.28%; }
  .sm-1-8 { width: 12.5%; }
  .sm-1-9 { width: 11.1%; }
  .sm-1-10 { width: 10%; }
  .sm-1-11 { width: 9.09%; }
  .sm-1-12 { width: 8.33%; }
  .sm-2-3, .sm-8-12 { width: 66.66%; }
  .sm-5-12 { width: 41.66%; }
  .sm-7-12 { width: 58.33%; }
  .sm-9-12, .sm-3-4 { width: 75%; }
  .sm-4-5 { width: 80%; }
  .sm-10-12 { width: 83.333%; }
  .sm-11-12 { width: 91.66%; }

  .show-on-max { display: none !important; }
  .show-on-xl { display: none !important; }
  .show-on-lg { display: none !important; }
  .show-on-md { display: none !important; }
  .hide-on-sm { display: none !important; }
  .show-on-xs { display: none !important; }
}

// - $xs
// hide-on-X
// show-on-X
@media screen and (max-width: $xs) {
  .xs-1-1, .xs-12-12 { width: 100%; }
  .xs-1-2, .xs-6-12 { width: 50%; }
  .xs-1-3, .xs-4-12 { width: 33.3333%; }
  .xs-1-4, .xs-3-12 { width: 25%; }
  .xs-1-5 { width: 20%; }
  .xs-1-6, .xs-2-12 { width: 16.667%; }
  .xs-1-7 { width: 14.28%; }
  .xs-1-8 { width: 12.5%; }
  .xs-1-9 { width: 11.1%; }
  .xs-1-10 { width: 10%; }
  .xs-1-11 { width: 9.09%; }
  .xs-1-12 { width: 8.33%; }
  .xs-2-3, .xs-8-12 { width: 66.66%; }
  .xs-5-12 { width: 41.66%; }
  .xs-7-12 { width: 58.33%; }
  .xs-9-12, .xs-3-4 { width: 75%; }
  .xs-4-5 { width: 80%; }
  .xs-10-12 { width: 83.333%; }
  .xs-11-12 { width: 91.66%; }

  .show-on-max { display: none !important; }
  .show-on-xl { display: none !important; }
  .show-on-lg { display: none !important; }
  .show-on-md { display: none !important; }
  .show-on-sm { display: none !important; }
  .hide-on-xs { display: none !important; }
}
```
