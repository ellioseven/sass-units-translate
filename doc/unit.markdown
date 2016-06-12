# Unit

## sut-unit-em

### Since

1.0.0

### Source

```scss
@function sut-unit-em($input, $base) { 
  $_return: $input;
  $_return: _sut-unit-calc-value(em, $_return, $base);
  @return $_return;
}
```

### Description

Calculate and convert a single or list of numbers to ems.

### Parameters

| Name  | Description                  | Type   | Default Value |
| ----- | ---------------------------- | ------ | ------------- |
| input | Number/s to convert from.    | Number |               |
| base  | Base number to convert from. | Number |               |

### Returns

`Number | List` — Calculated and converted number/s.

### Example

Calculate and convert 32px into em.

```scss
sut-unit-em(32px)
// 2em
```

Calculate and convert (32px 2em 2rem 200% 2) into ems.

```scss
sut-unit-em(32px 2em 2rem 200% 2);
// 2em 2em 2em 2em 2em
```

Calculate and convert 32px with a base of 8px into em.

```scss
sut-unit-em(32px, 8px)
// 4em
```

### Used By

* [function] `em`

### Since

1.0.0

---

## sut-unit-rem

### Since

1.0.0

### Source

```scss
@function sut-unit-rem($input, $base) { 
  $_return: $input;
  $_return: _sut-unit-calc-value(rem, $_return, $base);
  @return $_return;
}
```

### Description

Calculate and convert a single or list of numbers to rems.

### Parameters

| Name  | Description                  | Type   | Default Value |
| ----- | ---------------------------- | ------ | ------------- |
| input | Number/s to convert from.    | Number |               |
| base  | Base number to convert from. | Number |               |

### Returns

`Number | List` — Calculated and converted number/s.

### Example

Calculate and convert 32px into rem.

```scss
sut-unit-rem(32px)
// 2rem
```

Calculate and convert (32px 2em 2rem 200% 2) into rems.

```scss
sut-unit-rem(32px 2em 2rem 200% 2);
// 2rem 2rem 2rem 2rem 2rem
```

Calculate and convert 32px with a base of 8px into em.

```scss
sut-unit-rem(32px, 8px)
// 4rem
```

### Used By

* [function] `rem`

### Since

1.0.0

---

## sut-unit-rel

### Since

1.0.0

### Source

```scss
@function sut-unit-rel($input, $base) { 
  $_return: $input;
  $_return: _sut-unit-calc-value(relative, $_return, $base);
  @return $_return;
}
```

### Description

Calculate and convert a single or list of numbers to relative numbers.

### Parameters

| Name  | Description                  | Type   | Default Value |
| ----- | ---------------------------- | ------ | ------------- |
| input | Number/s to convert from.    | Number |               |
| base  | Base number to convert from. | Number |               |

### Returns

`Number | List` — Calculated and converted number/s.

### Example

Calculate and convert 32px into a relative number.

```scss
sut-unit-rel(32px)
// 2
```

Calculate and convert (32px 2em 2rem 200% 2) into relative numbers.

```scss
sut-unit-rel(32px 2em 2rem 200% 2);
// 2 2 2 2 2
```

Calculate and convert 32px with a base of 8px into a relative number.

```scss
sut-unit-rel(32px, 8px)
// 4
```

### Used By

* [function] `rel`

### Since

1.0.0

---

## sut-unit-px

### Since

1.0.0

### Source

```scss
@function sut-unit-px($input, $base) { 
  $_return: $input;
  $_return: _sut-unit-calc-value(px, $_return, $base);
  @return $_return;
}
```

### Description

Calculate and convert a single or list of numbers to px.

### Parameters

| Name  | Description                  | Type   | Default Value |
| ----- | ---------------------------- | ------ | ------------- |
| input | Number/s to convert from.    | Number |               |
| base  | Base number to convert from. | Number |               |

### Returns

`Number | List` — Calculated and converted number/s.

### Example

Calculate and convert 2em into to px.

```scss
sut-unit-px(2em)
// 32px
```

Calculate and convert (32px 2em 2rem 200% 2) into px.

```scss
sut-unit-px(32px 2em 2rem 200% 2);
// 32px 32px 32px 32px 32px
```

Calculate and convert 2em with a base of 8px into a relative number.

```scss
sut-unit-px(2em, 8px)
// 16px
```

### Used By

* [function] `px`

### Since

1.0.0

---

## sut-unit-percent

### Since

1.0.0

### Source

```scss
@function sut-unit-percent($input, $base) { 
  $_return: $input;
  $_return: _sut-unit-calc-value(percent, $_return, $base);
  @return $_return;
}
```

### Description

Calculate and convert a single or list of numbers to percentages.

### Parameters

| Name  | Description                  | Type   | Default Value |
| ----- | ---------------------------- | ------ | ------------- |
| input | Number/s to convert from.    | Number |               |
| base  | Base number to convert from. | Number |               |

### Returns

`Number | List` — Calculated and converted number/s.

### Example

Calculate and convert 32px into a percentage.

```scss
sut-unit-percent(32px)
// 200%
```

Calculate and convert (32px 2em 2rem 200% 2) into percentages.

```scss
sut-unit-percent(32px 2em 2rem 200% 2);
// 200% 200% 200% 200% 200%
```

Calculate and convert 32px with a base of 8px into a percentage.

```scss
sut-unit-percent(32px, 8px)
// 400%
```

### Used By

* [function] `percent`

### Since

1.0.0

---