# Brief completo per AI esterna — Drakelya Maps

Sei un illustratore di asset modulari per Drakelya Maps. Non hai bisogno del repository: tutti i riferimenti necessari sono in questo pacchetto.

OBIETTIVO
Avvicinare la qualità pittorica alla reference originale reference/DRAKELYA_VISUAL_TARGET.jpg: suolo ocra/oliva articolato, valli e pieghe lunghe, rocce grigio-calde, boschi irregolari e continuità visiva fra figure e terreno. Servono componenti ricombinabili per una mappa generativa 2D veloce. Non produrre una mappa intera o un paesaggio indivisibile. La qualità del target guida il lavoro; la sola quantità di dettagli non dimostra di averla raggiunta.

GERARCHIA DELLE REFERENCE
1. DRAKELYA_VISUAL_TARGET.jpg: obiettivo visivo primario, non sprite da ritagliare e rivendere.
2. Le sorgenti incluse: forme e pittura da adattare. Correggerne incoerenze, non replicarne gli errori.
3. target-vs-current.webp: a sinistra target, a destra risultato attuale criticato. Le geografie differiscono; è un confronto qualitativo. NON imitare la colonna destra.
Le tavole hanno etichette e scacchiere diagnostiche: non dipingerli negli asset. Le vecchie istruzioni contenute nei README sorgenti documentano esperimenti passati e non prevalgono su questa commessa.

STILE COMUNE
Illustrazione cartografica 2D pittorica in vista obliqua: sommità e versanti leggibili, orizzonte assente, segno sottile bruno-grigio nelle pieghe e lavaggi delicati. Forme naturali asimmetriche, terra visibile fra i gruppi. Niente CGI, fotografia, pixel art, plastica lucida, contorni neri uniformi, pavimenti a rombo o griglie isometriche.
Luce proposta: alta da destra, NE del foglio, ombre proprie verso basso-sinistra. È una scelta da verificare sui due campioni, non una misura certa della reference. I vecchi sorgenti possono avere luce NW: armonizzali senza ruotare o specchiare le figure. I tile di terreno non devono contenere ombre direzionali forti.
Pigmenti comuni: ocra/oliva per pianura, terra calda, roccia grigio-calda con luci crema, chiome scure e variate. I colori HEX nelle singole schede sono ancore cromatiche, non una palette indicizzata rigida. Mantieni un fondo più quieto delle cime. Niente verde brillante universale, oro dominante, bordi bianchi o nero puro usato come chiave.

CONTATTO COL TERRENO
Non disegnare un piedistallo, un disco, un rettangolo o un ampio grembiule verde sotto ciascun soggetto. Le basi condivise sono file separati. Il piede dei rilievi è sottile e interrotto, con cime e creste integre: non cancellare una grossa fascia inferiore, perché il compositore applicherà la sua sfumatura. I margini forestali si alleggeriscono attraverso vuoti e alberi piccoli, non sfocando chiome e tronchi.
Le irregolarità del terreno attuale non vanno imitate né nascoste dentro nuovi PNG giganteschi. Non inserire città, acqua, strade o testi nei moduli di terreno. Non sono richiesti nuovi edifici né acqua in questo lotto.

FORMATO DI CONSEGNA
PNG a 8 bit per canale, sRGB, alfa non premoltiplicata, nomi e dimensioni finali esatti. Cinque tile completamente opachi e seamless X/Y; dieci componenti con alfa reale, sagoma completa e almeno 24–32 px liberi su tutti i lati (32 per MASSIF/SADDLE). Nessun pixel dipinto sul bordo esterno dei ritagli, nessun fondo bianco/nero/scacchiera/chroma key. DPI irrilevante; 72 nominale se necessario.
Se il servizio genera solo misure standard, conserva l'originale e prepara il canvas finale senza stirare la figura: padding trasparente per i ritagli, lavorazione seamless per i tile. Se non puoi ottenere vera trasparenza o dimensioni finali, dichiara il limite e marca il risultato NON PRONTO; non simulare l'alfa con uno sfondo dipinto. Un upscale non vale come nuovo dettaglio; rotazioni e mirror non valgono come nuove varianti.

