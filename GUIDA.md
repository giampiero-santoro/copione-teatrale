# Guida a Editor di Copioni

Guida pratica all'uso di **Editor di Copioni**. Se cerchi informazioni generali sul progetto, vedi [`README.md`](./README.md).

## Indice

1. [Primo avvio](#1-primo-avvio)
2. [Creare un nuovo copione](#2-creare-un-nuovo-copione)
3. [Struttura: atti, scene e blocchi](#3-struttura-atti-scene-e-blocchi)
4. [Personaggi](#4-personaggi)
5. [Diagramma delle relazioni](#5-diagramma-delle-relazioni)
6. [Personaggi in scena e lettura mirata](#6-personaggi-in-scena-e-lettura-mirata)
7. [Modalità prova e sintesi vocale](#7-modalità-prova-e-sintesi-vocale)
8. [Statistiche e piano di scena](#8-statistiche-e-piano-di-scena)
9. [Esportazione: PDF, testo, fountain, lettura HTML](#9-esportazione-pdf-testo-fountain-lettura-html)
10. [QR code in copertina](#10-qr-code-in-copertina)
11. [Salvataggio e dove va a finire il tuo lavoro](#11-salvataggio-e-dove-va-a-finire-il-tuo-lavoro)
12. [Progetto: esportazione, importazione, versioni](#12-progetto-esportazione-importazione-versioni)
13. [Aspetto: temi grafici e layout](#13-aspetto-temi-grafici-e-layout)
14. [Scorciatoie da tastiera](#14-scorciatoie-da-tastiera)
15. [Domande frequenti](#15-domande-frequenti)

---

## 1. Primo avvio

Apri `index.html` in un browser. Non serve creare un account: l'app parte già pronta all'uso, con un piccolo copione di esempio la prima volta che la apri, così puoi farti un'idea della struttura prima di iniziare il tuo.

L'interfaccia è divisa in tre zone:

- **Barra laterale** (sinistra): due schede, *Struttura* (atti e scene) e *Personaggi*.
- **Area centrale**: la scena attualmente aperta, mostrata come una pagina di copione.
- **Barra in alto**: titolo del copione, pulsanti di esportazione e impostazioni.

## 2. Creare un nuovo copione

Per iniziare un lavoro completamente nuovo, usa **"🆕 Nuovo copione"**. Ti verrà chiesta conferma, perché questa azione sostituisce quello attualmente aperto nella pagina.

Il nuovo copione parte **vuoto**: nessun personaggio, nessun atto già presente. Dovrai creare tu il primo atto (pulsante **"+ Nuovo atto"** nella barra laterale) e la prima scena.

> 💡 Se vuoi conservare il lavoro attuale prima di iniziarne uno nuovo, usa prima **"Salva progetto (.json)"** (vedi [sezione 12](#12-progetto-esportazione-importazione-versioni)).

## 3. Struttura: atti, scene e blocchi

Nella scheda **Struttura** della barra laterale trovi l'elenco di atti e scene. Ogni scena è composta da **blocchi**, di tre tipi:

- **Didascalia** — descrizione dell'azione scenica, sempre in corsivo nel PDF.
- **Battuta** — il nome del personaggio seguito dal testo che dice.
- **Fuori scena** — una battuta pronunciata da un personaggio non visibile sul palco.

Mentre scrivi il nome di un personaggio in una battuta, l'editor lo riconosce automaticamente e lo aggiunge, se non esiste già, all'elenco dei personaggi.

Ogni scena ha anche dei campi propri: titolo, ambientazione, note di regia, stato (es. "Bozza" / "Definitiva").

## 4. Personaggi

Nella scheda **Personaggi** trovi l'elenco completo. Aprendo la scheda di un personaggio puoi compilare:

- **Ruolo drammaturgico**: Protagonista, Deuteragonista, Antagonista, Confidente, Comprimario, Caratterista, Aiutante, Coro, Voce narrante, Comparsa.
- Descrizione, età, aspetto fisico, costume, oggetti di scena, foto.
- Relazioni con altri personaggi (es. "madre di", "rivale di"), usate anche per generare il diagramma delle relazioni.

Questi campi non sono obbligatori, ma più li compili più diventano utili le statistiche, il PDF "Personaggi" (dramatis personae) e il diagramma delle relazioni.

## 5. Diagramma delle relazioni

Dal pulsante dedicato nella scheda Personaggi si apre un diagramma generato automaticamente dalle relazioni inserite: i personaggi sono disposti lungo il perimetro di un quadrato, con le frecce delle relazioni etichettate direttamente lungo la linea.

Puoi scaricarlo come:
- **SVG** — immagine vettoriale, modificabile con un editor grafico.
- **PDF** — pronto per la stampa, dimensionato esattamente sul diagramma.

## 6. Personaggi in scena e lettura mirata

In cima a ogni scena trovi i chip con i nomi dei personaggi, sotto l'etichetta *"Personaggi in scena"*. Selezionandone uno o più:

- la scena mostra **solo** le battute dei personaggi selezionati (utile per isolare le battute di un attore durante una prova);
- le didascalie restano sempre visibili, perché non appartengono a un singolo personaggio.

Il chip **"TUTTI"** azzera la selezione e torna a mostrare tutto. Il pulsante **"rileva dai dialoghi"** seleziona automaticamente tutti i personaggi che effettivamente parlano in quella scena.

## 7. Modalità prova e sintesi vocale

Il pulsante **🎭** attiva la **modalità prova**: i campi di testo diventano di sola lettura, per evitare modifiche accidentali mentre reciti o dirigi, e alcuni controlli di modifica vengono nascosti.

Se le prove si svolgono con il cast non al completo, il pulsante **"🔊 leggi le battute degli assenti"** (accanto ai chip "Personaggi in scena") fa leggere ad alta voce, con la sintesi vocale del browser, tutte le battute dei personaggi **non** selezionati come presenti in quella scena — così gli attori presenti possono provare le proprie battute con le risposte "recitate" dal computer. Premi di nuovo il pulsante (diventa "⏹ interrompi lettura") per fermarla in ogni momento.

> Richiede un browser con supporto alla sintesi vocale (la maggior parte dei browser desktop e mobile moderni la supportano).

## 8. Statistiche e piano di scena

**"📊 Statistiche"** mostra:
- tempo di lettura stimato per ciascun atto (e totale);
- grafico a barre del bilanciamento delle battute tra i personaggi;
- elenco aggregato di oggetti di scena e costumi, raccolto dalle schede dei personaggi.

**"🎭 Piano scene"** mostra una tabella con i personaggi sulle righe e le scene sulle colonne: un pallino indica in quali scene compare ciascun personaggio (basato sui chip "Personaggi in scena", o — se non li hai impostati — dedotto automaticamente da chi parla in quella scena).

## 9. Esportazione: PDF, testo, fountain, lettura HTML

Dalla barra in alto:

- **"Esporta PDF" / "👁️ Anteprima PDF"** — il copione completo, con copertina, indice e pagina "Personaggi".
- **"📄 Per personaggio"** — un PDF ridotto con solo le battute di un personaggio scelto, utile per le prove individuali.
- **"Esporta .txt"** — il testo semplice del copione.
- **"Esporta .fountain"** — formato standard aperto per sceneggiature, leggibile da altri programmi compatibili (es. per un futuro adattamento cinematografico/televisivo).
- **"👁️ Copia di lettura (HTML)"** — un file HTML statico e di sola lettura, con lo stesso aspetto grafico dell'app, pensato per essere condiviso via email o chat con attori e collaboratori che non devono modificare nulla.

Formato pagina e margini del PDF si impostano da **"⚙️ Impostazioni PDF"** (A4 o Letter; margini normali, stretti o ampi).

## 10. QR code in copertina

Se pubblichi il tuo copione anche online (ad esempio su un sito, un Google Drive condiviso, o via GitHub Pages), puoi compilare il campo **"Link alla versione digitale"** in "⚙️ Impostazioni PDF": da quel momento, la copertina del PDF completo mostrerà un QR code che rimanda a quell'indirizzo, comodo per chi ha il copione stampato in mano e vuole aprire rapidamente la versione digitale sul telefono.

> Il QR code punta all'indirizzo che inserisci tu: l'app non pubblica né ospita nulla in autonomia.

## 11. Salvataggio e dove va a finire il tuo lavoro

Editor di Copioni salva **automaticamente** ogni modifica nel browser che stai usando (localStorage). Questo significa che:

- il lavoro resta sul dispositivo/browser in cui hai scritto;
- se cambi computer, o cancelli i dati di navigazione del browser, il salvataggio automatico locale va perso.

Per un salvataggio più solido, hai due alternative (dal menù di salvataggio in alto):

- **"📁 Collega un file sul mio computer"** — collega un file reale sul disco, che viene aggiornato automaticamente mentre scrivi.
- **"📁 Scegli dove salvare"** / **"Salva progetto (.json)"** — esporta manualmente un file di backup completo del progetto.

> 💡 Consiglio: anche se usi il salvataggio automatico nel browser, esporta periodicamente un `.json` di backup — è l'unico modo per portare il lavoro su un altro dispositivo o recuperarlo in caso di problemi col browser.

## 12. Progetto: esportazione, importazione, versioni

- **"Salva progetto (.json)"** — scarica l'intero copione (testo, personaggi, impostazioni) in un unico file.
- **"Importa progetto"** — carica un file `.json` precedentemente esportato. Se il copione attualmente aperto contiene già del lavoro, ti viene chiesto se vuoi salvarlo prima di sostituirlo.
- **"🕘 Versioni"** — cronologia delle versioni salvate nel tempo. Per ogni versione puoi:
  - **Ripristina** — torna a quella versione (sovrascrive il copione attuale);
  - **Confronta** — mostra un confronto riga per riga tra quella versione salvata e il copione attuale (righe rosse: solo nella versione salvata; righe verdi: solo nel copione attuale);
  - **Elimina** — rimuove quella versione salvata.

## 13. Aspetto: temi grafici e layout

Il pulsante **🎨** apre la scelta tra quattro temi grafici:

| Tema | Atmosfera |
|---|---|
| Velluto & oro | Il tema predefinito, ispirato al teatro all'italiana |
| Manoscritto d'archivio | Sobrio, ispirato ai copioni da regia annotati a macchina |
| Palcoscenico contemporaneo | Scuro, minimale, con un accento ambra |
| Carta di piazza | Caldo e popolare, ispirato alle locandine dei teatranti girovaghi |

Il pulsante **🌙** attiva/disattiva un tema scuro indipendente, che puoi combinare con qualsiasi tema grafico.

Il pulsante **▦** permette di mostrare/nascondere intestazione, barra laterale e barra inferiore, per avere più spazio quando scrivi. **A＋ / A－** regolano la dimensione del testo.

## 14. Scorciatoie da tastiera

| Scorciatoia | Azione |
|---|---|
| `Ctrl/Cmd + S` | Forza il salvataggio immediato |
| `Ctrl/Cmd + Invio` | Aggiunge rapidamente una nuova battuta nella scena aperta |
| `Ctrl/Cmd + Z` | Annulla l'ultima modifica |
| `Ctrl/Cmd + Maiusc + Z` (o `Ctrl/Cmd + Y`) | Ripete la modifica annullata |

## 15. Domande frequenti

**Devo installare qualcosa?**
No. Basta un browser. Nessun account, nessun server.

**I miei dati vengono inviati da qualche parte?**
No: tutto resta nel tuo browser, salvo le librerie esterne (jsPDF, il generatore di QR code, i font) caricate da CDN pubblici la prima volta che ti servono, e solo se hai una connessione internet attiva in quel momento.

**Posso usarlo da tablet?**
Sì, l'interfaccia è ottimizzata anche per schermi touch.

**Posso scrivere in team, con altre persone contemporaneamente?**
No: è uno strumento locale, pensato per un autore/una autrice alla volta. Per condividere il lavoro con altri, usa "Esporta progetto (.json)" o la "Copia di lettura (HTML)".

**Ho perso il lavoro cambiando browser: si può recuperare?**
Solo se avevi esportato un backup `.json` in precedenza, o collegato un file locale. Per questo è consigliato farlo periodicamente (vedi [sezione 11](#11-salvataggio-e-dove-va-a-finire-il-tuo-lavoro)).

---

Per domande o segnalazioni, apri una *Issue* sulla repository GitHub del progetto.
