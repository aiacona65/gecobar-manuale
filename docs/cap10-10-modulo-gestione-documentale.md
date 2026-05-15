# 10. Modulo Gestione Documentale

Il Modulo Gestione Documentale è l'archivio digitale dell'attività. Risolve uno dei problemi più concreti e quotidiani di qualsiasi esercizio commerciale: i documenti cartacei che si accumulano — fatture ricevute, comunicazioni da enti pubblici, contratti, licenze, autorizzazioni, verbali di ispezione, corrispondenza con il Comune o con l'Agenzia delle Entrate — e che normalmente finiscono in faldoni e cassetti, rendendo difficile ritrovarli quando servono.

Con questo modulo ogni documento viene registrato, catalogato e collegato al suo file digitale PDF. L'archivio è interrogabile in pochi secondi per data, tipo, destinatario, ufficio di provenienza o parola chiave. Quando il modulo è attivo, i pulsanti di navigazione principali vengono temporaneamente disabilitati per evitare operazioni accidentali.

## 1. Visualizzatore documenti

Schermata principale con l'elenco completo di tutti i documenti archiviati e una barra di ricerca testuale in tempo reale. Le righe della griglia vengono colorate in modo diverso a seconda che il documento abbia o meno un file PDF allegato: in questo modo l'operatore riconosce immediatamente quali documenti sono stati completamente digitalizzati e quali richiedono ancora la scansione.

Cliccando su un documento, il pannello di dettaglio mostra tutti i campi. Se al documento è collegato un file PDF, si apre direttamente nel visualizzatore integrato nell'applicazione, senza lanciare programmi esterni.

## 2. Inserimento e gestione documenti

Per ogni documento si compilano: data del documento, numero, tipo (con autocompletamento dai valori già usati), ufficio/ente di riferimento (con autocompletamento), destinatario (con autocompletamento), importo, e descrizione libera.

I campi tipo/ufficio/destinatario sono collegati a popup con liste popolate automaticamente dai valori già presenti in archivio, garantendo coerenza nella catalogazione nel tempo.

### Scansione diretta dallo scanner

Il modulo si connette allo scanner collegato al computer tramite il protocollo WIA (Windows Image Acquisition), lo standard Windows per i dispositivi di acquisizione immagini. Il sistema rileva automaticamente il tipo di scanner e si adatta:

- Alimentatore automatico (ADF) — acquisisce più pagine in sequenza automaticamente. Ideale per contratti o estratti conto multipagina.
- Piano fisso (flatbed) — acquisisce la singola pagina posizionata sul vetro.
- Sorgente automatica — se entrambe le sorgenti sono disponibili, il sistema prova prima l'alimentatore (se ha fogli caricati) e poi il piano fisso come fallback.

Ogni pagina acquisita viene salvata come file BMP temporaneo, quindi tutte le pagine vengono unite automaticamente in un unico file PDF, salvato nella cartella di archivio con nome generato automaticamente. I file temporanei vengono eliminati automaticamente.

### Organizzazione automatica dei file

I file PDF non vengono salvati in modo caotico. Il sistema costruisce automaticamente una struttura di cartelle gerarchica basata sui metadati del documento (anno, tipo, ufficio), mantenendo l'archivio su disco ordinato e navigabile anche dall'esterno dell'applicazione.

## 3. Ricerca parametrica

Ricerca avanzata con filtri combinabili: intervallo di date, testo libero su tipo/destinatario/ufficio/descrizione, e importo. Anche dai risultati della ricerca è possibile aprire il PDF nel visualizzatore integrato, scansionare un documento mancante, e modificare o eliminare i record trovati.
