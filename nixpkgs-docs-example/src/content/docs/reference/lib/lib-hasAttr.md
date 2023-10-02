---
title: lib.hasAttr
editUrl: https://www.github.com/nixos/nix/blob/master/src/libexpr/primops.cc
description: lib.hasAttr
sidebar:

    badge:
        text: Builtin
        variant: note

    order: 8
---

`hasAttr` returns `true` if *set* has an attribute named *s*, and
`false` otherwise. This is a dynamic version of the `?` operator,
since *s* is an expression rather than an identifier.


# Aliases

- [builtins.hasAttr](/reference/builtinshasAttr)
- [lib.attrsets.hasAttr](/reference/libattrsets.hasAttr)

