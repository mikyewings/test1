# Questionario — Indagine uso IA (per i dipendenti)

Applicazione web da inviare ai dipendenti **prima dell'avvio della consulenza**. Struttura e opzioni di risposta adattate da un questionario reale usato per un'indagine simile in ambito cooperativo, riportate al contesto di una piccola azienda.

**Link al questionario**: https://claude.ai/artifact/4Rgit3rF5MDczWcGa9UGq7

## Prima di condividerlo

1. Dal menu **"Share"** della pagina, imposta il link su **"Anyone with the link" con permesso di modifica (edit)** — non basta "può visualizzare": senza il permesso di modifica le risposte non vengono registrate e il questionario passa automaticamente alla modalità di riserva (vedi sotto).
2. Nessun altro segnaposto da personalizzare: a differenza della prima versione, non c'è più un indirizzo email da inserire.

## Come funziona la raccolta delle risposte

Le risposte si accumulano **direttamente nella pagina**: ogni invio la "ripubblica" con la nuova risposta aggiunta a quelle già raccolte, senza che il dipendente debba scaricare o inviare nulla. Tu vedi i risultati aprendo la stessa pagina (vedi sotto).

**Compromesso da conoscere**: perché questo funzioni senza chiedere un account Claude ai dipendenti, la pagina deve essere condivisa con permesso di modifica a chiunque abbia il link. Questo significa che, in teoria, una persona con competenze tecniche (es. leggendo il codice sorgente della pagina) potrebbe vedere le risposte già inviate dagli altri colleghi, incluse quelle su dati sensibili. Non c'è un modo per evitarlo restando su un'applicazione pubblica senza account — è il compromesso scelto per avere la raccolta centralizzata automatica invece dello scambio manuale di file.

**Riserva automatica**: se per un dipendente la raccolta centralizzata non dovesse funzionare (conflitto con un altro invio simultaneo, problema di permessi), il questionario scarica comunque un file Excel con la sua risposta e lo invita a inviartelo — nessuna risposta va persa.

## Come vedere i risultati

1. Apri il link del questionario da un account con permesso di modifica sulla pagina (il tuo).
2. In alto compare il pulsante **"Vedi i risultati raccolti"** (visibile solo a chi può modificare la pagina — i dipendenti non lo vedono).
3. Mostra il numero di risposte, i casi segnalati come "da approfondire" e un pulsante **"Esporta tutto in Excel"**: genera un unico file con una riga per ogni risposta ricevuta finora, pronto da usare.

## Struttura (26 domande, ~10 minuti)

1. **Il tuo profilo professionale** — area di lavoro, ruolo, contatto con dati di clienti, dimestichezza digitale
2. **Hai mai usato l'IA per lavoro?** — con salto logico: chi risponde "no" vede solo il perché (poi passa direttamente alle sezioni finali); chi risponde "sì" vede tutte le sezioni seguenti
3. **Utilizzo e strumenti** — frequenza, strumenti usati e, per **ciascuno strumento selezionato**, con che tipo di account lo usa (aziendale, personale gratuito, personale a pagamento, senza registrazione), dispositivo
4. **Attività** — per cosa la usa, tempo risparmiato percepito
5. **Dati inseriti** — che tipo di informazioni (con le categorie sensibili segnalate), se anonimizza prima di inserire un testo
6. **Controllo dei risultati** — come verifica l'output, errori o invenzioni trovati, uso in documenti ufficiali
7. **Percezioni** — benefici e rischi percepiti, accordo con l'uso dell'IA se regolato (tutti rispondono, anche chi non la usa)
8. **Competenze e formazione** / **Regole e aspettative** — formazione ricevuta e desiderata, conoscenza delle regole aziendali, aspettative, domanda finale libera

La colonna **"Account per strumento"** dell'export riporta, per ogni strumento selezionato, se l'account usato è aziendale o personale (es. "ChatGPT: Account personale gratuito; Copilot: Account aziendale"). La colonna **"Da approfondire"** è calcolata automaticamente: segna "Sì" quando la persona ha indicato di aver inserito dati personali o sensibili (clienti, colleghi, dati sanitari, dati finanziari) e usa almeno uno strumento con un account non aziendale — i casi da guardare per primi.

## Dopo la raccolta

Le righe esportate alimentano direttamente `01-censimento-strumenti-ai.md` (stesse colonne) e i casi segnalati come "da approfondire" vanno verificati con `02-checklist-pratiche-vietate-e-rischio.md`.
