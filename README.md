# Types for Rust

Types for Rust [Open Runtime](https://github.com/open-runtimes/open-runtimes/).

> **Note**: this is a temporary personal mirror published as
> `chiragagg5k-openruntimes-types-for-rust` on crates.io. The official
> upstream — once it exists at `github.com/open-runtimes/types-for-rust`
> — will publish under the bare `openruntimes` name; consumers should
> migrate at that point.

## Usage

Add the dependency to your `Cargo.toml`, aliased so your code can keep
using `openruntimes::*`:

```toml
[dependencies]
openruntimes = { version = "1.0", package = "chiragagg5k-openruntimes-types-for-rust" }
```

Then use it in your handler:

```rust
use openruntimes::Context;

pub fn main(context: Context) -> openruntimes::Response {
    context.log("Hello from Open Runtimes!");
    context.res.text("OK", None, None)
}
```

## License

[MIT](LICENSE)
