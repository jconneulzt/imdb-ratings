# slashDot Framework

> **Experimental classical hybrid runtime** built on Tokio async ecosystem

## 🚀 Quick Start

```toml
[dependencies]
slashDot-rust = "0.1.0"
tokio = { version = "1.0", features = ["full"] }
```

## ✨ Features
- **Circuit Simulation** - Qiskit integration via FFI
- **Async Runtime** - Tokio-based task scheduler
- **WASM Compilation** - WebAssembly target support
- **Hot Reload** - Runtime code replacement

## 📚 Examples

```rust
use slashDot_rust::slashDotRuntime;

#[tokio::main]
async fn main() {
    let runtime = slashDotRuntime::new();
    let result = runtime.execute_slashDot_circuit().await;
    println!("slashDot result: {:?}", result);
}
```

## 🔧 Configuration
Edit `slashDot.toml` to customize slashDot backend and async workers
