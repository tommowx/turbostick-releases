# TurboStick 0.9.5

## Avvio

Windows con .NET Framework 4.8. Estrai tutta la cartella e apri TurboStick.exe. Tieni la cartella su un disco o una chiavetta scrivibile. Non avviare direttamente dentro lo ZIP.
Start attiva il Pilota; Stop ripristina le modifiche. La X lascia il programma vicino all'orologio. Esci dal menu dell'icona ripristina e chiude. Il Tecnico offline e la pulizia file sono disponibili dalla Home.

## Protezione delle app

Nessuna chiusura automatica delle app. L'eventuale comando manuale Chiudi app richiede autorizzazione e conferma. I browser riconosciuti (Chrome, Edge, Firefox, Brave, Opera, Vivaldi e altri) sono esclusi dalle modifiche automatiche di priorità CPU e memoria, anche in background. La gestione della priorità memoria è disattivata per impostazione predefinita; rimane opzionale nelle preferenze. Il bilanciamento CPU degli altri processi idonei resta disponibile sotto carico sostenuto. Non è stato dimostrato che TurboStick abbia causato la chiusura segnalata di Chrome.

## Aggiornamenti

Al primo avvio scegli se attivare gli aggiornamenti automatici. Cambia scelta in Altri strumenti > Aggiornamenti. Non serve un account GitHub. Una volta al giorno, quando il desktop o TurboStick sono in primo piano e il PC è inattivo da due minuti, l'app cerca una nuova versione. Giochi riconosciuti, profili manuali e operazioni in corso rimandano l'aggiornamento. Puoi anche premere Controlla ora e Installa ora.

Solo pacchetti con firma RSA e hash verificati sono accettati. Prima della sostituzione vengono ripristinate le modifiche al PC. La nuova versione riparte in background e mantiene la pausa se era attiva. Impostazioni e quarantena rimangono nella cartella data. Se l'avvio fallisce, l'updater tenta di tornare alla versione precedente; non forza la chiusura di processi bloccati. In quest'ultimo caso conserva il backup e mostra un errore. Non eliminare .updates se segnala un recupero incompleto.

Offline il programma continua a funzionare. Gli aggiornamenti usano GitHub tramite HTTPS: GitHub riceve le normali informazioni di connessione, incluso l'IP. Non vengono inviati hardware, elenco processi o file personali. Gli aggiornamenti scaricano soltanto l'eseguibile; un futuro cambio di runtime/configurazione richiederà una migrazione dedicata.

La firma dei pacchetti è verificata dall'app: non è una firma Authenticode commerciale dell'eseguibile. Eventuali avvisi Windows vanno valutati senza disattivare le protezioni.

## Verifiche

469 controlli superati, test di interfaccia Start/Stop e X/tray, prova Windows di sostituzione dell'eseguibile e recupero con un programma di prova che fallisce all'avvio. Nessun miglioramento FPS o RAM promesso o misurato da questi test.

Release ufficiali: https://github.com/tommowx/turbostick-releases/releases

