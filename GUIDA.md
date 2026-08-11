# 📖 Guida utente — Copione, editor per il teatro

Questa guida spiega passo per passo come usare tutte le funzioni dell'editor. Per una panoramica generale del progetto vedi il [README](./README.md).

## Indice

1. [Avvio rapido](#avvio-rapido)
2. [Struttura del copione: atti e scene](#struttura-del-copione-atti-e-scene)
3. [Scrivere il testo: i tipi di blocco](#scrivere-il-testo-i-tipi-di-blocco)
4. [Personaggi e relazioni](#personaggi-e-relazioni)
5. [Salvataggio: automatico, locale e versioni](#salvataggio-automatico-locale-e-versioni)
6. [Strumenti di lavoro](#strumenti-di-lavoro)
7. [Esportazioni](#esportazioni)
8. [Modalità prova/lettura](#modalità-provalettura)
9. [Personalizzazione dell'aspetto](#personalizzazione-dellaspetto)
10. [Uso su tablet e smartphone](#uso-su-tablet-e-smartphone)
11. [Domande frequenti](#domande-frequenti)

---

## Avvio rapido

Apri il file `copione-teatrale.html` in un browser. All'apertura trovi già un copione vuoto pronto per iniziare, con un primo atto e una prima scena. Da qui puoi:

- modificare **titolo** e **autore** in alto nell'intestazione;
- iniziare a scrivere direttamente nella pagina centrale (il "palco");
- usare il pulsante **📖 Guida** nel menù laterale per rileggere in ogni momento le linee guida essenziali di scrittura teatrale integrate nell'app.

## Struttura del copione: atti e scene

Nella scheda **Struttura** (menù a sinistra) trovi l'elenco di atti e scene:

- ogni **atto** può essere rinominato cliccando sul suo titolo;
- ogni **scena** ha un pallino colorato che ne indica lo stato: grigio-blu = *bozza*, arancione = *da rivedere*, verde = *definitiva*. Lo stato si cambia dai pulsanti nella parte alta della pagina della scena;
- clicca su una scena per aprirla nel palco centrale;
- passando il mouse su una scena compaiono le icone per rinominarla o eliminarla;
- usa il pulsante **+** per aggiungere nuovi atti o nuove scene.

Ogni scena include automaticamente una **slug line** (es. "Cucina, sera") che puoi modificare liberamente, oltre a un campo per le informazioni di scena (ambientazione, note) e ai **chip di presenza** dei personaggi in scena.

## Scrivere il testo: i tipi di blocco

All'interno di una scena il testo è organizzato in blocchi. Puoi aggiungerne di nuovi con il pulsante flottante in basso a destra (o con `Ctrl+Invio` per una nuova battuta):

| Blocco | Icona | Uso |
|---|---|---|
| **Battuta** | 🗣️ | Dialogo di un personaggio: il nome va in maiuscolo, come da convenzione teatrale |
| **Didascalia** | 📝 | Indicazioni di regia, descrizioni di scena o azione |
| **Fuori scena** | 🔈 | Voci o suoni provenienti da fuori campo |

Ogni blocco di dialogo può avere anche una **nota tra parentesi** (es. *(sottovoce)*) e un'indicazione dopo la battuta. Passa il mouse su un blocco per vedere le icone di modifica/eliminazione ed eventuali azioni rapide.

## Personaggi e relazioni

Nella scheda **Personaggi** puoi creare una scheda per ciascun personaggio con:

- nome, colore identificativo, ruolo;
- dettagli opzionali: età, altezza, aspetto fisico, costume, descrizione, backstory;
- **relazioni** con altri personaggi, per costruire una vera e propria mappa dei rapporti.

Dal pannello puoi aprire il **diagramma delle relazioni**, generato automaticamente in SVG, utile per avere una visione d'insieme dei legami fra i personaggi dell'opera.

## Salvataggio: automatico, locale e versioni

- **Salvataggio automatico**: l'editor salva il lavoro periodicamente nel browser (nessuna azione richiesta). L'indicatore in alto a destra mostra lo stato del salvataggio; il pulsante 💾 forza un salvataggio immediato.
- **Scegli dove salvare** 📁: nei browser che lo supportano (Chrome/Edge desktop), puoi collegare l'editor a un file `.json` sul tuo disco, così ogni modifica viene scritta direttamente lì.
- **Nuovo copione** 🆕: crea un progetto vuoto (il copione attuale resta comunque salvato nella cronologia/versione locale finché non lo sovrascrivi).
- **Versioni** 🕘: salva "fotografie" del copione in momenti chiave e ripristinale in qualunque momento, utile prima di modifiche importanti o per confrontare riscritture diverse.

> 🔒 Tutto il lavoro resta **sul tuo dispositivo**: l'app non invia mai il testo del copione a server esterni.

## Strumenti di lavoro

Dal menù laterale hai accesso a:

- **🔍 Cerca**: cerca e sostituisci testo in tutto il copione, con opzione di distinzione maiuscole/minuscole.
- **📄 Per personaggio**: genera un PDF con solo le battute (e le rispettive cue) di un personaggio scelto — ideale da distribuire agli attori.
- **✅ Qualità**: un controllo automatico che segnala incongruenze comuni (es. personaggi presenti in scena senza battute, scene vuote, problemi di continuità).
- **📊 Statistiche**: bilanciamento delle battute/parole fra personaggi e tempo di lettura stimato per atto (regola pratica: circa un minuto a pagina).
- **🗂️ Insieme**: vista d'insieme di tutte le scene con una breve anteprima del contenuto, utile per la revisione strutturale.
- **📥 Importa testo**: incolla un copione già scritto altrove; l'editor prova a riconoscere automaticamente nomi dei personaggi e didascalie e a trasformarlo in una nuova scena strutturata.
- **⚙️ Impostazioni PDF**: personalizza i parametri di impaginazione prima dell'esportazione (inclusa la riga di copyright).

## Esportazioni

Dalla barra in fondo alla pagina puoi esportare il copione in diversi formati:

- **Copia testo** — copia il copione negli appunti;
- **Esporta .txt** — file di testo semplice;
- **Esporta .fountain** — formato [Fountain](https://fountain.io/), leggibile da molti altri programmi di scrittura per la scena/schermo;
- **👁️ Anteprima PDF** — visualizza il PDF prima di scaricarlo;
- **Esporta PDF** — copione completo, con pagina del titolo, pagina del cast, numerazione di pagina e (se il copione è segnato come bozza) filigrana "bozza";
- **Salva progetto (.json)** — backup completo del progetto, da poter reimportare in seguito o trasferire su un altro dispositivo;
- **Importa progetto** — carica un file `.json` esportato in precedenza.

## Modalità prova/lettura

Il pulsante 🎭 nella barra degli strumenti del palco attiva la **modalità prova**: nasconde tutti i controlli di modifica e lascia solo il testo, per leggere il copione come farebbe un attore durante una prova, senza distrazioni.

Accanto trovi anche:

- **▦** per mostrare/nascondere intestazione, menù laterale e barra inferiore e ottenere più spazio di scrittura;
- **A－ / A＋** per regolare la dimensione del testo nel copione.

## Personalizzazione dell'aspetto

Il pulsante 🌙 attiva il **tema scuro**, pensato per sessioni di scrittura serali o prolungate. Il tema predefinito ("velluto & oro") richiama l'estetica di un teatro classico, con sipario bordeaux e dettagli dorati.

## Uso su tablet e smartphone

L'interfaccia si adatta automaticamente a schermi più piccoli: il menù laterale diventa un pannello richiamabile (pulsante "🗂️ Struttura e personaggi"), e i controlli si riorganizzano per il tocco.

## Domande frequenti

**Devo installare qualcosa?**
No: è un unico file HTML che gira interamente nel browser.

**I miei dati vengono inviati a un server?**
No, restano sul dispositivo (salvataggio nel browser o, se scelto, in un file locale).

**Posso lavorare da più computer sullo stesso copione?**
Sì: esporta il progetto in `.json` (o collega un file locale condiviso, ad es. tramite una cartella sincronizzata da un servizio cloud) e importalo sull'altro dispositivo.

**Che differenza c'è fra "Esporta .txt" e "Esporta .fountain"?**
Il `.txt` è testo semplice, utile per incollare altrove. Il `.fountain` mantiene la struttura di scene/personaggi/didascalie in un formato standard riconosciuto da altri editor di sceneggiatura.

**Il PDF ha la filigrana "bozza": come la tolgo?**
La filigrana compare automaticamente quando il copione (o le scene) risulta segnato come bozza; passa lo stato a "definitiva" per rimuoverla dagli export successivi.
