# TurboStick
### Un alleato dentro il tuo PC.

**La tua cabina per monitoraggio, prestazioni e diagnosi locale su Windows.**
Portatile, utilizzabile offline e con interventi ripristinabili.

[![Windows](https://img.shields.io/badge/Windows-10%20%2F%2011-0078D4)](https://github.com/tommowx/turbostick-releases/releases/latest)
[![Ultima versione](https://img.shields.io/github/v/release/tommowx/turbostick-releases?label=Versione&color=11998e)](https://github.com/tommowx/turbostick-releases/releases/latest)

## ↓ Scarica l'app

### [Scarica TurboStick Portable per Windows](https://github.com/tommowx/turbostick-releases/releases/latest/download/TurboStick-Portable.zip)

[Novità e report della versione](https://github.com/tommowx/turbostick-releases/releases/latest) · [Tutte le versioni](https://github.com/tommowx/turbostick-releases/releases)

**Scegli `TurboStick-Portable.zip`.** Il pulsante Code → Download ZIP e i file Source code contengono la pagina del repository, non l'app Windows.

1. Scarica il pacchetto ed estrai **tutta la cartella**.
2. Apri **TurboStick.exe** da un disco o una chiavetta scrivibile.
3. Il pilota parte secondo le preferenze e i controlli di recupero. Usa **Stop** per fermare il controllo e ripristinare gli interventi.

Windows 10/11 con **.NET Framework 4.8**. Non avviare dentro lo ZIP.

## Gaming, prove e ripristino · 0.17.0

Dodici controlli Windows facoltativi con ripristino, prove guidate della fluidità e memoria locale dei peggioramenti. Confronto DNS senza modifiche automatiche e prova QoS temporanea BETA con ripristino. Nessuna chiusura automatica delle app personali.

**1.209 controlli superati**, integrazione updater e prove native DNS/QoS. Nessun guadagno FPS dimostrato in partita: risultati e limiti sono nel [report completo](https://github.com/tommowx/turbostick-releases/releases/tag/v0.17.0).

[Sorgenti ricompilabili della 0.17.0](https://github.com/tommowx/turbostick-releases/releases/download/v0.17.0/TurboStick-Sources-0.17.0.zip).

**Report tecnici facoltativi:** dopo un consenso iniziale, invio automatico a PC inattivo e tentativo allo spegnimento con coda offline. Archivio privato Cloudflare, 30 giorni; solo aggregati e conteggi, senza nomi, file, processi, log, chat o fotogrammi. Anteprima e disattivazione in Altri strumenti → Aiutaci a migliorare. L'app funziona offline senza report.

| Cosa trovi | A cosa serve |
| --- | --- |
| **Una schermata semplice** | Stato del controllo e dati CPU, memoria e GPU, se disponibili. |
| **Tiko** | Mascotte leggera, disegnata localmente, che apre il tecnico offline. |
| **Controllo adattivo** | Osserva il carico; riduce le letture durante il gioco e ripristina gli interventi quando il controllo supera il budget. |
| **Cosa sto facendo** | Mostra gli interventi registrati, il ripristino e le misure con/senza interventi, senza dedurre guadagni FPS. |
| **Parla con Tiko** | Descrivi il problema: analisi locale e controlli guidati, senza modifiche automatiche. |
| **Libera spazio** | Analisi e selezione dei file, cache Windows/NVIDIA/AMD e archivio recuperabile. Pulizia bloccata con gioco riconosciuto. |

Tiko usa il tecnico a regole locale: non è un modello linguistico e non richiede download di modelli o abbonamenti AI.

## Rimane vicino a te, anche in background

- **X:** nasconde la finestra e lascia l'app operativa vicino all'orologio.
- **Stop:** mette in pausa e ripristina gli interventi.
- **Esci:** ripristina e chiude normalmente.

## Misure di fluidità · 0.15.1

Il risultato finale resta aggiornato quando la raccolta finisce. Stop ripristina gli interventi e attende conferma della chiusura della propria sessione; anche Esci attende senza forzare processi. La misura live controlla prima i permessi necessari e spiega gli errori; i CSV restano importabili senza privilegi aggiuntivi. Test reali di fine temporizzata e arresto ETW superati. Nessun guadagno FPS è stato misurato.

## Pulizia passiva vecchi download

A PC inattivo TurboStick sposta nel Cestino i propri ZIP ed EXE di versioni precedenti presenti in Download, dopo verifica di firma e hash. Protegge la copia in uso e conserva impostazioni, quarantena e altri file nelle cartelle. I file bloccati o non verificabili restano dove sono. Non richiede una pulizia manuale.

## Aggiornamenti automatici

La 0.14.1 corregge il caso in cui il nuovo EXE riapriva la copia vecchia: riconosce separatamente le versioni e individua prima quella effettivamente in esecuzione. Il collegamento **Scarica TurboStick Portable** punta sempre alla release Latest; i tag precedenti sono archivio storico.


In **Altri strumenti → Aggiornamenti** puoi abilitare il controllo automatico. Non serve un account GitHub.

Il controllo avviene ogni sei ore, con avanzamento e annullamento del download. Durante un gioco riconosciuto il trasferimento viene interrotto dal controllo periodico. Con connessione disponibile, l'app controlla periodicamente e installa a PC inattivo. Giochi riconosciuti e operazioni in corso rimandano l'installazione. Puoi anche usare **Controlla ora** e **Installa ora**.

Il pacchetto è accettato solo dopo verifica della firma RSA, della dimensione e dell'hash. Prima della sostituzione vengono ripristinati gli interventi; dati, quarantena e impostazioni vengono conservati. Se il nuovo avvio fallisce, l'updater tenta il ritorno alla copia precedente senza forzare la chiusura di applicazioni.

<details>
<summary><strong>Hai una vecchia versione o un errore SSL/TLS?</strong></summary>

Scarica il ZIP Portable completo, estrailo e apri il nuovo TurboStick.exe. Il manifesto firmato incluso consente l'aggiornamento locale della vecchia copia riconosciuta. La sostituzione avviene dopo la chiusura normale e la verifica dell'avvio. Il backup viene rimosso dopo un avvio riuscito; altri download e altre copie non vengono cancellati indiscriminatamente.

Se il programma segnala un recupero incompleto, conserva la cartella `.updates` e il backup.

</details>

## Protezione delle app e privacy

Nessuna chiusura automatica delle app. Il comando manuale **Chiudi app** richiede autorizzazione e conferma. I browser riconosciuti sono esclusi dalle modifiche automatiche di priorità CPU e memoria. La priorità memoria resta opzionale e disattivata per impostazione predefinita.

Monitoraggio, tecnico e pulizia lavorano sul computer. Gli aggiornamenti contattano GitHub via HTTPS, che riceve le normali informazioni di connessione, incluso l'IP; elenco processi e file personali non vengono inviati. I report tecnici opzionali inviano solo i dati aggregati descritti sopra dopo consenso.

<details>
<summary><strong>Verifiche e limiti</strong></summary>

La 0.16.0 ha superato **769 controlli**, una prova di avvio reale isolato, la verifica X/background/riapertura/ripristino e **11 scenari di aggiornamento firmato e recupero**. Verificati anche sei test del servizio report, trasporto reale .NET/TLS, accesso privato, prove guidate e conservazione delle registrazioni. Il report completo è allegato alla release.

Queste prove non misurano guadagni FPS e non coprono ogni combinazione di gioco e hardware. Le metriche GPU possono essere N/D. Nessuna promessa di memoria liberata o FPS aggiuntivi.

La firma dei pacchetti viene verificata dall'app; non è una firma Authenticode commerciale. Valuta gli eventuali avvisi Windows senza disattivare le protezioni. Questo repository distribuisce i pacchetti dell'app: gli archivi Source code di GitHub non contengono i sorgenti di TurboStick.

</details>




- Controlla ora cerca subito il manifesto firmato anche con gioco/operazioni in corso, senza scaricare l'EXE. Download e installazione restano separati e rinviati a un momento sicuro. Verifica reale del manifesto GitHub durante gaming/pulizia simulati PASS; trasferimenti automatici ancora annullati durante gaming.


