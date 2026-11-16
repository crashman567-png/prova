# Testare con i pack: procedura, vincitori, perdenti, fatigue

Indice: 1. Cos'e' un pack · 2. Perche' non ABO e non creative testing · 3. La regola del minimo · 4. Procedura passo passo · 5. Leggere i risultati · 6. Vincitori, perdenti, fatigue · 7. Hit rate e volume

## 1. Cos'e' un pack

- **Pack = ad set = un concept:** un avatar + un angolo, con **4-8 ads** (luglio 2026: "More than that seems to be a little bit too crazy"; con meno "you might not be taking enough swings"). A febbraio diceva 2-8, a gennaio 2-12. Le ads sono di solito hook diversi sullo stesso video: "Hook one, hook two, hook three, and then iterations of those hooks".
- **Perche' si raggruppa per avatar e concept:** il raggruppamento "not only does the targeting for you, but it also groups the learnings together at the ad set level", senza interferire con gli altri pack. Senza, "your targeting is a little off".
- **Mai mescolare avatar diversi nello stesso pack.**
- **Concentrazione:** che una sola iterazione prenda quasi tutta la spesa del pack (7.300 $ su 7.382 $) e' "completely fine". Una spesa sparsa su molte ads e' "an indication that we haven't found a true winner".

## 2. Perche' non ABO e non creative testing

Sam considera "fundamentally broken" dopo GEM e Andromeda i tre metodi comuni:
1. **ABO con spesa forzata:**
   - l'operatore reagisce troppo lento e l'attribuzione mostra soprattutto l'ultimo tocco;
   - toglie budget ai vincitori, e "new ads have a lower hit rate than already scaled ads": "you're paying a premium to find winning ads".
2. **La funzione "creative testing" di Meta:** garantisce la delivery alle ads nuove. "We do not want insured delivery. This is a negative": la spesa si divide in parti uguali e "you are creating cost centers".
3. **CBO libera, senza minimi:** dopo Andromeda le ads nuove non ricevevano quasi spesa.

**L'eccezione:** ABO per biglietti oltre 1.000 $ per acquisto, lead gen inclusa.

## 3. La regola del minimo

- **Scopo del test:** "The simple purpose of testing is to find out if winners can scale." E "Proven is better than new": prima si spende sui vincitori attuali.
- **Il test perfetto** spende il meno possibile: "We don't need to spend 20% on testing. Get that out of your head."
- **Minimo del pack nuovo:** il piu' basso tra **1 CPA target al giorno** e il **20 % del budget totale** (in M1 il prospecting e' quasi tutto il budget), contando tutti i minimi attivi insieme ("we never want testing to represent more than 20% of our total account budget").
  - Esempi di Sam: CPA 47 $ con budget medio, minimo 47 $; budget 100 $ al giorno, minimo massimo 20 $.
  - Interpretazione: i pack in test in parallelo sono al massimo il 20 % del budget diviso il CPA. Con budget piccoli si testa un pack alla volta, con un minimo sotto 1 CPA e quindi un segnale piu' debole.
- **Durata:** 7 giorni, poi "we pause the minimum budget. We keep the ad set active. We just remove the minimum." Non preoccuparsi della learning phase quando si toglie.
- **Come si imposta:** ad set spending limits, minimo in valore in dollari ("use dollar value"), "average daily minimum".

## 4. Procedura passo passo

1. Prepara il batch: un concept (avatar + angolo) con 2-8 iterazioni, come ads separate.
2. Duplica un pack esistente, cancella le ads, rinominalo col numero successivo, carica le nuove.
3. Imposta il minimo (§3) e non toccare nulla per 7 giorni. Add to cart e initiate checkout sono segnali anticipatori; il verdetto e' sugli acquisti.
4. Al giorno 7 togli il minimo e lascia l'ad set attivo.
5. Leggi il risultato (§5).
6. Se e' un vincitore, lascialo dov'e': la CBO lo nutre. Ribriefa lo stesso concept: le nuove iterazioni vanno in un **pack nuovo**, mai in quello vecchio.
7. Se e' un perdente, non serve la pausa: la CBO lo affama da sola.
8. Lancia sempre creativita' nuova, perche' molti pack falliscono.
   - Cadenza: un pack nuovo "every one to two to three weeks consistent. Every week like a drum beat", cosi' "you always have one pack on a minimum consistently".
   - Interpretazione: 4-8 ads ogni 1-3 settimane fanno circa 6-32 ads nuove al mese. Sam non da' un numero mensile.

## 5. Leggere i risultati

- **Al giorno 7:**
  - un pack che ha speso esattamente il minimo e' un probabile perdente, che "fade down and die";
  - uno che ha speso oltre e' candidato vincente.
  - Col minimo un vincitore arriva prima al suo plateau, spesso con acquisti gia' nei primi giorni. Senza minimo puo' metterci 14, 21 o 30 giorni.
