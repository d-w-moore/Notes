# Python 3 on PREP

Python3 compatibility PREP (python rule engine plugin)

Progress - https://github.com/d-w-moore/irods_rule_engine_plugin_python/tree/python_3


## Notes so far
  - CMakefile can specify "2" for system Python but Python3.x will be used if 2.x is not available
  
---  
TODO

build alternative boost_python using Boost Jam / B2

master builds of externals:
```
  git clone / checkout tag : 1.67.0-0
  git submodules update --init
  set path to clang (for b2)
  for each system python to be supported (3.4 - 3.9):
    cp user-config.jam to $HOME dir ; use sed to set 2nd python config field path (pkg-config can provide this)
```
GIST

https://gist.github.com/d-w-moore/0d98dae0bc5452deddb1719a99072f16
