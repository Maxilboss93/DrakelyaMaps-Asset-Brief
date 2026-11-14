# Consegna per AI esterna — Drakelya Maps

Versione 1, 14 novembre 2026. Basata sull'inventario della PR13, commit50e1b81. Pacchetto autonomo: non occorre accesso al repository. Non contiene nuovi asset prodotti.

1. Allega lo ZIP all'AI esterna ed estrailo se la piattaforma lo richiede.
2. Incolla il testo di [00_PRIMO_MESSAGGIO_DA_COPIARE.txt](00_PRIMO_MESSAGGIO_DA_COPIARE.txt).
3. Se non legge ZIP/cartelle, allega almeno reference/DRAKELYA_VISUAL_TARGET.jpg, i quattro file massif/saddle del kit v4 sotto sorgenti/ e incolla le prime due schede prompt. In caso di limite agli allegati, per ciascun campione invia target + relativo WebP + relativo PNG sorgente e la sua scheda. Non procedere senza averle fatto vedere i riferimenti.
4. Rivedi i due campioni, quindi decidi se correggerli o autorizzare gli altri13.

Le15 schede in prompt/ sono autonome: ognuna include la direzione comune. [BRIEF_COMPLETO_AI_ESTERNA.md](BRIEF_COMPLETO_AI_ESTERNA.md) raccoglie tutto in un solo testo; il primo messaggio resta il punto di partenza. [02_DISTINTA_15_FILE.md](02_DISTINTA_15_FILE.md) e [03_CONSEGNA_E_QA.md](03_CONSEGNA_E_QA.md) definiscono quantità e restituzione.

## Reference e sorgenti

- reference/DRAKELYA_VISUAL_TARGET.jpg è l'obiettivo primario, invariato.
- reference/target-vs-current.webp mostra i problemi da correggere, non un risultato approvato.
- sorgenti/ contiene copie native non modificate, con percorsi conservati per evitare ambiguità.
- dati/MAPPA_SORGENTI.json risolve gli ID, le coordinate native dei crop e gli hash. Un atlas resta una tavola: non importarne automaticamente celle vicine o frammenti.
- Le tavole in reference/ servono per orientarsi; non sono sorgenti da ingrandire. Alcune contengono miniature di asset estranei al lotto: non ordinarli.
- dati/CONTRATTI_PROPOSTI_PILOTA.json descrive solo proposte, non un formato del motore già operativo.

La reference guida stile e composizione; non certifica il diritto di estrarne sprite. I termini di artwork/servizio restano quelli effettivi: documentare provenienza senza attribuire licenze libere per inferenza.

La commessa riguarda il primo pilota, non il catalogo completo. Città, edifici, mare, fiumi e altri16 file ipotizzati per il futuro non sono richiesti. Il perfezionamento e l'integrazione nel generatore verranno dopo la revisione degli asset.
