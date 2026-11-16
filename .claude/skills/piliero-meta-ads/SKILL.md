---
name: piliero-meta-ads
description: Sistema Meta Ads di Sam Piliero (agenzia The Moonlighters), il metodo M4 dell'era Andromeda, distillato da 23 suoi video del 2025-2026. Copre la struttura (prospecting in CBO diviso in pack per avatar e concept, retention, retargeting e scale facoltativi), il test con minimi di ad set per 7 giorni e la regola del 20 per cento, vincitori e potential, iterazioni dei winner, la creativita' per avatar (pattern interrupt, problema, meccanismo unico, prova, offerta; problema-soluzione a freddo e obiezioni a caldo), la scala verticale e orizzontale con le tre letture del ROAS, value rules e cost cap, la regola sugli enhancements e i flussi di lavoro con Claude e il connettore Meta. Include l'adattamento a lead gen e budget da 10-50 euro. Usala quando si parla di struttura delle campagne Meta, Andromeda, CBO o ABO, pack, minimi di ad set, come testare le creativita', quante ads per ad set, scalare il budget, ROAS che cala, creative fatigue, avatar e angoli, e-commerce su Facebook e Instagram, o di Piliero.
---

# Sistema Piliero (M4) per Meta Ads

Sam Piliero dirige The Moonlighters, agenzia quasi solo e-commerce DTC (circa 100 brand), e dichiara oltre 500 milioni $ gestiti. Vende anche una community Skool e, in affiliazione, uno strumento AI per creativita': i suoi casi sono autodichiarati. Questa skill nasce dallo studio delle trascrizioni complete di 23 suoi video, da dicembre 2025 a novembre 2026 (`references/fonti-e-dubbi.md`). Gli importi sono in dollari USA, come li cita lui.

Il suo sistema ha quattro livelli ("M4 system"):
- **M1, struttura:** "creating your foundation";
- **M2, creativita':** Sam non pronuncia mai "M2", e' la parte su avatar e concept;
- **M3, il cavallo piu' veloce:** breakdown e value rules;
- **M4, controlli di costo**, solo oltre circa 100.000 $.

Sam lavora su e-commerce: per lead gen, servizi, esperienze e budget piccoli leggi prima `references/adattamento-lead-gen-budget-piccoli.md`.

## I principi (il perche' dietro le regole)

1. **Il messaggio fa il targeting.** "creative is the targeting" e' troppo vago: conta chi chiami in causa. "whomever you're talking to or calling out in the ad itself is who is going to be naturally targeted by that ad." Audience broad, niente interessi. "If you don't hit avatars in your marketing, Andromeda does not know how to deliver your ads appropriately."
2. **L'algoritmo distribuisce il budget meglio di te, ma con vincoli.** "the AI is smarter than us": serve un ambiente "algorithm friendly aka CBO but we have constraints". Le leve sono minimi, maximums e value rules, non decine di ad set in ABO.
3. **L'unita' e' il concept.** Un pack (ad set) e' un avatar + un angolo, con 4-8 ads che di solito sono hook diversi sullo stesso body. Ne seguono tre divieti:
   - mai mescolare avatar nello stesso pack;
   - mai aggiungere ads a pack vecchi ("We never inject new ads into old packs. Let that sit with you. That is critical");
   - mai duplicare i winner.
4. **Il test perfetto spende il meno possibile.**
   - Il minimo del pack nuovo e' il piu' basso tra **1 CPA target** e il **20 % del budget totale**, per **7 giorni**, poi si toglie.
   - "Proven is better than new": prima si spende sui vincitori.
   - "We don't need to spend 20% on testing. Get that out of your head."
5. **Diversita' ragionevole, non volume.**
   - Hit rate normale: circa il 5 %. Il volume "sloppy" danneggia.
   - Per Meta (Matt Steiner) conta "a reasonable diversity of ads". Un'iterazione non e' "the same shoe with a different headline": "mimic but change the vibe".
