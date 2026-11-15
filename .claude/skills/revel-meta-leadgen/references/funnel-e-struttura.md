# Funnel e struttura

Indice: A. Funnel (A1 tre pezzi · A2 le quattro combinazioni · A3 quanta qualificazione · A4 lead form o landing · A5 evento di ottimizzazione · A6 come testare i funnel) · B. Struttura e budget (B1 processo di test · B2 scala orizzontale · B3 quando spegnere · B4 test a scaglioni · B5 geografia · B6 placement e impostazioni · B7 evoluzione 2025 → 2026)

## A. Funnel

### A1. I tre pezzi
Ogni funnel lead gen su Meta è fatto di: **tipo di ad** (immagine o video), **destinazione** (lead form nativo oppure landing/VSL), **livello di qualificazione** (numero e tipo di domande, più il lavoro dei setter).

### A2. Le quattro combinazioni

**1. Immagine → lead form**
- Regge solo con un follow-up feroce: chiamata entro 5 minuti (in orario lavorativo) o almeno un messaggio vocale entro 5 minuti.
- Le offerte irresistibili su immagine ("ti porto 10 clienti in 90 giorni o non paghi", "12 call in calendario in 30 giorni o non paghi") verso lead form o VSL sono "una pessima idea", a meno di avere setter esperti che chiamano a ciclo continuo entro 5 minuti. È l'unico scenario in cui Revel le ha viste funzionare.
- Lead economici, intento basso: "ti dimenticano entro 2 ore". La telefonata è il triage, ed è lì che avviene tutta la qualifica.
- Senza quella forza commerciale servono tantissime domande e tanti contatti: almeno 14 nella prima settimana.

**2. Immagine → landing/VSL**
- Usa il concept **us vs them**: una tabella "cosa succede se resti come sei" vs "cosa succede se lavori con noi o applichi questi cambiamenti". Va sempre verso una landing.
- **Variante opt-in**: immagine → pagina di opt-in per un video-training gratuito su un tema specifico → pagina col video e, sotto, un grande bottone "prenota una call". Usata su un solo cliente, ma funziona così bene che lì hanno spento la campagna lead form.
- La sua vecchia versione, nata all'epoca del boom di ClickFunnels: "Ti insegno esattamente come imposto le campagne lead" → opt-in → pagina col video tattico → bottone "Prenota una call se è il momento giusto per parlarne". **Una VSL scritta per insegnare è un lead magnet.**

**3. Video → lead form**
- Lo sketchbook verso lead form "va benissimo": molte delle sue ads sono così.
- Un video che insegna qualifica già nei primi 10 secondi con l'hook assumptivo, quindi servono meno domande.
- Per le aziende di servizi per la casa parte spesso così: il modulo si monta in 30 minuti e porta cassa entro 4 giorni, senza costruire landing.

**4. Video → VSL (il "santo graal" di oggi)**
- **Talking head brevissimi (5-6 secondi)**: "Se hai il problema di non avere abbastanza lead ogni settimana, clicca sotto: ti mostro come posso aiutarti." Per un fitness coach: "Questo video è solo per uomini. Se vuoi perdere X chili in 12 settimane senza perdere [...], clicca sotto per maggiori informazioni."
- Ipotesi di Revel, non verificata: video così brevi hanno un completion rate altissimo, quindi segnali di engagement forti, quindi CPM basso. A parità di budget raggiungi più persone e mandi più traffico alla VSL, che fa il lavoro pesante con le domande.
- In questa combinazione funzionano anche l'us vs them in video (l'immagine con un talking head in green screen sopra) e lo sketchbook.
- Risultato con l'evento sequence: 74 $ per call prenotata "senza compromettere la qualità".

