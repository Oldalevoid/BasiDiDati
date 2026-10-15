# E005 — Livelli di rappresentazione: vista esterna

**Modulo:** M1 — Sistemi informativi e basi di dati  
**Stato:** COMPLETATO (15 ottobre 2026) — prima risposta corretta  
**Argomento d'esame:** livelli di rappresentazione di una base di dati; livello esterno, logico (concettuale nell'architettura ANSI/SPARC) e interno.

## Descrizione e teoria minima
In un'azienda di dispositivi elettromedicali, l'applicazione per i tecnici visualizza soltanto matricola, modello e stato dei dispositivi. La base dati memorizza anche altre informazioni e usa un'organizzazione fisica sul disco che il tecnico non deve conoscere.

- **Livello esterno**: vista dei dati destinata a uno specifico utente/applicazione.
- **Livello logico/concettuale dell'architettura a tre livelli**: struttura complessiva dei dati e relazioni, indipendentemente dalla memorizzazione fisica.
- **Livello interno**: come i dati sono organizzati e memorizzati fisicamente.

```mermaid
flowchart TD
  A["Vista esterna: tecnici\nMatricola, Modello, Stato"] --> B["Schema logico: tutti i dati e le relazioni"]
  C["Vista esterna: amministrazione\nMatricola, Modello, Costo"] --> B
  B --> D["Livello interno: file, pagine, indici"]
```

### Esempio didattico: vista dei tecnici
| Matricola | Modello | Stato |
|---|---|---|
| EM-101 | Defibrillatore A | Operativo |
| EM-102 | Ecografo B | Manutenzione |

Non è richiesto codice SQL: l'esercizio serve a identificare il livello di rappresentazione.

## Consegna E005
Un tecnico può consultare soltanto matricola, modello e stato tramite la propria schermata, benché il database contenga molti altri dati. **Quale livello di rappresentazione descrive la schermata dedicata al tecnico?**

- **A.** Livello interno, perché mostra dati memorizzati su disco.
- **B.** Livello esterno, perché è una vista specifica destinata al tecnico.
- **C.** Livello logico complessivo, perché contiene necessariamente tutti i dati aziendali.
- **D.** Nessun livello: una schermata non può rappresentare dati di un database.

## Risposta effettiva dello studente
**B — Corretta al primo tentativo (15 ottobre 2026).** Il livello esterno descrive una vista specifica dei dati destinata a un utente o applicazione; non coincide necessariamente con l'intero schema logico o con l'organizzazione fisica.

## Soluzione effettivamente raggiunta e cosa ho imparato
Risposta B corretta senza ulteriori tentativi: riconoscimento del **livello esterno** in uno scenario reale. Non ancora provata la distinzione autonoma dei livelli logico e interno.

## Prossimo passo
Passare all'[E006 — Livelli logico e interno](006-livelli-logico-interno.md). Richiamare il riconoscimento delle modifiche di schema nelle prossime applicazioni.

Riferimento: [Programma M1](../PROGRAMMA_CORSO.md).
