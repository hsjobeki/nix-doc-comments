---
title: builtins.fetchTarball
editUrl: https://www.github.com/nixos/nix/blob/master/src/libexpr/primops.cc
description: builtins.fetchTarball
sidebar:

    badge:
        text: Builtin
        variant: note

    order: 0
---

Download the specified URL, unpack it and return the path of the
unpacked tree. The file must be a tape archive (`.tar`) compressed
with `gzip`, `bzip2` or `xz`. The top-level path component of the
files in the tarball is removed, so it is best if the tarball
contains a single directory at top level. The typical use of the
function is to obtain external Nix expression dependencies, such as
a particular version of Nixpkgs, e.g.

```nix
with import (fetchTarball https://github.com/NixOS/nixpkgs/archive/nixos-14.12.tar.gz) {};

stdenv.mkDerivation { … }
```

The fetched tarball is cached for a certain amount of time (1
hour by default) in `~/.cache/nix/tarballs/`. You can change the
cache timeout either on the command line with `--tarball-ttl`
*number-of-seconds* or in the Nix configuration file by adding
the line `tarball-ttl = ` *number-of-seconds*.

Note that when obtaining the hash with `nix-prefetch-url` the
option `--unpack` is required.

This function can also verify the contents against a hash. In that
case, the function takes a set instead of a URL. The set requires
the attribute `url` and the attribute `sha256`, e.g.

```nix
with import (fetchTarball {
  url = "https://github.com/NixOS/nixpkgs/archive/nixos-14.12.tar.gz";
  sha256 = "1jppksrfvbk5ypiqdz4cddxdl8z6zyzdb2srq8fcffr327ld5jj2";
}) {};

stdenv.mkDerivation { … }
```

Not available in [restricted evaluation mode](@docroot@/command-ref/conf-file.md#conf-restrict-eval).