- **Lettura d'account, a intervalli:**
  1. togli i filtri, guarda tutte le ads ordinate per spesa;
  2. accanto al ROAS standard metti incremental purchases e ROAS incrementale ("Compare attribution settings" > incremental attribution);
  3. cerca spesa alta e ROAS incrementale alto.
  - Esempio: ad A, 7.500 $ e ROAS 2,6 (incrementale 2,3); ad B, 5.500 $ e ROAS 3,6 (incrementale 3). B e' la piu' scalabile.
- **Finestra di giudizio:** nulla si tocca per 7-14 giorni dopo il lancio ("We then wait around 7 to 14 days before we touch anything"); l'analisi si fa a 7-14 giorni con l'attribuzione incrementale.
- **Due livelli di giudizio, con scopi diversi:**
  - il **pack** (il concept) si giudica dalla spesa: al giorno 7, se ha speso solo il minimo, e' un probabile perdente. Serve a decidere se il concept ha mercato;
  - la **singola ad** si classifica come sotto. Serve a decidere cosa iterare.
- **"Sopra target":** si guarda il ROAS standard come primo filtro e quello incrementale per decidere, quando e' disponibile. Sam sceglie i winner per spesa e ROAS incrementale.
- **Classificazione, a livello di singola ad:**
  - **winner:** spende oltre il 5 % del budget di campagna ed e' sopra target. Volume e valore insieme;
  - **potential:** soddisfa solo una delle due condizioni;
  - **sulla soglia:** non si tocca ("We're not going to touch those for now").
  - "Potential ads need to be tweaked. Winning ads need to be replicated."
- **Soglia assoluta** usata nei suoi prompt: ROAS sopra 2-2,1 e oltre 5.000 $ di spesa in 30 giorni.
- **Con meno di circa 20 ads attive** nella campagna, il 5 % e' troppo facile da superare. Interpretazione: usa come soglia di spesa la quota media, cioe' 1 diviso il numero di ads attive.
- **Breakdown:** placement, eta', genere, piattaforma, landing, giorno della settimana, orientati ai segmenti che spendono di piu' e rendono meglio. Hanno senso solo con abbastanza dati.

## 6. Vincitori, perdenti, fatigue

- **Vincitori:** restano nel loro pack, mai duplicati. Si fanno correre e si ribriefa lo stesso concept: "go brief those exact concepts over and over and over again". E' il creative flywheel.
  - Per ogni winner, 2-4 brief con 2 versioni ciascuno, con "moderately big changes", non ritocchi.
  - **Le mosse di iterazione:**
    - "take the first 3 seconds out of the video and run it from there";
    - "add a different hook to the front";
    - "take the hook and add a new body";
    - lo stesso template su altri prodotti o modelli.
  - **Mai solo** il titolo o un filtro: "Variations do not mean that we're just going to change the headline and move on."
  - Le iterazioni vanno in un **pack nuovo**, "as soon as possible".
  - Ogni concept sopra target resta attivo e si somma agli altri. Due concept vincenti si possono fondere in un terzo.
- **Mai in pausa le ads che spendono di piu'.** Alimentano il resto dell'account: "One of the worst things you can do in an ad account is pause your highest spending ads". L'errore gemello e' "making changes too early and too often".
- **Perdenti:** svaniscono dopo il minimo. Pause solo per pulizia ("remove this, move on" nelle versioni precedenti).
- **Fatigue:**
  - quando il ROAS cala ma la spesa no, perche' "Meta continues to spend after the return on ad spend has declined", si mette un **maximum** in percentuale (esempio: un pack che prende il 30 % del budget, limitato al 20 %);
  - la fatigue sull'avatar principale e' il segnale per aggiungerne un secondo.
- **Value rules:** bid modifier per eta', genere e altre coorti, a livello di ad set. Utili se una coorte converte molto peggio; vuote al lancio.

## 7. Hit rate e volume

- **Hit rate** = ads ad alta performance diviso ads lanciate, per 100. Normale circa il 5 %: "volume negates luck".
- **Volume:** "the total number of ads literally means nothing". Conta il volume di qualita', e il volume "sloppy" danneggia.
  - Spiegazione di Sam: il pixel si addestra anche sugli eventi negativi.
  - Altra spiegazione sua: Meta spende su ads che crede scalabili per volume.
- **Cosa dice Meta** (Matt Steiner, intervistato da Sam): "Creating an extremely large number of them probably isn't going to help you more than having a reasonable diversity of ads." Se crei 25 versioni, a una persona ne piaceranno forse 3. E "even if you build 20 and three get run... that's almost to be expected" (Sam).
