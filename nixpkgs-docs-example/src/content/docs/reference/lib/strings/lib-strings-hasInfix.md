---
title: lib.strings.hasInfix
editUrl: https://www.github.com/nixos/nixpkgs/blob/master/lib/strings.nix#L449C14
description: lib.strings.hasInfix
sidebar:

    order: 7
---

Determine whether a string contains the given infix

# Example

```nix
hasInfix "bc" "abcd"
=> true
hasInfix "ab" "abcd"
=> true
hasInfix "cd" "abcd"
=> true
hasInfix "foo" "abcd"
=> false
```

# Type

```haskell
hasInfix :: string -> string -> bool
```


# Aliases

- [lib.hasInfix](/reference/libhasInfix)