SCALA E COMPOSIZIONE
Riferimento visivo: picco maggiore alto 1; sella 0.25–0.55, collina 0.20–0.40, albero maturo 0.12–0.25. Sono proporzioni di prova della parte dipinta, non altezze geografiche. Verifica le forme anche con il master ridotto proporzionalmente a larghezza 512 px e a piccola scala cartografica. Non schiacciare gli asset per ottenere la proporzione.

CONFINI DEL LAVORO
Produci immagini e documentazione di consegna, nessun codice o modifica al motore. Gli ID ART-* sono nomi di commessa. Materiali RGB e basi avranno bisogno di integrazione successiva: non dichiarare gli asset già integrati, una mappa realmente generata o prestazioni misurate. Non inventare seed, diritti, misure o risultati di QA. Dichiara modello/servizio/versione se disponibili e le sorgenti effettivamente usate.

## Distinta esatta

| File | Dimensioni | Alfa | Tipo |
|---|---:|---|---|
| ART-MOUNTAIN-MASSIF-01.png | 832×672 | Trasparenza reale | Adattamento |
| ART-MOUNTAIN-SADDLE-01.png | 832×338 | Trasparenza reale | Adattamento |
| ART-SOIL-PLAIN-01.png | 512×512 | Opaco, seamless X/Y | Adattamento |
| ART-SOIL-EARTH-01.png | 512×512 | Opaco, seamless X/Y | Adattamento |
| ART-SOIL-DRY-01.png | 512×512 | Opaco, seamless X/Y | Adattamento |
| ART-SOIL-MINERAL-01.png | 512×512 | Opaco, seamless X/Y | Adattamento |
| ART-SOIL-FOREST-01.png | 512×512 | Opaco, seamless X/Y | Nuovo |
| ART-HILL-GRASS-A.png | 1024×448 | Trasparenza reale | Adattamento |
| ART-HILL-GRASS-B.png | 1024×448 | Trasparenza reale | Adattamento |
| ART-HILL-DRY-A.png | 1024×448 | Trasparenza reale | Adattamento |
| ART-HILL-DRY-B.png | 1024×448 | Trasparenza reale | Adattamento |
| ART-BASE-MOUNTAIN-TEMPERATE-01.png | 1024×256 | Trasparenza reale | Nuovo |
| ART-BASE-MOUNTAIN-DRY-01.png | 1024×256 | Trasparenza reale | Nuovo |
| ART-FOREST-EDGE-OPEN-01.png | 768×384 | Trasparenza reale | Adattamento |
| ART-FOREST-EDGE-INLET-01.png | 768×384 | Trasparenza reale | Adattamento |

## 1. ART-MOUNTAIN-MASSIF-01

FASE1: esegui solo questo campione; terminati i due high/low fermati e richiedi revisione prima degli altri13.

ASSET: ART-MOUNTAIN-MASSIF-01.png
Dimensioni finali: 832×672 px.
Tipo: Adattamento.
Palette di riferimento: #DDD0AC, #B8AB88, #77705A, #585848, #A49776.

Massiccio alto asimmetrico: un picco dominante, spalle e cime secondarie diseguali. Parti dal kit v4 massif.webp e dal suo massif-source.png; conserva la sagoma e la struttura riconoscibile, correggendo palette, luce e contatto. Corpo di riferimento 768×608, aggiungi almeno 32 px trasparenti per lato senza deformarlo. Contieni l’oro; conserva roccia e creste complete. Nessuna fila di picchi identici.

Ulteriori vincoli di famiglia: Conservare la differenza high/low del kit v4; armonizzare oro/roccia, luce e piedi, rimuovere frange. Massa integra, nessun grembiule enorme o paesaggio incorporato. Non clonare cinque picchi identici.
Trasparenza: Alfa reale; minimo 24–32 px liberi sui lati del master, sagoma completa, nessun frammento del vicino o fondo incorporato. Piede integro con bordo interrotto; evitare doppia sfumatura col runtime.
Riferimenti dichiarati: art-source/manual-mountain-kit-v4/massif.webp; art-source/manual-mountain-kit-v4/saddle.webp; kit v4 source PNG; W-REL-001 (controllo dettaglio); target: ROI 07. Gli ID si risolvono in dati/MAPPA_SORGENTI.json.

