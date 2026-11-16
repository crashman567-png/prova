# Adattamento a lead generation, esperienze e budget da 10-50 € al giorno

Sam lavora quasi solo con e-commerce DTC e budget da centinaia o migliaia di dollari al giorno. Sulla lead gen dice solo una cosa esplicita: per biglietti oltre 1.000 $ per acquisto, lead gen inclusa, "you might need to lean a little bit more on" ABO. Tutto il resto di questo file e' un **adattamento**: le regole citate sono sue, le traduzioni sono nostre, da validare sui dati dei clienti.

Indice: 1. Tabella di traduzione · 1b. Fasce di budget · 2. Cosa si rompe · 3. Versione minima da 20-50 € al giorno · 4. Varianti · 5. Quando usare Revel invece

## 1. Tabella di traduzione

| Regola di Sam | Per lead gen ed esperienze |
|---|---|
| Evento Purchase, "never anything else" | L'evento standard piu' profondo con volume: Lead (instant form, o sito con Conversions API); Purchase per booking pagati online solo con almeno 3-5 prenotazioni a settimana |
| CPA target | Costo per lead target, ricavato dalle unit economics (skill `revel-meta-leadgen`) |
| Pack = avatar + concept, 2-8 iterazioni | Un body del sistema modulare con 3-5 hook come ads separate |
| Minimo = il piu' basso tra 1 CPA e il 20 % del budget, 7 giorni | Uguale, con il costo per lead al posto del CPA |
| Winner oltre il 5 % della spesa e a target | Con 3-5 pack e' troppo debole: prende almeno un quarto della spesa nella seconda settimana, con costo per lead entro il target |
| Esclusione degli acquirenti entro la finestra di churn | Clienti nel CRM, piu' i lead degli ultimi 30-60 giorni |
| Retention a parte | Solo con riacquisto vero (rinnovi CSA, ospiti che tornano) e una lista di almeno circa 1.000 persone, a 3-5 € al giorno nella finestra di rinnovo |
| Tre letture del ROAS | Costo per lead in Meta; costo per lead nel CRM; costo per vendita vera (posto, abbonamento) su tutta la spesa |
| Funnel CPC, add to cart, checkout, acquisto | CPC, costo per visualizzazione della landing, costo per lead, costo per prenotazione o call, costo per vendita |
| Scale surfing per distanza dal target | Uguale sul costo per lead, con finestre piu' lunghe: pochi eventi al giorno equivalgono a un valore d'ordine alto |
| Obiezioni in fondo al funnel | I moduli O1-O4 del sistema modulare, in un pack dedicato |

## 1b. Fasce di budget (interpretazione)

