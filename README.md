# [autoprefixer](https://github.com/postcss/autoprefixer)_transformer 

> [pub](https://pub.dartlang.org/) transformer that parses css and
> adds vendor prefixes to css rules.

## Prerequisites

This transformer depends on
[autoprefixer](https://github.com/postcss/autoprefixer) CLI tool
that performs transformations.

## Usage example

### `pubspec.yaml`

```yaml
name: autoprefixer_example
dependencies:
  autoprefixer_transformer: any
transformers:
- autoprefixer_transformer:
    browsers:
    - "last 2 versions"
```

### `web/example.css`

```css
.noselect {
  user-select: none;
}
```

## Options

### `browsers`

Browsers you want to target.

TYPE: `List<String>`  
DEFAULT: `[> 1%]`
