# Restituzione e controllo del lotto

## Primo invio: due campioni

Consegna MASSIF e SADDLE nei canvas esatti e una tavola diagnostica separata su cinque fondi uniformi: ocra #B8A848, oliva #A3A65F, terra #B99A5B, neve #E5E4D7, petrolio #183848. Mostra master e riduzione proporzionale a512px di larghezza; nessun fondo nei PNG master. Confronta tratto, silhouette e palette con la reference. Fermati per revisione prima degli altri13.

## Consegna finale dopo revisione

Restituisci una cartella con masters/ (esattamente15 PNG della distinta), originals/ (output originali del servizio se diversi), previews/ (sole prove) e metadati-compilati.json. Nessun atlas o file del progetto.

- Cinque materiali: RGBA8 sRGB, 512×512, A=255, nessun bordo trasparente, anteprima seamless in ripetizione2×2 X/Y. Anche il taglio diagonale dell'insieme non deve rivelare una macchia ripetitiva dominante.
- Dieci ritagli/basi: RGBA8 sRGB e vera trasparenza; margini liberi, nessuna figura mozzata, nessuna frangia colorata sui cinque fondi.
- Basi: prova sotto almeno due rilievi, su PLAIN/EARTH/DRY/MINERAL; nessun ovale riconoscibile o fascia verde. Usa i materiali del lotto per i provini finali.
- Colline: A e B devono avere strutture diverse; le versioni DRY mantengono la famiglia ma hanno substrato e dettagli ridisegnati. Niente coni o montagne miniaturizzate.
- Bosco: chiome/tronchi nitidi, suolo leggibile nei vuoti; OPEN e INLET svolgono funzioni diverse. Non disegnare un altro nucleo forestale intero.
- Studio di composizione facoltativo ma utile: accosta materiali, high/low, colline e margine boschivo usando solo i componenti richiesti. Etichetta la tavola “studio di composizione”, mai “mappa generata” o “integrazione verificata”.

## Metadati, senza inventare misure

Usa dati/METADATI_DA_COMPILARE.json come modello. Coordinate in pixel, origine in alto a sinistra, X verso destra e Y verso il basso. Bbox [x,y,width,height] ricavato da alfa>7; crop suggerito esplicito; anchor anatomico di contatto riportato nel canvas e rispetto al crop, non semplicemente il bordo inferiore del file. Per i tile anchor e crop di posizionamento sono N/A.

I campi sconosciuti restano null, accompagnati dalla ragione. Dichiara misure ottenute con strumenti, valori proposti e valutazioni umane separatamente. Non trascrivere come misurati i valori dei contratti proposti. Seed del servizio solo se esposto realmente.

Se hai strumenti di analisi, allega istogramma alfa, occupazione conservativa64×64 (soglia alfa>=7) e inviluppo superiore/inferiore per64 fasce X, con origine e soglia dichiarate; preserva i vuoti. Sono metadati per successiva integrazione, non maschere già lette dal motore. Se non puoi calcolarli, lasciali null: li misureremo sui PNG consegnati. Non farli indovinare al modello visivo.

## Criteri di revisione

La parte tecnica può passare mentre l'immagine resta inadatta. Valutare continuità del piede, varietà strutturale, luce coerente, dettaglio leggibile e somiglianza stilistica al target. La sfumatura deve collegare le figure alla terra senza cancellare la loro struttura. Segnalare ogni limite; nessuna accettazione artistica automatica.
