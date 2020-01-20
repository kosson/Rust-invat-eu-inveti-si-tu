# Funcția `stdin()`

Aceasta poate fi apelată din modulul `io`. Această funcție returnează o instanță a tipului `Stdin` (`std::io::Stdin`). Acesta este un instrument de lucru cu inputul în terminal.

```rust
use std::io;

io::stdin().read_line(&mut numeIdentificator)
           .expect("Măi, ceva nu e ok!");
```

## Metoda `read_line()`

Această metodă este apelată pe instrumentul (*handle*) de lucru cu terminalul instanțiat prin `io::stdin()` pentru a prelua inputul de la utilizator și a-l introduce într-o structură de date pasată drept argument.

Această metodă va returna o valoare de tipul `io::Result`. Tipurile `Result` sunt enumerări (*enumerations*), denumite adesea **enums**. Pentru `Result`, *enum variants* sunt `Ok` și `Err`. Varianta `Ok` indică faptul că operațiunea s-a încheiat cu succes, iar în `Ok` vom găsi valoarea care a fost generată.
Varianta `Err` conține informații care privesc cum sau de ce operațiunea a eșuat.

Valorile unui tip `Result` pot avea metode așa cum este `expect()` din exemplul de mai sus. Dacă programul se va executa, dar are erori, mesajul pasat metodei `expect` va fi afișat. Dacă nu sunt erori, metoda `expect` va returna valoarea din *enum variant* `Ok` pentru a putea fi folosită mai departe.

În cazul în care nu este folosită metoda `expect`, la compilare, Rust va emite un warning. Rust se așteaptă să consumi rezultatul pentru că ar putea conține și erorile care au apărut.
