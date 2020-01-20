# Cargo

Pachetele software în Rust se numesc `crates`. Acestea sunt trecute în secțiunea `[dependencies]` a fișierului `Cargo.toml`.

Cargo așteaptă ca toate fișierele unui proiect să stea în directorul `src`. În rădăcina proiectului pui doar README, fișiere de configurare și licențe.

Pentru a construi proiectul, vei apela comanda `cargo build`. Rularea comenzii are ca finalitate crearea unui executabil în subdirectorul `target/debug`.

Rularea comenzii `cargo build` conduce la crearea în directorul rădăcină a fișierului `Cargo.lock`. Acest fișier ține evidența tuturor dependințelor necesare rulării programului.

## Compilare și rulare

Pentru a compila și rula în același pas, este nevoie să rulezi comanda `cargo run`. În cazul în care codul sursă nu a fost modificat, la rularea comenzii `cargo run` va fi rulat executabilul. Dacă sursa s-ar fi modificat, ar fi fost compilat din nou codul.

Comanda `cargo run` poate fi folosită pentru a testa noile lucruri adăugate în cod.

## Verificare codului fără compilare

Atunci când ai nevoie doar de o verificare a codului, vei folosi comanda `cargo check` pentru a verifica dacă se compilează corect codul. Este o bună practică verificarea din când în când. În momentul în care ești gata de a folosi executabilul, se va folosi comanda `cargo build`.

## Compilarea unui release

Atunci când codul este gata pentru un release, se va rula comanda `cargo build --release` pentru a compila codul. În cazul unui release, compilarea se va realiza folosindu-se și optimizări.
