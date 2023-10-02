---
title: lib.strings.escapeNixString
editUrl: https://www.github.com/nixos/nixpkgs/blob/master/lib/strings.nix#L733C21
description: lib.strings.escapeNixString
sidebar:

    order: 7
---

Turn a string into a Nix expression representing that string

# Example

```nix
escapeNixString "hello\${}\n"
=> "\"hello\\\${}\\n\""
```

# Type

```haskell
string -> string
```


