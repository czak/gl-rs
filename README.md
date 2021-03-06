# gl-rs

[![Build Status](https://travis-ci.org/brendanzab/gl-rs.svg?branch=master)](https://travis-ci.org/brendanzab/gl-rs)

## Overview

This repository contains the necessary building blocks for OpenGL wrapper
libraries. For more information on each crate, see their respective READMEs
listed below.

The following crates are contained in this repository:

### gl

[![Version](https://img.shields.io/crates/v/gl.svg)](https://crates.io/crates/gl) [![License](https://img.shields.io/crates/l/gl.svg)](https://github.com/brendanzab/gl-rs/blob/master/LICENSE) [![Downloads](https://img.shields.io/crates/d/gl.svg)](https://crates.io/crates/gl)

[README](https://github.com/brendanzab/gl-rs/tree/master/gl)

An OpenGL function pointer loader for the Rust Programming Language.

```toml
[dependencies]
gl = "0.6.0"
```

### gl_generator

[![Version](https://img.shields.io/crates/v/gl_generator.svg)](https://crates.io/crates/gl_generator) [![License](https://img.shields.io/crates/l/gl_generator.svg)](https://github.com/brendanzab/gl-rs/blob/master/LICENSE) [![Downloads](https://img.shields.io/crates/d/gl_generator.svg)](https://crates.io/crates/gl_generator)

[README](https://github.com/brendanzab/gl-rs/tree/master/gl_generator)

Code generators for creating bindings to the Khronos OpenGL APIs.

```toml
[build-dependencies]
gl_generator = "0.5.0"
```

### khronos_api

[![Version](https://img.shields.io/crates/v/khronos_api.svg)](https://crates.io/crates/khronos_api) [![License](https://img.shields.io/crates/l/khronos_api.svg)](https://github.com/brendanzab/gl-rs/blob/master/LICENSE) [![Downloads](https://img.shields.io/crates/d/khronos_api.svg)](https://crates.io/crates/khronos_api)

[README](https://github.com/brendanzab/gl-rs/tree/master/khronos_api)

The Khronos XML API Registry, exposed as byte string constants.

```toml
[build-dependencies]
khronos_api = "1.0.0"
```

## Compiling from source

`khronos_api` uses a git submodule. You will need to initialize it before building:

```sh
git submodule update --init
```

A batch cargo script is provided at `bin/cargo`. [See the script](https://github.com/brendanzab/gl-rs/blob/master/bin/cargo)
for some example usages.
