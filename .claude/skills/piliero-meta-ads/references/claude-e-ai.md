# Claude e AI nel sistema Piliero

Dal suo corso "Claude + Facebook Ads (FULL COURSE)" (16 luglio 2026) e dal video sulla Ads Library (31 agosto 2026). La sua avvertenza di partenza: "Claude is not as good as a regular media buyer or a growth director." Claude e' "the brain, the architect": legge, segnala e scrive brief. Le decisioni su budget e ads restano umane.

Indice: 1. Setup e permessi · 2. Prime domande · 3. Report programmati · 4. Anomaly detector · 5. Winner detector · 6. Skill di brand e avatar · 7. Workflow creativi · 8. Limiti · 9. Come usarlo con i clienti Stoic

## 1. Setup e permessi

- **Connettore personalizzato:** "Facebook Ads MCP" (in Claude: Customize > Connectors > Add custom connector), poi si sceglie il business manager. L'URL trascritto nei sottotitoli e' incerto: verifica quello ufficiale. A luglio 2026 l'accesso era disponibile per circa il 10-20 % degli account.
  - In questa sessione e in claude.ai il connettore Meta puo' essere gia' disponibile: controlla quali strumenti Meta Ads sono attivi.
- **Permessi:**
  - all'inizio tutto su "needs approval";
  - le letture (insights, entita') possono passare ad "always allow";
  - le scritture mai: "I don't want Claude to automatically be allowed to edit my budgets, change my ads, or change critical details."
- **Primo controllo:** "please list out all of the ad accounts that I have access to" e "specifically call out the ad accounts that have access to the MCP connection". Poi si indica l'account per numero.

## 2. Prime domande

- "what was yesterday's ROAS and spend?"
- "please plot the last 30 days spend, ROAS, purchases, impressions, and frequency in a very simple table", poi una dashboard: "Make it slightly interactive, but overall keep it pretty light and simple."
- Analisi lunghe: "do this broken out by week for data over the last 20 weeks", con "some sort of section that actually analyzes the patterns of this data".
- **Lezione:** senza contesto l'analisi sbaglia.
  - Nel suo esempio Claude giudicava in perdita settimane che, per quel brand, andavano bene a 0,8 di ROAS incrementale sui nuovi clienti.
  - Il valore non sta nel report singolo ("pretty basic") ma nella ripetizione programmata con il contesto giusto.

## 3. Report programmati

- **Tracker del mese corrente** con gli obiettivi scritti nel prompt. Esempio: "My return on ad spend target is a 1x during non-promo periods, and it's around a 4x during promo periods", piu' un "king goal" del mese.
- **Live artifact:**
  1. si salva il report come HTML;
  2. in Cowork > Live artifacts lo si ricrea con "Using the Facebook Ads MCP, build this exact HTML live artifact";
  3. "Reload" ripesca i dati live.
- **Pianificazione:** "Can you please schedule this to be updated and sent to me every single day at 9:00 a.m." Le scheduled tasks girano solo con l'app desktop aperta. Per il digest consiglia Slack o email.

## 4. Anomaly detector

- **Il prompt:** "any significant change over two standard deviations across the brand", anomalie "both good and bad".
- **Come gira:**
  - 4 volte al giorno (6, 11, 15, 19);
  - metriche core spesa, ROAS, CPA, piu' le secondarie come i picchi di CPM;
  - baseline giornaliera confrontata con 3, 7 e 14 giorni;
  - prima livello account, poi campagna;
  - significativita' segnalata;
  - uscita: messaggio su Slack.

## 5. Winner detector

- **Il prompt:** "a second anomaly detector", a livello di ad, nella stessa chat per conservare il contesto.
- **Definizione:** "any ad that drives more than 5% of the total campaign spend and is above my target return on ad spend". Esclusi i giorni di saldo.
- **Finestre:** "based on 3 days of data, 7 days of data, and 14 days of data. I'm not looking for a single day spike".
- **Rifiniture:**
  - separare retention e prospecting;
  - cercare i "persistent winners across all three windows";
  - aggiungere i link alle anteprime in Ads Manager.
- **Se l'artifact esce vuoto:** "take screenshots of your own artifact that you built here and try to figure out what went wrong, troubleshoot it, and create a new one".

## 6. Skill di brand e avatar

- **La richiesta:** "Build a skill that you could easily reference. This is going to contain my brand guidelines and my avatars for my brand."
- **La ricerca:**
  - si lancia nel modello piu' potente disponibile;
  - raccoglie i problemi da forum e Reddit e produce 20 problemi, 20 angoli e i cluster di avatar (`creativita-e-avatar.md` §2);
  - "this gets us like 98% of the way there".
- **Poi** in ogni prompt creativo si richiama la skill del brand.
- **Video:** una skill con il template di brief per i creator ("we are crafting individual hooks, we're crafting individual call-outs, and we're preparing additional shot lists"), poi: "please find my top-performing video ad, extract the transcript, and then using the skill that you've just made, write a new script and brief."

## 7. Workflow creativi

- **Top creativita' della settimana:** "focus on the top three highest spending ads in the account" degli ultimi 14 giorni, con anteprima. Claude vede le immagini e le descrive.
- **Iterazioni delle statiche vincenti:**
  - il prompt: "build a variety of dynamic iterations of the same ad", richiamando la skill del brand;
  - "We're not looking for tiny little tweaks or iterations, we're looking for moderately big changes based on an original ad";
  - controllo finale: "review them before you send them off to me to make sure they follow the brand guidelines".
- **Immagini:** Claude le genera male. Si collegano altri strumenti come connettori MCP: "since you can't generate images on your own, please use the MCP to build these images for me", con 2 varianti per iterazione, formato verticale.
- **Ads Library:**
  - le ads dei concorrenti hanno la filigrana "protected" e "Claude and ChatGPT will often see this ad and not do anything with it", quindi conviene descriverle a parole;
  - il workflow con piu' impatto non sono i concorrenti ma i propri winner: "locate the top 5% of ads in my ad account that specifically are over my average return on ad spend", con soglie (es. ROAS sopra 2,1 e spesa oltre 5.000 $), ogni giorno.
- **Ciclo:** per ogni winner 2-4 brief, su un ciclo di 7-14 giorni.

## 8. Limiti

- **Chi carica tutto** gonfia l'account con "a bunch of crappy ads that don't perform", oppure con poche buone che "never get adequate spend": un death loop.
- **Filtro umano:** alla Moonlighters questi strumenti sono "a filter, almost like a step one"; "you need to make sure you have a human filter at the end of that". "be careful, limit yourself, don't overdo it in your ad account".
- **Cosa non automatizza:** scritture su budget e ads, la decisione finale sulla spesa, i video generati, gli script a calendario.
- **Conflitto d'interessi:** lo strumento creativo che mostra (SuperScale) e' in affiliazione e ha una funzione costruita insieme a lui.

## 9. Come usarlo con i clienti Stoic (interpretazione)

- **Ruoli:** stesse approvazioni di Sam, Claude legge e Stefano scrive. Le scritture via connettore (pause, budget, ads nuove) solo dopo un "si'" esplicito.
- **Una skill per cliente** con brand, avatar, offerta, tetto di costo per risultato e risultato vero (posto prenotato, abbonamento, call).
- **Report del mese** sul costo per risultato e sul risultato vero, non sul ROAS.
- **Detector tarati sui piccoli.** Con 1-3 lead al giorno un detector a 2 deviazioni standard segnala solo rumore. Meglio:
  - spesa, CPM, CTR e frequenza ogni giorno;
  - costo per lead su finestre di 3 e 7 giorni;
  - 1-2 controlli al giorno;
  - winner e potential una volta a settimana.
- **Video:** dalla trascrizione della top ad si scrivono nuovi hook e body nel formato del documento del sistema modulare, al posto del brief per creator.
- **Ricerca avatar nella lingua dell'avatar:** forum e gruppi in francese per i clienti belgi, in spagnolo e italiano per gli altri, recensioni Google e TripAdvisor dei concorrenti. Reddit pesa meno fuori dal mondo anglofono.
