# Il sistema M4 e il setup dell'account

Indice: 1. Il sistema M4 a quattro livelli · 2. Come e' cambiata la struttura · 3. Struttura dell'account (M1) · 4. Campagna di prospecting · 5. Ad set (pack) · 6. Ad · 7. Enhancements e formati · 8. Retargeting e scale facoltativi · 9. Retention · 10. M3, il cavallo piu' veloce · 11. M4, controlli di costo · 12. Naming · 13. Cose da non fare · 14. Migrare un account esistente

Le fonti sono i video di Sam Piliero indicati con la data (elenco in `fonti-e-dubbi.md`). Gli importi sono in dollari USA, come li cita lui. L'interfaccia di Ads Manager cambia spesso, e Sam stesso dice che le opzioni "might change in just the next day": se una voce non c'e' piu', cerca l'equivalente e segnalalo.

## 1. Il sistema M4 a quattro livelli (luglio 2026)

| Livello | Cosa | Per chi |
|---|---|---|
| **M1, struttura** | "We call this M1 and it is creating your foundation": prospecting CBO a pack, retention, minimi di ad set | Tutti |
| **M2, creativita'** | Sam non pronuncia mai "M2"; dall'ordine del video e' la parte creativa: avatar, problemi, meccanismo, prova, offerta, flywheel (`creativita-e-avatar.md`) | Tutti |
| **M3, il cavallo piu' veloce** | Breakdown, value rules e budget spostati sui giorni forti (§10) | Account con dati sufficienti |
| **M4, controlli di costo** | Cost cap, bid cap, ROAS goal (§11) | Solo oltre circa 100.000 $ (probabilmente al mese) |

Sulla struttura: "Basically, we work in a modular system."

## 2. Come e' cambiata la struttura

| Elemento | Dicembre 2025 - gennaio 2026 ("M3 structure") | Maggio - luglio 2026 (M1 del sistema M4) |
|---|---|---|
| Campagne | 4: prospecting CBO, scale, retargeting, retention, con un "graduation system" dei winner | 2 core (prospecting e retention) e 2 facoltative (retargeting e scale) |
| Esclusioni del prospecting | Visitatori 30 giorni, add to cart 90, acquirenti | Solo gli acquirenti (entro la finestra di churn); chi ha visitato resta dentro |
| Pack | "broad pack N" + data, 2-12 ads | "avatar_concept pack N", 4-8 ads |
| Minimo sul pack nuovo | 1 CPA, controllo a 4-7 giorni | Il piu' basso tra 1 CPA e il 20 % del budget, per 7 giorni |
| Interessi | Ad set "interest_TBD" con ads provate | Tutto broad ("you also might add interest", mai spiegato) |

Perche' e' cambiato:
- Dopo Andromeda (effetti visti "since July of 2025") le ads nuove in CBO libera "hardly getting any spend at all". Da qui i minimi.
- Duplicare i vincitori fa perdere apprendimento: "keeping ads in their ad set outperform starting ads from zero" (maggio 2026).

## 3. Struttura dell'account (M1)

1. **Prospecting CBO:** "the driving force of your entire account", acquisizione e scala insieme.
2. **Retention:** chi ha gia' comprato; budget basso, regolato sulla frequenza (§9).
3. **Retargeting, facoltativo:** solo se gli audience segments mostrano troppa spesa sugli engaged (§8).
4. **Scale, facoltativa:** un ad set con circa 5 winner (§8).
5. **ABO solo per biglietti oltre 1.000 $ per acquisto,** lead gen inclusa, perche' "creative learnings" arrivano troppo lentamente. Nella sua agenzia circa il 90 % della spesa e' in CBO.
6. **Audience segments** nelle impostazioni dell'inserzionista:
   - engaged = visitatori 30 giorni + add to cart 90 "at least";
   - existing = acquirenti (180 giorni nei video di settembre e ottobre, "all time" in quello di fine luglio) + lista clienti dal CRM.
   - Servono a leggere in Breakdown dove va la spesa: "swim lanes", non le fasi del funnel.
   - Negli audit Sam vede spesso il 40-50 % della spesa sugli existing, con frequenza 25 in 30 giorni: "That is absurd". Gli existing e gli engaged "do not work without feeding new audiences first".

## 4. Campagna di prospecting

- **Impostazioni base:** obiettivo Sales, acquisto Auction, budget di campagna, highest volume or value, nessuno scheduling.
- **Budget:** almeno 1 CPA target al giorno ("generally one time your CPA is the sweet spot if you're just starting out"), oppure quanto si e' disposti a perdere. Al lancio e' quello che gia' spendi, e non va usato come leva per aumentare la spesa. Sopra il break-even si scala in verticale, il piu' aggressivamente possibile (`scala-e-metriche.md`).
- **Con highest volume or value** l'algoritmo guarda due cose: volume (riesce a spendere e scalare?) e valore (con che efficienza?).

