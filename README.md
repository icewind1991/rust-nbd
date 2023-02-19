rust-nbd
---

[Network block device](https://en.wikipedia.org/wiki/Network_block_device) protocol implementation in Rust. Not all features are currently supported in server.

Accepts a `Read`+`Write`+`Seek` as a data to be exposed in server mode. Provides `Read`+`Write`+`Seek` in client mode. Underlying connection is `Read`+`Write`, usage of `bufstream` crate is recommended.

This library is IO-agnostic, but async is not supported.

See [server example](https://github.com/vi/rust-nbd/blob/master/examples/server.rs) or [client example](https://github.com/vi/rust-nbd/blob/master/examples/client.rs).

This is a rather early version.
