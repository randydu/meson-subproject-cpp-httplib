# Meson build for CPP-HTTPLIB

URL: 

- [github repo](https://github.com/yhirose/cpp-httplib);

The subfolder "src" is a clone of git repository of a specified release version. 
unit-tests are not built as part of the meson-build.

## Versions

The "revision" of gsl.wrap and the version of this meson-build project matches the embedded submodule GSL version as following:

Meson-Build |  CPP-HTTPLIB 
------------|-----------
v1.0         | v0.10.7


## Usage

copy cpp_httplib.wrap to "subprojects" sub-folder of your main project directory.


in meson.build:

```
# import

cpp_httplib_dep = dependency('cpp_httplib')

# use
srcs = ['main.c', ...]

executable('test', srcs, dependencies: [cpp_httplib_dep, ...])

```

in main.c:

```c
#include <httplib.h>

void foo(){
}
```



