# Utilities

## sut-clear-unit

### Since

1.0.0

### Source

```scss
@function sut-clear-unit($value) { 
  $_return: $value;
  $_return: $_return / ($_return * 0 + 1);
  @return $_return;
}
```

### Description

Strip unit from a number.

### Parameters

| Name  | Description                   | Type   | Default Value |
| ----- | ----------------------------- | ------ | ------------- |
| value | Number to have unit stripped. | Number |               |

### Returns

`Number` — The stripped number.

### Example

Strip px from 24px.

```scss
sut-clear-unit(24px)
// 24
```

### Throws

* $value is not a number.

### Used By

* [function] `sut-make-unit`

### Since

1.0.0

---

## sut-make-unit

### Since

1.0.0

### Source

```scss
@function sut-make-unit($value) { 
  $_return: $value;
  @if _has($_sut-units, $unit) {
    $_return: sut-clear-unit($_return) * _get($_sut-units, $unit value);
  } @else {
    $warn: _sut-warn(sut-make-unit, '#{$value} is not a supported unit.');
  }
  @return $_return;
}
```

### Description

Creates a number with a unit.

### Parameters

| Name  | Description                      | Type   | Default Value |
| ----- | -------------------------------- | ------ | ------------- |
| value | Number to have unit appended to. | Number |               |

### Returns

`Number` — The number with unit appended.

### Example

Convert number 24px to em.

```scss
th-unit-convert-number(24px, em)
// 24em
```

Convert number 24 to em.

```scss
th-unit-convert-number(24, em)
// 24em
```

### Throws

* $value is not a number.

* $value is not a supported unit.

### Requires

* [function] `sut-clear-unit` 

### Since

1.0.0

---