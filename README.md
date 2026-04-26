# Types for Rust

Types for Rust [Open Runtime](https://github.com/open-runtimes/open-runtimes/).

## Usage

Add the dependency to your `Cargo.toml`:

```toml
[dependencies]
openruntimes = { git = "https://github.com/open-runtimes/types-for-rust" }
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
