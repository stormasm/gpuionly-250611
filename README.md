
#### How to get it working with gpui-component

This is in reference to getting [gpui-component](https://github.com/longbridge/gpui-component) to use zed locally instead of from github.

Cargo.toml

```rust
[workspace.dependencies]
#gpui = { git = "https://github.com/zed-industries/zed.git" }
gpui = { path = "/Users/ma/j/tmp11/zed/crates/gpui" }
#gpui = { path = "/Users/ma/j/tmp11/gpuionly-250611/crates/gpui" }
gpui-component = { path = "crates/ui" }
gpui-component-macros = { path = "crates/macros" }
story = { path = "crates/story" }
```

---

crates/story/Cargo.toml

```rust
#reqwest_client = { git = "https://github.com/zed-industries/zed.git" }
reqwest_client = { path = "/Users/ma/j/tmp11/zed/crates/reqwest_client" }
#reqwest_client = { path = "/Users/ma/j/tmp11/gpuionly-250611/crates/reqwest_client" }
```
