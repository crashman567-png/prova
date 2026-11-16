# Protocollo di lancio, test e scala (solo Stefano)

Questo file non entra mai nel documento del cliente. Sintetizza Revel Loughlin (struttura e disciplina di test), Sam Piliero (concept, struttura a pack, scala) e Alex Hormozi (produzione e riciclo dei vincitori). Dove una regola e' una nostra sintesi c'e' scritto "Interpretazione".

Indice: 0. Numeri prima di lanciare · 1. Struttura in base al budget · 2. Come si giudica · 3. Dopo il primo vincitore · 4. Scalare · 5. Retargeting e obiezioni · 6. Ciclo di feedback · 7. Naming e tracciamento · 8. Esperimenti aperti

## 0. Numeri prima di lanciare

- **Il risultato vero.** Per ogni cliente si definisce prima su cosa si giudica: posto prenotato, abbonamento, iscrizione, call prenotata. Il costo per lead e' solo un segnale intermedio.
- **Il tetto.** Valore di una vendita × % di lead che diventano vendita = costo per lead massimo sostenibile. Il tetto operativo si tiene sotto, in modo che la spesa rientri gia' dal primo incasso (Revel). Le formule complete sono nella skill `revel-meta-leadgen`, `references/unit-economics-e-diagnosi.md`.
- **Budget minimo per ad.** Il tetto di costo per lead diviso 4. Cosi' in 4 giorni ogni ad spende almeno un tetto, il minimo per una decisione keep/kill sensata.
  - Esperienza di Stefano: non scendere sotto circa 10 € al giorno; in molte nicchie locali 10-25 € bastano.
  - Interpretazione derivata dalle soglie di Revel, convertite da AUD a euro.
- **I prodotti a biglietto basso fanno eccezione.** Esperienze e abbonamenti possono andare benissimo con lead molto economici. Art of Waves: 420 lead a 0,42 €, 12 posti su 12 in 13 giorni, 179 € spesi per 9.480 € incassati.
  - La regola di Revel "lead sotto i 25 AUD = basso intento" nasce da servizi venduti con una call.
  - Si giudica sempre sul risultato vero.

## 1. Struttura in base al budget

**Da circa 20-30 € al giorno in su: metodo M4 di Piliero.** Dettagli nella skill `piliero-meta-ads`.
- Una campagna di prospecting con budget di campagna (CBO). Chi ha gia' visitato resta dentro. A parte c'e' solo la retention, e solo se c'e' riacquisto vero.
- Un **pack** (ad set) per avatar + concept: un body con 2-8 hook come ads separate. Gli avatar non si mescolano mai nello stesso pack.
- Ogni nuovo batch di creativita' va in un **pack nuovo**. Mai aggiungere ads a un pack vecchio, mai duplicare i vincitori.
- **Minimo del pack nuovo:** il piu basso tra 1 costo per lead target e il 20 % del budget, contando tutti i minimi attivi. Si tiene per 7 giorni, poi si toglie e l'ad set resta attivo.
- Con 20-50 € al giorno questo vuol dire un pack in test alla volta, con minimi di 4-10 € al giorno.
- I pack in calo non si spengono: si mette un tetto massimo di spesa in percentuale (maximum).

**Sotto i 20 € al giorno, oppure offerte da oltre circa 1.000 € a vendita: metodo Revel.**
- Campagna con budget a livello di ad set (ABO), un **ad set per concept**, con **un ad**: l'hook che si ritiene migliore. Ogni ad sopra il minimo (tetto diviso 4, mai sotto circa 10 €).
- Se i concept sono piu di quanti il budget ne regge, si lanciano a ondate di 4 giorni.
- Perche':
  - a 10-20 € al giorno i minimi di Piliero diventano quasi simbolici e le decisioni slittano a 14-21 giorni, mentre un ad per ad set si legge prima;
  - per il biglietto alto Piliero stesso ammette l'ABO, perche' "creative learnings" arrivano troppo lentamente.

**Sempre, qualunque sia il budget:**
- dal prospecting si escludono clienti e lead gia' presenti nel CRM;
- placement aperti, salvo click accidentali (Revel);
- niente interessi: il targeting lo fanno l'avatar chiamato in causa e la creativita' (tutti e tre gli autori, con sfumature);
- creative enhancements Advantage+:
  - Revel li spegne tutti;
  - Piliero spegne quelli che modificano immagine o video e tiene quelli che aggiungono elementi intorno (overlay, miglioramenti del testo);
  - generazione di immagini spenta per entrambi;
- per landing e form esterni serve la Conversions API, se no i numeri in Ads Manager non sono affidabili (Revel).

## 2. Come si giudica

- **Con l'ABO, giorno 4, keep or kill.** Ogni ad, o concept, si confronta con il tetto (Revel). Nei giorni 1-3 si guarda ma non si tocca.
- **Con i pack, giorno 7** (Piliero):
  - un pack che ha speso esattamente il suo minimo e' un probabile perdente: si toglie il minimo e lo si lascia svanire, senza pausa;
  - un pack che ha speso oltre e' candidato vincente;
  - con budget piccoli la conferma arriva al giorno 14 (adattamento nella skill `piliero-meta-ads`).
- **Vincitore.** In CBO un pack vince se spende piu' del 5 % del budget di campagna ed e' entro il tetto (Piliero).
- **Hit rate.** Un hit rate normale e' circa il 5 %, cioe' circa un vincitore ogni 20 ads. Si misura per cliente e per batch.
- **Segnale.** Secondo l'insider di Meta servono 40-50 conversioni per un segnale forte.
  - Gli account piccoli raramente ci arrivano: le modifiche costano poco, ma un giudizio al giorno 1-2 resta rumore.
  - Ogni modifica fa riapprendere il sistema: si cambia quando il guadagno atteso supera quella perdita.
