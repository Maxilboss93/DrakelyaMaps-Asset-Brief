# Feedback sul lotto pilota 01

Data: 16 novembre 2026. Riferimento analizzato: commit `8cdd3f3`.

Questo documento raccoglie osservazioni e proposte per il confronto fra chi prepara gli asset e chi li integrerà in Drakelya Maps. Non modifica la commessa vigente, non approva i campioni e non autorizza la produzione degli altri tredici master. Le decisioni ancora aperte sono indicate esplicitamente.

## Valutazione

Il brief è una buona base operativa: distingue correttamente qualità artistica, conformità tecnica e integrazione software. Sono particolarmente utili la revisione iniziale di MASSIF/SADDLE, la separazione fra materiali, basi e figure, i controlli sui cinque fondi e la richiesta di lasciare null i metadati non misurati.

Il confronto visivo incluso evidenzia soprattutto una differenza nella continuità del paesaggio: valli, pendii, piedi dei rilievi e margini boschivi. Migliorare le singole immagini è utile, ma non dimostra da solo che la composizione procedurale raggiungerà la reference. Il confronto riguarda geografie diverse e non costituisce una misura del motore attuale.

## Proposte da discutere prima del lotto completo

1. **Rendere obbligatorio uno studio di composizione nella revisione dei due campioni.** Accostare e sovrapporre MASSIF e SADDLE con terreno e vegetazione già disponibili, senza richiedere ulteriori master. Mostrare anche contatti laterali, ripetizioni e raccordi al piede. Etichettare la tavola come studio di composizione: non prova integrazione, generazione o prestazioni. Nella commessa attuale lo studio è facoltativo; questa modifica resta da concordare.
2. **Concordare una scala di accettazione.** Oltre alla riduzione a 512 px, mostrare gli asset alle dimensioni di visualizzazione proposte nei contratti, chiarendo larghezza del viewport e zoom. Valutare leggibilità, densità del tratto e ripetizione della sagoma. Questi provini non sostituiscono una successiva verifica nel renderer reale.
3. **Confermare la luce NE sulla composizione completa.** È una proposta correttamente dichiarata, ma va confrontata con vegetazione, edifici e rilievi esistenti. Evitare di approvare i due campioni isolatamente e scoprire incoerenze solo durante l'integrazione. Prima di estendere la scelta agli altri asset, registrare qui l'esito della revisione.
4. **Precisare le convenzioni dei metadati.** Dichiarare se `mustFitInside` usa `[xMin,yMin,xMax,yMax]`: i valori del massiccio `[32,32,800,640]` sembrano descrivere estremi, mentre il bbox è definito come `[x,y,width,height]`. Esplicitare inoltre se la differenza fra soglie alfa `>7` e `>=7` è intenzionale; altrimenti uniformarla. Si tratta di chiarimenti proposti, non di errori già corretti nei contratti.

## Passo successivo suggerito

Produrre e revisionare soltanto i due campioni previsti. Usare i cinque fondi per individuare aloni e frange; usare la composizione per valutare continuità, scala e luce. Un PNG tecnicamente conforme può ancora richiedere una revisione artistica.

Per ogni osservazione, il confronto può registrare: proposta, risposta del collega, decisione condivisa, file interessati e verifica attesa. Solo dopo la decisione aggiornare le istruzioni operative corrispondenti, mantenendo coerenti prompt, distinta, contratti, manifest ed eventuali pacchetti ZIP.

## Stato delle decisioni

| Tema | Proposta | Stato |
|---|---|---|
| Studio di composizione | Obbligatorio nella revisione dei due campioni | Da concordare |
| Scala | Provini alle dimensioni d'uso concordate | Da concordare |
| Luce | Confermare NE insieme agli asset esistenti | Da verificare sui campioni |
| Metadati | Esplicitare rettangoli e soglie alfa | Da chiarire |

## Verifiche svolte e limiti

Letti direzione comune, distinta, QA, prompt dei due campioni e metadati proposti; esaminati il confronto target/risultato incluso e il massiccio sorgente. Verificati i 62 file elencati nel manifest SHA-256, senza differenze.

Nessun nuovo master prodotto, nessuna modifica al motore, nessun test browser o collaudo di integrazione. Il presente feedback è una base di discussione, non un'accettazione artistica o tecnica del futuro lotto.
