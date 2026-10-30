# Questionario — Censimento uso IA (per i dipendenti)

Applicazione web da inviare ai dipendenti **prima dell'avvio della consulenza**, per capire quali strumenti di IA usano davvero, per cosa, e con quali dati — incluso un primo segnale sui rischi legati a dati personali o sensibili.

**Link al questionario**: https://claude.ai/artifact/4Rgit3rF5MDczWcGa9UGq7

> Il link è privato: va condiviso dal menu "Share" della pagina prima di inviarlo ai dipendenti. Una volta condiviso, chiunque può aprirlo e rispondere senza bisogno di un account.

## Come funziona la raccolta delle risposte

Non esiste un accesso automatico a un database condiviso per questa pagina: i dipendenti del cliente non hanno un account Claude, quindi la raccolta centralizzata in tempo reale (che richiederebbe l'accesso alla tua organizzazione) non era praticabile. Il flusso è invece:

1. Il dipendente compila il questionario (circa 5 minuti).
2. Alla fine, scarica automaticamente un file Excel con la propria risposta (un file a testa).
3. Lo invia all'indirizzo o canale indicato nella pagina stessa.
4. Tu raccogli i file ricevuti e **incolli le righe in un unico foglio**, usando le stesse colonne in ognuno: Data, Reparto, Ruolo, Strumento, Uso principale, Dati trattati, Account, Frequenza, Approvato da, Dubbi o incidenti, Da approfondire, Nota generale.

La colonna **"Da approfondire"** è già calcolata dal questionario stesso: segna "Sì" quando la persona ha indicato dati personali o sensibili (clienti, colleghi, dati sanitari, dati finanziari) su un account non aziendale o non specificato — i casi da guardare per primi.

## Prima di inviarlo

Nella pagina vanno personalizzati due segnaposto tra **[parentesi quadre]**:
- l'indirizzo email o il canale a cui i dipendenti devono inviare il file scaricato
- la data entro cui rispondere

## Dopo la raccolta

Le righe consolidate alimentano direttamente `01-censimento-strumenti-ai.md` (stesse colonne) e i casi segnalati come "da approfondire" vanno verificati con `02-checklist-pratiche-vietate-e-rischio.md`.