## 5. Ad set (pack)

- **Nome:** "avatar_concept pack N". L'avatar e' a chi parla l'ad, non un targeting; il concept e' l'angolo.
- **Customer lifecycle:** "acquire new customers", con esclusione degli acquirenti. Se la voce manca, sta in "show more controls".
- **Performance goal:** maximize number of conversions per chi parte, perche' da' piu' segnali; value of conversions con molti prodotti a prezzi diversi.
- **Evento:** Purchase "99.9% of the time". Ottimizzando su add to cart si ottengono "a whole lot of ads carts and a few purchases". L'algoritmo ottimizza solo l'evento scelto, e gli eventi standard imparano dai dati di tutti.
- **Campi vuoti al lancio:** cost per result goal e value rules.
- **Attribuzione:** standard 7 giorni click, 1 giorno engagement, 1 giorno view; "all conversions".
- **Audience:**
  - "fully broad"; "you can keep advantage plus on";
  - il confronto con "further limit the reach" non ha dato "statistical significance on either way";
  - tutte le lingue, tutti i sistemi operativi, piattaforme e placement.
- **Spending limits:** minimo sui pack nuovi per 7 giorni (`test-e-pack.md`); maximum solo sui pack in fatigue.

## 6. Ad

- **Una creativita' per ad:** niente flexible, niente dynamic creative, niente creative testing di Meta.
- **Formato:** un file unico "a 16x9 a vertical with a 4x5 safe zone", cioe' con ogni probabilita' 9:16 con area sicura 4:5, perche' "you're no longer able to upload individual ads in different sizes". Da verificare nell'interfaccia.
- **Testi:** 2-3 primary text, 2-3 headline e una description, semplici e "completely different" tra loro; "optimized text per person" attivo.
- **CTA:** "shop now" o "learn more", a volte "order now"; "get offer" con una promo.
- **Opzioni:**
  - multi-advertiser ads spente;
  - display link se l'URL e' brutto;
  - optimized website destination: "For the most part, I do shut this off nowadays";
  - browser add-ons spenti; promotions accese se ci sono;
  - site links e website highlights accesi ("not hard rules").
- **Tracking:** eventi del sito, eventi offline se esistono, parametri URL (li mette a tutti i clienti).

## 7. Enhancements e formati

- **La regola:** "if it impacts my media, I do not include it. If it doesn't impact the media, if it just enhances, I'm comfortable with that."
- **Spenti:** crop, colore, trasformazione in video, animazioni, visual touch-ups, musica, generate backgrounds, product touch-ups, luminosita'. Spenta anche la **image generation** ("Under no circumstances... just yet").
- **Accesi:** overlays, dynamic overlays, dynamic description, text improvements, show summaries, relevant comments, enhanced CTA, reveal details over time, show spotlights.
- **Business AI:** spenta a inizio luglio 2026 ("awkward"), accettata a fine luglio. Verifica.
- **Translations:** solo se si vende in piu' lingue.
- **Flexible ads:** usate fino a gennaio 2026, poi abbandonate. Nel feed producevano caroselli della stessa immagine e ritagli sbagliati: "the system just couldn't recognize when ads were similar to one another". Ad aprile 2026 sono diventate "flex media" tra gli enhancements; Sam lo accetta, anche se tocca il media. Verifica caso per caso.
- **Dynamic creative:** "I was never a fan".

## 8. Retargeting e scale facoltativi

- **Retargeting:**
  - di solito vive dentro il prospecting; si crea solo se gli audience segments mostrano troppa spesa sugli engaged ("you need to remove that from your prospecting");
  - pubblici: engager di Facebook e Instagram, visitatori 30-60 giorni, add to cart o checkout a 90 giorni; finestre piu' strette per i business grandi, piu' larghe per i piccoli;
  - ads: "objections, sales, and offers";
  - togliere la spunta "use as a suggestion": "Broad audiences are not for retargeting".
- **Scale:** "a broad single ad set smash of all our winners together", circa 5 ads, "nothing more". Serve solo a forzare spesa sui migliori.
  - Contraddizione: a maggio 2026 Sam diceva di non duplicare mai i winner. La scale campaign va trattata come un'eccezione, non come default.

## 9. Retention

- **Struttura:** si duplica il prospecting, sempre CBO, con 1-2 ad set ("purchase 180 days", "purchase all time") e nessuna esclusione. Lifecycle "get more conversions"; il custom audience in "further limit the reach", togliendo "use as a suggestion".
- **Budget:** "very low to start and work it up. Look at the frequency." Esempio 50 $ al giorno; budget grandi solo con centinaia di migliaia di clienti.
- **Dentro:** winner, evergreen, saldi e promo, upsell e downsell, obiezioni, novita', catalog ads. Pochi ad set, perche' "we want people to see a high frequency of our ads". "Most e-commerce businesses do not make their money on the first purchase."

