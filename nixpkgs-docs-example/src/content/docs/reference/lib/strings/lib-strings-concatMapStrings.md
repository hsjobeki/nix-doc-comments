---
title: lib.strings.concatMapStrings
editUrl: https://www.github.com/nixos/nixpkgs/blob/master/lib/strings.nix#L78C22
description: lib.strings.concatMapStrings
sidebar:

    order: 7
---

Map a function over a list and concatenate the resulting strings.

# Example

```nix
concatMapStrings (x: "a" + x) ["foo" "bar"]
=> "afooabar"
```

# Type

```haskell
concatMapStrings :: (a -> string) -> [a] -> string
```


# Aliases

- [lib.concatMapStrings](/reference/libconcatMapStrings)

