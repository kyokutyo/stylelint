---
layout: page
title: # block-opening-brace-newline-after
permalink: docs/src/rules/block-opening-brace-newline-after/README/
---

# block-opening-brace-newline-after

Require a newline after the opening brace of blocks.

```css
    a {
      ↑ color: pink; }
/**   ↑
 * The newline after this brace */
```

## Options

`string`: `"always"|"always-multi-line"|"never-multi-line`

### `"always"`

There *must always* be a newline after the opening brace.

The following patterns are considered warnings:

```css
a{ color: pink; }
```

```css
a{ color: pink;
}
```

The following patterns are *not* considered warnings:

```css
a {
color: pink; }
```

```css
a
{
color: pink; }
```

### `"always-multi-line"`

There *must always* be a newline after the opening brace in multi-line blocks.

The following patterns are considered warnings:

```css
a{color: pink;
}
```

The following patterns are *not* considered warnings:

```css
a { color: pink; }
```

```css
a {
color: pink; }
```

### `"never-multi-line"`

There *must never* be whitespace after the opening brace in multi-line blocks.

The following patterns are considered warnings:

```css
a { color: pink;
}
```

The following patterns are *not* considered warnings:

```css
a { color: pink; }
```

```css
a {color: pink;
}
```