Consegna il PNG singolo, originale del servizio se diverso, record metadati e anteprima di controllo separata. Non dipingere il nome file sul disegno.

## 2. ART-MOUNTAIN-SADDLE-01

FASE1: esegui solo questo campione; terminati i due high/low fermati e richiedi revisione prima degli altri13.

ASSET: ART-MOUNTAIN-SADDLE-01.png
Dimensioni finali: 832×338 px.
Tipo: Adattamento.
Palette di riferimento: #DDD0AC, #B8AB88, #77705A, #585848, #A49776.

Sella bassa complementare al massiccio, due spalle diseguali e apertura centrale leggibile. Parti dal kit v4 saddle.webp e saddle-source.png. Corpo di riferimento 768×274, almeno 32 px trasparenti per lato, senza stiramento. Conserva il disegno high/low come famiglia; non trasformarla in un altro picco alto.

Ulteriori vincoli di famiglia: Conservare la differenza high/low del kit v4; armonizzare oro/roccia, luce e piedi, rimuovere frange. Massa integra, nessun grembiule enorme o paesaggio incorporato. Non clonare cinque picchi identici.
Trasparenza: Alfa reale; minimo 24–32 px liberi sui lati del master, sagoma completa, nessun frammento del vicino o fondo incorporato. Piede integro con bordo interrotto; evitare doppia sfumatura col runtime.
Riferimenti dichiarati: art-source/manual-mountain-kit-v4/massif.webp; art-source/manual-mountain-kit-v4/saddle.webp; kit v4 source PNG; W-REL-001 (controllo dettaglio); target: ROI 07. Gli ID si risolvono in dati/MAPPA_SORGENTI.json.

Consegna il PNG singolo, originale del servizio se diverso, record metadati e anteprima di controllo separata. Non dipingere il nome file sul disegno.

## 3. ART-SOIL-PLAIN-01

FASE2: esegui questa scheda soltanto dopo approvazione esplicita di MASSIF e SADDLE.

ASSET: ART-SOIL-PLAIN-01.png
Dimensioni finali: 512×512 px.
Tipo: Adattamento.
Palette di riferimento: #B8A848, #C8B858, #A89848, #887838.

Pianura ocra/oliva con lavaggi ampi e micrograna tenue: niente prato verde brillante, colline dipinte, oggetto centrato o macchia ripetuta dominante. Usa W-TEX-001/GRASS-SOFT e il suolo della reference come riferimenti.

Ulteriori vincoli di famiglia: Pigmento basso contrasto a scale larghe/medie/minute; terreno vuoto, niente erba a ciuffi o colline dipinte.
Trasparenza: Interamente opaco (A=255), seamless su X/Y; nessun bordo/margine trasparente, oggetto riconoscibile, ombra direzionale o macchia ripetuta dominante.
Riferimenti dichiarati: W-TEX-001; W-TEX-GRASS-SOFT; target: ROI 01/02. Gli ID si risolvono in dati/MAPPA_SORGENTI.json.

Consegna il PNG singolo, originale del servizio se diverso, record metadati e anteprima di controllo separata. Non dipingere il nome file sul disegno.

## 4. ART-SOIL-EARTH-01

FASE2: esegui questa scheda soltanto dopo approvazione esplicita di MASSIF e SADDLE.

ASSET: ART-SOIL-EARTH-01.png
Dimensioni finali: 512×512 px.
Tipo: Adattamento.
Palette di riferimento: #B99A5B, #C6AA6A, #9B7D4D, #7E6B48.

Terra calda esposta, polvere e pietruzze minute. Niente solchi agricoli, filari o chiazza circolare. Adatta il ruolo di W-TEX-002 alla famiglia cromatica comune.

Ulteriori vincoli di famiglia: Terra/polvere irregolare e pietruzze minute; niente solchi a filari o chiazza circolare.
Trasparenza: Interamente opaco (A=255), seamless su X/Y; nessun bordo/margine trasparente, oggetto riconoscibile, ombra direzionale o macchia ripetuta dominante.
Riferimenti dichiarati: W-TEX-002; target: ROI 03/04. Gli ID si risolvono in dati/MAPPA_SORGENTI.json.

