[![SFML logo](https://www.sfml-dev.org/images/logo.png)](https://www.sfml-dev.org)

# sfml-graphics build2 package

[SFML](https://www.sfml-dev.org) is a simple, fast, cross-platform and object-oriented multimedia API. It provides access to windowing, graphics, audio and network. It is written in C++, and has bindings for various languages such as C, .Net, Ruby, Python.

This project builds and defines the build2 package for the `Graphics` module of SFML.

## Usage

Add `sfml-graphics` to your build2 `manifest` file.

```
depends: sfml-graphics ^2.5.1
```

You can specify your target platform directly or let build2 try to auto-detect your system:

```
config.sfml_graphics.platform = # SFML platform identifier
```

Supported platform identifiers are:

```
linux
macosx
windows
freebsd
openbsd
netbsd
android
ios
```

You can determine if you want to use OpenGLES (default is `false`).

```
config.sfml_graphics.use_opengles = # true or false
```

## Dependencies

This module requires certain

On Unix based system these are:

* `libx11-dev`
* `libxrandr-dev`
* `libudev-dev`
* `libegl-dev` and `libgles-dev` if OpenGLES is activates