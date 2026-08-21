# ✦ Editor di Copioni

**Editor di Copioni** è uno strumento gratuito, open source e completamente offline per scrivere, organizzare e stampare copioni teatrali. È pensato per compagnie amatoriali, scuole e cooperative teatrali che hanno bisogno di uno strumento pratico, senza account, senza cloud e senza costi.

Sviluppato da **Giampiero Santoro** per **Clan Destino**.

> 📖 Per la guida completa all'uso, vedi [`GUIDA.md`](./GUIDA.md).

---

## Perché questo progetto

La maggior parte degli editor di testo non è pensata per un copione: non gestisce bene i nomi dei personaggi, non separa didascalie e battute, non calcola quanto parla ciascun personaggio, non genera un PDF con l'impaginazione giusta. I software di sceneggiatura professionali, dall'altra parte, sono pensati per il cinema, sono a pagamento o richiedono un account online.

Editor di Copioni nasce per colmare questo spazio: **un solo file HTML**, senza installazione, che gira interamente nel browser e salva tutto in locale.

## Caratteristiche principali

**Scrittura**
- Struttura in atti, scene e blocchi (didascalie, battute, voci fuori scena)
- Riconoscimento automatico dei nomi dei personaggi mentre scrivi
- Importazione di testo incollato e di file `.fountain`
- Cerca e sostituisci nel testo del copione
- Annulla/ripeti (`Ctrl+Z` / `Ctrl+Y`)
- Salvataggio automatico nel browser, con possibilità di collegare un file locale o un servizio cloud

**Personaggi**
- Schede complete: ruolo drammaturgico, descrizione, età, aspetto fisico, costume, oggetti di scena, foto
- Diagramma delle relazioni tra personaggi (esportabile in SVG o PDF)
- Filtro "Personaggi in scena": mostra solo le battute dei personaggi selezionati

**Regia e prove**
- Modalità prova/lettura, con campi di sola lettura per non modificare il testo per errore
- Piano di scena: tabella che mostra in quali scene compare ogni personaggio
- Lettura ad alta voce (sintesi vocale) delle battute dei personaggi assenti, per le prove a organico ridotto
- Statistiche avanzate: tempo di lettura stimato per atto, bilanciamento delle battute tra personaggi, elenco aggregato di oggetti di scena e costumi

**Esportazione**
- PDF completo del copione, con copertina, indice, pagina "Personaggi" e numerazione pagine
- PDF "ridotto" per singolo personaggio (solo le sue battute, per le prove)
- Esportazione in `.txt` e `.fountain`
- Copia di lettura in HTML statico, di sola lettura, condivisibile col cast
- QR code opzionale in copertina, che rimanda a una versione digitale del copione online

**Personalizzazione**
- Quattro temi grafici selezionabili (incluso un tema scuro)
- Dimensione del testo regolabile
- Layout adattabile: mostra/nascondi intestazione, barra laterale, barra inferiore
- Ottimizzato anche per tablet e uso touch

**Progetto e versioni**
- Esportazione/importazione dell'intero progetto in `.json`
- Cronologia delle versioni salvate, con confronto (diff) tra una versione salvata e il copione attuale

## Come si usa

Non serve installare nulla:

1. Scarica il file `index.html` da questa repository (o clona la repository).
2. Aprilo con un doppio clic in un browser moderno (Chrome, Firefox, Safari, Edge).
3. Inizia a scrivere: il copione viene salvato automaticamente nel browser.

Se preferisci accedervi da qualsiasi dispositivo tramite un link, puoi pubblicare la repository con **GitHub Pages** (Impostazioni → Pages → seleziona il branch) e usare l'URL generato.

> ⚠️ Il salvataggio automatico è legato al browser e al dispositivo in uso. Per portare il lavoro su un altro computer, o per fare un backup sicuro, usa **"Salva progetto (.json)"** e conserva il file. Per un salvataggio ancora più solido, collega un file locale tramite **"📁 Collega un file sul mio computer"**.

## Requisiti tecnici

- Un browser moderno con supporto a JavaScript (nessuna estensione richiesta)
- Connessione internet solo per: caricare i caratteri Google Fonts, generare il QR code opzionale, ed esportare in PDF (le librerie sono caricate da CDN)
- Nessun server, nessun database, nessun account

## Struttura del progetto

Il progetto è deliberatamente un **singolo file HTML autonomo** (`index.html`), che contiene markup, stile e logica applicativa. Questa scelta è intenzionale: rende il progetto facile da scaricare, aprire, modificare e distribuire, anche per chi non ha esperienza di sviluppo web.

```
.
├── index.html      # l'intera applicazione
├── README.md        # questo file
└── GUIDA.md          # guida utente completa, in italiano
```

## Librerie di terze parti utilizzate

Caricate via CDN, nessuna installazione richiesta:

- [jsPDF](https://github.com/parallax/jsPDF) — generazione dei file PDF
- [qrcode.js](https://github.com/davidshimjs/qrcodejs) — generazione del QR code opzionale in copertina
- [Google Fonts](https://fonts.google.com/) — Playfair Display, Courier Prime, Inter, Space Grotesk

## Contribuire

Segnalazioni di bug, richieste di funzionalità e correzioni sono benvenute tramite le *Issue* e le *Pull Request* di questa repository.

## Licenza

Questo progetto è distribuito come software libero. Se intendi riutilizzarlo o adattarlo, cita l'autore originale.

## Crediti

Creato da **Giampiero Santoro** per **Clan Destino**.