Consegna il PNG singolo, originale del servizio se diverso, record metadati e anteprima di controllo separata. Non dipingere il nome file sul disegno.

## 5. ART-SOIL-DRY-01

FASE2: esegui questa scheda soltanto dopo approvazione esplicita di MASSIF e SADDLE.

ASSET: ART-SOIL-DRY-01.png
Dimensioni finali: 512×512 px.
Tipo: Adattamento.
Palette di riferimento: #C6AA6A, #B49A68, #928457, #77694A.

Suolo arido temperato senza erba incorporata, con variazioni terrose e minerali. Non deve diventare automaticamente deserto con dune e cactus. W-TEX-002/004 e terreno nudo del v2 sono riferimenti.

Ulteriori vincoli di famiglia: Ocra minerale asciutta, nessuna duna grande o grembiule verde; grana contenuta.
Trasparenza: Interamente opaco (A=255), seamless su X/Y; nessun bordo/margine trasparente, oggetto riconoscibile, ombra direzionale o macchia ripetuta dominante.
Riferimenti dichiarati: W-TEX-002; W-TEX-004; art-source/illustrated-v2/terrain-atlas.png: row3 col3. Gli ID si risolvono in dati/MAPPA_SORGENTI.json.

Consegna il PNG singolo, originale del servizio se diverso, record metadati e anteprima di controllo separata. Non dipingere il nome file sul disegno.

## 6. ART-SOIL-MINERAL-01

FASE2: esegui questa scheda soltanto dopo approvazione esplicita di MASSIF e SADDLE.

ASSET: ART-SOIL-MINERAL-01.png
Dimensioni finali: 512×512 px.
Tipo: Adattamento.
Palette di riferimento: #A49776, #B8AB88, #77705A, #585848.

Suolo grigio caldo e detrito minuto, non una distesa di massi identici o il disegno di un mucchio di rocce. Usa W-TEX-003 come riferimento del ruolo, armonizzato al pedemonte.

Ulteriori vincoli di famiglia: Pietra frammentata e terra grigio-calda, senza un ammasso di massi centrato.
Trasparenza: Interamente opaco (A=255), seamless su X/Y; nessun bordo/margine trasparente, oggetto riconoscibile, ombra direzionale o macchia ripetuta dominante.
Riferimenti dichiarati: W-TEX-003; P2D-SCREE-A/B/C; target: ROI 06. Gli ID si risolvono in dati/MAPPA_SORGENTI.json.

Consegna il PNG singolo, originale del servizio se diverso, record metadati e anteprima di controllo separata. Non dipingere il nome file sul disegno.

## 7. ART-SOIL-FOREST-01

FASE2: esegui questa scheda soltanto dopo approvazione esplicita di MASSIF e SADDLE.

ASSET: ART-SOIL-FOREST-01.png
Dimensioni finali: 512×512 px.
Tipo: Nuovo.
Palette di riferimento: #777347, #8C8350, #535A35, #A0925F.

Nuovo suolo boschivo di terra/lettiera e muschio rado, senza alberi. Terra leggibile, niente disco verde scuro. Deve ricevere i due margini boschivi senza salto cromatico.

Ulteriori vincoli di famiglia: Lettiera, terra ocra e piccole chiazze muschio; nessun albero, radice gigante o cerchio scuro.
Trasparenza: Interamente opaco (A=255), seamless su X/Y; nessun bordo/margine trasparente, oggetto riconoscibile, ombra direzionale o macchia ripetuta dominante.
Riferimenti dichiarati: target: ROI 08; P2D-FOREST-EDGE (solo palette); materiale procedurale forest: non è un file sorgente. Gli ID si risolvono in dati/MAPPA_SORGENTI.json.

Consegna il PNG singolo, originale del servizio se diverso, record metadati e anteprima di controllo separata. Non dipingere il nome file sul disegno.

## 8. ART-HILL-GRASS-A

FASE2: esegui questa scheda soltanto dopo approvazione esplicita di MASSIF e SADDLE.

ASSET: ART-HILL-GRASS-A.png
Dimensioni finali: 1024×448 px.
Tipo: Adattamento.
Palette di riferimento: #B8A848, #C8B858, #A89848, #887838, #A49776, #B8AB88, #77705A, #585848.

