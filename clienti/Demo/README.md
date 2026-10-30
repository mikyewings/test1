# Cliente Demo: scheda e fascicolo di adeguamento AI

Copia dei modelli di `consulenza-normativa-ai/modelli/`, personalizzata per un cliente dimostrativo. **Tutti i dati sotto sono fittizi**: servono a mostrare come appare un fascicolo compilato. Per un cliente reale, duplicare la cartella e sostituirli.

## Anagrafica

| Campo | Valore |
|---|---|
| Ragione sociale | Demo S.r.l. |
| Sede legale | Via dell'Esempio 1, 24121 Bergamo (BG) |
| P.IVA | 00000000000 |
| PEC | demo-srl@pec.example |
| Email generale | info@demo-srl.example |
| Legale rappresentante | Laura Bianchi, Amministratrice unica |

## Referente interno AI

| Campo | Valore |
|---|---|
| Nome | Marco Rossi |
| Ruolo | Responsabile amministrazione e IT |
| Email | marco.rossi@demo-srl.example |
| Telefono | +39 035 000 0000 |

## Calendario del percorso

| Data | Tappa | Documento |
|---|---|---|
| 05/11/2026 | Check iniziale gratuito | `00-scaletta-check-iniziale` |
| prima del 16/11/2026 | Invio questionario ai dipendenti | `08-questionario-censimento-ia.md` |
| 16/11/2026 | Censimento strumenti AI | `01-censimento-strumenti-ai` |
| 23/11/2026 | Checklist pratiche vietate e rischio | `02-checklist-pratiche-vietate-e-rischio` |
| 30/11/2026 | Approvazione policy e firma nomina referente | `03-policy-uso-ai-aziendale`, `04-nomina-referente-ai` |
| 01/12/2026 | Entrata in vigore policy e decorrenza nomina | |
| 10/12/2026 | Sessione di formazione | `05-registro-e-attestato-formazione`, `07-slide-alfabetizzazione-formazione.md` |
| 18/12/2026 | Consegna report finale | `06-report-finale-adeguamento` |
| 01/12/2027 | Revisione annuale della policy | |

## Cosa resta da compilare

Sono stati compilati solo i dati anagrafici, i contatti e le date. Restano volutamente tra `[parentesi quadre]`:

- **nome del consulente/formatore** (01, 04, 05, 06);
- **risultati del percorso**: righe del censimento, esiti della checklist, strumenti autorizzati, numero partecipanti, sintesi e raccomandazioni del report;
- **nominativi dei partecipanti** negli attestati (05, uno per persona) e la durata della formazione.

I file `07` e `08` sono copiati senza modifiche: puntano ad artifact condivisi (deck e questionario), che vanno personalizzati direttamente sulla pagina.
