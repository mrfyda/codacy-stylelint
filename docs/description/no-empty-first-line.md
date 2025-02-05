# no-empty-first-line

> **Warning** This rule is deprecated and will be removed in the future. See [the migration guide](https://github.com/stylelint/stylelint/tree/15.10.2/docs/migration-guide/to-15.md).

Disallow empty first lines.

<!-- prettier-ignore -->
```css
    \n
    /** ↑
     * This newline */
    a { color: pink; }
```

This rule ignores empty sources. Use the [`no-empty-source`](https://github.com/stylelint/stylelint/tree/15.10.2/lib/rules/no-empty-source/README.md) rule to disallow these.

The [`fix` option](https://github.com/stylelint/stylelint/tree/15.10.2/docs/user-guide/options.md#fix) can automatically fix all of the problems reported by this rule.

## Options

### `true`

The following patterns are considered problems:

<!-- prettier-ignore -->
```css
\n
a { color: pink; }
```

The following patterns are _not_ considered problems:

<!-- prettier-ignore -->
```css
a { color: pink; }
```