Dorsale lunga con due/tre pieghe diseguali e una spalla più bassa; profilo basso, parte dipinta H/W circa 0.25–0.35. Usa W-REL-003/F03 e foothills come struttura. NON una montagna alpina miniaturizzata o un cono tondo. Continuità verso la pianura, niente parete o basetta chiusa.

Ulteriori vincoli di famiglia: A: dorsale lunga con 2–3 pieghe diseguali; B: gruppo più largo con avvallamento aperto. Cresta bassa, poche rocce, erba rada senza base chiusa.
Trasparenza: Alfa reale; minimo 24–32 px liberi sui lati del master, sagoma completa, nessun frammento del vicino o fondo incorporato. Piede integro con bordo interrotto; evitare doppia sfumatura col runtime.
Riferimenti dichiarati: W-REL-003/F02/F03; art-source/regional-landmarks-v1/foothills.png; target: ROI 05. Gli ID si risolvono in dati/MAPPA_SORGENTI.json.

Consegna il PNG singolo, originale del servizio se diverso, record metadati e anteprima di controllo separata. Non dipingere il nome file sul disegno.

## 9. ART-HILL-GRASS-B

FASE2: esegui questa scheda soltanto dopo approvazione esplicita di MASSIF e SADDLE.

ASSET: ART-HILL-GRASS-B.png
Dimensioni finali: 1024×448 px.
Tipo: Adattamento.
Palette di riferimento: #B8A848, #C8B858, #A89848, #887838, #A49776, #B8AB88, #77705A, #585848.

Gruppo collinare più largo con avvallamento aperto: struttura realmente diversa da A. Parte dipinta H/W circa 0.25–0.35. Usa W-REL-003/F02 e foothills come struttura. Pieghe lunghe asimmetriche; nessun cono, anello d’ombra o lobo uniforme.

Ulteriori vincoli di famiglia: A: dorsale lunga con 2–3 pieghe diseguali; B: gruppo più largo con avvallamento aperto. Cresta bassa, poche rocce, erba rada senza base chiusa.
Trasparenza: Alfa reale; minimo 24–32 px liberi sui lati del master, sagoma completa, nessun frammento del vicino o fondo incorporato. Piede integro con bordo interrotto; evitare doppia sfumatura col runtime.
Riferimenti dichiarati: W-REL-003/F02/F03; art-source/regional-landmarks-v1/foothills.png; target: ROI 05. Gli ID si risolvono in dati/MAPPA_SORGENTI.json.

Consegna il PNG singolo, originale del servizio se diverso, record metadati e anteprima di controllo separata. Non dipingere il nome file sul disegno.

## 10. ART-HILL-DRY-A

FASE2: esegui questa scheda soltanto dopo approvazione esplicita di MASSIF e SADDLE.

ASSET: ART-HILL-DRY-A.png
Dimensioni finali: 1024×448 px.
Tipo: Adattamento.
Palette di riferimento: #C6AA6A, #B49A68, #928457, #77694A, #A49776, #B8AB88, #77705A, #585848.

Versione della famiglia strutturale A ridisegnata in terra arida e roccia localizzata. Conserva la parentela di profilo, cambia i dettagli del substrato: non semplice ricolorazione del prato. Zero grembiule verde. Riferimento terrain-atlas v2: riga3 colonna3 e riga4 colonna3, contando dall’alto/sinistra a partire da1; le celle sono indizi visivi, non crop già approvati.

Ulteriori vincoli di famiglia: Le stesse due famiglie di profilo di H01 con roccia/terra nuda e arbusti minimi; ridisegno coerente, non filtro seppia o erba rimasta sul piede.
Trasparenza: Alfa reale; minimo 24–32 px liberi sui lati del master, sagoma completa, nessun frammento del vicino o fondo incorporato. Piede integro con bordo interrotto; evitare doppia sfumatura col runtime.
Riferimenti dichiarati: art-source/illustrated-v2/terrain-atlas.png: row3 col3, row4 col3; art-source/regional-landmarks-v1/foothills.png; H01. Gli ID si risolvono in dati/MAPPA_SORGENTI.json.

