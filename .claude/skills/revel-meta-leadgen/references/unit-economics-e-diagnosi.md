# Unit economics e diagnosi

Indice: 1. Formule · 2. Tetto CPL · 3. Costo per call vs CPL · 4. Soglie di budget e volume · 5. Qualità vs intento · 6. Ads o vendite: di chi è la responsabilità · 7. Discovery vs proven · 8. Checklist di diagnosi estesa

Importi: come li cita Revel, quasi sempre dollari australiani (1 AUD ≈ 0,61-0,63 €). Le formule valgono in qualsiasi valuta.

## 1. Formule

| Grandezza | Formula | Nota |
|---|---|---|
| Valore cliente (V) | cash incassato per cliente | Revel ragiona sul *cash collected*, non sul fatturato teorico. Per un retainer: canone × mesi medi (LTV), ma guarda anche il primo incasso |
| Tasso lead → cliente (c) | clienti ÷ lead | Se hai solo il close rate sulle call: c = % lead che prenota × % che si presenta × % chiusura sulle call |
| Lead per cliente | 1 ÷ c | Esempio: close 20 % sui lead → 5 lead per cliente |
| CPL di break-even | V × c | Il massimo teorico, non il tetto operativo |
| Costo per call prenotata | CPL ÷ % lead che prenota | Il metro con cui si confrontano le ads |
| Costo per cliente (CAC) | CPL × lead per cliente | Da confrontare con il primo incasso e con il ciclo di cassa |

## 2. Il tetto CPL (soglia del kill al giorno 4)

Due modi, in ordine di preferenza:

1. **Dallo storico.** Se l'account ha anni di dati, il tetto è il CPL massimo che storicamente ha prodotto clienti redditizi. Esempio: per dei business coach con anni di ads alle spalle, Revel ha fissato il tetto a 65 $ guardando la storia dell'account e del CRM.
2. **Dalle unit economics.** Parti dal break-even e scegli un tetto ben più basso, che rispetti la cassa. Esempio di Revel (agenzia): retainer 2.500 $/mese, cliente medio 7 mesi (circa 15K+), close 20 % → 5 lead per cliente → tetto **150 $ a lead**.
   - *Interpretazione (non detta da Revel):* 5 × 150 $ = 750 $ di costo per cliente, ripagati già dal primo mese di canone. Il break-even teorico (oltre 3.000 $ a lead) non c'entra con la cassa. Regola pratica: il tetto deve far rientrare il CAC dal primo incasso, o comunque entro un tempo che il business regge senza stress di cassa.

Nota di Revel: un CPL più alto va benissimo "se ha accorciato il tempo in cui incassi".

## 3. Confronta le ads sul costo per call, non sul CPL

Esempio illustrativo (le percentuali sono ipotetiche):
- 4 $ a lead, prenota l'1 % → **400 $ per call**
- 29 $ a lead, prenota il 20 % → **145 $ per call**

Revel preferisce pagare il doppio, anche il triplo, per lead se la quota di chi prenota o risponde alle chiamate sale in modo netto ("parliamo di almeno il 20 %"). Lead sotto circa 25 $ (un anno fa diceva sotto 12 $) di solito vogliono dire che l'ad parla a un pubblico molto largo, con intento basso rispetto a un ad trust-first. "I lead economici sono una metrica di vanità."

Per i ticket alti la scala cambia: un cliente con fee da 35-50K paga circa 600 $ per call prenotata, ed è "niente" rispetto a quello che incassa.

## 4. Soglie di budget e volume

- **Minimo per ad:** circa 30 AUD/giorno per un business locale, circa 50 AUD per uno nazionale. Sotto quella cifra le sue strategie non hanno abbastanza dati.
  - La soglia nazionale non è un dogma: nel suo esempio a 100 AUD/giorno usa 3 ad set da 30 AUD anche per clienti non locali.
  - In euro e per l'Italia usa la regola derivata del budget minimo per ad = tetto CPL ÷ 4 (`profilo-strumenti-e-posizioni.md` §2).
- **4 giorni per ad** servono ad accumulare abbastanza impression per dire "buono" o "cattivo" con certezza.
- **Giudicare sulle call con budget piccoli:** con 30 $/giorno e un costo per call di 300 $ servono 10 giorni per vedere una sola call. In questi casi giudica l'ad sul CPL e misura le call a parte, oppure usa l'evento sequence se l'account lo ha.
- **B2B di nicchia** (es. agenzie che lavorano solo con aziende da 200K al mese): il pubblico è piccolo, quindi il CPL è più alto del B2C. È normale, a meno che il problema sia l'offerta.
- **Budget grandi e pubblico ampio** (es. 1.000 $/giorno con CPL qualificato storico di 30 $): si può decidere su un ad più in fretta.

## 5. Qualità vs intento

