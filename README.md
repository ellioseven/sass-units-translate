# Sass Units Translate

Easily convert units with Sass.

## 0. Install

```
npm install sass-units-translate --save-dev
```

Import into your stylesheet.

```sass
@import "sass-units-translate"
```

## 1. Set global base font size.

```scss
// Setup base font size
@include sut-core-set-base(16px);
// @include sut-core-set-base(100%);
// @include sut-core-set-base(1em);
// @include sut-core-set-base(1);
```

**Note:** This is only setting a global variable and will not output any CSS.

## 2. Translate

### Simple

Convert to em, rem, percent, relative and px.

```scss
h1 {
  $font-size: em(32px); // 2em
  $font-size: rem(2em); // 2rem
  $font-size: percent(2rem); // 200%
  $font-size: rel(200%); // 2
  $font-size: px(2); // 32px
}
```

### Simple Multiple

```scss
h1 {
  $font-size: em(2em 2rem 200% 2 32px); // 32px 32px 32px 32px 32px
}
```

### With Base Sizes

Convert from em, rem, percent, relative and px.

```scss
h1 {
  $font-size: em(32px, 2em); // 1em
  $font-size: rem(32px, 2rem); // 1rem
  $font-size: percent(32px, 200%); // 100%
  $font-size: rel(32px, 2); // 1
  $font-size: px(2em, 32px); // 64px
}
```

---

[View generated documentation](https://github.com/ellioseven/sass-units-translate/tree/master/doc)
