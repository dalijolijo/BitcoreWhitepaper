# Kapitel 3

## Lösung und technische Spezifikation

Bitcore zeichnet sich durch wichtige Innovationen aus, die es als alltägliches Zahlungsmittel sowohl im privaten als auch im geschäftlichen Kontext besonders gut einsetzbar machen. Jede dieser Innovationen, sowie ihre Rolle bei der Steigerung der Effizienz und Benutzerfreundlichkeit von Bitcore, wird in diesem Abschnitt erläutert.

Für einen schnellen Überblick sind die wichtigsten technischen Spezifikationen von Bitcore im Folgenden zusammengefasst:

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

> "[Bitcore] ist innovativ, indem es mit Dingen aufräumt" -- Jimmy Song (vii), Bitcoin Hauptentwickler

![Abbildung 1: Bitcoin, Bitcoin Cash, Bitcoin Gold und Bitcore - Vergleichstabelle.](images/BitcoreWhitepaperImg03.png)

## 3.1 Coin Verteilung
Die maximale Anzahl der Coins, die auf der Bitcore-Plattform erzeugt werden, ist auf 21 Millionen begrenzt. Diese Zahl wurde bewusst gewählt, um die gleiche Gesamtmenge an Coins wie Bitcoin (BTC)  zu entsprechen.

TODO:
Dieser begrenzte Münzvorrat ist das Ergebnis des Halbierungsalgorithmus von Bitcoin, der die Münzgeld-Belohnung für Bergleute alle 210.000 Blöcke um 50% reduziert und die Anzahl der neu abgebauten Münzen etwa alle vier Jahre verringert, bis sie im Jahr 2140 ungefähr null ist.

Die Blockbelohnung von Bitcore war identisch mit der Bitcoin-Blockbelohnung für die ersten 10.000 Blöcke: 12,5 BTX pro Block bei einer Blockzeit von 10 Minuten. Anschließend wurde die Belohnung durch ein Update auf 3,125 BTX bei einer durchschnittlichen Blockzeit von 2,5 Minuten reduziert.

Bitcore wendet den gleichen Halbierungsalgorithmus auf seine Coinbase-Belohnungen an, jedoch in Intervallen von 840.000 Blöcken. Daher ist das Bitcore-Angebot genauso begrenzt wie das Bitcoin-Angebot.

Die folgende Tabelle zeigt die Halbierung der Blockbelohnungen von Bitcore:

![Abbildung 2: Die Block Mining Belohnungsentwicklung von Bitcore](images/BitcoreWhitepaperImg04.png)

Diese Halbierung der Belohnung in festen Intervallen von Blöcken führt zu einer vorbestimmten Endanzahl von Münzen, einem Konzept, das als kontrolliertes Angebot bezeichnet wird.

## 3.2 Blockchain und Algorithmen
Bitcore verwendet einen Proof-of-Work-Algorithmus wie die von Bitcoin. Die Einstellung der Schwierigkeit wird jedoch auf innovative Weise gelöst, indem der Schwierigkeits-Retargeting-Algorithmus des Core Shield 64_15 wie nachstehend beschrieben verwendet wird.

Ein weiterer entscheidender Unterschied zu Bitcoin sind die reduzierten Blockzeiten von Bitcoin, ein Viertel der Blockzeiten von Bitcoin, die Bitcore sowohl nutzbarer als auch sicherer machen, wie weiter unten in diesem Abschnitt beschrieben. Gleichzeitig ist die Blockgröße deutlich größer, was wiederum zu einer höheren Transaktionsgeschwindigkeit und besseren Benutzerfreundlichkeit beiträgt.

Die Aktivierung von SegWit - 4,5 Monate früher als bei der Bitcoin-Blockchain - und die Lightning-Netzwerkkompatibilität machen Bitcore schließlich zu einem Zahlungsmittel, das ideal auf die Bedürfnisse von Einzelpersonen und Unternehmen von morgen abgestimmt ist.

### 3.2.1 Reibungslosen Schwierigkeitsanpassung durch diff64_15 Algorithmus
In Kryptowährungen, die auf Proof-of-Work basieren, dienen Schwierigkeiten beim Retargeting, dh das Anpassen der Schwierigkeit, mit denen Minenarbeiter den nächsten Block finden können, dazu, konsistente Blockzeiten zu gewährleisten. Ohne Schwierigkeiten beim Retargeting würden sich die Blockzeiten mit zunehmender Anzahl der auf der Blockchain aktiven Miner zu einem bestimmten Zeitpunkt verringern, da dies die Wahrscheinlichkeit erhöhen würde, dass der richtige Hashwert von einem dieser vielen Miner entdeckt wird.

