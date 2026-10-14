# TurboStick 0.19.0 — Mac Beta, 14 ottobre 2026

Release 413023903 pubblicata come pre-release alle 18:07:12 UTC:
https://github.com/tommowx/turbostick-releases/releases/tag/v0.19.0

## Modifiche
CPU e stima RAM Mach/sysctl; scansione CPU/RAM delle app, diagnostica DNS/gateway/destinazione con timeline e contatori; Tiko offline. Home Mac con controllo aggiornamenti e report locale.

Canale Mac Beta automatico: controllo a 15 secondi dall'apertura e ogni 24 ore, versione/architettura e firma RSA del progetto, verifica dimensione/SHA-256, URL GitHub/CDN consentiti, ZIP limitato con rifiuto di percorsi esterni, collegamenti e duplicati. Helper separato dopo normale chiusura, sostituzione tramite rinomina, conferma finestra nuova e rimozione copia precedente. Avvio fallito: tenta il ripristino; avvio senza conferma ma ancora in esecuzione: conserva backup senza terminare il processo. Cache delle transazioni completate rimossa al controllo successivo. Impostazioni e cache in Application Support dell'utente, fuori dal bundle.

## Verifiche effettuate da Windows
117 controlli PASS; desktop compilato senza avvisi/errori; sei RID compilati. I due archivi reali Intel e ARM verificati con la chiave editore embedded: firma metadata, dimensione, SHA-256 e layout del bundle. 454 file nei bundle confrontati tramite hash e CRC ZIP. Eseguibili nel ZIP con permessi 0755. Architettura e pagine delle code directory ad hoc dei quattro apphost verificate. Sorgenti distribuiti: 31 file confrontati; nessuna chiave privata inclusa. Tutti i sette asset caricati su GitHub con dimensioni e digest identici.

Apple Silicon: 44.580.092 byte, SHA-256 78acde91bdb09de7eeeaf3c8a5c4e59312181ab8b6ec1f9dc917640984af1ad4.
Intel: 46.799.172 byte, SHA-256 15592cee3138cc72236369732cbdf7042bab00bada74c79f508d057d9044a037.
Sorgenti: SHA-256 1ba22b8e4d83be7a844af99145e29da6cdc7af7379035a0e4e4c32b0b71ed6d9.

## Stato della prova Mac
L'utente richiede che il suo amico provi la beta dopo la pubblicazione. Nessuna esecuzione nativa Mac verificata finora: UI, API Mach e ciclo installazione/riavvio ancora da confermare. Nessuna firma Developer ID/notarizzazione; firma RSA del canale e ad hoc degli apphost sono cose distinte dalla certificazione Apple. macOS 15 o successivo; runtime incluso. Non portati gaming automatico, GPU/temperature, tweak/pulizia, login/background e invio cloud dei report. Nessun incremento FPS dimostrato.

Salva report Mac crea report-latest.json in ~/Library/Application Support/TurboStick/MacBeta e mostra il file nel Finder. È un report locale da inviare per la prova; non viene inviato automaticamente al servizio privato Windows.

Le future beta Mac devono aggiornare gli stessi percorsi mac-beta/osx-arm64.json e mac-beta/osx-x64.json, firmati con la chiave editore originale. La versione stabile Windows 0.18.1 mantiene il proprio canale.
