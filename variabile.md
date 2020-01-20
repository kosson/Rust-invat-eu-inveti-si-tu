# Variabile

Variabilele sunt declarate în program folosind cuvântul rezervat `let`.

În Rust, variabile sunt immutable din start. Pentru a face o variabilă să fie mutable, vei menționa înaintea identificatorului cuvântul cheie `mut`.

```rust
let prima = 10; // nu poate fi modificată
let mut ceva = String::new(); // modificabilă
```

Pentru a indica faptul că un identificator este mutabil atunci când este folosit ca argument, va fi semnalat acest lucru prin folosirea lui `&mut`.

```rust
io::stdin().read_line(&mut numeIdentificator).expect("Ceva care va apărea!");
```

## Referințe

Semnul `&` indică faptul că avem de-a face cu o *referință* către niște date care pot fi accesate din mai multe zone ale programului. Acest lucru elimină necesitatea de a copia datele de mai multe ori.

Referințele nu pot fi modificate din oficiu.
