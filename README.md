# Leptos Tutorial

[Leptos Book](https://book.leptos.dev)

## Editor Setup

[leptosfmt](https://github.com/bram209/leptosfmt) suggests per-workspace setup.

### Helix

`.helix/languages.toml`
```toml
[[language]]
name = "rust"

[language-server.rust-analyzer.config]
procMacro = { ignored = { leptos_macro = ["server"] } }
rustfmt = { overrideCommand = ["leptosfmt", "--stdin", "--rustfmt"] }
```
