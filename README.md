[![Build Status](https://travis-ci.org/nikomatsakis/ena.svg?branch=master)](https://travis-ci.org/nikomatsakis/ena)

An implementation of union-find / congruence-closure in Rust. Forked
from rustc for independent experimentation. My intention is to iterate
and improve this code and gradually bring back changes into rustc
itself, but also to enable other crates.io packages to use the same
code.

### Name

The name "ena" comes from the Greek word for "one".

### Features

By default, you just get the union-find implementation. You can
also opt-in to the following experimental features:

- `bench`: use to run benchmarks (`cargo bench --features bench`)
- `congruence-closure`: opt-in to the congruence closure
  implementation. This requires petgraph and is nightly only (since
  it uses `impl Trait`).

### License

Like rustc itself, this code is dual-licensed under the MIT and Apache
licenses. Pull requests, comments, and other contributions are assumed
to imply consent to those terms. Moreover, it is understood that any
changes here may well be used in rustc itself under the same terms.

