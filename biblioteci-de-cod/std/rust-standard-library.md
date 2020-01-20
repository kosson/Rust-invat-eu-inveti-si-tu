# Rust Standard Library

Rust Standard Library este fundamentul modularității ecosistemului Rust.
Această bibliotecă oferă tipuri nucleu ale limbajului precum `Vec<T>` sau `Option<T>`, primitive, macro-uri, biblioteci I/O și multe altele.

Biblioteca Standard este împărțită în module.

Primitivele în Rust sunt implementate de compilator, dar Rust Standard Library implementează metode direct pe aceste tipuri de primitive. Astfel că Standard Library exportă multe module care au numele primitivelor. Încercați să eliminați confuzia între modulele care poartă numele primitivelor și primitivele în sine.

Rust Standard Library exportă și o serie de macro-uri.

Tot Rust Standard Library definește o colecție de elemente numite generic *The Rust Prelude*, care sunt importate în fiecare modul al fiecărui crate. Multe dintre aceste elemente se numest *traits*.
