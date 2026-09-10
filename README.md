# byteview

Learning Rust by rewriting coreutils, one tool at a time

Started as a weekend hack, grew on me.

## Getting started

```bash
cargo build --release
```

## Examples

```bash
./target/release/byteview src/*.rs
cat README.md | ./target/release/byteview
```

## Features

- Reads stdin or multiple files
- Zero dependencies outside std
- Counts lines, words and bytes like wc
- Parallel over files with std threads

## Project structure

```text
├── .github/
│   └── workflows/
│       └── ci.yml
├── docs/
│   ├── development.md
│   ├── faq.md
│   └── usage.md
├── examples/
│   └── quickstart.md
├── src/
│   └── main.rs
├── .gitignore
├── CHANGELOG.md
├── CONTRIBUTING.md
├── Cargo.toml
└── SECURITY.md
```

## Development

```bash
cargo build
cargo clippy -- -D warnings
```

## Acknowledgments

- README structure inspired by popular OSS templates
- Thanks to everyone opening issues with ideas