Consegna il PNG singolo, originale del servizio se diverso, record metadati e anteprima di controllo separata. Non dipingere il nome file sul disegno.

## 11. ART-HILL-DRY-B

FASE2: esegui questa scheda soltanto dopo approvazione esplicita di MASSIF e SADDLE.

ASSET: ART-HILL-DRY-B.png
Dimensioni finali: 1024×448 px.
Tipo: Adattamento.
Palette di riferimento: #C6AA6A, #B49A68, #928457, #77694A, #A49776, #B8AB88, #77705A, #585848.

Profilo della famiglia B con avvallamento aperto in terra arida, vuoti leggibili e roccia locale. Non semplice ricolorazione del prato e non una quarta forma casuale. Usa foothills e il pedemonte della reference. Niente anello, piedistallo o base verde.

Ulteriori vincoli di famiglia: Le stesse due famiglie di profilo di H01 con roccia/terra nuda e arbusti minimi; ridisegno coerente, non filtro seppia o erba rimasta sul piede.
Trasparenza: Alfa reale; minimo 24–32 px liberi sui lati del master, sagoma completa, nessun frammento del vicino o fondo incorporato. Piede integro con bordo interrotto; evitare doppia sfumatura col runtime.
Riferimenti dichiarati: art-source/illustrated-v2/terrain-atlas.png: row3 col3, row4 col3; art-source/regional-landmarks-v1/foothills.png; H01. Gli ID si risolvono in dati/MAPPA_SORGENTI.json.

Consegna il PNG singolo, originale del servizio se diverso, record metadati e anteprima di controllo separata. Non dipingere il nome file sul disegno.

## 12. ART-BASE-MOUNTAIN-TEMPERATE-01

FASE2: esegui questa scheda soltanto dopo approvazione esplicita di MASSIF e SADDLE.

ASSET: ART-BASE-MOUNTAIN-TEMPERATE-01.png
Dimensioni finali: 1024×256 px.
Tipo: Nuovo.
Palette di riferimento: #B99A5B, #C6AA6A, #9B7D4D, #7E6B48, #A49776, #B8AB88, #77705A, #585848.

Nuova fascia di terra e detrito condivisa sotto 2–4 rilievi: niente cima o intero paesaggio. Substrato terra/minerale con pochi toni oliva; estensioni diseguali ai lati, lingue e vuoti. Margine sfumato irregolare per circa12–25% del raggio locale e nucleo visibile. Nessun ovale continuo, ombra ellittica o grembiule verde.

Ulteriori vincoli di famiglia: Lavaggio largo e basso, detriti e vene di terra asimmetriche, vuoti laterali e bordo spezzato. Zero cime/alberi/corsi d’acqua; deve servire 2–4 figure, non ripetere un cerchio sotto ciascuna.
Trasparenza: Alfa reale su tutti i lati; margine irregolare morbido 12–25% del raggio locale; nessun disco, rettangolo, ombra ellittica, acqua o edifici incorporati.
Riferimenti dichiarati: target: ROI 03/06/07; W-REL-001/F02/F03; P2D-SCREE-A/B/C. Gli ID si risolvono in dati/MAPPA_SORGENTI.json.

Consegna il PNG singolo, originale del servizio se diverso, record metadati e anteprima di controllo separata. Non dipingere il nome file sul disegno.

## 13. ART-BASE-MOUNTAIN-DRY-01

FASE2: esegui questa scheda soltanto dopo approvazione esplicita di MASSIF e SADDLE.

ASSET: ART-BASE-MOUNTAIN-DRY-01.png
Dimensioni finali: 1024×256 px.
Tipo: Nuovo.
Palette di riferimento: #B99A5B, #C6AA6A, #9B7D4D, #7E6B48, #A49776, #B8AB88, #77705A, #585848.

Nuova fascia condivisa sotto 2–4 rilievi in ocra/minerale arido, priva di erba. Non un altro massiccio e non un’ellisse ricolorata. Bordi irregolari e vuoti, nucleo visibile, sfumatura esterna circa12–25% del raggio locale. Deve raccordarsi con i tile DRY/MINERAL senza linea chiusa.

