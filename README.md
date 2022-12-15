# Il linguaggio di programmazione Rust

![Build Status](https://github.com/rust-lang/book/workflows/CI/badge.svg)

Questa repository contiene il libro intitolato "The Rust Programming Language" in versione italiana.

[Il libro é disponibile in forma cartacea da No Starch Press][nostarch]

[nostarch]: https://nostarch.com/rust

Puoi anche leggere il libro gratuitamente online.Si prega di consultare il libro 
incluso con le ultime versioni in inglese di Rust [stable], [beta] o [nightly].Tieni presente 
che eventuali problemi presenti in queste versioni potrebbero essere già stati risolti
in questa repository, poiché queste versioni vengono aggiornate meno frequentemente.

[stable]: https://doc.rust-lang.org/stable/book/
[beta]: https://doc.rust-lang.org/beta/book/
[nightly]: https://doc.rust-lang.org/nightly/book/

Consultando le [releases], puoi scaricare i codici sorgente che trovi presenti nel libro.

[releases]: https://github.com/rust-lang/book/releases

## Requisiti

Per costruire il libro è necessario [mdBook], idealmente la stessa 
versione utilizzata da `rust-lang/rust` in [questo file][rust-mdbook]. Per ottenerlo:

[mdBook]: https://github.com/rust-lang-nursery/mdBook
[rust-mdbook]: https://github.com/rust-lang/rust/blob/master/src/tools/rustbook/Cargo.toml

```bash
$ cargo install mdbook --version <version_num>
```

## Costruzione

Per costruire il libro, inserisci:

```bash
$ mdbook build
```

L'output sarà nella sottodirectory `book`. Per visualizzarlo, aprilo nel tuo web browser.

_Firefox:_
```bash
$ firefox book/index.html                       # Linux
$ open -a "Firefox" book/index.html             # OS X
$ Start-Process "firefox.exe" .\book\index.html # Windows (PowerShell)
$ start firefox.exe .\book\index.html           # Windows (Cmd)
```

_Chrome:_
```bash
$ google-chrome book/index.html                 # Linux
$ open -a "Google Chrome" book/index.html       # OS X
$ Start-Process "chrome.exe" .\book\index.html  # Windows (PowerShell)
$ start chrome.exe .\book\index.html            # Windows (Cmd)
```

Per avviare i tests:

```bash
$ mdbook test
```

## Contribuzione

Ci piacerebbe avere il tuo aiuto! Consulta [CONTRIBUTING.md](CONTRIBUTING.md) 
per scoprire i tipi di contributi che stiamo cercando.

Poiché il libro viene [stampato](https://nostarch.com/rust), e poiché vogliamo mantenere la versione online del libro il più possibile vicina alla versione stampata, potrebbe essere necessario più tempo del solito per affrontare il tuo problema o richiesta di pull.

Finora abbiamo effettuato una revisione più ampia per coincidere con [Rust Editions](https://doc.rust-lang.org/edition-guide/). Tra queste revisioni più ampie, correggeremo solo gli errori. Se il tuo problema o richiesta di pull non corregge esplicitamente un errore, potrebbe rimanere in attesa fino alla prossima volta in cui lavoriamo a una grande revisione: aspettati un ordine di mesi o anni. Grazie per la pazienza!

### Traduzioni

Ci piacerebbe aiuto con la traduzione del libro! Vedi etichetta [Translations] per unirti agli sforzi attualmente in corso. Apri una nuova 
issue per iniziare a lavorare su una nuova lingua! Stiamo aspettando il supporto [mdbook] per più lingue prima di unirli, ma sentiti libero di iniziare!

[Translations]: https://github.com/rust-lang/book/issues?q=is%3Aopen+is%3Aissue+label%3ATranslations
[mdbook support]: https://github.com/rust-lang-nursery/mdBook/issues/5

## Controllo ortografico

Per scansionare i file sorgente per errori di ortografia, puoi utilizzare lo script `spellcheck.sh` disponibile nella directory `ci`. Ha bisogno di un dizionario di parole valide, che è fornito in `ci/dictionary.txt`. Se lo script produce un falso positivo (ad esempio, hai usato la parola `BTreeMap` che lo script considera non valida), devi aggiungerla a `ci/dictionary.txt` (mantieni l'ordine ordinato per coerenza).
