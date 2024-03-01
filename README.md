This fork of [ABC](https://github.com/berkeley-abc/abc) is used to track changes needed to compile ABC as a static library and interface with [mockturtle](https://github.com/lsils/mockturtle) (and to easily pull the latest changes in ABC).

## Usage
Compile with command `make ABC_USE_NAMESPACE=abc ABC_USE_NO_READLINE=1 ABC_USE_NO_CUDD=1 libabc.a`, then move the obtained `libabc.a` file to `mockturtle/lib/abc_static/`.
