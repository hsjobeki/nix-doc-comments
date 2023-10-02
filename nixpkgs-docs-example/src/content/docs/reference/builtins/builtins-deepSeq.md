---
title: builtins.deepSeq
editUrl: https://www.github.com/nixos/nix/blob/master/src/libexpr/primops.cc
description: builtins.deepSeq
sidebar:

    badge:
        text: Builtin
        variant: note

    order: 0
---

This is like `seq e1 e2`, except that *e1* is evaluated *deeply*:
if it’s a list or set, its elements or attributes are also
evaluated recursively.


# Aliases

- [lib.deepseq](/nix-doc-comments/reference/lib/lib-deepseq)
- [lib.trivial.deepseq](/nix-doc-comments/reference/lib/trivial/lib-trivial-deepseq)


