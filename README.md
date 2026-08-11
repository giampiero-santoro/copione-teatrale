# 🎭 Copione — Editor per il teatro

Un editor di copioni teatrali completo, gratuito e **offline-first**, racchiuso in un unico file HTML. Nessuna installazione, nessun account, nessun server: apri il file nel browser e inizia a scrivere.

Pensato per drammaturghi, compagnie amatoriali e professionisti che vogliono un ambiente dedicato alla scrittura scenica, con formattazione automatica secondo le convenzioni del teatro (nomi personaggi in maiuscolo, slug line, didascalie, voci fuori scena) ed export pronti per prove e stampa.

> Ispirato all'esperienza di software come Final Draft o Fountain, ma pensato appositamente per il **teatro** (non per la sceneggiatura cinematografica) e disponibile in italiano, senza costi né limiti d'uso.

---

## ✨ Funzionalità principali

- **Struttura in atti e scene**, con riordino e stato di avanzamento per ogni scena (bozza / da rivedere / definitiva).
- **Blocchi di testo dedicati**: battute di dialogo, didascalie di regia, voci fuori scena, note a margine, indicazioni post-didascalia.
- **Scheda personaggi** completa: ruolo, età, aspetto fisico, costume, descrizione, backstory e relazioni fra personaggi, con **diagramma delle relazioni** generato automaticamente (SVG).
- **Modalità prova/lettura** 🎭 per leggere il copione senza le interfacce di editing.
- **Copione per personaggio ("sides")**: genera un PDF con le sole battute (e relative cue) di un singolo attore.
- **Controllo qualità** automatico: incoerenze di presenza in scena, personaggi senza battute, scene vuote, ecc.
- **Statistiche avanzate**: bilanciamento delle parole per personaggio, tempo di lettura stimato per atto, numero di battute.
- **Vista d'insieme (outline)** di tutte le scene con anteprima del contenuto.
- **Ricerca e sostituzione** nel testo, con opzione case-sensitive.
- **Importazione di testo già scritto**, con riconoscimento automatico di personaggi e didascalie.
- **Cronologia versioni**: salva snapshot del copione e ripristinali in qualsiasi momento.
- **Esportazioni multiple**:
  - PDF completo del copione (con pagina del titolo, cast e numerazione), con anteprima e impostazioni personalizzabili
  - PDF "sides" per singolo personaggio
  - `.txt` semplice
  - [`.fountain`](https://fountain.io/) (formato standard aperto per sceneggiature)
  - Progetto completo in `.json` (per backup o trasferimento su un altro computer)
- **Salvataggio automatico locale** (IndexedDB/File System Access API, a seconda del browser), con possibilità di scegliere un file locale su disco da tenere sincronizzato.
- **Tema chiaro (velluto & oro)** e **tema scuro**, entrambi pensati per lunghe sessioni di scrittura.
- **Layout adattivo** per desktop, tablet e smartphone, con menù laterale e intestazione richiudibili per massimizzare lo spazio di scrittura.
- **Gestione del copyright**: riga di copyright personalizzabile inclusa negli export.

## 📦 Come si usa

Non serve build, non servono dipendenze da installare: è un singolo file HTML autosufficiente.

1. Scarica il file [`copione-teatrale.html`](./copione-teatrale.html).
2. Aprilo con un doppio click in un browser moderno (Chrome, Edge o Firefox aggiornati).
3. Inizia a scrivere: il copione viene salvato automaticamente nel browser.

Per l'uso più avanzato (scelta di un file locale su disco, guida completa, scorciatoie da tastiera) consulta la **[Guida utente](./GUIDA.md)**.

### Pubblicarlo online (opzionale)

Il file può essere servito da qualsiasi hosting statico, incluso **GitHub Pages**:

1. Fai il push del file `copione-teatrale.html` (rinominalo eventualmente in `index.html`) su un repository GitHub.
2. Vai in **Settings → Pages** del repository e abilita la pubblicazione dal branch principale.
3. L'editor sarà raggiungibile all'indirizzo `https://<utente>.github.io/<repository>/`.

> Nota: essendo un'app che gira interamente nel browser dell'utente, i copioni **non vengono mai inviati a un server**: restano sul dispositivo di chi scrive.

## 🧱 Tecnologie

- HTML, CSS e JavaScript "vanilla" (nessun framework, nessuna build).
- [jsPDF](https://github.com/parallax/jsPDF) (via CDN) per la generazione dei PDF.
- Google Fonts: *Playfair Display*, *Courier Prime*, *Inter*.
- API del browser: `IndexedDB` / `localStorage` e, dove disponibile, *File System Access API* per il salvataggio su file locale.

## 🌐 Compatibilità

Funziona su tutti i browser moderni basati su Chromium (Chrome, Edge, Opera) e su Firefox. Alcune funzioni avanzate di salvataggio su file locale richiedono un browser con supporto alla *File System Access API* (Chrome/Edge desktop); negli altri browser il salvataggio automatico avviene comunque tramite lo storage del browser.

## 🤝 Contribuire

Le segnalazioni di bug e i suggerimenti sono benvenuti tramite le *Issues* del repository. Trattandosi di un progetto in un unico file, le modifiche via Pull Request sono semplici da proporre: basta modificare `copione-teatrale.html` e descrivere il cambiamento.

## 📄 Licenza

Aggiungi qui la licenza scelta per il progetto (ad es. MIT) prima della pubblicazione.

---

Per la guida completa a tutte le funzioni, vedi **[GUIDA.md](./GUIDA.md)**.
