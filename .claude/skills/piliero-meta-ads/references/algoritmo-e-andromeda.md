# Come funziona l'algoritmo secondo Sam e le fonti Meta che intervista

Indice: 1. Retrieval e ranking · 2. Andromeda 2.0 · 3. Il messaggio fa il targeting · 4. Cosa conta come "diverso" · 5. Learning phase e segnali · 6. Cosa resta all'umano · 7. Affermazioni da prendere con cautela

## 1. Retrieval e ranking (Matt Steiner, Meta, giugno 2026)

- **Due stadi.** Prima il **retrieval** personalizzato sceglie, tra gli inserzionisti che ti possono raggiungere, le ads candidate. Poi il **ranking** le ordina.
- **Andromeda** e' il sistema di retrieval, "co-designed, the hardware, the software, and the machine learning model". E' nato per gestire la "Cambrian explosion of creatives" prodotta dall'AI generativa.
- **GEM** e' il foundation model da cui imparano i modelli del secondo stadio di ranking.
- **Adaptive ranking model:** usa piu' calcolo per chi interagisce e compra molto, meno per gli utenti leggeri.
- **Lattice:** fonde in un solo modello i modelli separati, per esempio click e conversioni, Facebook e Instagram.
- **Effetti visti negli account:** Sam li data da luglio 2025.

## 2. Andromeda 2.0 (annuncio di novembre 2026, da un white paper non verificato)

- Il retrieval instrada ogni ad verso "specialized expert models", con un giudizio quasi da ranking gia' nella selezione.
- La frase che conta per Sam: "it considers more of your ads you've made", quindi "less and less ads go all the way down to the bottom and never get any spend".
- **GEM** modella anche il percorso verso l'acquisto, cioe' quale sequenza di ads serve a una persona.
- Il white paper cita +8,3 % di click e +15,7 % di conversioni nel secondo trimestre 2026. Va verificato su fonti Meta.

## 3. Il messaggio fa il targeting

- **La formula di Sam:** "creative is the targeting" e' "way too broad". Meglio un "avatar-based system": "whomever you're talking to or calling out in the ad itself is who is going to be naturally targeted by that ad".
- **Avatar:** una persona con un insieme di problemi che il prodotto risolve, non una demografia. "new moms who have no time", non "donne 35+".
- **Come lo usa il retrieval:** abbina l'ad a chi corrisponde all'avatar chiamato in causa e ha storia o probabilita' di compiere l'evento scelto, "based on the millions of signals".
- **L'esempio di Sam:** lui, giovane con mal di schiena, non starebbe in nessun interesse "55 plus men", ma "if you just talk to the problems, it finds the people for you".
- **Conseguenza pratica:** chiamare l'avatar direttamente, anche nella forma "If you're X person". Contano anche chi compare nell'ad e linguaggio e "vibe" adatti all'eta'.

## 4. Cosa conta come "diverso"

- **Chidi (Meta, team Disruptors):** una creativita' nuova deve sembrare diversa da cio' che hai fatto finora ("it looks different"), oppure imitarlo con un body, una demo, un linguaggio o un'offerta diversi.
- **Matt Steiner:** per una persona contano poche varianti su molte. Serve "reasonable diversity", non volume. Meta prova tutte le varianti e sposta la spesa sulle migliori; quelle escluse non sono per forza cattive, solo "lower performant".
- **Sam:**
  - un'iterazione non e' "the same shoe with a different headline";
  - l'ad con piu' probabilita' di vincere e' simile a una che ha gia' vinto: "mimic but change the vibe".
- **Il caso flexible ads:** fallite perche' "the system just couldn't recognize when ads were similar to one another".
- **Interpretazione:** per l'algoritmo conta la differenza di messaggio (a chi parla, di quale problema), poi quella visiva complessiva. Un filtro o un font non bastano. Nessuno dei video parla di raggruppamento delle ads simili per entity ID: quell'idea viene da altri media buyer, non da Sam.

## 5. Learning phase e segnali

- **Le modifiche** fanno riapprendere il sistema: si cambia quando il guadagno atteso supera la perdita (Chidi).
- **Il segnale forte** arriva con 40-50 conversioni (Chidi, senza finestra temporale). Gli account piccoli raramente ci arrivano: le modifiche costano poco, ma il rumore e' alto.
- **"Learning limited"** e' accettabile; va evitato il "death loop" di pause e riavvii.
- **Ottimizza sull'evento piu' profondo standard:** l'algoritmo spinge esattamente l'evento scelto.

## 6. Cosa resta all'umano (Matt Steiner)

- "Humans are never going to out optimize the machine", ne' sposteranno budget piu' in fretta.
- Restano le idee, i messaggi nuovi per un pubblico e le ipotesi sul perche' qualcosa ha funzionato, da cui nascono nuove varianti.
- "Every change is AB tested", e il ritmo dei cambiamenti accelerera'.

## 7. Affermazioni da prendere con cautela

- **Il pixel** "gets trained off of negative events" (Sam, senza fonte Meta).
- **I post ID** che "don't transfer perfectly like they used to" (Sam).
- **Il white paper di Andromeda 2.0:** titolo, data e numeri non verificati.
- **Conflitto d'interessi:** Sam vende agenzia, community e un tool AI in affiliazione, e i suoi casi sono autodichiarati.
