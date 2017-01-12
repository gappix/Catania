# Lambda Architecture -Overview

---

Con il termine **Lambda Architecture ** \(coniato da Nathan Marz\) si intende una generica architettura di **data processing  **che si prefigge lo scopo di gestire enormi quantità di dati, sfruttando metodi di processing sia **batch**, sia **real-time**. In particolare, scopo ultimo di una Lambda Architecture è ottenere un'infrastruttura con adeguate:

1. **latency: **il tempo necessario per eseguire una query,
2. **thoughput,**
3. **fault-tolerance.**

Un'architettura di questo tipo è solitamente possibile suddividerla nei seguenti tre layer.

![](/assets/la-overview_small.png)

### 1 - Data

Tutti i dati che arrivano al sistema sono inviati contemporaneamente sia al Batch Layer sia allo Speed Layer per il processing

### 2 - Batch Layer

### 3 - Serving Layer

### 4 - Speed Layer

### 5 - Query

Le query sui dati possono essere soddisfatte effettuando un merging di informazioni tra la batch-view e la realtime-view.

![](/assets/Sketch-Data.png)

---

###### REFERENCES

Wikipedia: [https://en.wikipedia.org/wiki/Lambda\_architecture](https://en.wikipedia.org/wiki/Lambda_architecture)  
Blog: [http://lambda-architecture.net/](http://lambda-architecture.net/)

