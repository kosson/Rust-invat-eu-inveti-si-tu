# Argumente

## Variabile mutabile cu `&mut`

Pentru a indica faptul că un identificator este mutabil atunci când este folosit ca argument, va fi semnalat acest lucru prin folosirea lui `&mut`.

```rust
io::stdin().read_line(&mut numeIdentificator).expect("Ceva care va apărea!");
```
