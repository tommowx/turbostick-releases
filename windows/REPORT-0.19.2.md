# TurboStick 0.19.2 — aggiornamenti e recupero più affidabili

Aggiornamento Windows del 15 ottobre 2026. Il canale Mac Beta 0.19.0 resta separato.

## Correzioni

- Conferme di avvio dell'aggiornamento pubblicate solo dopo il completamento della scrittura. Il vecchio updater non può più leggerle mentre il produttore le tiene aperte.
- Conferma durevole della nuova versione prima di eliminare il backup. Un errore di pulizia dopo un avvio verificato conserva la nuova app e rinvia la pulizia, senza avviare un ripristino improprio.
- Pulizia ritentata all'avvio successivo; controllo di firma, versione, hash e backup prima di rimuovere i file della transazione.
- Salvataggi XML con file temporanei unici, scrittura completata prima della sostituzione e letture coerenti durante la sostituzione. Limite di dimensione verificato anche in scrittura.
- Due registri di ripristino con la stessa revisione ma istruzioni diverse bloccano nuovi interventi: nessuna scelta arbitraria del registro.
- Preferenze corrotte, non valide, occupate o sostituite da una cartella aprono la modalità di recupero con automazioni sospese, conservando l'originale.
- Avvio dell'interfaccia consentito anche quando il marcatore di avvio è occupato: interventi automatici bloccati e problema visibile.
- Se non si possono salvare le preferenze, gli interruttori tornano al valore precedente e compare l'errore. Anche importazione profili e rimozione regole conservano il modello precedente se il salvataggio fallisce.

## Verifiche

- 1.424 controlli del motore superati, compresi salvataggi concorrenti, letture durante la sostituzione, errori di scrittura, registri discordanti e tre punti di interruzione della pulizia updater.
- 12 scenari nativi di aggiornamento e recupero, ripetuti sia con il worker attuale sia con il codice del vecchio client: aggiornamento riuscito, avvio fallito, eseguibile invalido, pacchetto alterato, destinazione occupata, pulizia bloccata, due passaggi locali, due interruzioni simili a un riavvio, pulizia interrotta e primo avvio del download. Verificata anche la conservazione della pausa scelta dall'utente.
- 32 verifiche dell'interfaccia sulle preferenze non salvabili; due avvii reali in recupero.
- 342 verifiche della chat e dei dialoghi. Regressioni di X/background/riapertura/uscita, blocchi durante gaming e contrasto del dialogo aggiornamenti superate; nessun comando tagliato sulle sei pagine controllate a 1280×900 e 1000×740.
- Avvio e osservazione reale con ottimizzazione in pausa; le misure descrivono il costo dell'app, non guadagni FPS. I test non chiudono app personali e usano copie e processi di prova per i guasti.

## Limiti e valutazione

Questa versione rafforza l'affidabilità; non aggiunge promesse di FPS o RAM liberata. Le prove native sono state eseguite sul PC di sviluppo. Mancano una campagna prolungata su diversi PC, prove fisiche di distacco USB/perdita di alimentazione e verifiche Mac native. La firma dei pacchetti è verificata dall'updater; non è una firma commerciale Authenticode.

Valutazione tecnica provvisoria dell'affidabilità: **da 7/10 a 8/10**. Un 10/10 non è ancora dimostrato dai test disponibili. Per avvicinarlo servono riscontri indipendenti su più configurazioni e nel tempo; non basta aumentare il numero di controlli.

## Uso e aggiornamento

Gli utenti con aggiornamenti automatici abilitati ricevono la versione dal canale Windows esistente; connessione, PC inattivo e controlli di recupero possono rinviarne l'installazione. «Controlla ora» cerca il manifesto; download e installazione restano soggetti ai controlli previsti.

Per un nuovo download, estrarre tutta la cartella del pacchetto Portable e aprire TurboStick.exe. Non cancellare manualmente `.updates` se viene segnalato un recupero incompleto. La copia precedente necessaria al recupero resta finché l'avvio è verificato e i file sono accessibili. Le altre copie vengono considerate dalla pulizia passiva solo se riconosciute e verificabili: non vengono cancellati file arbitrari.
