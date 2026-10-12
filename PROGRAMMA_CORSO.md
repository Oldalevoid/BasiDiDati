# Programma del corso — Basi di Dati (Pegaso)

## Metodo di ricostruzione
Fonte: 40 dispense PDF trasmesse in tre caricamenti, numerate 01–44 con lacune 09, 14, 31 e 34. I moduli sono raggruppamenti didattici derivati dalle dispense, non denominazioni ufficiali di unità d'esame. Contenuto originale sintetizzato, non copiato. Profondità: riconoscimento, interpretazione, applicazione pratica su piccoli casi, poi verifica autonoma, coerentemente con gli esempi e gli argomenti presenti. Non inferire formato di esame, programma di dispense mancanti o requisiti non presenti.

## Sequenza, dipendenze e criteri di superamento

### M1 — Sistemi informativi (01)
Contenuti: dati e informazioni; sistemi informativi e informatici; basi di dati e DBMS; modelli e livelli di rappresentazione; schema/istanza. Prerequisiti: nessuno. Superamento: distinguere i concetti su un caso e spiegare il ruolo di DBMS e livelli, senza suggerimenti.

### M2 — Modello relazionale e vincoli (02–04)
Contenuti: relazioni matematiche, attributi, tuple, domini, relazioni e basi relazionali; NULL; vincoli intrarelazionali; chiavi; integrità referenziale; violazioni e azioni compensative. Prerequisito: M1. Superamento: leggere schemi e istanze, identificare chiavi e vincoli, riconoscere violazioni e correzioni possibili.

### M3 — Algebra relazionale e viste (05–07)
Contenuti: linguaggi per basi di dati; operatori insiemistici, ridenominazione, selezione, proiezione; join naturale/esterno, semijoin, prodotto cartesiano, theta-/equi-join; relazioni di base/derivate; viste virtuali/materializzate e aggiornamenti. Prerequisito: M2. Superamento: calcolare risultati di operatori su tabelle piccole e motivare join e comportamento delle viste.

### M4 — SQL: definizione e vincoli (08, 10)
Contenuti: linguaggio SQL e standard; domini e tipi elementari; schemi, tabelle; vincoli intra/interrelazionali; modifica schemi. Prerequisiti: M2, M3 per il confronto teorico. Superamento: interpretare e produrre CREATE TABLE e vincoli, individuare errori pertinenti.

### M5 — SQL: interrogazioni e join (11–13)
Contenuti: SELECT/FROM/WHERE, LIKE, NULL, selezione/proiezione, equivalenze con algebra relazionale, interpretazione formale; duplicati e join espliciti interni/esterni. Prerequisiti: M3–M4. Superamento: formulare, eseguire mentalmente e correggere interrogazioni su una o più tabelle.

### M6 — SQL avanzato e modifica dei dati (15–19)
Contenuti: UNION, INTERSECT, EXCEPT/differenza; interrogazioni nidificate, ANY/ALL/EXISTS/IN; nidificazione in SELECT/FROM; aggregati COUNT/SUM/MAX/MIN/AVG; GROUP BY/HAVING; INSERT/UPDATE/DELETE e differenza da DROP; caso di studio di query avanzate. Prerequisito: M5. Superamento: risolvere autonomamente problemi misti con SQL e motivare risultati, inclusi NULL e duplicati quando rilevanti.

### M7 — Transazioni SQL (20)
Contenuti: specifica delle transazioni, atomicità, consistenza, isolamento e persistenza. Prerequisito: M6. Superamento: interpretare esiti di COMMIT/ROLLBACK e identificare proprietà interessate in scenari concreti.

### M8 — Progettazione concettuale e E-R (21–28)
Contenuti: ciclo di vita, livelli di progettazione; entità, relazioni, attributi; cardinalità; identificatori interni/esterni; generalizzazioni; regole aziendali e documentazione; raccolta/analisi requisiti, glossario e schema E-R. Prerequisiti: M1–M2; utilizzo applicativo di M4–M6 utile ma non indispensabile. Superamento: ricavare e giustificare autonomamente uno schema E-R e relativo glossario da requisiti narrativi.

### M9 — Pattern e progettazione logica (29, 30, 32, 33)
Contenuti: pattern base e avanzati, relazioni ricorsive, molti-a-molti, attributi su relazioni, gerarchie; analisi prestazionale con tavole dei volumi/accessi; ridondanze, eliminazione generalizzazioni; eliminazione attributi multivalore, accorpamenti e identificatori. Prerequisito: M8. Superamento: ristrutturare un E-R motivando le scelte e identificare chiavi e compromessi.

### M10 — Normalizzazione (35–38)
Contenuti: anomalie e ridondanze; dipendenze funzionali; BCNF; decomposizioni senza perdita e conservazione delle dipendenze; 3NF e limiti di BCNF; implicazione/copertura dipendenze; sintesi in 3NF. Prerequisiti: M2, M9. Superamento: riconoscere anomalie, verificare dipendenze su esempi, realizzare e valutare decomposizioni su casi semplici.

### M11 — Organizzazione fisica, prestazioni e transazioni (39–43)
Contenuti: memoria secondaria, buffer, DBMS e file system; pagine e tuple, indici primari/secondari, organizzazione sequenziale/hash/albero; gestione e costo delle interrogazioni, ottimizzazione; progettazione fisica e carico applicativo; log, checkpoint/dump, affidabilità e concorrenza. Prerequisiti: M3, M6–M7, M9. Superamento: confrontare accessi e indici, motivare costo/ottimizzazione di interrogazioni, descrivere recupero e anomalie di concorrenza su uno scenario.

### M12 — Evoluzione dei linguaggi e modelli (44)
Contenuti: dati strutturati, semistrutturati e non strutturati; XML, interrogazione e manipolazione XML, supporto in RDBMS; JSON, panoramica NoSQL. Prerequisiti: M1, M2, M6. Superamento: confrontare rappresentazioni e selezionare un modello spiegando i compromessi, entro la profondità introduttiva della dispensa.

## Prerequisiti trasversali
Lettura di tabelle, semplice logica e insiemi, confronto di valori, elementare interpretazione di espressioni. Richiamarli solo quando emerge una lacuna. SQL si esercita autonomamente; Python non è un prerequisito per comprendere il database.

## Verifica dei moduli
Ogni modulo: riconoscimento → spiegazione con parole proprie → applicazione guidata → autonomia → correzione di errore → verifica mista. Passaggio solo dopo almeno una applicazione autonoma significativa; per concetti fondamentali provare due abilità differenti. Verifica finale di ogni modulo separata dall'apprendimento; simulazioni d'esame dedicate dopo i moduli.

## Copertura e incertezze
Dispense mancanti nella numerazione: 09, 14, 31, 34. Nessuna attribuzione di contenuti non documentati. Eventuali approfondimenti tecnici sono marcati come esterni e opzionali. Le dispense non confermano modalità di prova, numero di domande, durata o soglia di promozione dell'esame.
