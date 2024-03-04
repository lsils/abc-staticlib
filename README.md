This fork of [ABC](https://github.com/berkeley-abc/abc) is used to track changes needed to compile ABC as a static library and interface with [mockturtle](https://github.com/lsils/mockturtle) (and to easily pull the latest changes in ABC).

Compilation with ABC as a static library is added to mockturtle in [PR #634](https://github.com/lsils/mockturtle/pull/634).

## Usage
Some code in mockturtle is only available when configured and compiled with the CMake option `ENABLE_ABC=1`, which will only work with a `libabc.a` file in `mockturtle/lib/abc_static/`. This repository serves to generate such file.

### Compile by yourself
Compile with command `make ABC_USE_NAMESPACE=abc ABC_USE_NO_READLINE=1 ABC_USE_NO_CUDD=1 libabc.a`, then move the obtained `libabc.a` file to `mockturtle/lib/abc_static/`.

### Download a precompiled library file
Download a precompiled library (.a) file according to your OS in [release](https://github.com/lsils/abc-staticlib/releases), then place it in `mockturtle/lib/abc_static/`.