6. **Due messaggi.** Problema + soluzione per il pubblico freddo, spesso in video lungo; obiezioni per quello caldo, un claim per ad. Niente produzione per il middle.
7. **Pazienza e coraggio.**
   - Nulla si tocca per 7-14 giorni.
   - Mai in pausa le ads che spendono di piu', e niente "death loop" di pause e riavvii.
   - Sopra target si scala in verticale: fermarsi a target "is how you get stuck forever".
8. **Si ottimizza sull'evento standard piu' profondo** (Purchase "99.9% of the time"), perche' l'algoritmo spinge esattamente l'evento scelto.

## Come usare questa skill

| Situazione | Percorso |
|---|---|
| Account nuovo | Passi 1-6 in ordine |
| Account esistente che non rende | Passo 1 (audit), poi Passo 3 |
| Nuove creativita' da lanciare | Passi 2 e 4 |
| Leggere i risultati, scegliere i vincitori | Passo 5 |
| Scalare | Passo 6 + `references/scala-e-metriche.md` |
| Lead gen, servizi, esperienze, budget da 10-50 € | Prima `references/adattamento-lead-gen-budget-piccoli.md` |
| Usare Claude e il connettore Meta | `references/claude-e-ai.md` |
| Capire perche' le regole funzionano (retrieval, Andromeda, cosa conta come diverso) | `references/algoritmo-e-andromeda.md` |

### Passo 1: numeri e audit
- **Il target si ricava dai numeri.**
  - CPA e ROAS target vengono da break-even e LTV. Sam: "a line in the sand"; conta il profitto prima del ROAS.
  - Se il target dichiarato e' sotto il pareggio (per esempio CPA 25 € su uno scontrino di 45 € con break-even a ROAS 2,2, cioe' ROAS 1,8), usa il pareggio come linea di decisione. Fa eccezione il caso in cui l'LTV (riacquisti) giustifichi di piu'.
  - Il target decide vincitori e scala: sbagliarlo falsa tutto il resto.
- **Tracciamento, prima di ogni giudizio** (interpretazione nostra, da un account lead gen reale nel 2026):
  - landing page view diviso link click: di solito sopra il 60 %; vicino a zero vuol dire che il pixel non carica sulla landing;
  - eventi dell'evento di ottimizzazione negli ultimi 7 giorni, per evento e per URL (con il connettore Meta, `ads_get_dataset_stats`): zero con spesa attiva vuol dire algoritmo cieco;
  - in UE il pixel spesso parte solo dopo il consenso del banner cookie, e da telefono quasi nessuno accetta. Si passa all'instant form o a un evento lato server con il consenso raccolto nel form, mai aggirando il banner;
  - finche' il tracciamento e' rotto nessun giudizio su ads o pack regge, e ripiegare sull'obiettivo Traffico compra solo clic.
- **Audience segments** (Breakdown): quanta spesa va su new, engaged ed existing. Nel prospecting gli existing devono essere quasi a zero; Sam vede spesso il 40-50 % con frequenza 25 in 30 giorni.
- **Struttura:**
  - quante campagne e ad set ci sono, e se ci sono ads nuove aggiunte a campagne consolidate o ad set in ABO a pioggia;
  - se si mettono in pausa i top spender;
  - se ci sono troppe ads non posizionate bene: da 165 a 62 ads attive il ROAS e' passato da 0,63 a 1,4.
- **Impostazioni:**
  - evento di ottimizzazione (Purchase o un proxy?);
  - enhancements che toccano il media;
  - flexible o dynamic creative.
- **Numeri:** le tre letture del ROAS (Meta, incrementale, blended) contro il target.

### Passo 2: avatar e concept (M2)
- **Avatar:** uno (al massimo 2-3), descritto come persona con problemi, non come demografia. Si parte dall'avatar, non dall'offerta o dal prodotto.
- **Ricerca:** 20 problemi della categoria, 20 angoli, meccanismo unico, obiezioni profonde, offerta sulle tre leve (valore, tempi, rischio).
- **Checklist di ogni ad:**
  1. pattern interrupt e chiamata dell'avatar nei primi 1-2 secondi;
  2. un solo avatar;
  3. il problema;
  4. il meccanismo unico;
  5. la prova (sociale e di comfort).
- **Dettagli, fonti dei concept e flywheel:** `references/creativita-e-avatar.md`.