La regola del minimo (il piu' basso tra 1 costo per risultato target e il 20 % del budget, per 7 giorni) regge a ogni budget, ma diventa sempre meno informativa. Le fasce si misurano in costi per risultato **attesi**, cioe' quello che paghi oggi o la stima, non nel tetto ricavato dalle unit economics. Un business ad alto margine puo' avere un tetto alto ma comprare solo 3 lead al giorno.

| Budget giornaliero | Cosa succede | Cosa fare |
|---|---|---|
| Almeno 5 costi per risultato attesi | Il sistema funziona come lo descrive Sam | M1 completo |
| Tra 2,5 e 5 costi per risultato attesi | Il minimo vale 0,5-1 risultato al giorno: regge, ma il test e' lento (30 € al giorno con costo per lead 10 €: minimo 6 €) | Versione minima (§3), verdetto al giorno 14 |
| Sotto 2,5 costi per risultato attesi | La spesa forzata non dice quasi nulla | ABO alla Revel per trovare i concept; pack CBO quando ci sono 2 o piu' vincitori da far convivere |

Con lead molto economici (sotto 1 €), 1 costo per lead al giorno non forza nulla: si usa il 20 % del budget.

**Vincitore con poche ads: due livelli con scopi diversi.**
- **Pack (il concept), verdetto al giorno 14:** vincente se nella seconda settimana prende almeno un quarto della spesa con costo per lead entro il target (§3). Serve a decidere se il concept resta.
- **Singola ad, per decidere cosa iterare:** il 5 % della spesa presuppone decine di ads, e con 8-16 ads attive quasi tutte lo superano.
  - Winner: quota di spesa sopra la media (1 diviso il numero di ads attive) e risultato vero entro il tetto.
  - Potential: una sola delle due condizioni.

**Non mescolare le regole.** Nei pack CBO niente decisioni prima di 7 giorni e giudizio a 14. Il keep or kill al giorno 4 resta per la struttura ABO di Revel, in una campagna separata.

## 2. Cosa si rompe

- **I minimi diventano piccoli.** Il minimo di 1 costo per lead supera quasi sempre il 20 % del budget, quindi vale il tetto: 2-10 € al giorno, cioe' 14-70 € in 7 giorni. Con un costo per lead di 10 € fanno 1-7 lead, spesso meno di una prenotazione. Il verdetto a 7 giorni sugli acquisti non regge con cosi' pochi eventi.
- **"Dozens of active ad sets" e' impossibile.** Con 30 € al giorno la CBO nutre 2-3 pack e lascia gli altri a zero.
- **Le metriche fini non servono.** Il 5 % della spesa, l'attribuzione incrementale e i breakdown per eta', genere o giorno sono rumore con poche decine di lead.
- **La vendita avviene fuori da Meta** (call, acconto, WhatsApp): si ottimizza su un proxy, Lead, contro la preferenza di Sam.
- **Traduzioni automatiche:** per un business locale portano reach in lingue che il cliente non serve.

## 3. Versione minima da 20-50 € al giorno

1. **Una campagna CBO:** Leads per lead gen e richieste di prenotazione, Sales per e-commerce e booking pagati online. Budget uguale a tutto il budget giornaliero, highest volume, nessuno scheduling.
2. **Niente retargeting a parte.** Chi ha visitato resta dentro, come in M4. Retention solo con riacquisto vero (§1).
3. **Pack:**
   - al massimo 3-5 attivi;
   - ognuno e' un avatar + un body, con 3-5 hook come ads separate;
   - 2-3 primary text diversi e 2-3 headline.
4. **Minimo:** il piu' basso tra 1 costo per lead target e il 20 % del budget, meno i minimi gia' attivi.
   - 20 € al giorno e costo per lead 8 €: minimo 4 €, 28 € in 7 giorni, cioe' circa 3-4 lead.
   - 50 € al giorno e costo per lead 10 €: minimo 10 €, 70 € in 7 giorni, cioe' circa 7 lead.
5. **Un pack in test alla volta.**
   - Il primo pack di un account nuovo parte senza minimo.
   - Se l'account ha gia' ads che portano risultati, restano dove sono come "pack 0", senza pause e senza duplicazioni. In quel caso anche il primo pack nuovo parte con il minimo, se no non riceve spesa.
6. **Giorno 7:** togli il minimo e lascia l'ad set attivo.
7. **Giorno 14:**
   - vincente se nella seconda settimana prende almeno un quarto della spesa con costo per lead entro il target;
   - perdente se scende sotto il 5 % della spesa;
   - se prende oltre il 30 % con costo per lead oltre 1,5 volte il target: maximum o pausa.
   - **Controllo a valle:** dopo 30-40 lead per pack si guardano le prenotazioni o le vendite di quei lead. Un pack con lead economici e zero prenotazioni e' un falso vincente, come i lead a 4 $ di Revel che "volevano un calcolatore gratis".
8. **Ritmo:** un pack nuovo ogni 7-14 giorni. I 4 body del sistema modulare diventano 4 pack in 4-6 settimane:
   - giorno 0: lancio di P1 (senza minimo se l'account e' nuovo, con il minimo se c'e' un pack 0);
   - giorno 7: via il minimo a P1, lancio di P2 con il minimo;
   - giorno 14: verdetto su P1, via il minimo a P2, lancio di P3;
   - giorno 21: verdetto su P2, via il minimo a P3, lancio di P4;
   - giorno 28: verdetto su P3, via il minimo a P4;
   - giorno 35: verdetto su P4.
   - Ogni pack si giudica 14 giorni dopo il suo lancio, mai prima.
9. **Dopo un vincitore:** nuove riprese sullo stesso body (hook nuovi, altra persona, altro luogo) in un pack nuovo, mai in quello vecchio.
10. **Impostazioni:**
    - enhancements con la regola di Sam e image generation spenta;
    - ad transparency compilata (UE) e multi-advertiser spento;
    - optimized website destination spento se la landing e' una pagina sola;
    - traduzioni spente, salvo dove arrivano davvero clienti stranieri (es. un surf camp alle Canarie) e il cliente risponde in quelle lingue;
    - breakdown solo dopo circa 50 lead.
11. **Scala:** solo con costo per lead stabilmente sotto il target.
    - Si usa la tabella di Sam (`scala-e-metriche.md` §4) applicata alla distanza del costo per lead dal target. Per esempio, 30-50 % sotto il target: +20-40 %.
    - Si giudica su finestre di 7 giorni, perche' a questi volumi un ciclo equivale a un valore d'ordine alto. Mai inseguire un singolo giorno.
    - Prima di alzare, controlla che il cliente abbia capacita' da vendere: posti liberi, quote della stagione.
12. **Quanti pack attivi:** al massimo circa 5 che ricevono spesa vera. I pack che dopo il giorno 14 spendono meno del 5 % si possono mettere in pausa solo per leggibilita': non spendono e non perdono nulla. Mai in pausa i top spender.
13. **Offerte riservate per natura** (per esempio un camp solo per donne): non sono un "segmento debole" da correggere con le value rules, sono un requisito dell'offerta. Interpretazione:
    - si parte broad, con una chiamata in causa esplicita nell'hook;
    - dopo circa 50 lead si guarda il breakdown per genere;
    - se una quota rilevante della spesa (oltre il 10-15 %) va a chi non puo' comprare, si restringe.
14. **Risultato vero dentro Meta:** quando si puo', le prenotazioni chiuse su WhatsApp o in call si rimandano a Meta come eventi offline o via Conversions API, cosi' l'account impara anche da quelle (Sam mette "eventi offline se esistono" nel tracking).

## 4. Varianti

- **10-20 € al giorno:** il minimo scende a 2-4 € e diventa quasi simbolico, con decisioni a 14-21 giorni. Qui la struttura di Sam aggiunge poco: un test alla Revel (un ad per ad set in ABO) e' piu' leggibile.
- **Piccolo e-commerce** (box CSA online, prodotti fisici), cioe' sotto circa 5 CPA attesi al giorno:
  - regole di Sam intatte con evento Purchase, ma verdetti a 14-21 giorni invece di 7;
  - retention solo con una lista di almeno circa 1.000 clienti, a partire dal 5-10 % del budget e alzandola guardando la frequenza ("very low to start and work it up").
- **Booking ad alto biglietto** (retreat oltre circa 1.000 €) ottimizzato sul pagamento: vale l'eccezione ABO di Sam. Con 30-50 € al giorno pero' conviene ottimizzare su Lead e qualificare dopo, con il metodo Revel.

## 5. Quando usare Revel invece di Sam

- **Budget sotto circa 20 € al giorno.**
- **Servizi ad alto biglietto venduti in call,** dove pesano fiducia, qualifica e velocita' di richiamo.
- **Quando serve un verdetto rapido su un singolo ad.**

Il confronto completo, con l'esperimento per decidere (pack CBO contro ad set ABO sullo stesso body vincente), sta nella skill `modular-video-ads-system`, `references/tre-metodi-a-confronto.md` e `references/lancio-e-test.md`.
