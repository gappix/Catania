# Missing Values — General Overview

---

I dati presenti nei dataset reali sono spesso affetti dal problema di **dati mancanti \(missing values\).            
**Questi _vuoti di informazione_ possono determinare problemi a diversi algoritmi di machine learning, condizionandone sensibilmente il risultato. Per questo motivo è molto importante trattarli in modo opportuno a seconda dell'esperimento che si vuole compiere.  
Per poter agire efficacemente sul dataset per affrontare problemi di missing values è molto importante **conoscere il significato dei dati **di cui si dispone.

![](/assets/missing_values.jpg)

## La prima domanda...

Quando si rriscontrano dei missing values nel proprio dataset di indagine la prima domanda da porsi è: **la mancanza di queste informazioni può avere un significato?            
**Ovvero: c'è un motivo particolare per cui sono mancanti? Potrebbe darsi che la procedura di raccolta dei dati prevedesse il **non-inserimento **nel caso di valori sopra/sotto una certa soglia, di valori non ritenuti significativi, di condizioni particolari di incertezza.

Qualora la risposta fosse _SI, la mancanza di un valore in un determinato dato è significativa, _ i Missing Values vanno trattati alla stregua di un **nuovo tipo di valore.**

Possono quindi essere sostituiti con una simbologia particolare adeguata al contesto e **devono essere considerati **dagli algoritmi usati nell'esperimento.

Qualora la risposta invece fosse _NO, non vi è un forte motivo che ne giustifichi la mancanza, _ allora si dorvà procedere con ulteriori analisi volta a riconoscere la **tipologia **delle lacune riscontrate.

## Tipologie di Missing Values

Vi possono essere sostanzialmente **3 tipologie **di dati mancanti:

1. Missing Completely At Random — **MCAR**
2. Missing At Random — **MAR**
3. Not Missing At Random — **NMAR**

### 1. MCAR — Missing Completely At Random

La distribuzione della loro occorrenza non dipende dai dati presenti ne dai dati mancanti. I motivi della lorto assenza non dipendono dalle variabiili o dai parametri di interesse.

É la situazione migliore: lla mancanza di informazione è un  problema **accidentale, **probabilemnte dovuto ad imprevisti occorsi durante la raccolta dei dati.

### 2. MAR — Missing At Random

La distribuzione dei valori mancanti dipende dai **dati presenti. **La tendenza di un un  determinato attributo a presentare informazioni lacunose dipende dai valori assunti da qualche altro dato del dataset.

|  |  |
| :--- | :--- |
| EXAMPLE | In un dataset di tipo **medico** la mancanza di informazione dell'esame _T3_ per un certo paziente può essere dovuto al fatto che gli esiti degli esami _T2 e T1_ erano positivi. Non era necessario pertanto che il paziente si sottoponesse all'esame _T3._ |

### 3. NMAR — Not Missing At Random

La distribuzione dei valori mancanti dipende da **dati non presenti nel datset.  **Hanno spesso un preciso significato legato al contesto. Sono anche indice di una necessità di reperire **ulteriori informazioni **per poter procedere efficacemente con l'esperimento.



## Come capire la tipologia di Missing Value?

Non è possibile testare la tiipologia di missing values. É assolutamente prioritario avere una grande conoscenza dell'ambito generale e di **come i dati sono stati raccolti/creati. **L'ideale sarebbe sapere anche il **perchè **vi sono lacune nei dati.

In generale un approccio cauto consiste nell'utilizzare metodi adatti a una situazione MAR ed evitare quei metodi validi soltanto per MCAR.

---

###### REFERENCES

* [https://gallery.cortanaintelligence.com/Experiment/Methods-for-handling-missing-values-1](https://gallery.cortanaintelligence.com/Experiment/Methods-for-handling-missing-values-1)
* [http://diggdata.in/post/90435663721/dealing-with-missing-values-introduction](http://diggdata.in/post/90435663721/dealing-with-missing-values-introduction)
* Appunti corso DataMining — Politecnico di Milano



