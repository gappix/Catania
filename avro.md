# Avro - Overview

---

### Cos'è

Avro è un **sistema di serializzazione dei dati.    
**Permette di trasformare i dati di un certo ambiente in una forma **binaria ** o **testuale **facilamente trasportabile.

Meccanismi di serializzazione simili e alternativi ad Avro sono:

* Thrift
* Protocol Buffers
* Sequence files

### Caratteristiche

Avro è:

* language independent
* schema-based.

Inoltre:

* può essere processato da diversi linguaggi \(C, C++, C\#, Java, Python, Ruby\),
* essendo comprimibile e splittabile può essere utilizzato per fornire gli input ai jobs **map-reduce.**
* la presenza dello schema consente di comprimere dati strutturati perticolarmente ricchi.

Per queste caratteristiche è il sistema preferito per lo scambio di dati all'interno di Hadoop.



### Funzionamento generale

Avro diichiara uno **schema json**, sulla base del quale **serializza i dati.    
**Questa caratteristica dello schema rende la serializzazione più **veloce **e **leggera.**

Passaggi necessari per l'utilizzo di AVRO:

1. Creare uno schhema adatto ai dati che si viogliono trasportare.
2. Leggere glli schemi creati all'interno del programma
   1. generando una classe corrispondente alllo schema \(compilazione delllo schema attraverso AVRO\)
   2. usando parser già presenti.
3. Serializzare i dati usando le API di serializzazione fornite da AVRO \(org.apache.avro.specific\).
4. Deserializzare i dati nel programma di destinazione con le stesse API di cui sopra.



