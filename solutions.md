# Reverse a string

```rust
// src/lib.rs
use unicode_segmentation::UnicodeSegmentation;

pub fn reverse(input: &str) -> String {
    input.graphemes(true).rev().collect()
}


// Cargo.toml
[dependencies]
unicode-segmentation = "1.8.0"

[features]
grapheme = []

[package]
edition = "2021"
name = "reverse_string"
version = "1.2.0"
```
