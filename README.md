# Uno.Wasm.MonoRuntime

The [Uno.Wasm.MonoRuntime](https://www.nuget.org/packages/Uno.Wasm.MonoRuntime) package provides the binaries and toolchain of the mono-wasm runtime.

This package requires the use of [Uno.Wasm.Bootstrap](https://github.com/unoplatform/Uno.Wasm.Bootstrap) to work properly.

## Why does this package exist ?
Currently, as of this writing, the mono-wasm runtime is not distributed in an easy-to-consume manner, which 
forces users of the runtime to reference the mono CI artifacts for building WebAssembly applications.

This packages provides a stable and persistent source for the runtime, but is probably only temporary, until the mono
team decides on the best way to publish those binaries.

## Why is there a dependency on Uno.Wasm.Bootstrap
The toolchain requires the use of a set of prerequisites, and build step which are currently not provided by the mono SDK, 
and the [Uno.Wasm.Bootstrap](https://github.com/unoplatform/Uno.Wasm.Bootstrap) provides this additional tooling.

## How often is this package updated?
This repository will be regularly updated with newer versions of the mono-wasm SDK, using the [mono projects CI output](https://jenkins.mono-project.com/).
