# TurboStick

## [↓ Scarica TurboStick](https://tommowx.github.io/turbostick-releases/)

Un solo punto di download: la pagina riconosce Windows o Mac e propone un solo pacchetto. Su Mac scegli il processore indicato in «Informazioni su questo Mac».

**Windows:** stabile 0.19.3. **Mac:** beta 0.19.0 di diagnostica, con aggiornamenti separati e ottimizzazioni complete ancora in sviluppo. Non sono ancora la stessa versione funzionale.

I file delle release sono disponibili per gli aggiornamenti automatici. Le versioni precedenti restano nell’archivio per compatibilità; per scaricare usa sempre il pulsante qui sopra.

## Tiko ti guida un passo alla volta · 0.19.3

Domande di chiarimento, percorsi per nove argomenti, un controllo alla volta e contesto conservato. Migliorati annullamento, negazioni, dati recenti, salvataggio e ripresa storica. **1.627 controlli del motore**, 41 verifiche della conversazione nella UI e regressioni superate. Resta un tecnico offline a regole: comprensione e sensori limitati, nessun 10/10 o guadagno FPS dichiarato.

[Report e verifiche](windows/REPORT-0.19.3.md) · [Release](https://github.com/tommowx/turbostick-releases/releases/tag/v0.19.3)

## Aggiornamenti e recupero più affidabili · 0.19.2

Conferme di avvio atomiche, pulizia del backup rinviata senza annullare un aggiornamento riuscito, salvataggi concorrenti e recupero delle preferenze. **1.424 controlli**, prove native anche con il vecchio updater e sorgenti ricompilati. Verifiche sul PC di sviluppo: affidabilità rafforzata, nessun 10/10 universale o guadagno FPS dichiarato.

[Report e verifiche](windows/REPORT-0.19.2.md) · [Release](https://github.com/tommowx/turbostick-releases/releases/tag/v0.19.2)

## Nuova interfaccia e chat Tiko · 0.19.1

Una sola conversazione, scrittura in basso e indicatore di analisi. Pulsanti centrati, Tweaks in righe leggibili, colori e finestre uniformati.

[Report e verifiche](windows/REPORT-0.19.1.md) · [Release](https://github.com/tommowx/turbostick-releases/releases/tag/v0.19.1)

<details>
<summary>Istruzioni, funzionalità e report</summary>

# TurboStick
### Un alleato dentro il tuo PC.

**La tua cabina per monitoraggio, prestazioni e diagnosi locale su Windows.**
Portatile, utilizzabile offline e con interventi ripristinabili.

[![Windows](https://img.shields.io/badge/Windows-10%20%2F%2011-0078D4)](https://github.com/tommowx/turbostick-releases/releases/latest)
[![Ultima versione](https://img.shields.io/github/v/release/tommowx/turbostick-releases?label=Versione&color=11998e)](https://github.com/tommowx/turbostick-releases/releases/latest)

## Mac Beta · 0.19.0

La prima beta per Mac è disponibile per la prova su **macOS 15 o successivo**, con runtime incluso.

**Scarica l'app:** [Apple Silicon — M1/M2/M3/M4 e successivi](https://github.com/tommowx/turbostick-releases/releases/download/v0.19.0/TurboStick-0.19.0-osx-arm64.zip) · [Mac Intel](https://github.com/tommowx/turbostick-releases/releases/download/v0.19.0/TurboStick-0.19.0-osx-x64.zip)

Estrai lo ZIP e sposta TurboStick.app in una cartella scrivibile. La beta include CPU/RAM, scansione delle app, diagnostica rete, Tiko offline e **il proprio canale di aggiornamento automatico**: controllo all'apertura e giornaliero, pacchetti firmati, installazione alla chiusura con conferma di apertura della nuova app. Dalla Home puoi salvare il report locale per la prova.

**È una beta di diagnostica:** il port delle ottimizzazioni gaming complete è ancora in sviluppo; UI/API Mach e installazione degli aggiornamenti devono essere verificati sul Mac. Firma Apple Developer ID e notarizzazione non sono presenti, quindi macOS può chiedere l'autorizzazione al primo avvio. Il report Mac non viene inviato automaticamente al servizio privato Windows.

[Release e modifiche](https://github.com/tommowx/turbostick-releases/releases/tag/v0.19.0) · [Istruzioni Mac](mac-beta/README.md) · [Report di verifica](mac-beta/REPORT.md) · [Sorgenti completi Mac Beta](https://github.com/tommowx/turbostick-releases/releases/download/v0.19.0/TurboStick-0.19.0-MacBeta-source.zip)

## Avvio leggero e Home gaming · 0.18.1

Nelle prime fasi di boot/accesso TurboStick riduce le proprie scansioni e rinvia le attività automatiche non urgenti. Nomi più chiari per le app all'avvio e ultimo tempo Windows quando leggibile. La Home usa le misure recenti dei fotogrammi già raccolti, con controlli di identità e freschezza condivisi con Tiko.

**1.379 controlli superati**, sorgenti ricompilati e avvio reale verificato. Nessun tempo risparmiato all'accensione o incremento FPS garantito: mancano riavvii comparativi e prove durante partita. Non vengono disattivati servizi, sicurezza o app personali automaticamente.

[Report 0.18.1](https://github.com/tommowx/turbostick-releases/releases/tag/v0.18.1) · [Sorgenti 0.18.1](https://github.com/tommowx/turbostick-releases/releases/download/v0.18.1/TurboStick-Sources-0.18.1.zip)

## Gaming più leggero · 0.18.0

Scansione dei processi alleggerita, ripristino completo delle misure gaming, driver GPU nel contesto delle prove e protezioni aggiuntive per cattura e overlay. Corretto l'aggiornamento scaricato quando la conferma del worker è temporaneamente occupata. **1.356 controlli superati**, sorgenti ricompilati e avvio reale verificato.

Sul PC di sviluppo, CPU propria media nelle osservazioni nascoste: **3,53% → 0,58%**. Otto scansioni: circa **21–23 → 1,52 secondi CPU**. Sono costi di TurboStick, non guadagni FPS; condizioni e limiti nel report. Il piano gaming esteso resta aperto.

[Report 0.18.0](https://github.com/tommowx/turbostick-releases/releases/tag/v0.18.0) · [Sorgenti 0.18.0](https://github.com/tommowx/turbostick-releases/releases/download/v0.18.0/TurboStick-Sources-0.18.0.zip)

## Misure gaming affidabili · 0.17.3

Peggior 1%, P95/P99 e tempo degli scatti; Tiko usa misure fresche senza scansioni aggiuntive. Contenimento gaming limitato nel tempo. CSV CPU/GPU con copertura esplicita e confronti ripetuti con variabilità e condizioni registrate. **1.337 controlli superati**, prove native ripetute e sorgenti ricompilati. Nessun incremento FPS in partita dimostrato; il piano completo 0.18 resta in sviluppo.

[Report 0.17.3](https://github.com/tommowx/turbostick-releases/releases/tag/v0.17.3) · [Sorgenti 0.17.3](https://github.com/tommowx/turbostick-releases/releases/download/v0.17.3/TurboStick-Sources-0.17.3.zip)

## Bilanciamento CPU adattivo · 0.17.2

Soglie adattate ai core disponibili, interventi quotidiani limitati nel tempo e ripristino dell'app in uso. Corretto lo stato delle sessioni automatiche e il conteggio del piano energetico. **1.247 controlli superati**, prove native ripetute e confronto sintetico alternato su un core: redistribuzione del tempo CPU verificata; nessun guadagno FPS in partita dichiarato.

[Report della 0.17.2](https://github.com/tommowx/turbostick-releases/releases/tag/v0.17.2) · [Sorgenti della 0.17.2](https://github.com/tommowx/turbostick-releases/releases/download/v0.17.2/TurboStick-Sources-0.17.2.zip)

## Interfaccia più chiara · 0.17.1

Home con una sola azione principale, Tiko con un solo menu di opzioni e Libera spazio con comandi mostrati quando servono. I dodici controlli Windows sono visibili nei Tweaks, con spiegazioni semplici e un solo pulsante per aprire la scelta. Le sei opzioni avanzate restano richiudibili.

[Report della 0.17.1](https://github.com/tommowx/turbostick-releases/releases/tag/v0.17.1) · [Sorgenti della 0.17.1](https://github.com/tommowx/turbostick-releases/releases/download/v0.17.1/TurboStick-Sources-0.17.1.zip)

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





</details>
