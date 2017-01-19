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



### 2. MAR — Missing At Random



### 3. NMAR — Not Missing At Random



---

###### REFERENCES

* [https://gallery.cortanaintelligence.com/Experiment/Methods-for-handling-missing-values-1](https://gallery.cortanaintelligence.com/Experiment/Methods-for-handling-missing-values-1)
* [http://diggdata.in/post/90435663721/dealing-with-missing-values-introduction](http://diggdata.in/post/90435663721/dealing-with-missing-values-introduction)
* Appunti corso DataMining — Politecnico di Milano