### A3. Quanta qualificazione
- **La prima domanda** che Revel fa a ogni cliente: quanto è robusto ed esperto il team di appointment setting e follow-up?
- **Lo spettro:**
  - Da un lato, un'immagine si "consuma" in 3 secondi. Con poche domande arrivano tanti lead a basso intento (sotto 25 $ a lead): può funzionare, ma solo con un follow-up aggressivo.
  - Dall'altro, un video che insegna (anche 5 minuti, una lunghezza comune per lui) qualifica senza dirlo, e chi lo guarda fino in fondo è un clic di tutt'altra qualità. Lì bastano 2-3 domande.
- **La scelta:** pagare di più per un lead qualificato a monte, con più filtri prima di poter prenotare, oppure pagare poco e qualificare a valle con le persone.
- **Come chiedere:**
  - Mai "qual è il tuo budget?" in modo diretto: non c'è ancora abbastanza fiducia, è troppa resistenza. Chiedilo in modo indiretto, per esempio "Hai investito tra 10 e 30K in Facebook ads negli ultimi 3 mesi?".
  - Le domande sull'**obiettivo** funzionano meglio di quelle sull'"intenzione di cambiare". Nel caso del broker di mutui: "estinguere prima il mutuo / costruire un portafoglio immobiliare / entrambi".
  - Usa la logica condizionale per escludere chi non è idoneo (soglie di fatturato, importo del mutuo, tipo di business).
- I tipi di domande di qualifica nel dettaglio Revel li ha rimandati a un altro video: vedi le Lacune in `fonti-e-casi-studio.md`.

### A4. Lead form o landing?
- Senza una landing o VSL provata → **lead form**: velocità di lancio e cassa. "La velocità di lancio è molto importante per i clienti, a patto di rispettare la qualità del lavoro."
- Se sai costruire una landing (anche "vibe-coded" con Claude) e collegare pixel e Conversions API end-to-end → **landing**.
- Entrambe le strade funzionano. Dopo l'aggiornamento di Apple sulla privacy (ATT) Revel era passato ai lead form, poi è tornato anche alle conversion campaign: "ho due strade per lo stesso problema".
- Speculazione sua: un lead form e una conversion campaign colpiscono "pezzi" diversi dello stesso pubblico anche con ads e targeting identici.
- **CAPI è obbligatorio** se mandi traffico a una landing. Il beneficio principale è vedere numeri più accurati in Ads Manager: con un event match quality più alto Meta attribuisce più risultati ad ads e ad set, e tu non prendi decisioni su dati sbagliati. Che Meta "trovi più persone simili" grazie alla CAPI è secondo lui più merito dell'ad e del livello di spesa.

### A5. Evento di ottimizzazione

| Evento | Quando | Come |
|---|---|---|
| **Lead** (opt-in o invio del modulo) | Per partire, quando niente funziona, sotto circa 100 $/giorno | Offri comunque la prenotazione (thank-you page) ma non ottimizzare per quella; chiama tutti i lead, perché la maggior parte non prenota da sola. Lo scopo non è "far imparare Meta": è vedere ogni mattina un numero nella colonna risultati per capire quali ads generano lead. Entro 7 giorni conti le call uscite da quella campagna |
| **Schedule** (call prenotata) | Flusso di lead costante settimana su settimana e circa 300-500 $/giorno | Sposta 100-150 $/giorno su una seconda campagna ottimizzata per schedule, per "coprire la scommessa" e cercare un costo per call più basso senza toccare quello che funziona |
| **Sequence** (lead + call nello stesso ad set) | Dove disponibile: funzione nuova, che Revel ha visto comparire verso settembre-ottobre 2026 e che non tutti gli account hanno | A livello di ad set, scegliendo "massimizza il numero di lead qualificati" con CRM e Conversions API collegati. Meta vede sia i lead sia le call prenotate. Verifica nome e disponibilità in Ads Manager |

**Risultati del sequence**: a parità di ads, landing, VSL e copy, cambiando solo l'evento il costo per call è sceso di circa 100 $; un cliente paga 67-77 $ per call, un altro 74 $. Per Revel è "la cosa più vicina a un trucco" per ottimizzare sulle call. Risolve il problema dei budget piccoli, dove giudicare sulle call richiederebbe 10 giorni per ad.

