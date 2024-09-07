# KV-RS Key value store

Log-structured, append-only database, stores and retrieves sequences
of bytes ([u8]) of arbitrary length

## Usage

The database file is `db.kv` is an implementation of the Bitcask storage backend.

## Build locally
1. Once the repository is cloned run `cargo build`
2. You will have a `kv_rs || kv_rs.exe` executable in the `target/debug` directory.

## Options
You can also create your own db file. To use the built in db update `FILE` to `db.kv`
```
kv_rs FILE get KEY 
kv_rs FILE delete KEY
kv_rs FILE insert KEY VALUE
kv_rs FILE update KEY VALUE
```
