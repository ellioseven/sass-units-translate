# alias

## em

### Since

1.0.0

### Source

```scss
@function em($input, $base) { 
  @return sut-unit-em($input, $base);
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
em(32px)
// 2em
```

Calculate and convert (32px 2em 2rem 200% 2) into ems.

```scss
em(32px 2em 2rem 200% 2);
// 2em 2em 2em 2em 2em
```

Calculate and convert 32px with a base of 8px into em.

```scss
em(32px, 8px)
// 4em
```

### Requires

* [function] `sut-unit-em` 

### Since

1.0.0

---

## rem

### Since

1.0.0

### Source

```scss
@function rem($input, $base) { 
  @return sut-unit-rem($input, $base);
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
rem(32px)
// 2rem
```

Calculate and convert (32px 2em 2rem 200% 2) into rems.

```scss
rem(32px 2em 2rem 200% 2);
// 2rem 2rem 2rem 2rem 2rem
```

Calculate and convert 32px with a base of 8px into em.

```scss
rem(32px, 8px)
// 4rem
```

### Requires

* [function] `sut-unit-rem` 

### Since

1.0.0

---

## rel

### Since

1.0.0

### Source

```scss
@function rel($input, $base) { 
  @return sut-unit-rel($input, $base);
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
rel(32px)
// 2
```

Calculate and convert (32px 2em 2rem 200% 2) into relative numbers.

```scss
rel(32px 2em 2rem 200% 2);
// 2 2 2 2 2
```

Calculate and convert 32px with a base of 8px into a relative number.

```scss
rel(32px, 8px)
// 4
```

### Requires

* [function] `sut-unit-rel` 

### Since

1.0.0

---

## px

### Since

1.0.0

### Source

```scss
@function px($input, $base) { 
  @return sut-unit-px($input, $base);
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
px(2em)
// 32px
```

Calculate and convert (32px 2em 2rem 200% 2) into px.

```scss
px(32px 2em 2rem 200% 2);
// 32px 32px 32px 32px 32px
```

Calculate and convert 2em with a base of 8px into a relative number.

```scss
px(2em, 8px)
// 16px
```

### Requires

* [function] `sut-unit-px` 

### Since

1.0.0

---

## percent

### Since

1.0.0

### Source

```scss
@function percent($input, $base) { 
  @return sut-unit-percent($input, $base);
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
percent(32px)
// 200%
```

Calculate and convert (32px 2em 2rem 200% 2) into percentages.

```scss
percent(32px 2em 2rem 200% 2);
// 200% 200% 200% 200% 200%
```

Calculate and convert 32px with a base of 8px into a percentage.

```scss
percent(32px, 8px)
// 400%
```

### Requires

* [function] `sut-unit-percent` 

### Since

1.0.0

---