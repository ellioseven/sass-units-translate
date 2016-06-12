# Core

## sut-core-set-base

### Since

1.0.0

### Source

```scss
@mixin sut-core-set-base($input) { 
  $_sut-base: _memo('sut', 'base', $input);
}
```

### Description

Set global base font size.

### Parameters

| Name  | Description                              | Type   | Default Value |
| ----- | ---------------------------------------- | ------ | ------------- |
| input | Number to set for global base font size. | Number |               |

### Example

Set global base font size to 16px.

```scss
@include sut-core-set-base(16px)
```

Set global base font size to 150%.

```scss
@include sut-core-set-base(150%)
```

Set global base font size to 1.5em.

```scss
@include sut-core-set-base(1.5em)
```

Set global base font size to 2.

```scss
@include sut-core-set-base(2)
```

### Since

1.0.0

---