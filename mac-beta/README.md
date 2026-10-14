# TurboStick 0.19.0 — Mac Beta

Questa è la prima beta per Mac Intel e Apple Silicon. Include diagnostica e il nuovo canale di aggiornamento Mac; il port completo delle ottimizzazioni Windows è ancora in sviluppo. Non sono dimostrati guadagni FPS su Mac.

## Avvio

1. Scarica il file osx-arm64 per un Mac con chip Apple (M1/M2/M3/M4 e successivi) oppure osx-x64 per Intel. Serve macOS 15 o successivo; .NET è incluso.
2. Estrai lo ZIP. Sposta TurboStick.app nella cartella Applicazioni del tuo utente, o in un'altra cartella scrivibile. Aprila dal Finder.
3. La beta non è firmata Developer ID né notarizzata. Se macOS la blocca, segui la procedura ufficiale in Impostazioni di Sistema > Privacy e sicurezza per un'app di uno sviluppatore non identificato, solo se riconosci questo download. Non disattivare Gatekeeper o l'antivirus. Guida Apple: https://support.apple.com/102445

## Funzioni disponibili

- Home con CPU, RAM totale e stima della memoria recuperabile.
- Uso CPU/RAM delle app tramite scansione manuale locale, rispettando i processi protetti da macOS.
- Diagnosi esplicita DNS, gateway e destinazione; timeline dei ping, jitter, P95, timeout e contatori di rete.
- Tiko offline basato sulle misure raccolte.
- Aggiornamenti automatici dal canale Mac Beta, con firma RSA e SHA-256 del pacchetto, scelta della stessa architettura e protezioni contro archivi non validi.
- Report JSON locale tramite il pulsante Salva report Mac.

## Aggiornamenti

Il controllo parte circa 15 secondi dopo l'apertura, poi ogni 24 ore mentre l'app rimane aperta. Puoi controllare subito dalla Home. Se arriva una beta più recente, viene scaricata e verificata; alla normale chiusura TurboStick la installa e la riapre. Non termina altri programmi. La copia precedente viene rimossa soltanto dopo la conferma che la nuova finestra si è aperta. In caso di avvio fallito tenta il ripristino; se la nuova app resta avviata ma non conferma l'apertura, conserva la copia precedente e il risultato della transazione per il recupero. Una cartella senza permessi di scrittura o un'app in App Translocation impedisce l'installazione.

Il canale è pubblicato in mac-beta/osx-arm64.json e mac-beta/osx-x64.json sul repository tommowx/turbostick-releases. Solo pacchetti firmati con la chiave del progetto possono essere accettati. Il controllo richiede Internet; diagnosi locale e Tiko restano utilizzabili offline. Impostazioni e file temporanei degli aggiornamenti sono in ~/Library/Application Support/TurboStick/MacBeta, fuori dal bundle sostituito.

## Prova sul Mac

Controlla l'apertura, le misure nella Home, la scansione delle app, Tiko, una misura rete e il pulsante aggiornamenti. Poi premi Salva report Mac: Finder mostrerà report-latest.json, da inviare al proprietario del progetto insieme agli eventuali messaggi di errore. Il report registra sistema, architettura, fonti e valori CPU/RAM, versione e data. Non registra nomi delle app, SSID o documenti e non viene inviato automaticamente al servizio privato dei report.

Il ciclo completo installazione/riavvio dell'updater, le API Mach e la UI devono ancora essere provati su un Mac reale. Compilazione, firme del canale, archivi e controlli automatici sono verificati da Windows: questo non costituisce una prova nativa macOS. Attualmente non sono portati ottimizzazione gaming automatica, sensori GPU/temperature, tweak e pulizia, avvio automatico/background o invio remoto dei report. Non cambiare impostazioni di sistema per cercare di abilitarli.
