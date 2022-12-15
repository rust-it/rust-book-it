# Introduzione

Benvenuti in *Il Linguaggio di Programmazione Rust*, un libro introduttivo su Rust.
Il linguaggio di Programmazione Rust ti aiuta a scrivere software più veloce e affidabile.
L'ergonomia ad alto livello e il controllo a basso livello spesso sono in contrasto nella progettazione dei linguaggi di programmazione; Rust sfida questo conflitto. Attraverso l'equilibrio di una potente capacità tecnica e un'ottima esperienza dagli sviluppatori, Rust ti offre l'opzione di controllare i dettagli a basso livello (come l'utilizzo della memoria) senza tutti i problemi tradizionalmente associati a tale controllo.

## A chi è destinato Rust

Rust è ideale per molte persone per una varietà di motivi. Diamo un'occhiata a alcuni dei gruppi più importanti.

### Team di sviluppatori

Rust si sta dimostrando uno strumento produttivo per la collaborazione tra grandi team di sviluppatori con diversi livelli di conoscenza della programmazione di sistema. Il codice a basso livello è suscettibile a vari bug sottili, che in altri linguaggi possono essere individuati solo attraverso un'ampia quantità di test e un attento controllo del codice da parte di sviluppatori esperti. In Rust, il compilatore svolge il ruolo di guardiano rifiutando di compilare codice con questi bug difficili da individuare, compresi i bug di concorrenza. Lavorando insieme al compilatore, il team può concentrarsi sulla logica del programma piuttosto che sulla caccia ai bug.

Inoltre, Rust porta gli strumenti per sviluppatori contemporanei nel mondo della programmazione di sistema:

* *Cargo*, il gestore delle dipendenze e lo strumento di compilazione inclusi, rende semplice e coerente l'aggiunta, la compilazione e la gestione delle dipendenze all'interno dell'ecosistema Rust.
* Lo strumento di formattazione *Rustfmt* garantisce uno stile di codifica coerente tra gli sviluppatori.
* Il Rust Language Server alimenta l'integrazione di Integrated Development Environment (IDE) per il completamento del codice e i messaggi di errore in linea.

Utilizzando questi e altri strumenti nell'ecosistema Rust, gli sviluppatori possono essere produttivi mentre scrivono codice a livello di sistema.

### Studenti

Rust è destinato agli studenti e a coloro che sono interessati a imparare i concetti di sistema. Utilizzando Rust, molte persone hanno appreso argomenti come lo sviluppo di sistemi operativi. La comunità è molto accogliente e felice di rispondere alle domande degli studenti. Attraverso sforzi come questo libro, i team di Rust vogliono rendere i concetti di sistema accessibili a un numero sempre maggiore di persone, specialmente a coloro che si avvicinano per la prima volta alla programmazione.

### Imprese

Centinaia di aziende, grandi e piccole, usano Rust in produzione per una varietà di attività, tra cui strumenti da riga di comando, servizi web, strumenti DevOps, dispositivi incorporati, analisi audio e video e transcodifica, criptovalute, bioinformatica, motori di ricerca, applicazioni Internet of Things, apprendimento automatico e persino parti principali del browser web Firefox.

### Sviluppatori open source

Rust è per le persone che vogliono contribuire alla costruzione del linguaggio stesso, la comunità, gli strumenti per sviluppatori e le librerie. Saremmo felici di averti come contributore del linguaggio Rust.

### Persone che valorizzano velocità e stabilità

Rust è per le persone che desiderano velocità e stabilità in un linguaggio. Con velocità, intendiamo sia la velocità con cui può essere eseguito il codice Rust sia la velocità con cui Rust ti consente di scrivere programmi. I controlli del compilatore Rust garantiscono stabilità attraverso l'aggiunta di funzionalità e il refactoring. Ciò contrasta con il codice legacy fragile in linguaggi senza questi controlli, che gli sviluppatori spesso hanno paura di modificare. Sforzandosi per le astrazioni a costo zero, le funzionalità ad alto livello che compilano il codice a basso livello velocemente quanto il codice scritto manualmente, Rust si sforza di rendere il codice sicuro anche veloce.

Il linguaggio Rust spera di supportare molti altri utenti; quelli menzionati qui sono solo alcuni degli stakeholder più importanti. In generale, la più grande ambizione di Rust è quella di eliminare i compromessi che i programmatori hanno accettato per decenni fornendo sicurezza e produttività, velocità e ergonomia. Dai un'occhiata a Rust e vedi se le sue scelte funzionano per te.

## A chi è destinato questo libro

Questo libro assume che tu abbia scritto codice in un altro linguaggio di programmazione, ma non fa alcuna ipotesi su quale sia. Abbiamo cercato di rendere il materiale accessibile a un ampio pubblico di sviluppatori con diverse esperienze di programmazione. Non trattiamo a lungo di cosa sia la programmazione o di come pensarci. Se sei completamente nuovo alla programmazione, saresti meglio servito leggendo un libro che fornisce specificamente un'introduzione alla programmazione.

## Come utilizzare questo libro

In generale, questo libro assume che lo stiate leggendo in sequenza dall'inizio alla fine. I capitoli successivi si basano sui concetti dei capitoli precedenti, e i capitoli precedenti potrebbero non approfondire i dettagli su un argomento specifico, ma lo riprenderanno in un capitolo successivo.

Troverete due tipi di capitoli in questo libro: capitoli concettuali e capitoli di progetto. Nei capitoli concettuali, imparerete un aspetto di Rust. Nei capitoli di progetto, costruiremo insieme piccoli programmi, applicando ciò che avete imparato finora. I capitoli 2, 12 e 20 sono capitoli di progetto; il resto sono capitoli concettuali.

Il capitolo 1 spiega come installare Rust, come scrivere un programma “Hello, world!” e come utilizzare Cargo, il gestore delle dipendenze e lo strumento di compilazione di Rust. Il capitolo 2 è un'introduzione pratica alla scrittura di un programma in Rust, facendovi costruire un gioco in cui bisogna indovinare i numeri. Qui copriamo i concetti a un livello elevato e i capitoli successivi forniranno ulteriori dettagli. Se desiderate mettere le mani nella pasta subito, il capitolo 2 è il posto giusto per farlo. Il capitolo 3 copre le funzionalità di Rust simili a quelle di altri linguaggi di programmazione e nel capitolo 4 imparerete il sistema di proprietà di Rust. Se siete un apprenditore particolarmente meticoloso che preferisce imparare ogni dettaglio prima di passare al successivo, potreste voler saltare il capitolo 2 e andare direttamente al capitolo 3, tornando al capitolo 2 quando desiderate lavorare a un progetto applicando i dettagli appresi.

Il capitolo 5 discute le structs e i metodi, mentre il capitolo 6 copre gli enum, le espressioni `match` e la costruzione di un controllo di flusso con `if let`. Utilizzerete structs e enum per creare tipi personalizzati in Rust.

Nel capitolo 7, imparerete il sistema dei moduli di Rust e le regole di privacy per organizzare il vostro codice e la sua Application Programming Interface (API). Il capitolo 8 discute alcune strutture di dati comuni fornite dalla libreria standard, come vettori, stringhe e hashmap. Il capitolo 9 esplora la filosofia e le tecniche di gestione degli errori di Rust.

Il capitolo 10 scava nei generics, trait e durata, che vi danno il potere di definire codice che si applica a più tipi. Il capitolo 11 tratta solo il testing, che anche con le garanzie di sicurezza di Rust è necessario per garantire che la logica del vostro programma sia corretta. Nel capitolo 12, costruiremo la nostra implementazione di un sottoinsieme della funzionalità del comando da riga di comando grep che cerca testo all'interno dei file. Per fare ciò, utilizzeremo molti dei concetti discussi nei capitoli precedenti.

Il capitolo 13 esplora le chiusure e gli iteratori: funzionalità di Rust che provengono da linguaggi di programmazione funzionale. Nel capitolo 14, esamineremo in modo più approfondito Cargo e parleremo delle migliori pratiche per condividere le vostre librerie con gli altri. Il capitolo 15 discute i puntatori intelligenti forniti dalla libreria standard e i trait che abilitano la loro funzionalità.

Nel capitolo 16, esamineremo diversi modelli di programmazione concorrente e parleremo di come Rust vi aiuti a programmare in più thread senza paura. Il capitolo 17 esamina come gli idiomatismi di Rust si confrontano con i principi di programmazione orientata agli oggetti con cui potreste avere familiarità.

Il capitolo 18 è una guida sui pattern e il pattern matching, che sono modi potenti per esprimere idee in tutti i programmi Rust. Il capitolo 19 contiene una vasta gamma di argomenti avanzati, tra cui il Rust non sicuro, le macro e altre informazioni su vita, proprietà, tipi, funzioni e closures.

Nel capitolo 20, completeremo un progetto in cui implementeremo un server web multithreaded a basso livello!

Infine, alcuni appendici contengono informazioni utili sulla lingua in un formato più simile a una guida di riferimento. L'appendice A copre le parole chiave di Rust, l'appendice B copre gli operatori e i simboli di Rust, l'appendice C copre le proprietà derivabili forniti dalla libreria standard, l'appendice D copre alcuni strumenti di sviluppo utili e l'appendice E spiega le edizioni di Rust. Nell'appendice F, è possibile trovare traduzioni del libro e nell'appendice G copriremo come viene realizzato Rust e cosa è il Rust nightly.

Non c'è un modo sbagliato per leggere questo libro: se vuoi saltare avanti, fallo pure! Potresti dover tornare indietro ai capitoli precedenti se ti senti confuso. Ma fai quello che funziona per te.

<span id="ferris"></span>

Un importante parte del processo di apprendimento di Rust è imparare a leggere i messaggi di errore che il compilatore mostra: questi ti guideranno verso un codice funzionante. Di conseguenza, forniremo molti esempi che non compilano correttamente insieme al messaggio di errore che il compilatore mostrerà in ogni situazione. Sappi che se inserisci ed esegui un esempio a caso, potrebbe non compilare! Assicurati di leggere il testo circostante per vedere se l'esempio che stai cercando di eseguire è destinato a generare un errore. Ferris ti aiuterà anche a distinguere il codice che non è destinato a funzionare:

| Ferris                                                                                                           | Significato                                            |
|------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------|
| <img src="img/ferris/does_not_compile.svg" class="ferris-explain" alt="Ferris with a question mark"/>            | Questo codice non compila!                             |
| <img src="img/ferris/panics.svg" class="ferris-explain" alt="Ferris throwing up their hands"/>                   | Questo codice causa un panico!                         |
| <img src="img/ferris/not_desired_behavior.svg" class="ferris-explain" alt="Ferris with one claw up, shrugging"/> | Questo codice non produce il comportamento desiderato. | 

Nella maggior parte delle situazioni, ti guideremo verso la versione corretta di qualsiasi codice che non compili.

I file sorgenti da cui è stato generato questo libro si possono trovare su [GitHub][book].
