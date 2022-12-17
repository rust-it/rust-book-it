# Hello, World!

Adesso che hai installato Rust, è il momento di scrivere il tuo primo programma in Rust.
Tradizionalmente quando si impara un nuovo linguaggio si scrive un piccolo programma che
stampa il testo `Hello, world!` sullo schermo, quindi faremo lo stesso qui!

> Nota: questo libro assume una familiarità di base con la riga di comando. Rust non fa
> richieste specifiche sulla tua modifica o sullo strumento o su dove si trova il tuo codice, 
> quindi se preferisci utilizzare un ambiente di sviluppo integrato (IDE) invece della riga di comando,  
> sentiti libero di  utilizzare il tuo IDE preferito. Molti IDE adesso hanno un certo grado di supporto per  
> Rust; consulta la documentazione dell'IDE per i dettagli. Il team di Rust si è concentrato sull'abilitare un
> ottimo supporto IDE tramite 'rust-analyzer'. Vedi l'Appendice D per maggiori dettagli.

### Creare una Directory per il progetto


Inizierai creando una directory per archiviare il tuo codice Rust. A Rust non importa dove si trova il tuo codice, ma per gli esercizi e i progetti di questo libro, suggeriamo di creare una directory progetti nella tua directory home e di mantenere tutti i tuoi progetti lì.

Apri un terminale e inserisci i seguenti comandi per creare una directory *projects* 
e una directory per il progetto `Hello, world!` all'interno della directory *projects*.

Per Linux, macOS e PowerShell su Windows, inserisci questo:

```console
$ mkdir ~/projects
$ cd ~/projects
$ mkdir hello_world
$ cd hello_world
```

Per Windows CMD, inserisci questo:

```cmd
> mkdir "%USERPROFILE%\projects"
> cd /d "%USERPROFILE%\projects"
> mkdir hello_world
> cd hello_world
```

### Scrivere e eseguire un programma Rust

Successivamente, crea un nuovo file sorgente e chiamalo main.rs. I file Rust terminano sempre con
l'estensione .rs. Se stai utilizzando più di una parola nel tuo nome file, la
convenzione è quella di utilizzare un underscore per separarle. Ad esempio, usa
hello_world.rs invece di helloworld.rs.