**Se lead e call divergono molto**: troppe domande o troppa frizione? L'ad promette una cosa diversa da quella che dice la VSL? Esempio di una ditta di coperture: una landing per ogni dolore, e tutte le ads di quel dolore portano lì.

**Il metro finale**: riduzione del costo per appuntamento o per call prenotata senza compromettere la qualità. "Le tue ads vanno giudicate solo su questo."

### A6. Come testare i funnel
- Concedi circa **4 giorni per funnel** e guarda il **flusso di lead**. Se non arriva, passa al successivo.
- **Storia vera.** Un cliente faceva oltre 100K al mese con i funnel DM. Con Revel, nell'ordine:
  1. DM: risultati pessimi in 4-5 giorni.
  2. DM con domande di qualifica: 4 giorni, niente.
  3. Lead form: niente, anche se nel solare funzionano benissimo.
  4. Landing VSL, quella che il cliente aveva già: da 6 settimane è il suo "pane quotidiano", redditizio.
- **Morale:** capita spesso che un funnel non dia abbastanza lead in rapporto alla spesa. Si decide con poche regole e in fretta, per non sprecare soldi.

## B. Struttura e budget

### B1. Il processo di lancio e test
- **Ad set e ad**: un ad per ad set, ciascuno con il suo budget (ABO). Ogni 4 giorni si tolgono i perdenti e si lasciano correre i vincenti.
- **Esempio a 100 $/giorno** (VSL nuova, ticket da 4K in su venduto in call):
  - 3 ad set da 30 $, ognuno con un video.
  - Tetto CPL di 65 $, preso dalla storia dell'account. Sotto il tetto l'ad continua.
  - Poi si controllano nel CRM le vendite e il cash generati dai lead del test. Per esempio 90 $ al giorno per 8 giorni fanno circa 720 $ spesi per una vendita da 5K.
  - A quel punto: "Ti va se spendo altri 30 $ al giorno per provare un altro ad?", e si ripete il processo.
- **Esempio a 1.000 $/giorno o più** (cliente in Germania):
  - 20 ads da 15 secondi, tutte a risposta diretta: hook assumptivo, richiamo veloce del dolore, offerta irresistibile, CTA.
  - La VSL e la landing fanno il lavoro pesante, con 5-6 domande.
  - Risultati: CPL circa 55 $, call auto-prenotata 164 $, scesa da 260 $ in un mese. Chi non prenota da solo viene chiamato dai setter in outbound.
  - Vantaggio pratico: niente 10 sketchbook da girare. 20 video da 15 secondi si fanno in un paio di giorni.

### B2. Scala orizzontale e riduzione del rischio
- **Perché non aumentare il budget** dei vincenti (per esempio da 30 a 36 $): Revel vuole ridurre il rischio, soprattutto in un anno di aggiornamenti e turbolenze. Preferisce riempire l'account di ads provate.
- **Cosa si ottiene**: lead flow costante, quindi nessun problema di volume. Questo crea il margine per spendere un 10 % in più in scoperta.
- **Consiglio tipo a fine incarico**: "D'ora in poi prendi il 10 % del budget mensile, o aggiungilo sopra, e mettilo sull'evento sequence o su ad types molto sperimentali".
- **Il rischio da evitare** è il lead flow che va a zero perché hai un solo ad provato.
- **Rory Sutherland (Alchemy)**: non gestire l'account al 100 % come un contabile. Dai il 10 % del budget a un creativo "strano" e lascialo fare. Sbaglierà molte volte, ma l'unica volta che ha ragione sei in testa al gruppo, perché è lui che trova gli outlier.

