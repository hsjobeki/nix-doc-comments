---
title: lib.getFiles
editUrl: https://www.github.com/nixos/nix/blob/master/src/libexpr/primops.cc
description: lib.getFiles
sidebar:

    badge:
        text: Builtin
        variant: note

    order: 8
---

Apply the function *f* to each element in the list *list*. For
example,

```nix
map (x: "foo" + x) [ "bar" "bla" "abc" ]
```

evaluates to `[ "foobar" "foobla" "fooabc" ]`.


# Aliases

- [lib.getValues](/reference/libgetValues)
- [lib.options.getFiles](/reference/liboptions.getFiles)
- [lib.options.getValues](/reference/liboptions.getValues)
- [pkgs.copyPathsToStore](/reference/pkgscopyPathsToStore)