- **Vincitori.** Si fanno correre a lungo. Hormozi: "use and abuse it until it doesn't work at all". Si spengono solo quando superano il tetto in modo stabile.

## 3. Dopo il primo vincitore: profondo (Hormozi + Piliero)

- **70/20/10** (Hormozi). Ogni nuova produzione si divide cosi':
  - 70 % varianti del vincitore:
    - l'hook vincente trapiantato sugli altri body;
    - nuovi hook sul body vincente;
    - lo stesso body detto da un'altra persona, in un altro luogo o con un altro ritmo;
  - 20 % idee vicine: un nuovo angolo per lo stesso avatar;
  - 10 % esperimenti: un nuovo avatar o un formato nuovo.
- **Trapianto.** Si archiviano hook e body come file separati, come fa gia' il sistema. A ogni giro si rimonta l'hook vincente sugli altri body (Hormozi: i primi 3 secondi dei vincitori incollati su "another 100 plus ads").
- **Varianti solo estetiche.** Filtro, font, bianco e nero valgono poco per Andromeda (interpretazione condivisa da Hormozi e Piliero nelle rispettive note). Le varianti devono cambiare persona, luogo, primo fotogramma o vibe: "mimic but change the vibe".
- **Prima largo, poi profondo** (Piliero): nuovi concept finche' uno vince, poi iterazioni di quello, e in parallelo un nuovo angolo.

## 4. Scalare

- **Orizzontale** (Revel): nuovi ad set con concept o iterazioni nuove, invece di gonfiare il budget del vincitore. Riduce il rischio di restare con un solo ad.
- **Verticale** (Piliero), quando il costo per risultato e' molto sotto il tetto:
  - 30-50 % sotto: +20-40 %;
  - a tetto: +10-20 %;
  - si decide su finestre di 3-4 giorni intorno ai 100 €/giorno, piu' lunghe se arrivano pochi risultati.
  - Interpretazione: Piliero ragiona in ROAS e qui la regola e' tradotta in costo per lead.
- **Dopo ogni aumento** si guardano CPC, costo per visualizzazione della landing, costo per lead e costo per risultato. Se sale solo l'ultimo anello si aspetta; se salgono tutti, si ritira l'aumento.

## 5. Retargeting e obiezioni (Hormozi, Piliero)

- **Con budget piccoli: niente campagna di retargeting a parte.**
  - Nel metodo M4 di Piliero (luglio 2026) chi ha gia' visitato resta nella campagna di prospecting.
  - Revel mette tutto nello stesso ad.
  - I moduli O1-O4 (un'obiezione per video) vanno in un pack "fondo del funnel", oppure si montano dentro le ads principali.
- **Con budget grandi e pubblico caldo numeroso** si puo' tenere un ad set separato e stabile con O1-O4 e un riepilogo dell'offerta: prezzo, risultato, rischio azzerato, una scadenza vera. Il pubblico e' piccolo e si rinnova, quindi la stessa creativita' regge a lungo (Hormozi).
- **Retention** (clienti che riacquistano: rinnovi CSA, ospiti che tornano): campagna piccola a parte, solo con una lista di almeno circa 1.000 persone.

## 6. Ciclo di feedback

- **Commenti, DM, domande su WhatsApp e motivi di non prenotazione** diventano il prossimo batch: una nuova obiezione, un nuovo body (Hormozi).
- **Prima di ogni cliente nuovo** si cercano nella Meta Ads Library le ads piu' longeve della nicchia, nei paesi del cliente: "the longer the ad's been running the more likely that ad has worked" (Hormozi).
- **Organico:**
  - i reel migliori del cliente diventano ads con un banner di CTA (Hormozi, Piliero);
  - 3-5 hook si possono pre-testare come reel o stories prima delle riprese definitive.
- **Le parole dei clienti** (chiamate, WhatsApp, recensioni) sono il carburante di hook e body. Revel considera le trascrizioni delle conversazioni di vendita "l'asset piu' sottoutilizzato".

## 7. Naming e tracciamento

- **Nomi:**
  - campagne `CLIENTE_PROSP` e `CLIENTE_RETARGET`;
  - ad set `P03_avatar_angolo_TOF` (o `BOF`);
  - ad `H04-B2-CTA1`, aggiungendo `-V2` se parla un'altra voce e `-P1` se c'e' un pretesto.
- **Foglio di tracciamento per ad:** spesa, risultati in Meta e nel CRM, costo per lead, risultati veri (prenotazioni, vendite), decisione. Cosi' si vede quale modulo vince.
- **Ogni 2 giorni** si confrontano i lead in Meta con quelli nel CRM: oltre il 10 % di scarto, si controlla il tracciamento (Revel).

## 8. Esperimenti aperti (dove gli autori non sono d'accordo)

1. **Hook con chiamata in causa diretta contro hook assumptivo**, a parita' di body e CTA.
   - Piliero: "If you're X person" fa arrivare l'ad a X.
   - Revel: meglio dare per scontato che chi guarda sia il cliente giusto e aggiungere un qualificatore.
   - Interpretazione: la chiamata in causa funziona se e' specifica (avatar + problema), non generica.
2. **Lo stesso body vincente in un pack CBO da 4-6 varianti contro 4-6 ad set ABO da un ad ciascuno**, confrontati sul costo per risultato a due settimane.
3. **Scala verticale contro orizzontale**, su due clienti con numeri simili.

Si registra l'esito in Notion (CRM cliente) a fine test, cosi' la regola diventa nostra.
