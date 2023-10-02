---
title: builtins.match
editUrl: https://www.github.com/nixos/nix/blob/master/src/libexpr/primops.cc
description: builtins.match
sidebar:

    badge:
        text: Builtin
        variant: note

    order: 0
---

Returns a list if the [extended POSIX regular
expression](http://pubs.opengroup.org/onlinepubs/9699919799/basedefs/V1_chap09.html#tag_09_04)
*regex* matches *str* precisely, otherwise returns `null`. Each item
in the list is a regex group.

```nix
builtins.match "ab" "abc"
```

Evaluates to `null`.

```nix
builtins.match "abc" "abc"
```

Evaluates to `[ ]`.

```nix
builtins.match "a(b)(c)" "abc"
```

Evaluates to `[ "b" "c" ]`.

```nix
builtins.match "[[:space:]]+([[:upper:]]+)[[:space:]]+" "  FOO   "
```

Evaluates to `[ "FOO" ]`.


# Aliases

- [lib.strings.match](/reference/libstrings.match)

