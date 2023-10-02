---
title: lib.strings.toJSON
editUrl: https://www.github.com/nixos/nix/blob/master/src/libexpr/primops.cc
description: lib.strings.toJSON
sidebar:

    badge:
        text: Builtin
        variant: note

    order: 7
---

Return a string containing a JSON representation of *e*. Strings,
integers, floats, booleans, nulls and lists are mapped to their JSON
equivalents. Sets (except derivations) are represented as objects.
Derivations are translated to a JSON string containing the
derivation’s output path. Paths are copied to the store and
represented as a JSON string of the resulting store path.


# Aliases

- [builtins.toJSON](/reference/builtinstoJSON)


