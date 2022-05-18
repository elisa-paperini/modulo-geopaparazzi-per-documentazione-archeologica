# Modulo di Geopaparazzi per la documentazione archeologica in ricognizione
Modulo di Geopaparazzi per la documentazione archeologica in ricognizione
Modulo da inserire all'interno dell'applicazione Geopaparazzi (https://www.geopaparazzi.org/geopaparazzi/), utile per la documentazione archeologica in ricognizione. Il modulo comprende quattro diverse tipologie di schedatura: "Scheda_UT", "Scheda_Oggetto", "Scheda_tombe", "Tracce" ed è stato elaborato seguendo le istruzioni presenti all'interno del manuale fornito dagli sviluppatori dell'applicazione (HydroloGIS). 

## Scheda_UT
Scheda per la documentazione di Unità Topografiche. I campi presenti all'interno della scheda sono illustrati in Gattiglia, Stagno 2005 (GATTIGLIA G., STAGNO A. M. 2005, La documentazione scritta nella ricognizione archeologica sul territorio: un "vecchio" sistema di schedatura, "Archeologia Medievale", 35, 453-459). La scheda digitale è composta dai seguenti campi:

- **UT**: campo integer, obbligatorio. Nel quale va inserito un numero arabo progressivo, con valenza non gerarchica, per identificare l’unità topografica.
- **Provincia**: campo string, obbligatorio, preimpostato. Provincia alla quale appartiene l’UT soggetta a ricognizione.
- **Comune**: campo string, obbligatorio, preimpostato. Comune nel quale si trova l’UT.
- **Toponimo**: campo string. Toponimo presente nelle carte 1:25.000.
- **Microtoponimo**: campo string. Toponimo presente sulle carte a maggiore dettaglio o nella tradizione orale. 
- **Toponomastica**: campo string. Inserire il significato, quando possibile, del toponimo.
- **Altitudine**: campo double, automatico. Ricavata dalla cartografia a maggiore dettaglio disponibile.
- **Sit. Topografica**: campo stringcombo. Molto importante soprattutto in fase di analisi dei dati, per compilare la quale conviene utilizzare una serie di voci standardizzate da decidere all’inizio della ricerca alla luce delle caratteristiche orografiche, paesaggistiche, del territorio. Voci predefinite: "Costa", "Costa#Spiaggia", "Costa#Scogliera", "Pianeggiante", "Pedecollinare", "Versante collinare", "Sommità collinare", "Fondo valle", "Pedemontana", "Montana", "Versante montano", "Sommità montana", "Altro".
- **Sit. Topografica**: campo string. Situazione topografica da compilare nel caso in cui la voce da utilizzare è assente tra quelle del campo.
- **Longitudine**: campo double, automatico. Longitudine del punto documentato.
- **Latitudine**: campo double, automatico. Latitudine del punto documentato.
- **Altri elementi di localizzazione**: campo dynamicstring. Ogni elemento utile per individuare l’UT, soprattutto nel caso si voglia ritornare nella località indagata; è utile specificare elementi caratterizzanti e stabili come ad esempio casolari, pali della luce, corsi d’acqua, ponti ecc.
- **Strade d’accesso**: campo string. La strada più vicina alla UT.
- **Materie prime**: campo dynamicstring. Indicare quali materie prime sono presenti nelle zone limitrofe all’UT.
- **Litologia**: campo string. Desunta dalla carta geologica. 
- **Pedologia**: campo stringcombo. Si intende il tipo di sedimento. Voci predefinite: "Argilla", "Argilla limosa", "Argilla sabbiosa", "Limo sabbioso", "Limo argilloso", "Limo", "Sabbia argillosa", "Sabbia limosa", "Sabbia", "Torbe".
"Sabbia": particelle di minerali di 0.06-2 mm. I granelli sono visibili ad occhio nudo e danno impressione di ruvidezza quando vengono sfregati tra pollice ed indice.
"Limo": particelle minerali di 0.002-0.06 mm. Le particelle non sono distinguibili ad occhio nudo. I suoli che contengono alte percentuali di limo danno una sensazione saponosa o setosa al tatto e sono solo leggermente adesive (sporcano poco le dita).
"Argilla": particelle minerali inferiori a 0.002 mm. L’argilla dà forte coesione ai suoli e quando è umida dà una sensazione di forte plasticità (si può appallottolare e modellare) e di adesività (si incolla alle dita).
"Torbe": le deposizioni che contengono grandi quantità di materiali organici possono essere  solitamente definiti "torbe". Quando si possono ancora identificare singole parti dei componenti vegetali si parla di "torba strutturata"; se i componenti vegetali sono decomposti si parla di "torba amorfa". La presenza della materia organica tende a modificare le strutture del suolo, dandogli un aspetto ‘grasso’, avvertibile anche al tatto, rendendo i suoli sabbiosi più ‘pesanti’ (compatti) e i suoli argillosi più ‘leggeri’ (friabili o sciolti).
- **Vegetazione/utilizzazione del suolo**: campo string. Inserire la vegetazione o la cultura arborea nell’area delimitata dall’UT e l’uso del suolo: coltivato, specificando il tipo di coltura (monocoltura, coltura mista o ortivo); incolto. Descrivere sempre che tipo di lavorazione ha subito il terreno: aratura, il terreno si presenta a zolle, distinguere se ha subito solo l’azione del coltro (lama verticale, zolle di grandi dimensioni) o anche quella del vomere (lama orizzontale dell’aratro, zolle più piccole); fresatura, il terreno appare "frullato"; erpicatura, il terreno appare sminuzzato; lavorazione manuale, lavorato a zappa o vanga. Le voci possono essere associate nel caso si individuino successive azioni di lavorazione del terreno.
- **Coltivato**: campo stringcombo. Indicare se il terreno è coltivato e il tipo di coltura. Voci predefinite: "No", "Monocoltura", "Coltura mista", "Ortivo".
- **Incolto**: campo stringcombo. Indicare se il terreno è incolto. Voci predefinite: "No",  "Sì".
- **Aratura**: campo stringcombo. Indicare se il terreno è arato e con quale mezzo. Voci predefinite: "No", "Coltro", "Vomere".
- **Fresatura**: campo stringcombo. Indicare se il terreno si presenta fresato. Voci predefinite: "No",  "Sì".
- **Erpicatura**: campo stringcombo. Indicare se il terreno si presenta erpicato. Voci predefinite: "No",  "Sì".
- **Terra in situ / di riporto**: campo stringcombo. Indicare se la terra dell’UT in esame sia in situ o di riporto. Questa voce si può compilare solo grazie all’ausilio delle fonti orali, risulta fondamentale per l’interpretazione del ritrovamento cercare di identificare la provenienza della terra. Voci predefinite: "In situ", "Di riporto".
- **Zona di provenienza della terra di riporto**: campo string. Indicare la zona di provenienza della terra.
- **Proprietà**: campo string. Cognome e nome del proprietario della particella catastale nella quale è sita l’UT in esame. 
- **Fonti orali**: campo string. Cognome e nome delle fonti orali intervistate che hanno fornito indicazioni sull’UT.
- **Ric. N°**: campo integer, preimpostato. Indicare con un numero ordinale se sia la prima ricognizione di quell’unità topografica o una delle successive ripetizioni.
- **Metodo**: campo stringcombo. Si compila con la dizione intensivo, quando sia possibile effettuare una ricognizione sistematica per file parallele (campi, uliveti, vigneti, e simili) o che permetta di individuare i limiti di un’attività sepolta (a.e. carbonaie) o estensivo, quando non sia possibile coprire uniformemente l’area indagata (fitta copertura vegetale, strutture murarie che non vengano indagate analiticamente); shovel test, nel caso si effettui una tale indagine stratigrafica. Voci predefinite: "Intensivo", "Estensivo", "Shovel test".
- **N° Ricognitori**: campo integer. Numero dei ricercatori che hanno effettuato la ricognizione dell’UT.
- **Equidistanza**: campo integer. Equidistanza tra i ricognitori, da indicare solo nel caso sia stato effettuata una ricognizione per file parallele.
- **Condizioni di visibilità**: campo connectedstringcombo, obbligatorio. Viene compilata con una griglia standardizzata di 5 valori: ottima, buona, media, scarsa, nulla nei quali si tengono presenti sia il tipo di condizione del terreno (arato, fresato, incolto, ecc.) sia il grado di copertura vegetale, quindi la porzione percentuale, intuitiva, di terreno visibile. Voci predefinite: "Seminativo e Seminativo arborato":["Ottima", "Buona","Media"], "Colture arboree e promiscue":["Buona", "Media", "Scarsa", "Nulla" ], "Terreno non lavorato":["Media", "Scarsa", "Nulla"], "Bosco":["Ottima", "Buona", "Media", "Scarsa", "Nulla"].
- **Data**: campo date, automatico. Giorno, mese, anno.
- **Ora**: campo time, automatico. Ora di inizio della ricognizione dell’UT.
- **Condizioni di luce**: campo string, obbligatorio. Condizioni meteorologiche e grado di incidenza dei raggi solari, luce radente, luce diffusa.
- **Definizione**: campo string. Deve essere il più possibile oggettiva e generica a.e. struttura muraria, casolare, area sporadica, concentrazione, carbonaia.
- **Cronologia Iniziale-Finale**: campo multistringcombo. Indicare il periodo dell’UT. Voci predefinite: "Preistoria", "Protostoria", "Periodo etrusco", "Periodo ligure", "Periodo romano repubblicano", "Periodo romano imperiale", "Alto medioevo", "Basso medioevo", "Età moderna", "Età contemporanea", "Età subcontemporanea", "Età subattuale", "Età attuale".
- **Secoli**: campo string. Specificare la cronologia dell’UT documentata in secoli con numeri arabi.
- **Anno**: campo double. Specificare la cronologia dell’UT documentata in anni con numeri arabi.
- **Asse max**: campo double. Inserire le misure dell’asse massimo dell’UT. 
- **Asse min**: campo double. Inserire le misure dell’asse minimo dell’UT.
- **Orientamento Asse max**: campo string. Indicare l’orientamento dell’asse massimo dell’UT.
- **Orientamento Asse min**: campo string. Indicare l’orientamento dell’asse minimo dell’UT.
Andamento del terreno: campo string. Specificare se il terreno è pianeggiante o se si tratta di un pendio più o meno lieve.
- **Quota min**: campo double. Segnalare la quota minima s.l.m.
- **Quota max**: campo double. Segnalare la quota massima s.l.m.
- **Descrizione**: campo string. Deve essere compilata nella maniera più obiettiva e dettagliata possibile, descrivendo l’UT in maniera fotografica; è importante che il ricercatore annoti ogni minimo particolare, soprattutto la disposizione topografica dei vari componenti dell’UT, ceramici, laterizi, litici, ecc. nonché la loro quantità e concentrazione.
Nel caso si documenti un casolare all’interno di questa voce si inseriranno i rapporti stratigrafici (si immorsa, si appoggia) tra i vari corpi di fabbrica riscontrati di cui si compilerà a parte l’apposita scheda CF.
- **Stato di Conservazione/Leggibilità**: campo connectedstringcombo. La prima voce va compilata solo nel caso di strutture in elevato, mentre la seconda nel caso di concentrazioni:
- **Stato di conservazione**: Ottimo (strutture interamente conservate con l’alzato dei muri e la copertura del tetto); Buono (strutture che conservano solo l’alzato dei muri, ma non la copertura del tetto); Discreto (strutture di cui è conservata solo una traccia dei muri, dalla quale si può tuttavia individuare almeno parte della pianta della struttura in esame); Cattivo (strutture delle quali non restano che tracce sparse non interpretabili o riconducibili ad una pianta). Leggibilità: Ottimo (nel caso in cui dalla superficie dell’area è possibile individuare la pianta delle strutture sottostanti), Buono (nel caso, in cui, pur non essendo possibile individuare la pianta, è tuttavia possibile ricostruire con esattezza il perimetro della struttura sottostante), Cattivo (nel caso in cui la concentrazione non sia rapportabile, in modo chiaro, alla pianta delle strutture sottostanti). Voci predefinite: "Stato di Conservazione (strutture in elevato)": ["Ottimo", "Buono", "Discreto", "Cattivo"], "Leggibilità (concentrazioni)": ["Ottimo", "Buono", "Discreto", "Cattivo"].
- **Ceramica**: campo dynamicstring.  Classi ceramiche immediatamente riconoscibili e datanti. Reperti geologici: campo dynamicstring.  Arenaria, calcare, pietra serena, travertino, ecc.
- **Reperti organici**: campo dynamicstring. Carboni, semi, ossa umane, fauna, malacofauna, legno.
- **Altri manufatti**: campo dynamicstring. Laterizi, metalli, monete, vetri, scorie, scarti di lavorazione, ossa lavorate, malta, calce, litici lavorati, intonaci.
- **Rilievi**: campo string. Tipo di rilievo eventualmente eseguito (sezione, pianta, prospetto), scala, numero relativo all’elenco dei rilievi grafici.
- **Fotografie**: campo string. Presenza di fotografie scattate con macchina fotografica.
- **Dati Ambientali**: campo string. Descrizione sintetica del paesaggio circostante l’UT in esame, annotando tipo di vegetazione, andamento del terreno, corsi d’acqua, presenza di strutture di qualsiasi genere, specificandone i limiti spaziali. Se possibile documentare eventuali cambi di destinazione dell’uso del suolo (riconversioni agricole o arboree).
- **Interpretazione**: campo string. Analisi delle tracce archeologiche che formano l’unità topografica, conclusioni generali relative alla funzione dell’UT; deve essere compilata sul campo in base alle impressioni del ricercatore. Se non si è potuti giungere ad una definizione di questi aspetti, questo deve essere scritto, specificando con chiarezza il motivo. Possono essere inseriti in questo spazio i particolari dell’identificazione dell’UT e l’eventuale rapporto con le ipotesi iniziali di lavoro.
- **Prospettive di ricerca**: campo string. Da compilare nel caso che si ritenga  interessante approfondire lo studio dell’UT, con ulteriori ricognizioni o, se possibile, con saggi di scavo.
- **Problemi di tutela**: campo string. Inserire se l’UT è considerata a rischio, specificando i motivi della sua possibile totale o parziale scomparsa.
- **Foto dell’UT**: campo pictures. Fotografia dell’UT e dell’eventuale schizzo dell’unità topografica eseguito a mano su un foglio, annotando sempre la scala adottata e l’orientamento.
- **Fonti indirette**: campo string. Documenti archivistici e/o cartografici inerenti l’UT.
Nel caso di casolari lo schizzo dovrà rappresentare la pianta generale con le divisioni numerate dei vari corpi di fabbrica per ognuno dei quali si compilerà, con la medesima numerazione, l’apposita scheda CF.
- **Bibliografia**:  campo string. Bibliografia consultata riferibile all’UT.
- **Data del controllo finale**: campo string. Data revisione scheda.
- **Responsabile ricognizione**: campo string, preimpostato. Nome responsabile scientifico.
- **Responsabile scheda**: campo string, obbligatorio. Nome compilatore scheda.

## Scheda_Oggetto
Scheda per la documentazione di manufatti di età contemporanea. La scheda è composta dai seguenti campi:

- **ID**: campo integer, obbligatorio. Numero identificativo progressivo del manufatto.
- **Provincia**: campo string, obbligatorio, preimpostato. Provincia del luogo in cui si effettua la ricognizione.
- **Comune**: campo string, obbligatorio, preimpostato. Comune del luogo in cui si effettua la ricognizione.
- **Anno**: campo double, obbligatorio, preimpostato. Anno in cui si effettua la ricognizione.
- **Sigla**: campo string, obbligatorio, preimpostato. Sigla arbitraria utilizzata per identificare la ricognizione. Solitamente composta dalle iniziali del posto in cui è effettuata la ricognizione e dall'anno.
- **Toponimo**: campo string. Toponimo del luogo in cui viene effettuata la ricognizione. Solitamente si ricava dalla carta geografica, è possibile utilizzare anche il nome di una strada o di una piazza.
- **UT di riferimento**: campo string. Numero dell'UT a cui è collegato l'oggetto.
- **Foto sul campo1**: campo stringcombo, obbligatorio. Presenza di fotografie dell'oggetto scattate sul campo. Voci predefinite: "Sì", "No".
- **Foto sul campo2**: campo pictures, obbligatorio. Fotografia scattata nelle condizioni di ritrovamento dell'oggetto con indicazione della misura e del Nord.
- **Definizione oggetto**: campo string, obbligatorio. Breve definizione della traccia utile per caratterizzarla.
- **Posizione**: campo stringcombo, obbligatorio. Disponibilità di raggiungere e raccoglie l'oggetto. Voci predefinite: "Raggiungibile", "Non raggiungibile".
- **Luogo di ritrovamento1**: campo stringcombo, obbligatorio. Caratteristiche del luogo in cui viene ritrovato l'oggetto. Voci predefinite: "Scogliera", "Spiaggia", "Strada", "Discarica", "Cimitero", "Radura", "Spiazzo urbano", "Altro".
- **Luogo di ritrovamento2**: campo string. Indicazione delle caratteristiche del luogo in cui viene ritrovato l'oggetto, da compilare nel caso in cui la voce da utilizzare è assente tra quelle del campo Luogo di ritrovamento1.
- **Condizioni metereologiche**: campo stringcombo, obbligatorio. Indicazione delle condizioni metereologiche presenti nel momento della documentazione. Voci predefinite: "Soleggiato", "Nuvoloso", "Pioggia", "Vento".
- **Visbilità**: campo stringcombo, obbligatorio. Indicazione delle condizioni di visibilità al momento della ricognizioni. La scelta dell'aggettivo tiene presente delle condizioni dell'ambiente circostante l'oggetto documentato come per esempio la diffusione della luce o elementi di disturbo (presenza di fattori naturali come vegetazione folta, diffusione di foglie secche sulla superficie). Voci predefinite: "Ottima", "Buona", "Sufficiente", "Scarsa".
- **Contesto di ritrovamento1**: campo stringcombo, obbligatorio. Relazione tra l'oggetto documentato e altri elementi presenti nelle immediate vicinanze. Viene scelta la voce "Isolato" per indicare che nell'ambiente circostante l'oggetto sono assenti altri elementi; Viene scelta la voce "Accumulo" se l'oggetto è collocato insieme ad altro materiale spazialmente accatastato; Viene scelta la voce "Dispersione" nel caso in cui l'oggetto è collocato nelle vicinanze di altro materiale. Viene scelta la voce "Altro" se nessusa delle precedenti voci rispecchia il contesto di ritrovamento dell'oggetto. Voci predefinite: "Isolato", "Accumulo", "Dispersione", "Altro".
- **Contesto di ritrovamento2**: campo string. Relazione tra l'oggetto documentato e altri elementi presenti nelle immediate vicinanze. da compilare nel caso in cui la voce da utilizzare è assente tra quelle del campo Contesto di ritrovamento1.
- **Stato di conservazione**: campo stringcombo, obbligatorio. Indicazione dello stato di conservazione dell'oggetto documentato. Viene scelta la voce "Integro" nel caso in cui l'oggetto si presenta completo degli elementi che lo caratterizzano; viene scelta la voce "Frammentato" nel caso in cui l'oggetto si presenta suddiviso in più elementi rinvenuti nelle vicinanze dello stesso. viene scelta la voce "Parziale" se l'oggetto presenta elementi mancanti non rinvenuti nell'ambiente circostante. Voci predefinite: "Integro", "Frammentato", "Parziale".
- **Dimensioni**: campo string. Indicazione delle misure dell'oggetto. Per omologare il contenuto dei campi è possibile scegliere un'unità di misura (per esempio centimetri) e un metodo standard di trascrizione delle misure (per esempio basexaltezzaxprofondità). 
- **Colore**: campo string. Elenco dei colori che caratterizzano l'oggetto.
- **Superficie**: campo string. Elenco delle caratteristiche fisiche dell'oggetto (per esempio: ruvida, liscia, deteriotata, opaca).
- **Materiali**: campo string, obbligatorio. Elenco dei materiali di cui è composto l'oggetto (per esempio: plastica, metallo, vetro).
- **Tipologia**: campo string, obbligatorio. Classe di oggetti a cui appartiene l'oggetto documentato (per esempio bottiglia, attrezzatura navale, legname, farmaco). Il campo aperto "Tipologia" può essere utilizzato con l'ausilio di un elenco di classi tipologiche esterno all'applicazione in modo da avere una linea guida che aiuti a normalizzare i dati già nella fase della raccolta.
- **Presenza marchi**: campo stringcombo, obbligatorio. Presenza o assenza di marchi che caratterizzano l'oggetto (per esempio: Coca-Cola, Dixan, Nestlè). Voci predefinite: "Sì", "No".
- **Posizione marchio**: campo string. Indicazione della collocazione del marchio (per esempio: corpo, centrale, in basso a destra).
Leggibilità marchio, campo stringcombo. Leggibilità del marchio presente sull'oggetto.
- **Trascrizione marchio1**: campo string. Trascrizione del marchio, nella trascrizione del marchio sono impiegati i criteri di trascrizione tipici dell'epigrafia classica.
- **Trascrizione marchio2**: campo pisctures. Foto del marchio presente sull'oggetto.
Elementi identificativi, campo stringcombo, obbligatorio. Presenza o assenza di elementi identificativi che caratterizzano l'oggetto (per esempio: etichetta con indicazioni del lavaggio, codice a barre). Voci predefinite: "Sì", "No".
- **Posizione elementi identificativi**: campo string. Indicazione della collocazione degli elementi identificativi (per esempio: corpo, centrale, in basso a destra).
- **Leggibilità elementi identificativi**: campo stringcombo, Leggibilità degli elementi identificativi presenti sull'oggetto.
- **Trascrizione elementi identificativi1**: campo string. Trascrizione degli elementi identificativi, nella trascrizione degli elementi identificativi sono impiegati i criteri di trascrizione tipici dell'epigrafia classica.
- **Trascrizione elementi identificativi2**: campo pictures. Foto degli elementi identificativi presenti sull'oggetto.
- **Elementi datanti**: campo string. Trascrizione degli elementi datanti presenti sull'oggetto documentato.
- **Foto in laboratorio**: campo stringcombo. Presenza di fotografie dell'oggetto documentato scattate in laboratorio. Voci predefinite: "Sì", "No".
- **Prelievo**: campo stringcombo, obbligatorio. Indicazione riguardante l'operazione di raccolta dal luogo di ritrovamento dell'oggetto documentato. Voci predefinite: "Sì", "No".
- **Descrizione**: campo string, obbligatorio. Descrizione oggettiva degli elementi caratterizzanti l'oggetto documentato.
- **Interpretazione**: campo string, obbligatorio. Osservazioni, pensieri e ipotesi sull'oggetto documentato.
- **Note**: campo string. Eventuali note, solitamente utilizzato per comunicazioni di servizio volte ad agevolare il lavoro post-ricognizione.
- **Note_schizzo**: campo sketch. Eventuali note in modalità di disegno a mano libera.
- **Longitudine**: campo double, automatico. Longitudine del punto documentato.
- **Latitudine**: campo double, automatico. Latitudine del punto documentato.
- **Oggetto associabile a fonte orale**: campo stringcombo. Presenza o assenza di fonti orali associabili all'oggetto documentato. Voci predefinite: "Sì", "No".
- **Informazioni fonte orale**: campo string. Descrizione delle fonti orali associabili all'oggetto documentato.
- **Analisi effettuate sull'oggetto**: campo string. Indicazione delle eventuali analisi di laboratorio effettuate sull'oggetto documentato.
- **Data**: campo date, automatico. Giorno, mese e anno del momento in cui viene documentata la traccia.
- **Ora**: campo time, automatico. Ora del momento in cui viene documentata la traccia.
- **Compilatore scheda**: campo string, obbligatorio. Nome e cognome della/e persona/e che ha/hanno compilato la documentazione.
- **Responsabile progetto**: campo string, obbligatorio. Nome e cognome del responsabile progetto.
- **Revisione scheda**: campo stringcombo, preimpostato. Indicazione che riguarda l'esecuzione della revisione della scheda da parte del responsabile progetto. Voci predefinite: "Sì", "No".

## Scheda_tombe
Scheda per la documentazione veloce di tombe elaborata ai fini di rilevare posizione, quantità e aspetto delle tombe presenti all'interno di un cimitero. La scheda è composta dai seguenti campi:

- **ID**: campo integer, obbligatorio. Numero identificativo progressivo dell'elemento documentato.
- **Provincia**: campo string, obbligatorio, preimpostato. Provincia del luogo in cui si effettua la ricognizione.
- **Comune**: campo string, obbligatorio, preimpostato. Comune del luogo in cui si effettua la ricognizione. 
- **Località**: campo string, obbligatorio, preimpostato. Luogo in cui si effettua la ricognizione.
- **Sigla**: campo string, obbligatorio, preimpostato. Sigla arbitraria utilizzata per identificare la ricognizione. Solitamente composta dalle iniziali del posto in cui è effettuata la ricognizione e dall'anno.
- **Foto**: campo pictures, obbligatorio. Foto dell'elemento documentato.
- **Longitudine**: campo double, automatico. Longitudine del punto documentato.
- **Latitudine**: campo double, automatico. Latitudine del punto documentato.
- **Tipologia sepoltura**: campo multistringcombo, obbligatorio. Tipologia della tomba documentata. Voci predefinite: "Singola", "Multipla", "Loculo", "A terra", "Terragna", "Cappella".
- **Collocazione**: campo stringcombo, obbligatorio. Contesto di ritrovamento e relazione con gli elementi circostanti. Voci predefinite: "Isolata a terra", "Inserita in cappella comune", "Inserita in campo comune", "item":"In colombaia".
- **Materiali**: campo multistringcombo, obbligatorio. Materiali di cui è composto l'elemento documentato. Voci predefinite: "Cemento", "Muratura", "Ceramica", "Marmo", "Granito", "Altra pietra", "Terra", "Legno".
- **Orientamento**: campo string. Indicazione dell'orietamento della tomba secondo i punti cardinali.
- **Numero corpi sepolti**: campo integer. Numero dei corpi sepolti.
- **Nome1**: campo stringcombo, obbligatorio. Presenza del nome e del cognome della/e persona/e sepolta/e. Voci predefinite: "Sì", "No", "Incerto".
- **Nome2**: campo string. Trascrizione del nome e del cognome della/e persona/e sepolta/e.
- **Data di nascita1**: campo stringcombo, obbligatorio. Presenza della data di nascita della/e persona/e sepolta/e. Voci predefinite: "Sì", "No", "Incerta".
- **Data di nascita2**: campo string. Trascrizione della data di nascita della/e persona/e sepolta/e.
- **Data di morte1**: campo stringcombo, obbligatorio. Presenza della data di morte della/e persona/e sepolta/e. Voci predefinite: "Sì", "No", "Incerta".
- **Data di morte2**: campo string. Trascrizione della data di nascita della/e persona/e sepolta/e.
- **Età1**: campo stringcombo, obbligatorio. Presenza dell'età di morte della/e persona/e sepolta/e. Voci predefinite: "Sì", "No", "Incerta".
- **Età2**: campo string. Trascrizione dell'età di morte della/e persona/e sepolta/e.
- **Sesso**: campo multistringcombo, obbligatorio. Indicazione del sesso della/e persona/e sepolta/e.  Voci predefinite: "Maschio", "Femmina", "Ignoto".
- **Paese di provenienza dell'imbarcazione1**: campo stringcombo, obbligatorio. Presenza del paese di provenienza dell'imbarcazione della/e persona/e sepolta/e. Voci predefinite: "Sì", "No", "Incerto".
- **Paese di provenienza dell'imbarcazione2**: campo string. Trascrizione dell'indicazione del paese di provenienza dell'imbarcazione della/e persona/e sepolta/e.
- **Paese di origine delle persone1**: campo stringcombo, obbligatorio. Presenza del paese di origine della/e persona/e sepolta/e. Voci predefinite: "Sì", "No", "Incerto".
- **Paese di origine delle persone2**: campo string. Trascrizione dell'indicazione del paese di origine della/e persona/e sepolta/e.
- **Presenza fotografia defunto**: campo stringcombo, obbligatorio. Presenza dell'immagine del/i defunto/i. Voci predefinite: "Sì", "No".
- **Altri elementi scritti/figurativi/altro1**: campo stringcombo, obbligatorio. Presenza sulla tomba di ogni elemento scritto o figurativo in grado di caratterizzarla. Voci predefinite: "Sì", "No".
- **Altri elementi scritti/figurativi/altro2**: campo string. Trascrizione di ogni elemento scritto o figurativo in grado di caratterizzarla.
- **Elementi regiosi1**: campo stringcombo, obbligatorio. Presenza di elementi religiosi. Voci predefinite: "Sì", "No", "Incerto".
- **Elementi religiosi2**: campo string. Descrizione degli elementi religiosi presenti.
- **Pulizia**: campo stringcombo, obbligatorio. Indicare se l'ambiente circostante la tomba è mantenuto pulito. Voci predefinite: "Sì", "No", "Media".
- **Presenza elementi di cura1**: campo stringcombo, obbligatorio. Presenza di elementi di cura (per esempio sassi, giocattoli, piccole statue). Voci predefinite: "Sì", "No".
- **Presenza elementi di cura2**: campo string. Descrizione degli elementi di cura.
- **Presenza Fiori**: campo stringcombo, obbligatorio. Presenza o assenza di fiori. Voci predefinite: "No", "Veri", "Finti".
- **Trascrizione targa/lapide**: campo string. Trascrizione delle informazioni presenti su targhe o lapidi appartenenti all'elemento documentato.
- **Descrizione**: campo string, obbligatorio. Descrizione oggettiva degli elementi caratterizzanti l'elemento documentato.
- **Interpretazione**: campo string, obbligatorio. Osservazioni, pensieri e ipotesi sull'elemento documentato.
- **Compilatore scheda**: campo string, obbligatorio. Nome e cognome della/e persona/e che ha/hanno compilato la documentazione.
- **Data**: campo date, automatico. Giorno, mese e anno del momento in cui viene documentata la traccia.
- **Responsabile**: campo string, obbligatorio, preimpostato. Nome e cognome del responabile progetto.

## Tracce
Scheda per la documentazione di generiche tracce del paesaggio antropizzato. La scheda è composta dai seguenti campi:

- **Definizione**: campo string. Breve definizione della traccia utile per caratterizzarla.
- **Foto**: campo pictures. Fotografia della traccia da documentare.
- **Data**: campo date, automatico. Giorno, mese e anno del momento in cui viene documentata la traccia.
- **Ora**: campo time, automatico. Ora del momento in cui viene documentata la traccia.
- **Longitudine**: campo double, automatico. Longitudine del punto documentato.
- **Latitudine**: campo double, automatico. Latitudine del punto documentato.

## Installazione
Per utilizzare il modulo è necessario scaricare l'applicazione sul prorpio dispositivo mobile e inserire il file "tags.json" all'interno della cartella Geopaparazzi. Di seguito sono illustrati due metodi con cui è possibile caricare il file nell'applicazione.

A. Caricare il file "tags.json" con cavo USB
  1. Scaricare sul pc il file "tags.json";
  2. Collegare il cellulare al computer e abilitarlo al trasferimento dei dati;
  3. Seguire il percorso "esplora file"> nome_smartphone> "gestione file"> "memoria interna"> "geopaparazzi";
  4. Sostituire il file "tags.json" già presente nell’applicazione con il file "tags.json" scaricato sul pc.

B. Caricare il file "tags.json" con cavo USB
  1. Aprire Github dallo smartphone e scaricare il file "tags.json";
  2. Seguire il percorso "gestione file"> "memoria interna"> "download";
  3. Selezionare il file "tags.json" tenendolo premuto. Cliccare sulla funzione "sposta" in basso a destra. Tornare indietro nel percorso cliccando su "memoria interna" in alto a sinistra;
  4. Cercare la cartella "geopaparazzi" e cliccarci. Confermare il comando "sposta" in basso a destra;
  5. Cliccare su "sostituisci".
In entrambi i casi è necessario evitare di rinominare il file "tags.json". Se l’operazione è andata a buon fine, nella funzione "note" di Geopaparazzi compare una schermata che presenta la possibilità di scegliere uno tra i quattro tipi di schedatura sopracitati presenti nel modulo. In base alle impostazioni e al modello dello smartphone i percorsi indicati potrebbero essere leggermente diversi.

## Modifiche
Il presente modulo può essere modificato e aggiornato in base alle proprie esigenze. Nella scheda il nome dei campi è scritto tra due asterischi in modo da facilitare l'operazione di pulizia del file kml esportato dall'applicazione. I campi indicati come preimpostati presentano un valore di esempio inserito in fase di programmazione del file .json, in ogni scheda tali campi saranno autocompilati con lo stesso contenuto. Per modificare il modulo è possibile aprire il file "tags.json" con un editor di testo (per esempio Sublime, Notepad++, o il blocco note presente di default sul proprio computer) e seguire le istruzioni presenti alla sezione 13 del manuale fornito dagli sviluppatori dell'applicazione (HydroloGIS).

## Licenza
CC BY-SA 4.0

## Autori
Elisa Paperini, Francesca Anichini, Gabriele Gattiglia