Ulteriori vincoli di famiglia: Lavaggio largo e basso, detriti e vene di terra asimmetriche, vuoti laterali e bordo spezzato. Zero cime/alberi/corsi d’acqua; deve servire 2–4 figure, non ripetere un cerchio sotto ciascuna.
Trasparenza: Alfa reale su tutti i lati; margine irregolare morbido 12–25% del raggio locale; nessun disco, rettangolo, ombra ellittica, acqua o edifici incorporati.
Riferimenti dichiarati: target: ROI 03/06/07; W-REL-001/F02/F03; P2D-SCREE-A/B/C. Gli ID si risolvono in dati/MAPPA_SORGENTI.json.

Consegna il PNG singolo, originale del servizio se diverso, record metadati e anteprima di controllo separata. Non dipingere il nome file sul disegno.

## 14. ART-FOREST-EDGE-OPEN-01

FASE2: esegui questa scheda soltanto dopo approvazione esplicita di MASSIF e SADDLE.

ASSET: ART-FOREST-EDGE-OPEN-01.png
Dimensioni finali: 768×384 px.
Tipo: Adattamento.
Palette di riferimento: #485828, #384828, #283818, #758041, #777347, #8C8350, #535A35, #A0925F.

Gruppo aperto con3–7 chiome di altezze diverse, tronchi visibili e vuoti crescenti verso la pianura. Usa vegetation-atlas v2, riga2 colonne5/6 (conteggio1 dall’alto/sinistra), e P2D-FOREST-EDGE/SHRUB come riferimenti. Non includere un terreno esteso; conserva chiome e tronchi definiti. Niente siepe rettilinea, griglia o tappeto uniforme.

Ulteriori vincoli di famiglia: OPEN: 3–7 chiome di altezze diverse con vuoti crescenti verso il bordo; INLET: due piccoli lati diseguali e centro trasparente aperto per radura. Tronchi visibili, niente muro verde, niente terreno incorporato esteso.
Trasparenza: Alfa reale; minimo 24–32 px liberi sui lati del master, sagoma completa, nessun frammento del vicino o fondo incorporato. Piede integro con bordo interrotto; evitare doppia sfumatura col runtime.
Riferimenti dichiarati: art-source/illustrated-v2/vegetation-atlas.png: row2 col5/6; P2D-FOREST-EDGE; P2D-SHRUB; target: ROI 08. Gli ID si risolvono in dati/MAPPA_SORGENTI.json.

Consegna il PNG singolo, originale del servizio se diverso, record metadati e anteprima di controllo separata. Non dipingere il nome file sul disegno.

## 15. ART-FOREST-EDGE-INLET-01

FASE2: esegui questa scheda soltanto dopo approvazione esplicita di MASSIF e SADDLE.

ASSET: ART-FOREST-EDGE-INLET-01.png
Dimensioni finali: 768×384 px.
Tipo: Adattamento.
Palette di riferimento: #485828, #384828, #283818, #758041, #777347, #8C8350, #535A35, #A0925F.

Due lati boschivi diseguali con un rientro centrale trasparente da comporre come apertura di radura; aperture comunicanti col bordo, non un foro artificiale circondato da una corona identica. Stessa famiglia di OPEN, chiome e tronchi definiti, nessun fondo di terreno esteso o taglio al bordo. Riferimenti vegetation-atlas v2 e P2D-FOREST-EDGE/SHRUB.

Ulteriori vincoli di famiglia: OPEN: 3–7 chiome di altezze diverse con vuoti crescenti verso il bordo; INLET: due piccoli lati diseguali e centro trasparente aperto per radura. Tronchi visibili, niente muro verde, niente terreno incorporato esteso.
Trasparenza: Alfa reale; minimo 24–32 px liberi sui lati del master, sagoma completa, nessun frammento del vicino o fondo incorporato. Piede integro con bordo interrotto; evitare doppia sfumatura col runtime.
Riferimenti dichiarati: art-source/illustrated-v2/vegetation-atlas.png: row2 col5/6; P2D-FOREST-EDGE; P2D-SHRUB; target: ROI 08. Gli ID si risolvono in dati/MAPPA_SORGENTI.json.

Consegna il PNG singolo, originale del servizio se diverso, record metadati e anteprima di controllo separata. Non dipingere il nome file sul disegno.


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
