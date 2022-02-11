# Boost

> https://www.boost.org/ 
> 
> [Boost releases download link](https://www.boost.org/users/news/boost_has_moved_downloads_to_jfr.html)
## Installation

With Command Prompt:

```shell
install.bat
```


In the `install.bat`, refer to the link to install. 
- [installation](https://www.boost.org/doc/libs/1_78_0/tools/build/doc/html/index.html#bbv2.installation)
- [build-binaries-from-source](https://www.boost.org/doc/libs/1_78_0/more/getting_started/windows.html#or-build-binaries-from-source)
- [guide-on-compiling-and-linking-boost-c-libraries-for-visual-studio-projects](https://levelup.gitconnected.com/the-definite-guide-on-compiling-and-linking-boost-c-libraries-for-visual-studio-projects-c79464d7282d)

where invoke b2 option
> b2 --help

```
B2 4.7-git

Project-specific help:

  Project has jamfile at Jamroot

Usage:

  b2 [options] [properties] [install|stage]

  Builds and installs Boost.

Targets and Related Options:

  install                 Install headers and compiled library files to the
  =======                 configured locations (below).

  --prefix=<PREFIX>       Install architecture independent files here.
                          Default: C:\Boost on Windows
                          Default: /usr/local on Unix, Linux, etc.

  --exec-prefix=<EPREFIX> Install architecture dependent files here.
                          Default: <PREFIX>

  --libdir=<LIBDIR>       Install library files here.
                          Default: <EPREFIX>/lib

  --includedir=<HDRDIR>   Install header files here.
                          Default: <PREFIX>/include

  --cmakedir=<CMAKEDIR>   Install CMake configuration files here.
                          Default: <LIBDIR>/cmake

  --no-cmake-config       Do not install CMake configuration files.

  stage                   Build and install only compiled library files to the
  =====                   stage directory.

  --stagedir=<STAGEDIR>   Install library files here
                          Default: ./stage

Other Options:

  --build-type=<type>     Build the specified pre-defined set of variations of
                          the libraries. Note, that which variants get built
                          depends on what each library supports.

                              -- minimal -- (default) Builds a minimal set of
                              variants. On Windows, these are static
                              multithreaded libraries in debug and release
                              modes, using shared runtime. On Linux, these are
                              static and shared multithreaded libraries in
                              release mode.

                              -- complete -- Build all possible variations.

  --build-dir=DIR         Build in this location instead of building within
                          the distribution tree. Recommended!

  --show-libraries        Display the list of Boost libraries that require
                          build and installation steps, and then exit.

  --layout=<layout>       Determine whether to choose library names and header
                          locations such that multiple versions of Boost or
                          multiple compilers can be used on the same system.

                              -- versioned -- Names of boost binaries include
                              the Boost version number, name and version of
                              the compiler and encoded build properties. Boost
                              headers are installed in a subdirectory of
                              <HDRDIR> whose name contains the Boost version
                              number.

                              -- tagged -- Names of boost binaries include the
                              encoded build properties such as variant and
                              threading, but do not including compiler name
                              and version, or Boost version. This option is
                              useful if you build several variants of Boost,
                              using the same compiler.

                              -- system -- Binaries names do not include the
                              Boost version number or the name and version
                              number of the compiler. Boost headers are
                              installed directly into <HDRDIR>. This option is
                              intended for system integrators building
                              distribution packages.

                          The default value is 'versioned' on Windows, and
                          'system' on Unix.

  --buildid=ID            Add the specified ID to the name of built libraries.
                          The default is to not add anything.

  --python-buildid=ID     Add the specified ID to the name of built libraries
                          that depend on Python. The default is to not add
                          anything. This ID is added in addition to --buildid.

  --help                  This message.

  --with-<library>        Build and install the specified <library>. If this
                          option is used, only libraries specified using this
                          option will be built.

  --without-<library>     Do not build, stage, or install the specified
                          <library>. By default, all libraries are built.

Properties:

  toolset=toolset         Indicate the toolset to build with.

  variant=debug|release   Select the build variant

  link=static|shared      Whether to build static or shared libraries

  threading=single|multi  Whether to build single or multithreaded binaries

  runtime-link=static|shared
                          Whether to link to static or shared C and C++
                          runtime.


General command line usage:

    b2 [options] [properties] [targets]

  Options, properties and targets can be specified in any order.

Important Options:

  * --clean Remove targets instead of building
  * -a Rebuild everything
  * -n Don't execute the commands, only print them
  * -d+2 Show commands as they are executed
  * -d0 Suppress all informational messages
  * -q Stop at first error
  * --reconfigure Rerun all configuration checks
  * --debug-configuration Diagnose configuration
  * --debug-building Report which targets are built with what properties
  * --debug-generator Diagnose generator search/execution

Further Help:

  The following options can be used to obtain additional documentation.

  * --help-options Print more obscure command line options.
  * --help-internal B2 implementation details.
  * --help-doc-options Implementation details doc formatting.
```

### Additional information
- limiting which libraries get built with the --with-library-name:  List of all libs [here](https://www.boost.org/doc/libs/). Non header-only [libraries](https://www.boost.org/doc/libs/1_78_0/more/getting_started/unix-variants.html#header-only-libraries) (via b2 --show-libraries)






---------------------------------------------
### Boost parameter
#### [Invocation](https://www.boost.org/doc/libs/1_78_0/tools/build/doc/html/index.html#bbv2.overview.invocation)
To invoke B2, type b2 on the command line. Three kinds of command-line tokens are accepted, in any order:

`options`

Options start with either one or two dashes. The standard options are listed below, and each project may add additional options

`properties`

Properties specify details of what you want to build (e.g. debug or release variant). Syntactically, all command line tokens with an equal sign in them are considered to specify properties. In the simplest form, a property looks like feature=value

`target`

All tokens that are neither options nor properties specify what targets to build. The available targets entirely depend on the project you are building.

[Properties](https://www.boost.org/doc/libs/1_78_0/tools/build/doc/html/index.html#bbv2.overview.invocation.properties)
[toolset](https://www.boost.org/doc/libs/1_78_0/tools/build/doc/html/index.html#bbv2.reference.tools.compiler.msvc)







* The option “--build-type=complete” causes Boost.Build to build all supported variants of the libraries. For instructions on how to build only specific variants, please ask on the [Boost Users' mailing list](https://www.boost.org/community/groups.html#users)







# $$REPO

> $$1LINER

background details relevant to understanding what this module does

## Usage

```javascript
$$EXAMPLE
```

## API

```js
const $$rePo = require('$$REPO')
```

See [api_formatting.md](api_formatting.md) for tips.

## Installation

With [npm](https://npmjs.org/):

```shell
npm install $$REPO
```

With [yarn](https://yarnpkg.com/en/):

```shell
yarn add $$REPO
```

## Acknowledgments

$$REPO was inspired by...

## See Also

- [`noffle/common-readme`](https://github.com/noffle/common-readme)
- ...

## License

$$ZEE_LICENSE
