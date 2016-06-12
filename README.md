# Sass Units Translate

Easily convert units with Sass.

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
  $font-size: em(32px, 2em); // 16px
  $font-size: rem(32px, 2rem); // 16px
  $font-size: percent(32px, 200%); // 16px
  $font-size: rel(32px, 2); // 16px
  $font-size: px(2em, 32px); // 16px
}
```

---

[View generated documentation](https://github.com/ellioseven/sass-units-transform/tree/unit-map/doc)