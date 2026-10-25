# CHASE third party

This repository contains the third party libraries required to compile CHASE.
Currently, it provides the C++ runtime of [ANTLR4][ANTLR], version 4.5.4, used
by the [DSL_tool][DSL_TOOL] and the [logics_tool][LOGICS_TOOL]. Due to
possible incompatibilities of CHASE with other releases of ANTLR4, we suggest
to use this version.

To compile and install the library in the `CHASE_INSTALL_DIR` directory:

`$> cmake -S third_party -B third_party/build`

`$> cmake --build third_party/build`

`$> cmake --install third_party/build`

The library will be installed in the `CHASE_INSTALL_DIR/third_party/antlr4`
directory. On Linux, the library requires `libuuid` (e.g., the `uuid-dev`
package on Ubuntu).

For the installation of the other CHASE modules, please refer to the
[CHASE website][WEB]. ANTLR4 is released under its own license, available in
`antlr4/License.txt`.

[ANTLR]: https://www.antlr.org/
[DSL_TOOL]: https://github.com/chase-cps/DSL_tool
[LOGICS_TOOL]: https://github.com/chase-cps/logics_tool
[WEB]: https://chase-cps.github.io/doc/md/install.html
