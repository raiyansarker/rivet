# Rivet 🔩

A lightweight, minimal Redis-compatible in-memory datastore written in Rust.

> **Note**: This project is built purely for learning and educational purposes. It is currently under active development and not intended for production use.

---

## ✨ Features & Goals

- **Redis Protocol (RESP)**: Speaks the standard Redis Serialization Protocol.
- **In-Memory Storage**: Fast, ephemeral key-value store.
- **Minimal & Educational**: Clean codebase focused on core database & networking fundamentals without external bloat.
- **CLI Compatible**: Works seamlessly with official Redis clients like `redis-cli`.

---

## 🗺️ Roadmap & Commands

- [ ] **RESP Parser**: Basic parsing of Simple Strings, Errors, Integers, Bulk Strings, and Arrays
- [ ] **Connection Handling**: TCP listener with concurrent client handling
- [ ] **Basic Commands**:
  - [ ] `PING`
  - [ ] `ECHO`
  - [ ] `SET` / `GET`
  - [ ] `DEL`
  - [ ] `EXISTS`
- [ ] **Key Expiration**: TTL / `EXPIRE` support

---

## 🚀 Getting Started

### Prerequisites

- [Rust](https://www.rust-lang.org/tools/install)
- `redis-cli` (optional, for testing commands)

### Running the Server

```bash
# Clone the repository
git clone https://github.com/raiyansarker/rivet.git
cd rivet

# Run the server
cargo run
```

### Connecting with `redis-cli`

Once running, connect using standard Redis tooling:

```bash
redis-cli -p 6379
127.0.0.1:6379> PING
PONG
```

---

## 📄 License

Licensed under the [MIT License](LICENSE).
