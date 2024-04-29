# Repository Github del Progetto LEO - open data

Questo è il repository ufficiale degli open data del progetto LEO. In questo repository pubblico potete trovare tutte le ontologie e vocabolari controllati, e le relative versioni, che sono state sviluppate nel progetto, nonché altro materiale prodotto a supporto della componente open data.

Le ontologie sono organizzate in una rete interconnessa, seguendo lo stesso approccio metodologico della [rete nazionale di ontologie OntoPiA](ttps://github.com/italia/daf-ontologie-vocabolari-controllati). Le ontologie del progetto LEO riusano poi direttamente alcune ontologie di OntoPiA, in particolare [l'ontologia fondazionale di OntoPiA L0](https://github.com/italia/daf-ontologie-vocabolari-controllati/tree/master/Ontologie/l0/latest).

Al momento la rete si compone dei seguenti moduli:

1.	[**il modulo leo**](https://w3id.org/leo/onto/leo) – rappresenta l'intera rete di ontologie del progetto LEO,; essa importa tutti gli altri moduli, sviluppati a seguito dell’analisi dei modelli concettuali delle fonti interne. Questo significa che il modulo LEO è il punto d’entrata a tutta la rete di ontologie del progetto LEO;
2.	[**il modulo animal**](https://w3id.org/leo/onto/animal)  – tale modulo modella le informazioni anagrafiche degli animali d’allevamento quali per esempio, il nome corto, il numero unico associato all’animale (matricola), la razza, la sua destinazione (vita o macello).
3.	[**il modulo AnimalLifeEvent (ale)**](https://w3id.org/leo/onto/ale) – è il modulo ontologico utilizzato per modellare tutte le informazioni relative agli eventi della vita degli animali da allevamento come per esempio, la nascita, lo spostamento, l’identificazione, la morte, l’aborto, ecc. Ogni evento accade in un’azienda ed è caratterizzato da specifiche informazioni che si possono applicare a uno o più animali;
4.	[**il modulo analysis**](https://w3id.org/leo/onto/analysis)  –  è il modulo ontologico utilizzato per modellare tutte le informazioni relative ai dati di laboratorio (come per esempio le analisi sul totale degli acidi grassi saturi nel campione di latte dell’animale, le analisi sulla concentrazione di urea nel latte, ecc.). Esso modella le specifiche misurazioni di laboratorio. All’interno di questo modulo sono contenute anche informazioni relative alla salute dell’animale (health data) come per esempio l’analisi IBR (per una descrizione più dettagliata ci si riferisca alla sezione “Modulo ontologico Analysis”);
5.	[**Il modulo company (co)**](https://w3id.org/leo/onto/co) – è il modulo ontologico utilizzato per modellare tutte le informazioni sull’ubicazione in aziende, di tipo diverso, dell’animale d’allevamento. Il modulo modella inoltre informazioni sull’ubicazione fisica degli animali (caratteristiche dell’ambiente o fabbricato rurale), nonché la loro localizzazione geografica (in quest'ultimo caso riutilizzando direttamente [l'ontologia dei luoghi di OntoPiA](https://github.com/italia/daf-ontologie-vocabolari-controllati/tree/master/Ontologie/CLV/latest);
6.	[**Il modulo livestock indicator**](https://w3id.org/leo/onto/livestock-indicator) – questo modulo consente di gestire tutta una serie di indicatori dell’ambiente zootecnico. In particolare, il modulo ontologico include la modellazione dell’indicatore di benessere animale, calcolato sulla base di misurazioni periodiche svolte nell’ambiente rurale, e una serie di indicatori genetici associato all’animale;
7.	[**Il modulo weather**](https://w3id.org/leo/onto/weather) – è il modulo ontologico utilizzato per rappresentare i dati sulle rilevazioni meteo fatti da stazioni meteo. Il modulo, di fatto, specializza [l’ontologia della rete nazionale OntoPIA IoT](https://github.com/italia/daf-ontologie-vocabolari-controllati/tree/master/Ontologie/IoT/latest), modellando solo gli aspetti specifici relativi alle rilevazioni meteo e lasciando ogni altro elemento di modellazione all’ontologia nazionale, quest’ultima già allineata a diversi standard internazionali;
8. [**il modulo livestockfarm building description**](https://w3id.org/leo/onto/livestockfarm-building-description) - è il modulo ontologico utilizzato per rappresentare i dati sugli edifici (insediamenti) di un'azienda d'allevamento. Nel contesto del dominio LEO i dati modellati con questa ontologia sono quelli del questionario del sistema Si@llEvA relativamente alla parte 'Configuratore Insediamento';
9. [**il modulo livestockfarm description**](https://w3id.org/leo/onto/livestockfarm-description) - è il modulo ontologico utilizzato per rappresentare i dati sull'azienda d'allevamento. Nel contesto del dominio LEO i dati modellati con questa ontologia sono quelli del questionario del sistema Si@llEvA relativamente alla parte 'Configuratore';
10. [**il modulo livestock assessment**](https://w3id.org/leo/onto/livestock-assessment) - è un modulo ontologico tecnico usato per definire generici controlli che vengono effettuati nel contesto zooetecnico. Tale modulo è specializzato poi in moduli ontologici utilizzati per rappresentare specifici controlli come gli accertamenti sanitari, i controlli funzionali, i controlli sull'efficienza della mungitura, i controlli a seguito della lattazione;
11. [**il modulo health assessmnet**](https://w3id.org/leo/onto/health-assessment) - è il modulo ontologico utilizzato per rappresentare i dati sugli accertamenti sanitari e sugli screening aziendali. I dati provengono da servizi di cooperazione applicativa direttamente dall’Istituto Zooprofilattico Umbria-Marche;
12. [**il modulo milking efficiency assessment**](https://w3id.org/leo/onto/milking-efficiency-assessment) - è il modulo ontologico utilizzato per rappresentare tutti i tipi di controlli effettuati per la valutazione dell'efficienza della mungitura. Alcuni dei controlli variano a seconda dello strumento utilizzato (Vadia, Lactocorder) e mirano anche a valutare aspetti tecnici degli stessi impianti usati nella mungitura;
13. [**il modulo milk functional testing**](https://w3id.org/leo/onto/milk-functional-assessment) - è il modulo ontologico utilizzato per rappresentare i controlli funzionali sul latte;
14. [**il modulo lactation assessment**](https://w3id.org/leo/onto/lactation-assessment) - è un modulo ontologico utilizzato per rappresentare le informazioni di controllo collezionate sulla lattazione degli animali da latte e da carne. Il modello rappresenta i dati provenienti dal sistema SIALL attraverso servizi di cooperazione applicativa messi a punto per il progetto LEO.
15. [**il modulo apiary**](https://w3id.org/leo/onto/apiary) - è un modulo ontologico utilizzato per rappresentare le informazioni relative ad apiari nelle aziende proprietarie.


Oltre alle ontologie, il presente repository include inoltre una serie di vocabolari controllati:

1. [**Razze (breed)**](https://w3id.org/leo/controlled-vocabulary/breed): è il vocabolario controllato delle razze degli animali dell'ambiente zootecnico. Il vocabolario include collegamenti a dataset esterni disponibili come Linked Open Data (e.g., wikidata);
2. [**Specie zootecniche (livestock-species)**](https://w3id.org/leo/controlled-vocabulary/livestock-species): è il vocabolario controllato delle specie zootecniche. Il vocabolario include collegamenti a dataset esterni disponibili come Linked Open Data (e.g., Agrovoc, Eurovoc);
3. [**Unità di misura (measurement-unit)**](https://w3id.org/leo/controlled-vocabulary/measurement-unit): è il vocabolario controllato delle unità di misura utilizzate nel progetto LEO. Il vocabolario include collegamenti a dataset esterni disponibili come Linked Open Data (e.g., Wikidata, EU vocabulary del EU Publication Office).
4. [**Categoria delle carcasse dei bovini**](https://w3id.org/leo/controlled-vocabulary/bovine-carcass-category): è il vocabolario controllato per la categorizzazione delle carcasse dei bovini.  Il sistema di categorizzazione di riferimento, che definisce le categorie in cui sono ripartite le carcasse bovine, è definito nel regolamento (UE) n. 1308/2013 del Parlamento europeo e del Consiglio del 17 dicembre 2013.
5. [**Classificazione delle carcasse dei bovini**](https://w3id.org/leo/controlled-vocabulary/bovine-carcass-classification): è il vocabolario controllato per la classificazione delle carcasse dei bovini. Il sistema di classificazione di riferimento è definito nel regolamento (UE) n. 1308/2013 del Parlamento europeo e del Consiglio del 17 dicembre 2013. La classificazione delle carcasse di bovini si effettua valutando la conformazione e lo stato d'ingrassamento della carcassa.
6. [**Motivi di ingresso**](https://w3id.org/leo/controlled-vocabulary/entry-in-farm-reason): è il vocabolario controllato utilizzato per indicare i motivi di ingrasso di un animale d'allevamento in una azienda;
7. [**Motivi di uscita**](https://w3id.org/leo/controlled-vocabulary/exit-from-farm-reason): è il vocabolario controllato utilizzato per indicare i motivi di uscita di un animale d'allevamento da un'azienda;
8. [**Indirizzi/Orientamenti produttivi**](https://w3id.org/leo/controlled-vocabulary/production-type): è il vocabolario controllato sugli orientamenti e indirizzi produttivi di un animale d'allevamento (e.g., carne, latte, lana, etc.)
9. [**Stato del capo**](https://w3id.org/leo/controlled-vocabulary/farm-animal-status): è il vocabolario controllato dello stato dell'animale d'allevamento.
10. [**Famiglie Zootecniche**](https://w3id.org/leo/controlled-vocabulary/livestock-family): è il vocabolario controllato delle famiglie zootecniche (equidi, bovidi, ecc.).
11. [**Frequenze del controllo funzionale del latte** ](https://w3id.org/leo/controlled-vocabulary/milk-functional-testing-frequencies): è il vocabolario controllato delle frequenze con cui vengono eseguiti i controlli funzionali sul latte


## Maintainers
-	Mario Rossi: git (mariorossi12345) - email (mariorossi12345@mail.it)
-	Giovanni Verdi: git (giovanniverdi12345) - email (giovanniverdi1234@mail.it)