Daher wird beim Schwierigkeits-Retargeting der Schwierigkeitsgrad beim Erkennen des nächsten Blocks erhöht, wenn viele Miner auf dem Protokoll aktiv sind, und nimmt ab, wenn weniger Miner aktiv sind.

In Bitcoin wird der Schwierigkeitsgrad alle 2016-Blöcke angepasst. Bei einer Blockzeit von etwa 10 Minuten entspricht dies einer Anpassung etwa alle zwei Wochen - eine eher langsame Rate, die nicht auf kurzfristige Erhöhungen oder Abnahmen der Bergbautätigkeit anspricht. Solche kurzfristigen Schwankungen der Bergbauaktivität werden jedoch häufig beobachtet, wenn die Bergleute zwischen Bitcoin und seinen Gabeln hin und her wechseln, um nach dem besten Verhältnis zwischen Bergbaubemühung (bestimmt durch den Schwierigkeitsgrad) und Belohnung zu suchen.

Um diese Herausforderung zu lösen, hat Bitcore die schwierige Retargeting-Methode von Bitcoin durch einen neuartigen Algorithmus namens Core Shield 64_15 ersetzt.

In Core Shield 64_15 wird die Blockschwierigkeit alle 64 Blöcke neu eingestellt. Bei einer Bitcore-Blockierzeit von nur 2,5 Minuten wird die Schwierigkeitsanpassung alle 2 Stunden und 40 Minuten durchgeführt. Dies macht Bitcores Blockschwierigkeiten schneller als die von Bitcoin, aber gleichzeitig werden zu turbulente kurzfristige Anpassungen vermieden: Die Schwierigkeit wird bei jeder Neueinstellung nicht um mehr als 15% geändert, was zu allmählichen statt dramatischen Änderungen führt.

Der schwierige Retargeting-Algorithmus von Bitcore ist daher nicht nur effizienter, sondern führt zu besser vorhersagbaren Blockierungszeiten und sichert das Netzwerk zusätzlich gegen Angriffe mit doppeltem Aufwand, die in Zeiten mit unverhältnismäßig geringen Hash-Problemen wahrscheinlich erfolgreich sind.

![Abbildung 3: Die Mining Schwierigkeitsanpassung bei Bitcore (Beispieldaten vom Mai 2018).](images/BitcoreWhitepaperImg05.png)

### 3.2.2 Kürzere Blockzeiten
Das Bitcore-Protokoll ist auf eine Blockzeit von 2,5 Minuten ausgelegt - ein Viertel der 10-Minuten-Blockzeiten von Bitcoin.

Kürzere Blockzeiten sind aus verschiedenen Gründen vorteilhaft.

Der erste ist, dass sie schnellere Bestätigungen ermöglichen. Jede Transaktion in der Blockchain beginnt ihre Existenz als unbestätigte Transaktion, die schließlich von Bergleuten aufgegriffen wird, die um den nächsten Block konkurrieren. Jedes Mal, wenn ein gültiger Block in der Blockchain erstellt wird, gelten die darin enthaltenen Transaktionen als bestätigt.

Da mehrere derzeit gültige Blöcke mit unterschiedlichen bestätigten Transaktionen in der Blockkette parallel vorhanden sein können, beweist nur das Anlegen weiterer Blöcke nach dem aktuellen Block, dass eine Transaktion tatsächlich Teil der aktiven Kette geworden ist, d. H. Der längsten derzeit vorhandenen Kette. Diese Richtlinie ist Teil des Proof-of-Work-Konsensmechanismus, um Angriffe mit doppeltem Aufwand durch böswillige Knoten zu verhindern: Der Arbeitsaufwand (und damit die Energie) für die Erstellung eines einzelnen Blocks mit einer betrügerischen Transaktion ist für einen Angreifer möglicherweise noch überschaubar. Diese betrügerische Transaktion wird jedoch auf lange Sicht nicht Teil der aktiven Blockchain sein, es sei denn, der Angreifer kann sogar erheblich mehr Arbeit aufwenden, um danach eine ausreichende Anzahl von Blöcken zu erstellen, damit diese Kette die längste Kette wird.

