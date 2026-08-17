# Editor di Copioni — Clan Destino

Un editor per copioni teatrali che gira interamente nel browser: nessuna installazione, nessun account, nessun server. Un solo file HTML che scrive, formatta, esporta in PDF e gestisce personaggi e scene di un copione teatrale, pensato per l'uso quotidiano di una compagnia amatoriale.

di Giampiero Santoro — Clan Destino

## Cos'è

Il copione è organizzato in **atti → scene → blocchi** (battute, didascalie, voci fuori scena). Ogni personaggio ha una scheda con dati anagrafici, aspetto, costume, relazioni con gli altri personaggi e, se serve, una foto di riferimento. Tutto resta salvato nel browser, oppure — se il browser lo permette — direttamente in un file sul computer.

Non serve internet dopo il primo caricamento della pagina, a parte per il font e la libreria di generazione PDF (caricati da CDN).

## Funzionalità principali

- **Struttura**: atti e scene organizzati in un pannello dedicato, riordinabili, con stato di avanzamento (bozza/definitiva) e ambientazione per scena
- **Scrittura**: tre tipi di blocco (battuta, didascalia, voce fuori scena), tasto rapido sempre visibile che inserisce il nuovo blocco subito dopo il cursore, note per l'attore, didascalie aggiuntive dopo una battuta
- **Personaggi**: scheda completa con ruolo drammaturgico, età, aspetto fisico, costume, voce, obiettivo, conflitto, arco di trasformazione, retroscena, note di trucco/parrucco, nomignoli, attore assegnato, oggetti caratteristici, foto di riferimento, colore identificativo e relazioni con gli altri personaggi (con diagramma generato automaticamente)
- **Esportazione**: PDF completo con copertina, pagina personaggi e indice; PDF ridotto per singolo attore ("copione per personaggio"); .txt; .fountain; salvataggio dell'intero progetto in .json
- **Importazione**: incolla di un testo già scritto altrove, oppure import di un file .fountain (si aggiunge al copione esistente, senza sostituirlo)
- **Anteprima PDF**: statica su richiesta, oppure in tempo reale in un pannello affiancato al testo mentre si scrive
- **Strumenti di scrittura**: ricerca e sostituisci in tutto il copione, controllo qualità (personaggi mai usati, battute vuote, scene senza ambientazione, monologhi troppo lunghi), statistiche per atto (parole, minuti di lettura stimati), vista d'insieme dell'intera struttura
- **Cronologia**: annulla/ripeti con scorciatoie da tastiera, versioni salvate con nome a cui tornare in qualsiasi momento
- **Aspetto**: tema chiaro/scuro, dimensione del testo regolabile, modalità prova/lettura che evidenzia la battuta corrente, possibilità di nascondere intestazione/menù laterale/barra inferiore per avere più spazio di scrittura
- **Mobile**: su smartphone la struttura e i personaggi si aprono a schermo intero invece di occupare una striscia laterale

## Come usarlo

Basta aprire il file HTML in un browser (va bene anche solo con un doppio clic) oppure pubblicarlo online. Non serve altro.

Per la guida completa a tutte le funzioni, vedi **[guida.md](guida.md)**.

## Pubblicarlo su GitHub Pages

1. Carica il file `.html` in un repository GitHub (rinominalo `index.html` se vuoi che sia la pagina principale)
2. Vai in **Settings → Pages** del repository
3. In "Source" scegli il branch (di solito `main`) e la cartella `/root`
4. Salva: dopo un paio di minuti il sito sarà raggiungibile all'indirizzo indicato da GitHub

Da quel momento chiunque abbia il link può usare l'editor dal proprio browser, senza installare nulla.

## Salvataggio dei dati

- **Salvataggio automatico nel browser**: sempre attivo, scatta pochi istanti dopo ogni modifica
- **File locale reale** (facoltativo): su Chrome/Edge è possibile collegare un file sul proprio computer che si aggiorna a ogni modifica, per avere un backup vero; va ricollegato a ogni apertura della pagina, per motivi di sicurezza del browser
- **Esportazione manuale**: in qualsiasi momento si può scaricare una copia completa del progetto in `.json`, da reimportare in seguito

Nessun dato lascia il dispositivo dell'utente: non c'è un server che riceve o conserva i copioni.

## Compatibilità

Funziona su tutti i browser moderni (Chrome, Edge, Firefox, Safari). Il collegamento a un file locale reale richiede un browser basato su Chromium (Chrome, Edge, Opera); sugli altri browser resta comunque attivo il salvataggio automatico nel browser.

## Tecnologie

Un unico file HTML/CSS/JavaScript, senza framework né build. Per la generazione dei PDF viene usata la libreria [jsPDF](https://github.com/parallax/jsPDF), caricata da CDN.

## Crediti

Realizzato da **Giampiero Santoro** per **Clan Destino**.
