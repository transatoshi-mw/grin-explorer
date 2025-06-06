# Grincoin.org (GRIN) Blockchain Explorer Re-skin
Fork of the Grincoin.org blockchain explorer for the Grin cryptocurrency with proper theming.

![Screenshot from 2025-05-26 22-54-37](https://github.com/user-attachments/assets/3c4a39b0-49c0-4b5d-aef2-22d32b2de28c)

## What is Grin?
Grin is the very first, simple and fair MimbleWimble blockchain implementation.

- Scalable, privacy-preserving blockchain.
- Fair and verifiable coin distribution.
- Not controlled by any company, foundation or individual.

## Prerequisites

- Rust: https://www.rust-lang.org/tools/install.
- SQLite: `sudo apt install sqlite3 libsqlite3-dev`
- Grin node: https://github.com/mimblewimble/grin. You need to enable archival mode, so the explorer can see all the blocks, otherwise only the recent blocks can be explored.


## Installation

1. Clone repository: `git clone https://github.com/aglkm/grin-explorer.git`
2. Build explorer:
   ```
   cd grin-explorer
   cargo build --release
   ```
4. Run executable: `RUST_LOG=rocket=warn,grin_explorer ./target/release/grin-explorer`

   You will see the following output:

   ```
   [2024-09-30T13:30:02Z INFO  grin_explorer] starting up.
   [2024-09-30T13:30:02Z WARN  rocket::launch] 🚀 Rocket has launched from http://127.0.0.1:8000
   [2024-09-30T13:30:03Z INFO  grin_explorer] worker::data ready.
   [2024-09-30T13:30:10Z INFO  grin_explorer] worker::stats ready.
   ```

5. Open explorer in your browser: http://127.0.0.1:8000
