---
title: lib.mapNullable
editUrl: https://www.github.com/nixos/nixpkgs/blob/master/lib/trivial.nix#L214C5
description: lib.mapNullable
sidebar:

    order: 8
---

Apply function if the supplied argument is non-null.

# Example

```nix
mapNullable (x: x+1) null
=> null
mapNullable (x: x+1) 22
=> 23
```


# Aliases

- [lib.trivial.mapNullable](/reference/libtrivial.mapNullable)

