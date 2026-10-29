# TurboStick 0.19.5 — Tweaks gaming, griglia compatta e memoria sotto pressione

Windows · 29 ottobre 2026. Il canale Mac Beta resta separato alla 0.19.0.

## Novità

- Nuova schermata Tweaks: griglia scura con accenti viola, schede allineate, interruttori compatti e testo leggibile. Da due a quattro colonne in base allo spazio. Tag BETA conservato.
- Undici controlli reali, con condizioni e compromessi descritti. Acceso indica una preferenza salvata, non una modifica sempre attiva né un incremento FPS misurato.
- Profilo gaming prudente: attiva priorità dinamica, contenimento dello sfondo e protezione voce/audio. Disattiva gli interventi avanzati e la nuova gestione memoria; conserva la scelta Silenziosa. Aggiorna gli interruttori e recupera la configurazione precedente se il salvataggio fallisce.
- Accesso diretto al confronto guidato della fluidità. Si confronta la stessa scena mantenendo costanti risoluzione e impostazioni; non dedurre causalità da un picco FPS.
- Nuovo controllo **Memoria allo sfondo sotto pressione**, inizialmente spento: nel percorso gaming autorizzato dai controlli di carico, con RAM almeno all'85%, interviene su massimo due app da almeno 512 MB scelte esplicitamente come Sfondo. Ricontrolla la memoria del processo prima dell'intervento. Browser, voce/streaming, app in primo piano e loro processi con lo stesso percorso, giochi, app protette e configurazioni avanzate esplicite sono esclusi.
- Per quelle app riduce la priorità memoria da Normale a Media tramite l'API Windows. Non libera forzatamente il working set, non svuota standby/cache e non termina processi. Una priorità già personalizzata resta invariata.
- Ripristino quando cambia il contesto, torni all'app o la RAM scende sotto l'80%; la fascia 80–84% mantiene solo interventi già applicati. Stop/Esci e recupero dopo riapertura usano il registro esistente. Può rallentare le app designate: non è un beneficio garantito.
- Sei schede aprono i controlli: grafica/HAGS, rete/QoS, Windows/input, scelta app Sfondo, avvio e pulizia.
- Pannello grafica con GPU già rilevate, limiti di compatibilità HAGS, ottimizzazioni in finestra e latenza nel gioco. Apre la pagina ufficiale Grafica Windows su scelta dell'utente; non applica preset driver NVIDIA/AMD o HAGS tramite registro.

## Incluso il lavoro Silenziosa, precedentemente non pubblicato

Apri **Tweaks → Silenziosa fuori dai giochi**. È inizialmente spenta: attivarla è una scelta, perché può ridurre le prestazioni fuori dai giochi.

Quando l'automazione è attiva e non è riconosciuto un gioco, TurboStick sostituisce il piano standard **Prestazioni elevate** con **Bilanciato**, se presente. Conserva i piani personalizzati, Risparmio e Bilanciato già in uso. Non crea piani e non cambia i loro parametri.

Prima di entrare nella sessione gaming ripristina il piano precedente; i controlli gaming scelti continuano a seguire le proprie condizioni. Anche **Ferma TurboStick** ed **Esci** ripristinano. La X mantiene l'app in background. Una preferenza attiva riprende quando l'automazione torna all'uso quotidiano.

## Affidabilità e chiarezza

- Registro di ripristino scritto prima di cambiare il piano; recuperabile alla riapertura.
- Verifica del piano dopo l'applicazione. Se il cambio non è confermato, resta il registro per il recupero.
- Ripristino energetico verificato rileggendo il piano: se Windows ignora la richiesta, il registro non viene eliminato come se fosse riuscita. La correzione riguarda anche il normale ripristino energetico.
- Un piano cambiato esternamente viene conservato; TurboStick sospende ulteriori cambi energetici nella stessa apertura.
- La Home distingue la scelta pronta, il cambio registrato, la pausa e la sospensione durante gaming. Un solo intervento energetico non è descritto come modifica delle priorità dei processi.
- Tiko spiega quando l'opzione può essere provata e quando non cambia nulla. Pulsanti e interruttore seguono lo stile della sezione Tweaks.
- Opzione salvata nei profili; i vecchi profili senza il nuovo campo rimangono inizialmente disattivati.

## Limiti

Non controlla le ventole, non legge dB o temperature, non limita gli FPS e non modifica tensioni, BIOS, driver o sicurezza. Nessun guadagno FPS o riduzione del rumore è stato misurato. Se il rumore è meccanico, oppure il PC usa già Bilanciato, questa funzione può non cambiarlo. Il firmware e i parametri già presenti nel piano determinano il comportamento effettivo.


## Verifiche e limiti

- 1.724 controlli motore passati, inclusi selezione, esclusioni, pressione RAM, dati mancanti, errori e ripristino. Priorità memoria realmente cambiata e ripristinata su un processo di test temporaneo; le condizioni di pressione/ammissibilità sono simulate per evitare carico artificiale sul PC.
- 273 controlli della nuova interfaccia: mappatura degli undici interruttori, salvataggio, profilo e rollback, testo e pulsanti a tre dimensioni, finestra grafica reale ispezionata senza cambiare Windows.
- 17 controlli UI Silenziosa; 341 controlli chat/dialoghi; test background/gaming e ripristino passati. Sei pagine a due dimensioni: zero pulsanti tagliati.
- Nessun confronto in un gioco reale eseguito in questa sessione; nessun aumento FPS, riduzione dei tempi dei fotogrammi, ping, rumore o temperature dimostrato. Non promettiamo 1.000 FPS o superiorità rispetto all'app nella fotografia.
- I nomi generici Kernel Tweaks, Optimize GPU o Power Tweaks nella foto non documentano le operazioni sottostanti: non sono stati copiati come interruttori fittizi. Nessuna disattivazione di sicurezza, servizi critici o timer di sistema.
- Firma, canale automatico, download pubblico e sorgenti ricompilati vengono verificati prima del completamento del rilascio.

## Fonti tecniche

[Microsoft: priorità memoria](https://learn.microsoft.com/en-us/windows/win32/api/processthreadsapi/ns-processthreadsapi-memory_priority_information) · [Microsoft: SetProcessInformation](https://learn.microsoft.com/en-us/windows/win32/api/processthreadsapi/nf-processthreadsapi-setprocessinformation) · [Microsoft: ottimizzazioni giochi in finestra](https://support.microsoft.com/en-au/windows/hardware/display-graphics/optimizations-for-windowed-games-in-windows-11) · [Microsoft: collegamenti Impostazioni](https://learn.microsoft.com/en-us/windows/apps/develop/launch/launch-settings) · [Epic: Reflex in Fortnite](https://www.fortnite.com/news/a-new-light-fortnite-pc-now-supports-ray-tracing)


## Verifica pubblicazione

Release 427837960 pubblicata come Latest il 2026-10-29T12:28:55Z. Cinque download pubblici verificati per SHA-256/dimensione; firma RSA verificata dal trasporto Windows effettivo. Il client 0.19.4 distribuito accetta il manifesto 0.19.5 come più recente. Download Portable Latest confermato. Sorgenti ZIP estratti e ricompilati: 1724 controlli passati. Installazione personale lasciata al canale automatico; nessun file dati del cliente incluso nei pacchetti.