## 10. M3, il cavallo piu' veloce

- **Il principio:** "You would never equally distribute your bets in a horse race."
- **Breakdown:** di primo livello eta', genere, piattaforma, placement; di secondo livello giorno della settimana e ora.
- **Escludere un segmento debole:** "Don't do that. You will lose a lot of money. You will lose a lot of scale potential". Il caso tipico e' togliere i 65+. Si osserva e si corregge con le value rules.
- **Value rules:**
  - procedura: advertiser settings > value rules > create rule set, poi la si applica dall'ad set;
  - esempio: "decrease my bid by a small percentage, 10%, 20%" sui 18-24 anni ("We're not trying to kill this age group");
  - si testano in un **ad set nuovo** con i winner, "just like an AB test in a way".
- **Giorni della settimana:** se domenica-martedi' rendono molto peggio di mercoledi'-sabato, -20 % di budget nei giorni deboli e +15-20 % in quelli forti, fino a -50 % se i dati lo dicono. Non dice se lo fa a mano o con regole.

## 11. M4, controlli di costo

- **Soglia:** "We generally like to think about this at $100,000 plus", perche' "Facebook blows by these objectives all the time".
- **Mai insieme a highest volume:** "Do not run bid caps and cost caps at the same time that you're running highest volume". Il cap prende gli acquisti migliori e la campagna highest volume, che alimenta il pubblico freddo, sembra peggiore.
- **Valori:**
  - bid cap = massimo per conversione; cost per result goal = media;
  - per chi inizia, ROAS goal o cost per result goal;
  - goal a break-even o al target esatto (50 $, "I don't set this to 53");
  - col ROAS goal l'attribuzione passa a solo 7 giorni click.
- **Cosa sono:** "They are a stability tool". Il rischio: "you might find days where you spend nothing. That'll kill the operational side of your business."
- **Con poca spesa:** "If you don't have enough signal in your account, this will never work perfectly for you". L'alternativa per chi spende meno sono i minimi di ad set.

## 12. Naming

- Campagne: "prospecting CBO" (o `ML_prospecting`), "retention".
- Ad set: "avatar_concept pack N"; il pack di obiezioni dichiara "bottom of funnel".
- Ad: un nome per iterazione, cosi' si legge quale hook vince (per il sistema modulare: `H04-B2-CTA1`).

## 13. Cose da non fare

- Testare in ABO, in campagne di test o con il creative testing di Meta.
- Lanciare pack nuovi in CBO senza minimo, o tenere il minimo oltre 7 giorni.
- Aggiungere ads nuove a pack o campagne esistenti: "We never inject new ads into old packs". Un caso: un'ad passata da 11 $ a 2.000 $ in una campagna consolidata ha affondato il ROAS.
- Mettere in pausa le ads che spendono di piu': "One of the worst things you can do in an ad account".
- Fare aumenti enormi di budget o decine di modifiche insieme. Un caso: costo per acquisto da 88 $ a 299 $ dopo un salto di budget.
- Escludere segmenti invece di correggerli con le value rules.
- Usare cost cap insieme a highest volume, o sotto circa 100.000 $.
- Ottimizzare per add to cart, initiate checkout o eventi custom.
- Mettere in pausa e riavviare per paura della learning phase.
- Usare enhancements che toccano il media, o image generation.
- Tenere tante ads non posizionate bene: da 165 ads attive a 62 il ROAS e' passato da 0,63 a 1,4.

## 14. Migrare un account esistente

Sam non da' una procedura di migrazione: mostra solo esiti, come un brand passato da ABO a "full holistic CBO" con +84 % di spesa e +107 % di fatturato in 60 giorni. Le regole che seguono sono un'**interpretazione** costruita con le sue stesse regole: mai in pausa i top spender, mai duplicare i winner, niente salti enormi di budget.

1. **Pack 0.** Le ads e gli ad set che oggi portano risultati restano dove sono, senza pause ne' duplicazioni.
2. **Nuova campagna di prospecting accanto.** Si costruisce secondo il §5. Il primo pack nuovo parte con il minimo, perche' deve competere con un pack 0 che gia' spende.
3. **Budget a scalini.** Si sposta budget dalla vecchia struttura alla nuova del 20-30 % ogni 5-7 giorni, guardando le colonne anticipatrici.
4. **Cosa spegnere prima.** Gli ad set a interessi e le ads che non spendono o sono sotto target in modo stabile. I top spender si spengono per ultimi, quando la nuova campagna porta da sola il volume.
5. **I concept vincenti della vecchia struttura** non si duplicano: si ribriefano come pack nuovi, con iterazioni.
6. **Evento.** Se la vecchia struttura ottimizza su un proxy (add to cart, checkout), la nuova parte su Purchase. Il confronto si fa sul costo per acquisto vero, non sui risultati della colonna.
7. **Retention.** Si crea subito, piccola, solo se c'e' una lista clienti utile.

