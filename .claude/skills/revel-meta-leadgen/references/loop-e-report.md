# Loop di ottimizzazione e report

Indice: 1. Calendario · 2. Regole keep/kill · 3. Sostituire i perdenti · 4. Template di report · 5. Precisione dei dati · 6. Feedback dalle vendite · 7. Automazione con Claude · 8. Lavorare con un connettore Meta Ads

## 1. Calendario
| Quando | Cosa |
|---|---|
| Giorno 0 | Lancio: un ad per ad set, budget sopra la soglia, tetto CPL già deciso e scritto |
| Giorni 1-3 | Si guarda (ogni mattina la colonna risultati) ma non si tocca |
| Giorno 4 | Keep-or-kill per ogni ad contro il tetto. I perdenti si sostituiscono con ads nuove |
| Giorni 7-8 | Call prenotate, vendite e cash generati da quei lead (dal CRM). Se è positivo, si aggiunge un ad set con un ad nuovo: è la scala orizzontale |
| Ogni 2 giorni | Confronto tra i lead riportati da Meta e quelli nel CRM |
| Ogni settimana | Report su call prenotate e sentiment qualificato/non qualificato dei setter, per campagna e per ad |
| Ogni 3 settimane (a circa 100 $/giorno) | Decisioni su fenomeni "ambientali" come lead fuori zona o cali stagionali. Con budget molto più alti si accorcia |

## 2. Regole keep/kill
- **Keep**: CPL entro il tetto e, quando c'è abbastanza volume per misurarlo, costo per call entro il tetto. L'ad continua finché porta call e vendite.
- **Kill**: al giorno 4 il CPL è sopra il tetto. Si spegne e si sostituisce.
- **Eccezioni**:
  - si spegne prima se le unit economics lo permettono;
  - si aspetta 5 giorni o più se si giudica sulle call e il costo per call è alto.
- **Non si giudica al giorno 1-2.** Un ad che funziona non si "ritocca".
- **Account nuovi**: il primo metro di successo è il numero di lead nella colonna risultati, perché serve volume per capire quali ads generano lead. Entro 7 giorni si guardano le call.

## 3. Sostituire i perdenti
- **Da dove pescare**: dalla banca delle idee e dal catalogo dei tipi di ad (`creativita-e-script.md`), scegliendo prima il topic.
- **Mix per ogni ciclo** (quello che usa nella sua automazione): 3 varianti dei concetti vincenti + 2 idee molto diverse ("left field").
- **Riciclo**: i vincenti si portano in altri formati.
- **Strategia deduttiva**: guarda cosa avevano in comune i perdenti (topic, hook, formato) e fanne meno.

## 4. Template di report
Usa questa tabella per il report del ciclo di 4 giorni:

| Ad | Tipo | Topic/hook | Giorni attivi | Spesa | Lead Meta | Lead CRM | CPL (CRM) | Call prenotate | Costo per call | Sentiment Q/NQ | Decisione |
|---|---|---|---|---|---|---|---|---|---|---|---|

Sotto la tabella:
- **Totali dell'account** e scarto % tra lead in Meta e nel CRM.
- **Dove cade il funnel**: lead → contattati → call prenotate → presentati → chiusi. Il punto in cui la percentuale crolla è il vincolo su cui lavorare.
- **Azioni del prossimo ciclo**: quali ads spegnere, quali nuove lanciare (tipo + topic + hook) e quali ad set aggiungere.
- **Ipotesi e dubbi** da verificare con le vendite.

## 5. Precisione dei dati
- **Obiettivo**: oltre il 90 % di accuratezza tra i lead in Meta e quelli nel CRM. Il 100 % non c'è mai, per i fusi orari e i lead a cavallo della mezzanotte. Scarti sotto il 5 % "chi se ne frega".
- **Se Meta riporta molti più lead del CRM**: controlla i workflow che rimandano i parametri della Conversions API, per alzare l'event match quality.
- **Per decidere** usa il CPL calcolato sui lead del CRM.
- **Il beneficio principale della CAPI** è proprio questo: numeri attendibili a livello di ad e ad set, così non fai modifiche basate su dati sbagliati.

## 6. Feedback dalle vendite
- **Sentiment strutturato**: nel CRM dopo ogni chiamata, per esempio 5 opzioni per la chiamata del setter e 5 per la call del venditore.
- **Note sul contatto o sull'opportunità.**
- **Canale diretto**: un gruppo WhatsApp o Slack con i venditori per le note a caldo. Claude le estrae e le riassume.
- **Trascrizioni**: si analizzano con domande precise (prezzo, obiezioni, citazioni delle ads, motivi di non chiusura).
- **Pulizia dei dati**: i venditori vanno resi responsabili, perché da soli tendono a non tenerla.
- **Aneddoti**: ogni segnalazione del team ("tanti lead fuori zona", "lead scarsi") si verifica con i dati prima di toccare una campagna.

## 7. Automazione con Claude: cosa ha fatto Revel (ottobre 2026, sperimentale)
- **Il setup**: prima campagna lead completamente automatizzata, sull'azienda solare, con un budget dedicato. Claude ha accesso a una skill che sceglie tipi e formati di ad basandosi sul suo metodo (tipi, struttura degli script, formati).
- **Solo ads statiche**: le immagini le genera un modello di immagini; niente video AI.
- **Il ciclo, ogni 4 giorni**:
  1. Legge il CPL delle ads e lo confronta con il KPI.
  2. Controlla nel CRM gli appuntamenti prenotati rispetto al KPI di costo per appuntamento.
  3. Lascia attive le ads che rispettano i KPI e spegne le altre.
  4. Crea 3 varianti e 2 idee molto diverse, e le carica nella campagna.
- **Dopo 4 giorni**: CPL in linea con il solito e circa un appuntamento. "Onestamente le ads sono un po' bruttine": è proprio il test.
- **Il piano**: se funziona, proporre a ogni cliente circa 100 $/giorno di test di automazione su campagne VSL con immagini. Anche così, ogni account richiederà rifinitura: account diversi si comportano in modo diverso anche con stesse ads, stesso settore e stesso pubblico.
- **Già oggi**: Revel lancia la maggior parte delle sue ads tramite Claude. Carica i creativi nella libreria media e dice "ecco i prossimi 10 ads".
- **Collegamento**: un connettore. Lui è andato su una soluzione più tecnica, ma suggerisce l'MCP ufficiale di Meta.

## 8. Lavorare con un connettore Meta Ads (se disponibile nella sessione)
1. **Leggi**: insight per ad degli ultimi 4 giorni (spesa, risultati/lead, CPL, impression, CPM) e la struttura (campagna → ad set → ad, budget, evento di ottimizzazione).
2. **Incrocia**: con i dati del CRM, se c'è un connettore o un export (lead, call prenotate, sentiment, vendite).
3. **Proponi**: la tabella del §4 con le decisioni keep/kill, i nuovi creativi (tipo, topic, hook, testo o script) e gli eventuali nuovi ad set.
4. **Esegui solo dopo un "sì" esplicito** dell'utente, perché spostano soldi veri:
   - mettere in pausa;
   - creare ads o ad set;
   - cambiare budget o eventi.
   Dopo l'esecuzione, verifica che le modifiche siano andate a buon fine e riportalo.
5. **Senza connettore**: chiedi un export CSV da Ads Manager (livello ad, ultimi 4 giorni) e uno dal CRM, e lavora su quelli.
