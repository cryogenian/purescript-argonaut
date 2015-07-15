# PureScript-Argonaut

[![Build Status](https://travis-ci.org/purescript-contrib/purescript-argonaut.svg)](https://travis-ci.org/purescript-contrib/purescript-argonaut)

This is an implementation of [Argonaut][argonaut] for the PureScript language.

While not as feature rich as the Scala version, it still supports encoding and decoding.

A recent change is using native Javascript data types and functionality for parsing and rendering. If you don't use lenses, performance should be extremely good.

## Installation

This can be installed with bower:

```shell
bower i purescript-argonaut
```

__purescript-argonaut__ depends only on 

* __purescript-argonaut-core__ -- basic types and folds, printing, parsing
* __purescript-argonaut-codecs__ -- typeclasses for encoding and decoding `Json`, useful combinators
* __purescript-argonaut-traversals__ -- prisms and traversals for `Json` type

and reexport all public functions and types from them in `Data.Argonaut` module

## Usage

If you have some data type, and you want to encode it into JSON,
you need to define an instance for Encode.

If you have some JSON, and you want to decode it into some data type,
you need to define an instance for Decode.

[argonaut]: http://argonaut.io/

