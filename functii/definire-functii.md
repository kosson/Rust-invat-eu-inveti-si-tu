# Definirea funcțiilor

Pentru a declara o funcție în Rust, vei folosi cuvântul cheie `fn` urmat de paranteze rotunde și acolade. În momentul în care programul este rulat, Rust caută funcția numită `main`. În cazul în care programul nu are o funcție main, nu este un program, ci este o bibliotecă de cod.

## Funcția `main()`

Fiecare program în Rust trebuie să aibă o funcție `main()`. Acest lucru este necesar pentru că va fi prima funcție care va fi executată la rularea programului.
Cel mai simplu program valid în Rust este chiar declararea funcției `main()`.

```rust
fn main(){}
```

Exemplu va conduce la o compilare corectă a codului, dar fără niciun rezultat concret. Pentru a afișa un mesaj pe ecran în scopul de a vedea concret un rezultat, putem folosi funcția (*macro*) `print!`.

```rust
fn main () {
    print!("Salutare");
}
```