### Passo 3: struttura (M1)
- **Prospecting CBO:**
  - Sales, highest volume or value, almeno 1 CPA al giorno, nessuno scheduling;
  - pack "avatar_concept pack N" con "acquire new customers" ed esclusione degli acquirenti;
  - evento Purchase, attribuzione 7-1-1 con all conversions, audience broad (Advantage+ si puo' tenere), tutti i placement.
- **Ad:**
  - una creativita' per ad, file verticale con area sicura 4:5;
  - 2-3 primary text davvero diversi e 2-3 headline;
  - enhancements: spenti se toccano il media, accesi se aggiungono intorno; image generation spenta;
  - optimized website destination di norma spenta.
- **Retention:** CBO piccola sugli acquirenti, regolata sulla frequenza.
- **Retargeting e scale:** solo se servono (retargeting quando gli engaged assorbono troppa spesa; scale con circa 5 winner).
- **Tutte le impostazioni**, M3 (value rules, giorni della settimana) e M4 (cost cap): `references/struttura-e-setup.md`.
- **Account gia' attivo:** non si smonta tutto in un giorno.
  - Le ads che oggi portano risultati restano dove sono ("pack 0"): non si mettono in pausa e non si duplicano.
  - La nuova struttura parte accanto, e il budget si sposta a scalini.
  - Dettagli: `references/struttura-e-setup.md` §14.

### Passo 4: lanciare un pack
1. Un concept (avatar + angolo) con 4-8 ads separate, cioe' gli hook.
2. Duplica un pack, svuotalo, rinominalo col numero successivo, carica le ads nuove.
3. Minimo: il piu' basso tra 1 CPA target e il 20 % del budget totale, contando tutti i minimi attivi. Il primo pack parte senza minimo solo in un account nuovo; se c'e' un pack 0 che gia' spende, anche il primo pack nuovo ha il minimo.
4. Sette giorni senza toccare nulla, poi togli il minimo e lascia l'ad set attivo.
5. Un pack nuovo ogni 1-3 settimane, "like a drum beat".

Procedura completa e motivazioni: `references/test-e-pack.md`.

### Passo 5: leggere e iterare
- **Quando:** a 7-14 giorni, con l'attribuzione incrementale, ordinando le ads per spesa.
- **Classificazione, per singola ad:**
  - **winner:** oltre il 5 % della spesa di campagna e sopra target;
  - **potential:** una sola delle due;
  - **sulla soglia:** non si tocca.
  - "Potential ads need to be tweaked. Winning ads need to be replicated."
- **Perdente:** il pack che ha speso solo il minimo svanisce da solo, senza pausa.
- **Iterazioni** (2-4 brief per winner, cambi "moderatamente grandi"):
  - tagliare i primi 3 secondi;
  - un hook diverso davanti;
  - lo stesso hook con un body nuovo.
  - Sempre in un pack nuovo. Ogni concept sopra target resta e si somma agli altri.

### Passo 6: scalare
- **Prerequisiti:** solo a target o sopra, dopo le tre letture del ROAS.
- **Taglie:** +10-20 % a target, +20-30 % di norma, +50 % e oltre molto sopra, raddoppio a 2-3 volte il target. Finestre piu' brevi con piu' spesa, piu' lunghe con pochi acquisti.
- **Dopo l'aumento:** colonne anticipatrici (costo per click, per add to cart, per checkout, per acquisto). Se sale solo l'ultimo anello si aspetta, se salgono tutti si ritira.
- **Twin engine:** verticale sul budget di campagna e orizzontale con le iterazioni in pack nuovi.
- **M3 e M4:**
  - M3 (value rules, giorni della settimana) solo con dati sufficienti;
  - M4 (cost cap) solo oltre circa 100.000 $ e mai insieme a highest volume.

## Cose da non fare
- Testare in ABO, in campagne di test o con il creative testing di Meta (eccezione: biglietti oltre 1.000 $, anche in lead gen).
- Pack nuovi senza minimo, o minimo tenuto oltre 7 giorni.
- Ads nuove in pack o campagne esistenti: un'ad e' passata da 11 $ a 2.000 $ e ha affondato il ROAS.
- Pause dei top spender, salti enormi di budget, decine di modifiche insieme.
- Ads con piu' media quasi uguali (il vecchio formato flexible, sparito ad aprile 2026), dynamic creative, enhancements che toccano il media, image generation.
  - "Flex media" tocca il media: tienilo solo se le anteprime nei placement sono corrette.
- Escludere segmenti deboli invece di correggerli con le value rules; interessi e audience ristrette.
- Ottimizzare per add to cart, checkout o eventi custom.
- Ripiegare sull'obiettivo Traffico quando il pixel non registra: si ripara il tracciamento o si passa all'instant form.
- Varianti che cambiano solo il titolo o un filtro.

## Lead gen, esperienze e budget piccoli (sintesi)
- **Sam dice una sola cosa esplicita sulla lead gen:** l'ABO puo' servire per biglietti oltre 1.000 $.
- **Il resto e' un adattamento:**
  - costo per lead target al posto del CPA;
  - evento Lead standard;
  - un pack in test alla volta;
  - minimi di 4-10 € al giorno con 20-50 € di budget;
  - verdetto al giorno 14;
  - vincitore = quota di spesa sopra la media e costo per lead entro il tetto;
  - controllo a valle: dopo 30-40 lead per pack si guardano prenotazioni o vendite. Lead economici con zero prenotazioni sono un falso vincente;
  - niente retargeting a parte.
- **Budget piccolo** vuol dire meno di circa 5 costi per risultato *attesi* al giorno: conta quello che paghi oggi, o la stima, non il tetto delle unit economics.
- **Sotto circa 2,5 costi per risultato al giorno** la spesa forzata non dice quasi nulla: meglio trovare i concept con l'ABO di Revel e passare ai pack quando ci sono 2 o piu' vincitori.
- **Tutto qui:** `references/adattamento-lead-gen-budget-piccoli.md`.

## Rapporto con le altre skill
- **`revel-meta-leadgen`:** servizi ad alto biglietto venduti in call, budget sotto i 20 € al giorno, un ad per ad set con giudizio al giorno 4. Il disaccordo con Sam e' piu' piccolo di quanto sembri, perche' Sam stesso ammette l'ABO per il biglietto alto.
- **`modular-video-ads-system`:** la produzione dei moduli.
  - Il pack di Sam e' un body con gli hook come iterazioni.
  - Le sue mosse di iterazione (via i primi 3 secondi, nuovo hook, stesso hook con nuovo body) sono esattamente le combinazioni del sistema modulare.
  - Il confronto tra i metodi sta in `modular-video-ads-system/references/tre-metodi-a-confronto.md`.

## Formato di output
Quando progetti o rivedi un account, consegna in quest'ordine e adatta la lunghezza alla richiesta:
1. **Diagnosi:** i risultati dell'audit, con i numeri.
2. **Struttura:** campagna → ad set → budget e minimi → ads.
3. **Piano dei pack:** per ogni pack avatar, concept, ads (hook), testi.
4. **Calendario:** giorno 0, giorno 7, giorno 14, cadenza dei pack nuovi.
5. **Regole:** winner, potential e perdenti, e quando scalare.
6. **Cosa verificare in Ads Manager**, perche' l'interfaccia cambia spesso.

Scrivi nella lingua dell'utente. Con importi in euro e budget piccoli usa l'adattamento, non i numeri di Sam. Se usi il connettore Meta per pause, budget o ads nuove, chiedi sempre prima una conferma esplicita all'utente: sono azioni che spostano soldi veri, e Sam stesso tiene tutte le scritture su "needs approval".

## Limiti
- **Fonti:** Sam parla quasi solo di e-commerce, e i suoi risultati e le sue affiliazioni vanno tenuti presenti.
- **Andromeda 2.0:** il white paper che cita non e' verificato.
- **Contraddizioni:** tra i suoi video ce ne sono diverse (scale campaign, finestra degli existing, business AI, ads per pack), elencate in `references/fonti-e-dubbi.md`.
- **Interfaccia:** nomi e posizioni delle impostazioni in Ads Manager cambiano spesso. Se una voce non c'e' piu', cerca l'equivalente e dillo.