### B3. Quando spegnere
- **Di norma al giorno 4.**
- **Prima** solo se le unit economics lo permettono: budget grandi (per esempio 1.000 $/giorno) con un CPL qualificato storico basso (per esempio 30 $), tipico di pubblici grandi e offerte che parlano a tanti.
- **Più tardi** (5 giorni o più) quando giudichi sulle call e il costo per call è alto.
- **La regola di kill chiara** serve a non reagire ai numeri del giorno 1.
- **Se funziona, non toccarlo.**
- **Learning phase**: Revel dice di non preoccuparsene.

### B4. Test a scaglioni
- Non metti mai un ad senza almeno 30 $/giorno. 4 ads quindi vogliono dire 120 $/giorno.
- **Esempio**: un cliente immobiliare con 20 ads e budget fisso. Sono state testate 7 ads nei primi 4 giorni, 7 nei 4 successivi e 6 negli ultimi 4: 20 ads validate in 12 giorni con la stessa spesa giornaliera.
- **Perché non CBO**: "Voglio sapere se ognuna di queste ads, per cui abbiamo messo sforzo, risorse e tempo, è buona o cattiva", quindi serve un test equo con budget proprio.
- Cambiare CBO/ABO "raramente è la soluzione". Il caso dell'agenzia con 13 ads era l'eccezione, l'"unicorno": lì la struttura soffocava tutto.

### B5. Geografia
- **Più stati o regioni**: campagne e budget separati per ciascuno, sempre. I motivi:
  - i lead si taggano facilmente per area;
  - regole o normative diverse non contaminano le altre campagne;
  - si possono fare offerte diverse e messaggi specifici per area.
- **Aree rurali e pubblici piccoli**: servono più ads e più produzione creativa. "Chi fa le ads per le zone rurali deve aspettarsi molto più lavoro."
- **Business locali** (dentista, solare): la rotazione creativa deve essere molto più alta di quella di un brand nazionale. I lead duplicati, cioè chi aveva già chiesto informazioni, al 5-10 % a settimana sono normali: sono una seconda occasione di vendita.
- **Lead fuori zona**:
  - Prima i dati, non l'aneddoto.
  - A circa 100 $/giorno si cambia qualcosa solo dopo 3 settimane di monitoraggio. In quel tempo vedi il calo, la turbolenza e la ripresa, e capisci se era un effetto stagionale (per esempio festività o turisti di passaggio).
  - Oltre 1.200-1.500 $/giorno i tempi si accorciano, per non perdere troppi soldi.
  - Soglia indicativa per intervenire: oltre il 10 % di lead fuori zona, in modo stabile.

### B6. Placement e impostazioni
- **Esclusioni**: Revel non esclude placement, salvo per i click accidentali.
  - Anni fa, un carosello di immagini verso un bot ManyChat: la gente cliccava per ingrandire le foto e finiva in Messenger.
  - Recentemente, le Instagram Stories in una campagna DM: togliendole è sparito almeno il 15 % dei click accidentali.
- **Immagini**: per il 90 % e oltre finiscono nel feed di Facebook e Instagram.
- **Video 9:16**: vanno nei feed ma spingono una buona parte della spesa anche sui Reels.
  - I **Reels di Facebook** sono il "cavallo nero" sottovalutato: per le aziende di servizi per la casa almeno il 30 % della spesa può e deve finire lì.
  - Le Stories hanno meno inventario.
- **Audience Network**: in 13 anni mai un problema di troppa spesa lì, probabilmente perché i suoi video sono lunghi.
- **Advantage+**: nel setup tiene spenti i creative enhancements e la generazione automatica dei testi.

### B7. Evoluzione 2025 → 2026 (vale la versione più recente)
- **Struttura di test**:
  - 2025 (dallo script di un suo ad): "almeno 4 ads alla volta, almeno 2 pubblici diversi, almeno 4 giorni".
  - 2026: un ad per ad set, niente pubblici per interessi, 4 giorni.
- **Audience Network**:
  - 2025: nel setup la deselezionava.
  - 2026: dichiara di non escludere placement, anche perché Meta ha reso impossibile escluderne alcuni. Decidi caso per caso, guardando i dati.
