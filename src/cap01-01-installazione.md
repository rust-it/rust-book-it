# Installazione

Il primo passo è installare Rust. Scaricheremo Rust tramite `rustup`, uno strumento da linea di comando per gestire le versioni di Rust e gli strumenti associati. Avrai bisogno di una connessione a internet per il download.

> Nota: Se per qualche motivo preferisci non usare `rustup`, consulta la pagina
> [Altri Medoti di Installazione Rust][otherinstall] per altre opzioni.

I passi seguenti installano l'ultima versione stabile del compilatore Rust. La stabilità di Rust garantisce che tutti gli esempi del libro che compilano correttamente continueranno a compilare con nuove versioni di Rust. L'output potrebbe differire leggermente tra le versioni perché Rust spesso migliora i messaggi di errore e gli avvisi. In altre parole, qualsiasi versione più recente e stabile di Rust che installi usando questi passi dovrebbe funzionare come previsto con il contenuto di questo libro.

> ### Notazione da linea di comando `$`
>
> In questo capitolo e per tutto il libro, mostreremo alcuni comandi utilizzati
> nel terminale. Le linee che devi inserire in un terminale iniziano tutte con `$`. 
> Non è necessario digitare il carattere `$`; è il prompt della riga di comando che 
> viene mostrato per indicare l'inizio di ogni comando. Le linee che non iniziano 
> con `$` di solito mostrano l'output del comando precedente. Inoltre, gli esempi 
> specifici per PowerShell utilizzeranno `>` invece di `$`.

### Installare `rustup` su Linux o macOS

Se stai utilizzando Linux o macOS, apri un terminale e inserisci il seguente comando:

```console
$ curl --proto '=https' --tlsv1.3 https://sh.rustup.rs -sSf | sh
```

Il comando scarica uno script e avvia l'installazione dello strumento `rustup`, che installa l'ultima versione stabile di Rust. Potrebbe essere richiesta la tua password. Se l'installazione ha successo, verrà visualizzata la seguente riga:

```text
Rust is installed now. Great!
```

Avrai anche bisogno di un *linker*, che è un programma che Rust utilizza per unire i suoi output compilati in un unico file. È probabile che tu ne abbia già uno. Se ottieni errori di linker, dovresti installare un compilatore C, che di solito include un linker. Un compilatore C è utile anche perché alcuni pacchetti Rust comuni dipendono dal codice C e avranno bisogno di un compilatore C.

Su macOS, puoi ottenere un compilatore C eseguendo:

```console
$ xcode-select --install
```

Gli utenti Linux dovrebbero in generale installare GCC o Clang, secondo la documentazione della loro distribuzione. Ad esempio, se si utilizza Ubuntu, è possibile installare il pacchetto `build-essential`.

### Installare `rustup` su Windows

Su Windows, vai a [https://www.rust-lang.org/tools/install][install] e segui le istruzioni per installare Rust. In un determinato momento dell'installazione, riceverai un messaggio che spiega che avrai anche bisogno degli strumenti di compilazione MSVC per Visual Studio 2013 o successivi.

Per acquisire gli strumenti di compilazione, è necessario installare [Visual Studio 2022][visualstudio]. Quando viene chiesto quale set di funzionalità installare, includere:

* “Desktop Development with C++”
* The Windows 10 or 11 SDK
* Il componente del pacchetto lingua inglese, insieme ad ogni altro pacchetto lingua a tua scelta

Il resto di questo libro utilizza comandi che funzionano sia in *cmd.exe* che in *PowerShell*. Se ci sono differenze specifiche, spiegheremo quale usare.

### Risoluzione dei problemi

Per verificare se hai installato correttamente Rust, apri una shell e inserisci questa riga:

```console
$ rustc --version
```

Dovresti vedere il numero di versione, l'hash di commit e la data di commit dell'ultima versione stabile rilasciata, nel seguente formato:

```text
rustc x.y.z (abcabcabc yyyy-mm-dd)
```

Se vedi queste informazioni, hai installato Rust con successo! Se non vedi queste informazioni, verifica che Rust sia nella variabile di sistema `%PATH%` come segue.

In Windows CMD, usa:

```console
> echo %PATH%
```

In PowerShell, usa:

```powershell
> echo $env:Path
```

In Linux e macOS, usa:

```console
$ echo $PATH
```

Se tutto è corretto e Rust ancora non funziona, ci sono una serie di posti dove puoi ottenere aiuto. Scopri come entrare in contatto con gli altri Rustacei (un nomignolo sciocco con cui veniamo chiamati) sulla [pagina della community][community].

### Aggiornamento e Disinstallazione

Una volta che Rust è stato installato tramite  `rustup`, aggiornare a una nuova versione rilasciata è facile. Dalla shell, esegui lo script di aggiornamento seguente:

```console
$ rustup update
```

Per disinstallare Rust e `rustup`, esegui lo script di disinstallazione seguente dalla shell:

```console
$ rustup self uninstall
```

### Documentazione Locale

L'installazione di Rust include anche una copia locale della documentazione in modo che tu possa leggerla offline. Esegui `rustup doc` per aprire la documentazione locale nel tuo browser.

In qualsiasi momento un tipo o una funzione è fornita dalla libreria standard e non sei sicuro di cosa fa o come usarla, usa la documentazione dell'application programming interface (API) per scoprirlo!

[otherinstall]: https://forge.rust-lang.org/infra/other-installation-methods.html
[install]: https://www.rust-lang.org/tools/install
[visualstudio]: https://visualstudio.microsoft.com/downloads/
[community]: https://www.rust-lang.org/community