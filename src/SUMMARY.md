# Il linguaggio di programmazione Rust

[Il Linguaggio di Programmazione Rust](titolo-pagina.md)
[Prologo](prologo.md)
[Introduzione](cap00-00-introduzione.md)

## Iniziamo

- [Iniziamo](cap01-00-iniziamo.md)
    - [Installazione](cap01-01-installazione.md)
    - [Hello, World!](cap01-02-hello-world.md)
    - [Hello, Cargo!](cap01-03-hello-cargo.md)

- [Programmare un gioco di indovinelli](cap02-00-gioco-di-indovinelli-tutorial.md)

- [Concetti comuni di programmazione](cap03-00-concetti-comuni-programmazione.md)
    - [Variabili e Mutabilità](cap03-01-variabili-e-mutabilita.md)
    - [Tipi di dati](cap03-02-tipi-di-dati.md)
    - [Funzioni](cap03-03-funzioni.md)
    - [Commenti](cap03-04-commenti.md)
    - [Flusso di Controllo](cap03-05-flusso-controllo.md)

- [Comprendere il concetto di proprietà](cap04-00-concetto-di-proprieta.md)
    - [Cos'è la proprietà?](cap04-01-proprieta.md)
    - [Riferimenti e Prestito](cap04-02-riferimenti-e-prestito.md)
    - [Il Tipo Slice](cap04-03-slice.md)

- [Organizzare dati correlati con struct](cap05-00-struct.md)
    - [Definizione e Istanza struct](cap05-01-definizione-struct.md)
    - [Un Esempio di Programma usando struct](cap05-02-esempio-struct.md)
    - [Sintassi Metodo](cap05-03-sintassi-metodo.md)

- [Enum e Corrispondenza di Modelli](cap06-00-enum.md)
    - [Definizione Enum](cap06-01-definizione-enum.md)
    - [`match` , Il Costrutto di Flusso di Controllo](cap06-02-match.md)
    - [Flusso di Controllo Conciso usando `if let`](cap06-03-if-let.md)

## Conoscenza di base di Rust

- [Gestione Grandi Progetti con Packages, Crates, e Moduli](cap07-00-gestione-progetti.md)
    - [Packages e Crates](cap07-01-packages-e-crates.md)
    - [Definire i moduli per controllare l'ambito e la privacy](cap07-02-definizione-moduli.md)
    - [Utilizzo dei percorsi per fare riferimento agli elementi nell'albero dei moduli](cap07-03-utilizzo-percorsi-albero-moduli.md)
    - [Portare percorsi nel campo di applicazione con `use`](cap07-04-portare-percorsi-nel-campo-di-applicazione-use.md)
    - [Separare i Moduli in diversi file](cap07-05-separare-i-moduli-in-diversi-file.md)

- [Collezioni più comuni](cap08-00-collezioni-comuni.md)
    - [Memorizzare Liste di Valori in Vettori](cap08-01-vettori.md)
    - [Memorizzare il testo codificato in UTF-8 con le stringhe](cap08-02-strings.md)
    - [HashMap](cap08-03-hash-map.md)

- [Gestione degli errori](cap09-00-gestione-errori.md)
    - [Errori Irrecuperabili con `panic!`](cap09-01-errori-irrecuperabili.md)
    - [Errori Recuperabili con `Result`](cap09-02-errori-recuperabili.md)
    - [Panico o non panico?](cap09-03-panico-o-non-panico.md)

- [Tipi Generici, Tratti, Durata](cap10-00-tipi-generici.md)
    - [Tipi Generici](cap10-01-sintassi.md)
    - [Tratti: definire comportamenti condivisi](cap10-02-tratti.md)
    - [Convalidare riferimenti con la durata](cap10-03-sintassi-durata.md)

- [Scrivere test automatizzati](cap11-00-test-automatizzati.md)
    - [Come scrivere test](cap11-01-come-scrivere-test.md)
    - [Controllo Esecuzione Test](cap11-02-controllo-esecuzione-test.md)
    - [Organizzazione Test](cap11-03-organizzazione-test.md)

- [Un Progetto I/O: costruire un programma riga di comando](cap12-00-progetto-io.md)
    - [Accettare argomenti da riga di comando](cap12-01-accettazione-argomenti.md)
    - [Leggere un File](cap12-02-leggere-un-file.md)
    - [Refactoring per migliorare la modularità e la gestione degli errori](cap12-03-refactoring.md)
    - [Sviluppo funzionalità della libreria utilizzanto TDD](cap12-04-testare-la-funzionalità.md)
    - [Lavorare con Variabili d'Ambiente](cap12-05-variabili-ambiente.md)
    - [Scrivere messaggi di errore sullo Standard Error invece cape sullo Standard Output](cap12-06-stderr-invece-stdout.md)

## Saper pensare in Rust

- [Carattarestiche del linguaggio funzionale: iterator e closures](cap13-00-caratteristiche-funzionali.md)
    - [Closures: Funzioni Anonime che hanno accesso alle variabili d'ambiente](cap13-01-closures.md)
    - [Processare una serie di elementi con gli Iterators](cap13-02-iterators.md)
    - [Migliorare il Progetto I/O](cap13-03-migliorare-io-project.md)
    - [Confronto delle Prestazioni: Cicli contro Iterators](cap13-04-prestazioni.md)

- [Note aggiunte su Cargo e Crates.io](cap14-00-note-aggiuntive-cargo.md)
    - [Personalizzazione delle build con profili di rilascio](cap14-01-profili-di-rilascio.md)
    - [Pubblicare una Crate in Crates.io](cap14-02-pubblicazione-crates.md)
    - [Ambienti di Lavoro Cargo](cap14-03-ambienti-lavoro-cargo.md)
    - [Installare binari da Crates.io con `cargo install`](cap14-04-installazione-binari.md)
    - [Estendere Cargo con comandi personalizzati](cap14-05-cargo-comandi-personalizzati.md)

- [Puntatori Intelligenti](cap15-00-puntatori-intelligenti.md)
    - [Fare riferimento a dati nella Heap utilizzando `Box<T>`](cap15-01-box.md)
    - [Utilizzare i puntatori intelligenti come riferimenti normali con `Deref`](cap15-02-deref.md)
    - [Eseguire codice durante la pulizia con il trait `Drop`](cap15-03-drop.md)
    - [`Rc<T>`, il puntatore intelligente a conteggio di riferimenti](cap15-04-rc-puntatore-intelligente.md)
    - [`RefCell<T>` e il Modello di Mutabilità Interna](cap15-05-mutabilita-interna.md)
    - [I cicli di riferimento possono causare perdite di memoria](cap15-06-cicli-di-riferimento.md)

- [Concorrenza senza paura](cap16-00-concorrenza.md)
    - [Usare i thread per eseguire il codice contemporaneamente](cap16-01-threads.md)
    - [Utilizzare il passaggio di messaggi per trasferire i dati tra i thread](cap16-02-passaggio-di-messaggi.md)
    - [Concorrenza basata sullo stato condiviso](cap16-03-concorrenza-stato-condiviso.md)
    - [Concorrenza estendibile con `Sync` e `Send`](cap16-04-concorrenza-estendibile-sync-send.md)

- [Proprietà di programmazione orientata agli oggetti di Rust](cap17-00-oop.md)
    - [Caratteristiche dei linguaggi orientati agli oggetti](cap17-01-caratteristiche-linguaggi-oggetti.md)
    - [Utilizzare gli oggetti tratto per consentire valori di tipi diversi](cap17-02-trait-oggetti.md)
    - [Implementare un modello di progettazione orientato agli oggetti](cap17-03-oo-design-patterns.md)

## Argomenti Avanzati

- [Pattern e Corrispondeze](cap18-00-patterns.md)
    - [Tutte le situazioni in cui i pattern possono essere utilizzati](cap18-01-situazioni-pattern.md)
    - [Rifiutabilità: quando un pattern potrebbe non corrispondere](cap18-02-refutability.md)
    - [Sintassi Pattern](cap18-03-sintassi-pattern.md)

- [Funzionalità Avanzate](cap19-00-funzionalità-avanzate.md)
    - [Rust Pericoloso](cap19-01-rust-pericoloso.md)
    - [Traits Avanzati](cap19-03-traits-avanzati.md)
    - [Tipi Avanzati](cap19-04-tipi-avanzati.md)
    - [Funzioni e Closures Avanzati](cap19-05-funzioni-e-closures-avanzati.md)
    - [Macros](cap19-06-macros.md)

- [Progetto finale: costruire un Server Web Multithread](cap20-00-server-web-multithread.md)
    - [Realizzare un Server Web Monothread](cap20-01-server-web-monothread.md)
    - [Trasformare il nostro Server Monothread in un Server Multithread](cap20-02-da-monothread-a-multithread.md)
    - [Arresto Elegante e Pulizia](cap20-03-arresto-anomalo-pulizia.md)

- [Appendice](appendice-00.md)
    - [Appendice A - Parole chiave](appendice-01-parole-chiave.md)
    - [Appendice B - Operatori e Simboli](appendice-02-operatori.md)
    - [Appendice C - Proprietà derivabili](appendice-03-proprietà-derivabili.md)
    - [Appendice D - Strumento di Sviluppo Utili](appendice-04-strumento-di-sviluppo.md)
    - [Appendice E - Edizioni](appendice-05-edizioni.md)
    - [Appendice F - Traduzioni del Libro](appendice-06-traduzioni.md)
    - [Appendice G - Come é stato creato Rust e “Nightly Rust”](appendice-07-nightly-rust.md)
