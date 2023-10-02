---
title: builtins.unsafeGetAttrDoc
editUrl: https://www.github.com/nixos/nix/blob/master/src/libexpr/primops.cc
description: builtins.unsafeGetAttrDoc
sidebar:

    badge:
        text: Builtin
        variant: note

    order: 0
---

For attribute `path` in `set` returns the doc-comment.

Return value: AttributeSet containing the `content` of a multiline doc-comment (format: `    */`)

The doc-comment must be placed before the attribute path or name.