- **Qualità** = il lead supera le domande di qualifica, cioè è qualificato "sulla carta".
- **Intento** = quanto vuole davvero parlarti: si presenta alla call, cita le tue ads durante la call, ti segue.
- Si può avere qualità alta e intento basso: succede spesso. Se deve sceglierne uno, Revel sceglie l'intento.
- La qualità si ottiene con buone domande. L'intento nasce dall'**ad**, cioè dalla prima impressione: un ad che insegna, educa o sposta una convinzione.
- Errore comune: "se dichiarano di avere soldi, sono qualificati". Falso: chi ha soldi non li ha fatti spendendoli a caso. Restano decisivi la velocità del follow-up, il posizionamento, l'offerta e come viene presentata in call.
- "Pixel conditioning" è un termine sbagliato: il pixel è solo un messaggero che riporta gli eventi all'ad set, ed è lì che avviene l'apprendimento. Per "condizionare" verso l'intento si lavora sull'ad.

## 6. Ads o vendite: di chi è la responsabilità

- L'advertising ha un KPI chiaro: il **costo per appuntamento o call**. Nell'azienda solare di Revel il lavoro delle ads è tenerlo sotto circa 212 $ (dato a memoria). Lo stesso vale per tutti i suoi clienti.
- Le vendite devono lasciare tracce:
  - sentiment nel CRM dopo ogni chiamata (Revel imposta 5 opzioni su come è andata la chiamata del setter e 5 sulla call del venditore);
  - note sul contatto o sull'opportunità;
  - meglio ancora, un gruppo WhatsApp o Slack con i venditori dove lasciano note a caldo subito dopo l'appuntamento; poi Claude le riassume. Così sono responsabilizzati e hai una linea diretta con il punto vendita.
- Gerarchia delle fonti di verità: 1) **trascrizioni delle presentazioni di vendita** (il "santo graal"); 2) molto più indietro, note o tag di sentiment; 3) trascrizioni e note dei setter.
- I venditori raramente tengono i dati puliti da soli: serve qualcuno che li segua.
- Con 30-50 lead al giorno probabilmente basta un setter o closer con un dialer, che fa anche i richiami.

## 7. Discovery vs proven

**Discovery**: non hai ads provate e non sai se il problema è la landing, l'offerta o il targeting (il targeting no: lo fanno le ads). Sembra di bruciare soldi, ma stai pagando per scoprire cosa non funziona, ed è una strategia deduttiva: ci passano tutti, la "valle della disperazione".
- 20 ads, 4K spesi, zero vendite: se gli script sono pensati bene (anche con le trascrizioni delle call), ci saranno almeno 2 vincenti o quasi. Il 10 % è generoso, realisticamente è più vicino al 2 %. Analizza le 18 perdenti, fanne meno di quel tipo, e lascia che le vincenti guidino il giro successivo: "il 10 % diventa il 90 %".
- Esempio dell'azienda solare: 20K a un videomaker per circa 30 ads. Il ragionamento era che, se anche solo un ad "funziona" (cioè resta attivo più di 2 settimane), porta almeno 2 vendite e la spesa rientra. Quei 30 video sono poi diventati oltre 320 ads riciclandoli in formati diversi, e alcuni girano ancora.
- Una landing nuova senza lead dopo 2 giorni: troppo presto per giudicare.
- Atteggiamento: in discovery serve qualcuno con "due mani sul volante" che tenga la rotta finché, verso il giorno 10-14, le performance salgono.

**Proven**: qualcosa ha funzionato. La trappola è il "prima funzionava": si insiste su tattiche, script e hero ad vecchi invece di tornare in discovery.

**A regime**: circa il 10 % del budget resta alla scoperta continua (ad types sperimentali, evento sequence). Così il lead flow non va mai a zero se l'unico ad provato si esaurisce.

## 8. Checklist di diagnosi estesa

1. **Lead o vendite?** Chiedi i numeri del funnel completo: lead → contattati → call prenotate → presentati → chiusi → cash. Il collo di bottiglia è dove la percentuale crolla.
2. **Tetto:** calcola il tetto CPL (§2) e confrontalo con il CPL reale dal CRM. Se il CPL è dentro il tetto, il costo non è il problema.
3. **Struttura:** budget ÷ numero di ads ≥ soglia? Una sola ad per ad set? CBO che concentra la spesa su 2-3 ads?
4. **Volume:** quanti lead a settimana? Bastano per una decisione in 4 giorni?
5. **Ads:** l'ad insegna o chiede soltanto? L'hook qualifica? È riconoscibile o "copia-incolla" dei concorrenti? Ad e VSL o landing dicono la stessa cosa?
6. **Funnel e capacità:** chi richiama, quanto in fretta, quante volte? Il livello di qualificazione è coerente con quella capacità (§ regola: meno qualifica il funnel, più devono farlo form o setter)?
7. **Frizione:** tanti lead ma poche call? Troppe domande, thank-you page poco chiara, nessun link al calendario?
8. **Speed to lead:** misura il tempo tra ingresso del lead e prima chiamata (dal dialer o CRM).
9. **Tracking:** CAPI configurato? Lead in Meta e nel CRM allineati oltre il 90 %?
10. **Fase e aspettative:** discovery o proven? Si sta reagendo a un aneddoto ("arrivano un sacco di lead fuori zona") invece che ai dati? Esempio: dati alla mano erano 3-4 lead in un giorno, e nulla di anomalo su 4 settimane.
11. **Stagionalità e calendario:** prima di ipotesi come "facciamo girare le ads solo in certi giorni", verifica con i dati del cliente se c'è davvero evidenza. Revel non vede differenze stagionali, per esempio nell'acquisizione clienti di un'agenzia a novembre e dicembre.
