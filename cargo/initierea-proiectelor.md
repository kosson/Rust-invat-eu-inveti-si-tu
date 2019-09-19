# Inițierea proiectelor

Pentru a genera un nou proiect Rust, vom folosi Cargo pentru a face setările preliminare.

```bash
cargo new proiect_cargo
```

Inițierea se face prin crearea directorului cu numele specificat în comandă. În interiorul directorului vei găsi un fișier `Cargo.toml`, git-ul deja inițiat prin directorul `.git`, un fișier `.gitignore` și un director `src` în care se află un fișier `main.rs`.

Întreg codul sursă va sta în directorul `src`.

## Cargo.toml

Fișierul `Cargo.toml` este redactat în [Tom’s Obvious, Minimal Language](https://github.com/toml-lang/toml), care este și formatul de configurare adoptat de Rust.
Acest format indică secțiunile folosind croșetele drepte. Prima este `[package]`, care indică faptul că următoarele enunțuri sunt utilizate pentru configurarea unui pachet.

Pachetele software în Rust sunt numite *crates*.

### Construcția proiectului

Pentru a construi proiectul, vom iniția comanda `cargo build`.
