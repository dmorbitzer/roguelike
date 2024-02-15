# Roguelike Rust Game

A small roguelike game written in Rust

## Requirements
* rustup: 1.26.0

## Start local
`cargo run`

## Build
`cargo build`

## Compile for Web
### Setup
`rustup target add wasm32-unknown-unknown`
`cargo install wasm-bindgen-cli`

### Compile
`cargo build --release --target wasm32-unknown-unknown`

### Prepare wasm File
`wasm-bindgen target\wasm32-unknown-unknown\release\yourproject.wasm --out-dir wasm --no-modules --no-typescript`