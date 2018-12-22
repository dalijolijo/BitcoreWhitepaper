# Kapitel 3

## Lösung und technische Spezifikation

Da Bitcore wichtige Innovationen implementiert hat, ist Bitcore sowohl im persönlichen als auch im geschäftlichen Kontext besonders gut als täglichen Zahlungsmittel geeignetet. 
Jede dieser Innovationen und ihre jeweilige Rolle in der gesteigerten Effizienz und Benutzbarkeit von Bitcore, werden in diesem Abschnitt detailliert beschrieben.

Für einen schnellen Überblick sind die wichtigsten technischen Spezifikationen von Bitcore hier zusammengefasst:

**Name Bitcore**

**Ticker BTX**

* Gestartet am 24. April 2017
* Maximale Coinanzahl von 21 Millionen
* Blockgröße 10MB (20MB SegWit)
* Durchschnittliche Blockzeit von 2,5 Minuten
* Aktuelle Blockchaingröße ca. 950 MB
* Timetravel10 (GPU) Mining Algorithmus
* SegWit und Bloom aktiviert
* Reibungslosen Schwierigkeitsanpassung durch diff64_15 Algorithmus
* Faire Verteilung durch BTC Claiming und Airdrops

> "[Bitcore] ist innovativ, indem es die Dinge reinigt" -- Jimmy Song (vii), Bitcoin Hauptentwickler

![Figure 1: Bitcoin, Bitcoin Cash, Bitcoin Gold and Bitcore - comparison chart.](images/BitcoreWhitepaperImg03.png)

## 3.1 Coin Verteilung

![Figure 2: Block reward halving over time for Bitcore](images/BitcoreWhitepaperImg04.png)

## 3.2 Blockchain und Algorithmen


### 3.2.1 Reibungslosen Schwierigkeitsanpassung durch diff64_15 Algorithmus


![Figure 3: Difficulty retargeting in Bitcore (sample data from May 2018).](images/BitcoreWhitepaperImg05.png)

### 3.2.2 Kürzere Blockzeiten


### 3.2.3 Größere Blockgröße


### 3.2.4 Aktivierung von Segregated Witness (SegWit)
Der abgetrennte Zeuge (SegWit) wurde im April 2017 auf der Bitcore Blockchain mit Block #3, 000 – ein halbes Jahr früher als in Bitcoin aktiviert. Vor der Aktivierung begannen bitcore Timetravel10 Miners erfolgreich mit der Erstellung von segwit-konformen Blöcken.

SegWit bietet mehrere unmittelbare Vorteile:

* Eliminierung unerwünschter Transaktionsveränderungen
* Kapazitätssteigerung
* Gewichtung der Daten in Abhängigkeit der Bitcore-Node Performance
* Signature Wertabdeckung
* Lineare Skalierung von sighash Operationen
* Erhöhte Sicherheit für Multisig
* Effizientere Bitcore-Node Sicherheit
* Script Versionierung


### 3.2.5 Lightning Network Kompatibilität


### 3.2.6 Geringe Gebühren

![Figure 4: Comparison chart, Bitcore against other cryptocurrencies.](images/BitcoreWhitepaperImg04.png)

---

**Quellen**

*(v) https://opensource.org/osd*

*(vi) Siehe https://www.reddit.com/r/Bitcoin/comments/18qy88/bitcoin_message_signing_and_verification/ für weitere Details bezüglich Nachrichten Signierung bei Bitcoin.*

*(vii) https://medium.com/@jimmysong/bitcoin-diamond-super-bitcoin-bitcore-what-you-need-to-know-f49c35688a39*

*(viii) https://blog.ethereum.org/2015/09/14/on-slow-and-fast-block-times/*

*(ix) https://lightning.network/*
