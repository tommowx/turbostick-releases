# TurboStick 0.19.3 — Tiko ti guida un passo alla volta

Aggiornamento Windows del 15 ottobre 2026. Il canale Mac Beta 0.19.0 resta separato.

## Cosa cambia

- Nuovo percorso di conversazione locale: Tiko chiede un chiarimento, conserva il problema e sceglie un controllo in base alla risposta.
- Nove argomenti: lentezza/gaming, rete e ping, rumore/calore, audio, accensione, schermo, batteria, spazio e memoria. Le varianti distinguono, fra l'altro, un browser da tutta la rete, ping da FPS, attesa prima/dopo il desktop, microfono da uscita audio e disco pieno da attività al 100%.
- «Non risolto» avanza una sola volta; «non capisco» spiega senza avanzare; un peggioramento propone di fermare e ripristinare l'intervento prima di altri tentativi. Non viene applicata alcuna modifica dalla risposta.
- A fine percorso Tiko smette di ripetere la lista e spiega quali informazioni conservare per l'assistenza. Un nuovo sintomo apre un percorso diverso; «non so» permette un controllo generale.
- «Risolto» è registrato come riscontro dell'utente, non come verifica automatica. Negazioni e risposte incerte non diventano successi. Le frasi supportate restano un vocabolario limitato.
- Dati recenti e dati mancanti distinti: CPU/RAM non valide, future o più vecchie di 30 secondi non vengono presentate come misure attuali. Configurazioni di rete incomplete non diventano schede mancanti. Se c'è carico alto, i dettagli possono mostrare fino a tre app con misure valide, senza chiuderle.
- Le domande di chiarimento non enumerano rete e dischi. Le richieste esplicite di misure FPS e stato interventi conservano l'uso dei dati già disponibili; la diagnosi che richiede letture resta bloccata durante un gioco riconosciuto.
- Analisi annullate non fanno avanzare il percorso e conservano il messaggio per riprovare. I messaggi rifiutati durante gaming compaiono come uno scambio distinto senza sovrascrivere la risposta precedente.

## Interfaccia e correzioni

- Una risposta con un controllo alla volta, dati essenziali e indicazione di come rispondere. Rimangono al massimo due comandi nella riga delle azioni; dati, salvataggio, ripresa e scheda PC sono nel menu.
- Corretto il ridimensionamento della riga dei comandi: i pulsanti devono avere spazio visibile, oltre a essere abilitati. Campo di scrittura in basso e indicatore di analisi conservati.
- La domanda salvata non viene più persa quando il campo viene svuotato e conserva il contesto dell'argomento.
- Una diagnosi ripresa viene aggiunta alla chat come storica, con domanda e data; non riattiva il controllo suggerito della conversazione precedente né presume che il vecchio percorso descriva il PC attuale.
- Gli errori di salvataggio o ripresa dal menu vengono mostrati, senza lasciare un'eccezione non gestita.
- Allineati gli elenchi dei sorgenti dei progetti C# al layout di compilazione corrente.

## Verifiche

- **1.627 controlli del motore superati**, inclusi **203 nuovi controlli** della conversazione, dei percorsi, delle negazioni, degli esiti, dei dati vecchi/non validi e delle richieste arbitrarie.
- **41 verifiche della conversazione nell'interfaccia**, con il normale ciclo eventi Windows e controllo degli accessi fra thread: domanda, risposta specifica, annullamento/riprova, spiegazione, peggioramento, fine percorso, risoluzione, cambio argomento, ripresa storica e blocco durante gaming.
- Regressioni di chat, dialoghi, contrasto, impaginazione, X/background/riapertura/uscita e protezioni durante gaming controllate sulla build finale. I test usano copie, dati e processi propri; non chiudono app personali.
- Prima della distribuzione: ricompilazione dei sorgenti estratti dal pacchetto, verifica del manifesto firmato e dei file pubblicati.

## Valutazione onesta e limiti

**Tiko e diagnosi: da 5/10 a 7/10 provvisorio. Il traguardo 10/10 non è raggiunto.** Il nuovo percorso è più utile e verificabile, ma resta un tecnico a regole, non un modello linguistico generalista. Non comprende ogni formulazione libera, non misura tutti i dispositivi e non verifica da solo che un problema sia risolto. Mancano prove di comprensione con utenti indipendenti e una casistica ampia su più PC; il numero di test non sostituisce queste prove.

Non vengono promessi guadagni FPS, eliminazione universale del lag o riparazioni automatiche. Non sono stati aggiunti modelli da scaricare, abbonamenti o invio della chat a servizi online. Tiko continua a funzionare offline.

## Download e aggiornamento

Gli aggiornamenti automatici Windows conservano preferenze e controlli della 0.19.2. Con connessione disponibile e aggiornamenti abilitati, la nuova versione viene proposta/installata secondo le condizioni previste, a PC inattivo. Per il primo avvio estrai tutta la cartella Portable e apri TurboStick.exe.