Aus diesem Grund warten viele Händler und andere Entitäten, die Krypto-Zahlungen akzeptieren, auf mehr als einen gültigen Block, bis sie eine bestimmte Transaktion als bestätigt akzeptieren. Generell besteht bei Zahlungen größerer Beträge ein höheres Fälschungsrisiko, so dass längere Bestätigungszeiten erforderlich sind, damit der Händler sicher ist.

Satoshi Nakamoto hatte ursprünglich Blockzeiten von 10 Minuten gewählt, um das Bitcoin-Netzwerk in seiner Größe vor fast 10 Jahren zu sichern. Seitdem ist das Netzwerk erheblich gewachsen, was es für böswillige Akteure schwieriger macht, betrügerische Transaktionen in das Netzwerk einzuführen.

Vitalik Buterin, Gründer von Ethereum, argumentiert, dass kürzere Blockzeiten gegenüber längeren vorzuziehen sind (viii), da sie eine höhere Granularität der Informationen bieten: Korrekte aktive Ketten werden schneller erkannt und falschen Ketten vorgezogen und ein akzeptables Sicherheitsniveau für Kleine bis mittlere Transaktionen werden früher erreicht. Die Verkürzung der Blockzeiten erhöht jedoch das Zentralisierungsrisiko von arbeitsnachweisbasierten Blockketten, wodurch größere Spieler erheblich mehr Macht erhalten, um möglicherweise das Netzwerk zu betrügen. Blockzeiten können daher nicht beliebig reduziert werden, sondern müssen unter Berücksichtigung dieser gegensätzlichen Tendenzen sorgfältig gestaltet werden.

Angesichts all dieser Überlegungen hat sich Bitcore entschieden, die Privilegien und Vorteile, die mit einer geringfügigen Reduzierung der Gesamtblockzeit auf 2,5 Minuten einhergehen, voll zu nutzen.

### 3.2.3 Größere Blockgröße
Die Blöcke von Bitcore haben derzeit eine Größe von 10 MB, ohne auf den zusätzlichen Raum einzukalkulieren, der durch das „Wiegen“ der Daten aufgrund von SegWit entsteht, wodurch die Größe auf 20 MB erhöht wird. Daher kann Bitcore 80 MB in Blöcken (davon 40 MB aufgrund von SegWit) in demselben Intervall erzeugen, in dem Bitcoin 2 MB (1 MB ohne SegWit) erzeugt.

Größere Blöcke können mehr Transaktionen enthalten, was zu einer konstanten Blockzeit einem schnelleren Transaktionsdurchsatz entspricht. Der Transaktionsdurchsatz war schon immer ein kritischer Punkt im Hinblick auf die Konkurrenzfähigkeit von Cryptowährung mit Fiat-Zahlungslösungen: Die etablierte VISA kann 1.700 Transaktionen pro Sekunde (TPS) und mindestens 115 TPS pro PayPal abwickeln.

Mit aktiviertem SegWit kann Bitcoin etwa 11 TPS verarbeiten, obwohl es in sehr kurzen Zeitabständen Spitzen von bis zu 20 TX / Sekunde gab.

Um eine breite Akzeptanz von Krypto-Zahlungsmethoden zu ermöglichen, muss die Skalierbarkeit von Blockchain-Netzwerken offensichtlich verbessert und der Durchsatz erhöht werden. Häufig werden zwei Lösungen für diese Herausforderung diskutiert: Erhöhen der Blockgröße oder Einführung einer Off-Chain-Skalierungslösung wie Lightning Network.

Die Bitcore-Community hat sich dafür entschieden, die Blockgröße auf 10 MB zu erhöhen. Bei einem Durchschnitt von 224 Bytes / TX kann die BTX-Kette ungefähr 310 TX / Sekunde verarbeiten. Mit SegWit wird die potenzielle maximale Blockgröße sogar auf 20 MB erhöht. Die BTX-Kette kann unter optimalen Bedingungen 550 TX / Sekunde verarbeiten, auch wenn dabei nicht berücksichtigt wird, dass einige Transaktionen außerhalb des Netzwerks geroutet werden können Blitz-Netzwerk.

