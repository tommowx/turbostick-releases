# TurboStick 0.19.1 — interfaccia e chat Tiko

Aggiornamento dell'app Windows completa. La beta Mac 0.19.0 conserva il proprio canale separato.

## Modifiche

- Tiko diventa una sola chat: messaggi sopra, campo per scrivere sotto, Invia e Annulla nella stessa posizione. Invio manda, Maiusc+Invio va a capo.
- Risposte con indicatore a tre puntini durante l'analisi e una transizione minima di 750 ms. Nessuna richiesta a un modello online: resta il tecnico a regole locali.
- Problemi, annullamenti e controlli suggeriti compaiono nella conversazione. Le opzioni di diagnosi, salvataggio, ripresa, dati e spiegazioni rimangono raggiungibili dal menu.
- Conversazione visiva limitata a 16 messaggi; il contesto tecnico conserva fino a otto scambi. Testi lunghi vanno a capo e scorrono verticalmente.
- Un solo fondo nel campo di scrittura, bordo sottile uniforme e colori coerenti. Eliminati i riquadri separati di riepilogo, cronologia e controllo.
- Pulsanti con testo centrato, margini uniformi, focus da tastiera visibile, stati disabilitati e passaggio del mouse leggibili.
- Interruttori dei Tweaks completamente visibili: descrizione, costo e comando in righe a tutta larghezza. Le opzioni avanzate restano richiudibili.
- Home più compatta, titoli ridimensionati, grafico con colori leggibili. Ridotti i comandi visibili nella pagina delle app a un menu «Gestisci app».
- Tema condiviso anche per pulizia, recupero file, notifiche, avvio, controlli Windows, rete, fluidità, dati e aggiornamenti. Intestazioni degli elenchi uniformate.

## Verifiche

- 1.379 controlli del motore PASS.
- 342 verifiche UI PASS: chat, invio vuoto/doppio, attesa, annullamento, messaggi lunghi, contrasto e 14 finestre secondarie.
- Audit delle pagine a 1280×900 e 1000×740: nessun pulsante o interruttore ritagliato rispetto al proprio contenitore.
- Regressioni UI PASS: blocchi durante gaming, ripristino su backend simulato, X/background/riapertura, aggiornamenti e arresto della propria raccolta.
- Avvio Windows reale isolato PASS: rilevamento hardware, processi e tray, senza applicare ottimizzazioni personali.

## Limiti

Le anteprime della chat e l'audit usano dati di prova. La cattura della finestra con Computer Use sul PC ha avuto timeout: verificati i render prodotti dall'app e il suo avvio reale. Non testati nativamente tutti i DPI, temi di sistema, lettori di schermo o configurazioni dei clienti. I dialoghi nativi di Windows e la barra del titolo seguono Windows.

Questa versione migliora la presentazione; non aggiunge ottimizzazioni e non dimostra guadagni FPS. Nessuna modifica automatica alle app personali o ai consensi. Aggiornamenti Windows tramite il manifesto RSA originale e il pacchetto completo.
