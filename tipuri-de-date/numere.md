# Numere

## Unsigned numbers

Numerele care nu au semn sunt cele care vor fi mereu pozitive. Un număr `u8` este un număr de 8 biți unsigned. În cazul nostru, litera `u` din `u8` va marca faptul că vorbim despre un număr întreg *unsigned*.

```rust
fn main () {
  let a:u8 = 123; // un singur byte
  println!("a este {}", a);
}
```

În exemplul nostru, avem un număr de 8 biți, care pornește de la 0, la 255.

## Signed numbers

Un număr întreg (**integer**) este un număr care poartă un semn. Acesta pornește de la -128 la 128.

```rust
fn main () {
  let a:i8 = 123; // un singur byte signed
}
```

## Numere pe 32 de biți signed

```rust
use std::mem;

fn main () {
  let a = 200032432; // un număr signed pe 32 de biți (4bytes)
  println!("a are valoarea {} și dimensiunea {}", a, mem::size_of_val(&a));
}
```

## Numere întregi

Putem avea numere întregi care să aibă dimensiunea cuvântului (dimensiunea pointer-ului). Aceste valori pot fi marcate ca *usize* și *isize*.

```rust
use std::mem;
fn main () {
  let b:isize = 200032432; // un număr signed pe 32 de biți (4bytes)
  let dimensiunea_lui_b = mem::size_of_val(&b);
  println!("b are valoarea {}, are dimensiunea de {} de tipul {}-bit", b, mem::dimensiunea_lui_b, dimensiunea_lui_b*8);
}
```

## Numere fracționare

Numerele fracționare sunt considerate a fi double-precision, adică 8 bytes sau altfel 64 biți, iar tipul datelor este scris ca `f64` (floating-points).

```rust
let o_valoare:f64 = 3.1;
```
