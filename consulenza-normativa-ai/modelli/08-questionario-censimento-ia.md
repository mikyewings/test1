# Questionario — Indagine uso IA (per i dipendenti)

Applicazione web, **anonima**, da inviare ai dipendenti **prima dell'avvio della consulenza**. Struttura e opzioni di risposta adattate da un questionario reale usato per un'indagine simile in ambito cooperativo, riportate al contesto di una piccola azienda.

**Link al questionario**: https://claude.ai/artifact/4Rgit3rF5MDczWcGa9UGq7

> Il link è privato: va condiviso dal menu "Share" della pagina prima di inviarlo ai dipendenti. Una volta condiviso, chiunque può aprirlo e rispondere senza bisogno di un account.

## Struttura (26 domande, ~10 minuti)

1. **Il tuo profilo professionale** — area di lavoro, ruolo, contatto con dati di clienti, dimestichezza digitale
2. **Hai mai usato l'IA per lavoro?** — con salto logico: chi risponde "no" vede solo il perché (poi passa direttamente alle sezioni finali); chi risponde "sì" vede tutte le sezioni seguenti
3. **Utilizzo e strumenti** — frequenza, strumenti usati e, per **ciascuno strumento selezionato**, con che tipo di account lo usa (aziendale, personale gratuito, personale a pagamento, senza registrazione), dispositivo
4. **Attività** — per cosa la usa, tempo risparmiato percepito
5. **Dati inseriti** — che tipo di informazioni (con le categorie sensibili segnalate), se anonimizza prima di inserire un testo
6. **Controllo dei risultati** — come verifica l'output, errori o invenzioni trovati, uso in documenti ufficiali
7. **Percezioni** — benefici e rischi percepiti, accordo con l'uso dell'IA se regolato (tutti rispondono, anche chi non la usa)
8. **Competenze e formazione** / **Regole e aspettative** — formazione ricevuta e desiderata, conoscenza delle regole aziendali, aspettative, domanda finale libera

## Come funziona la raccolta delle risposte

Non esiste un accesso automatico a un database condiviso per questa pagina: i dipendenti del cliente non hanno un account Claude, quindi la raccolta centralizzata in tempo reale (che richiederebbe l'accesso alla tua organizzazione) non era praticabile. Il flusso è invece:

1. Il dipendente compila il questionario (circa 10 minuti).
2. Alla fine, scarica automaticamente un file Excel con la propria risposta (un file a testa, una riga per persona).
3. Lo invia all'indirizzo o canale indicato nella pagina stessa.
4. Tu raccogli i file ricevuti e **incolli le righe in un unico foglio**, usando le stesse colonne in ognuno (corrispondono 1 a 1 alle domande: area di lavoro, ruolo, uso dell'IA, strumenti, account, dati inseriti, rischi percepiti, formazione, ecc.).

La colonna **"Account per strumento"** riporta, per ogni strumento selezionato, se l'account usato è aziendale o personale (es. "ChatGPT: Account personale gratuito; Copilot: Account aziendale"). La colonna **"Da approfondire"** è calcolata dal questionario stesso: segna "Sì" quando la persona ha indicato di aver inserito dati personali o sensibili (clienti, colleghi, dati sanitari, dati finanziari) e usa almeno uno strumento con un account non aziendale — i casi da guardare per primi.

## Prima di inviarlo

Nella pagina vanno personalizzati due segnaposto tra **[parentesi quadre]**:
- l'indirizzo email o il canale a cui i dipendenti devono inviare il file scaricato
- la data entro cui rispondere

## Dopo la raccolta

Le righe consolidate alimentano direttamente `01-censimento-strumenti-ai.md` (stesse colonne) e i casi segnalati come "da approfondire" vanno verificati con `02-checklist-pratiche-vietate-e-rischio.md`.