Bitcore hat seine Fähigkeit unter Beweis gestellt, eine große Anzahl von Transaktionen in kurzer Zeit abzuwickeln, als am 2. November 2017 nach Aktivierung der Hybridgabel innerhalb von wenigen Tagen etwa 5 Millionen Transaktionen verarbeitet wurden (siehe Abschnitt 2.2 der vorliegenden Veröffentlichung).

### 3.2.4 Aktivierung von Segregated Witness (SegWit)
Segregated Witness (SegWit) wurde im April 2017 auf der Bitcore Blockchain mit Block #3, 000 – ein halbes Jahr früher als in Bitcoin aktiviert. Vor der Aktivierung begannen bitcore Timetravel10 Miners erfolgreich mit der Erstellung von segwit-konformen Blöcken.

SegWit bietet mehrere unmittelbare Vorteile:

* Eliminierung unerwünschter Transaktionsveränderungen
* Kapazitätssteigerung
* Gewichtung der Daten in Abhängigkeit der Bitcore-Node Performance
* Signature Wertabdeckung
* Lineare Skalierung von sighash Operationen
* Erhöhte Sicherheit für Multisig
* Effizientere Bitcore-Node Sicherheit
* Skript Versionierung


### 3.2.5 Lightning Network Kompatibilität
Das Lightning-Netzwerk (ix) ist ein Übertragungsnetzwerk, das auf einer Ebene oberhalb der Bitcore-Blockchain arbeitet. Durch die Verwendung intelligenter Vertragsfunktionalität werden sofortige Zahlungen über ein Teilnehmernetzwerk ermöglicht, sodass keine Wartezeiten auf die Bestätigung erforderlich sind, wie in den vorangegangenen Abschnitten dieses Whitepapers beschrieben.

Neben den Sofortzahlungen bietet das Blitznetzwerk weitere Vorteile:

Erhöhte Skalierbarkeit als Nebeneffekt von Sofortzahlungen
Niedrigere Kosten, so dass diese Lösung auch für Mikrozahlungen interessant ist
Cross-Chain-Atom-Swaps mit heterogenen Block-Konsensus-Regeln ermöglichen
Bitcore ist vollständig mit dem Lightning-Netzwerk kompatibel und kann daher sofortige Zahlungen sowie Mikropayments unterstützen.

### 3.2.6 Geringe Gebühren
Mit einer durchschnittlichen Gebühr von 0,0003 USD pro Kilobyte und einer durchschnittlichen Gebühr von 0,0002 USD pro Kilobyte sind die Gebühren von Bitcore deutlich niedriger als die Gebühren anderer wichtiger Kryptowährungen (siehe auch Abbildung 4). Da 1 Kilobyte ungefähr 3 Transaktionen entspricht, entspricht dies einer Gebühr von etwa 0,0001 USD oder 0,01 US-Cent pro Transaktion.

Diese günstige Gebührenstruktur trägt weiter zur Eignung von Bitcore für alltägliche Transaktionen und sogar für Mikrozahlungen bei.

![Abbildung 4: Vergleichsdiagramm, Bitcore im Vergleich zu anderen Kryptowährungen.](images/BitcoreWhitepaperImg04.png)

Für Bitcore ist eine Mindestgebühr von 0,0001 BTX pro Kilobyte erforderlich. Die empfohlene Gebühr zur Unterstützung von Denkern beträgt derzeit (Juli 2018) etwa 0,001 BTX pro Kilobyte. Da Bitcore-Blöcke derzeit nicht voll sind, bietet die Transaktionsgeschwindigkeit keinen Vorteil, wenn eine höhere Gebühr bezahlt wird. Dies kann jedoch in Zukunft der Fall sein, da die Belastung des Bitcore-Netzwerks zunimmt.

---

**Quellen**

*(v) https://opensource.org/osd*

*(vi) Siehe https://www.reddit.com/r/Bitcoin/comments/18qy88/bitcoin_message_signing_and_verification/ für weitere Details bezüglich Nachrichten Signierung bei Bitcoin.*

*(vii) https://medium.com/@jimmysong/bitcoin-diamond-super-bitcoin-bitcore-what-you-need-to-know-f49c35688a39*

*(viii) https://blog.ethereum.org/2015/09/14/on-slow-and-fast-block-times/*

*(ix) https://lightning.network/*
