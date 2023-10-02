---
title: lib.recurseIntoAttrs
editUrl: https://www.github.com/nixos/nixpkgs/blob/master/lib/attrsets.nix#L1302C5
description: lib.recurseIntoAttrs
sidebar:

    order: 8
---

Make various Nix tools consider the contents of the resulting
attribute set when looking for what to build, find, etc.

This function only affects a single attribute set; it does not
apply itself recursively for nested attribute sets.

# Example

```nix
{ pkgs ? import <nixpkgs> {} }:
{
myTools = pkgs.lib.recurseIntoAttrs {
inherit (pkgs) hello figlet;
};
}
```

# Type

```haskell
recurseIntoAttrs :: AttrSet -> AttrSet
```


# Aliases

- [lib.attrsets.recurseIntoAttrs](/reference/libattrsets.recurseIntoAttrs)
- [pkgs.recurseIntoAttrs](/reference/pkgsrecurseIntoAttrs)

