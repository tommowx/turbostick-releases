# TurboStick 0.19.4 — Tiko e AI locale

Aggiornamento Windows del 15 ottobre 2026. Il canale Mac Beta 0.19.0 resta separato.

## Funzioni implementate

- Collegamento opzionale a un modello già caricato nel server locale di LM Studio. Configurazione in Tiko → Altre opzioni → AI locale. Disattivato per impostazione iniziale; il tecnico a regole continua a funzionare senza modelli e offline.
- Cronologia limitata per le richieste AI, dati diagnostici di contesto e risposte brevi. La risposta del modello è distinta dai dati verificati; non esegue comandi né sceglie gli interventi dell'app.
- Solo connessione a 127.0.0.1, nessun download o caricamento automatico di modelli, nessun token incluso. Il server deve accettare richieste locali senza autenticazione. Per un uso completamente offline anche il modello/server deve essere locale.
- Richieste rinviate durante gaming, CPU almeno 85%, RAM almeno 90% o misure non recenti. Annullamento della richiesta se la situazione cambia; timeout totale di 30 secondi. L'annullamento HTTP non garantisce che il server esterno interrompa immediatamente il calcolo.
- Risposte assenti, non valide o non disponibili tornano al tecnico a regole. I testi generati restano interpretazioni non verificate.
- Letture facoltative di controller audio, schermo e batteria con raccolta limitata. Lo stato WMI di un controller non dimostra che il volume o il microfono funzionino.
- Migliore comprensione di RAM piena, domande sulla rete, sintomi audio e accensione. «Fatto» chiede l'esito; «non riesco» mantiene il passo invece di avanzare.
- Storico salvato distinto dalle misure attuali e contesto storico esplicito per il modello.
- Correzione del ciclo di rimozione dei vecchi messaggi della chat; pianificazione della diagnosi inclusa nella gestione degli errori.

## Verifiche e limiti

- Compilazione e 1.663 controlli automatici passati.
- 19 controlli dell'interfaccia AI, compreso HTTP reale verso un server locale di prova; 341 controlli chat/dialoghi e 41 controlli di conversazione passati. Dopo i risultati iniziali intermittenti sono passate 16 esecuzioni complete consecutive della build finale, di cui cinque con traccia conservata solo in memoria. Nessuna causa certa dei primi esiti attribuita al modello.
- Letture native audio/schermo/batteria riuscite su questo PC; disponibilità dipendente da hardware e driver.
- Sei schermate a due dimensioni: nessun pulsante fuori dal proprio contenitore.
- Nessuna prova di generazione con Bonsai effettuata: circa 8 GB RAM installata e meno di 1 GB libera al controllo. Il test HTTP usa risposte preparate, non misura l'intelligenza del modello.
- Nessun voto 10/10 dichiarato; qualità del modello, compatibilità e impatto vanno misurati in condizioni reali.
- La futura sezione Rete e Wi-Fi è registrata nella roadmap e non fa parte di questa versione.

## Riferimenti tecnici

- [LM Studio: compatibilità OpenAI](https://lmstudio.ai/docs/developer/openai-compat)
- [LM Studio: endpoint REST e stato dei modelli](https://lmstudio.ai/docs/developer/rest/endpoints)
- [Microsoft: Win32_SoundDevice](https://learn.microsoft.com/en-us/windows/win32/cimwin32prov/win32-sounddevice)


## Verifica del rilascio

- Pubblicata come Latest: v0.19.4, release 413802699, 15 ottobre 2026 ore 12:47:15 UTC.
- Tutti i cinque file pubblici riscaricati e confrontati per dimensione e SHA-256.
- Manifesto RSA e binario verificati anche dal trasporto Windows effettivo.
- La versione distribuita 0.19.3 riconosce 0.19.4 come aggiornamento firmato più recente.
- Sorgenti del pacchetto estratti, ricompilati e testati: 1663 controlli passati.
- Nessuna sostituzione manuale dell’installazione personale; resta il canale automatico secondo preferenze e condizioni di inattività.
