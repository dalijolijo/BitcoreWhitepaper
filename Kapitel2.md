# Kapitel 2
## Von Bitcoin zu Bitcore

> "Eine reine Peer-to-Peer Version von elektronischem Bargeld würde es ermöglichen, Online-Zahlungen direkt von einer Partei zur anderen zu schicken, ohne dass ein Finanzinstitut involviert sein muss. Digitale Signaturen sind ein Teil der Lösung, aber die Hauptvorteile gehen verloren, wenn ein vertrauenswürdiger Dritter weiterhin benötigt wird, um Doppelausgaben zu vermeiden. Wir schlagen eine Lösung für das Problem der doppelten Ausgaben vor, indem wir ein Peer-to-Peer-Netzwerk verwenden."
*-- Satoshi Nakamoto, 2008*


Es war diese Aussage, die das moderne Konzept der Kryptowährung und der dezentralen Finanzen hervorbrachte. Bis Satoshi Nakamoto das ursprüngliche Bitcoin-Konzept entwarf, verließ sich praktisch die ganze Finanzwelt auf die Zentralbehörden, genauer gesagt: Zentrale Schwachstellen. Die Sicherheit des Geldes aller war abhängig von der Sicherheit und der wirtschaftlichen Gesundheit der Bank oder des Finanzinstituts, die im Besitz der Mittel war.

Jeder Fall von Sicherheitsverletzungen, Fehlverhalten oder Konkurs in der Finanzwelt bedeutete, dass diejenigen, die sich auf diese Institute verlassen haben, um ihre Ersparnisse zu schützen, möglicherweise ohne die Ersparnisse zurückbleiben würden.

Ohne irgendeine Art von bisher nicht existierender Technologie erfinden zu müssen, kombinierte Satoshi Nakamoto bestehende Paradigmen auf neuartige Weise, um dieses Problem zu lösen: Ein durch Arbeitsnachweis gesichertes verteiltes Hauptbuch würde fortan einen Rahmen bieten, in dem die Teilnehmer gezwungen wären, ehrlich zu bleiben, ohne Eingriffe - und das Potenzial der Manipulation - durch irgendeine Art von zentraler Autorität.

Der Anreizprozess "Mining" war und ist für das Funktionieren dieses Systems von zentraler Bedeutung. Ein Regelwerk stellte sicher, dass das System im Wesentlichen autonom und nachhaltig ohne Anweisung von "Führungskräften" oder irgendeiner Art von Einzelpersonen oder Einzelunternehmen funktionieren konnte. Dies wurde mit der Absicht getan, das Prinzip der Dezentralisierung beizubehalten: Wenn ein einzelnes Unternehmen für den reibungslosen Betrieb des Systems verantwortlich wäre, dann würde diese Einheit einen potenziellen Single Point of Failure darstellen - was den Zweck des Protokolls zunichte machen würde.

In diesem Whitepaper werden wir uns die Funktionsweise des ursprünglichen Bitcoin-Protokolls genauer ansehen - und die Art und Weise, wie Bitcore das ursprünglichen Bitcoin-Protokoll weiterentwickelt und verbessert hat.

Dies wird zeigen, warum und wie das Bitcore-Protokoll eine leistungsfähige alternative Kryptowährung ist, um einige der Anwendungsfälle für Kryptowährungen zu erleichtern, die mit der derzeit verfügbaren Kryptotechnologie noch nicht erreichbar waren.


## 2.1 Bitcore als Open Source
Sowohl Bitcoin als auch Bitcore sind echte Open-Source Projekte. Die Bitcore-Community ist der Überzeugung, dass dies im Einklang mit dem dezentralen, partizipativen und gemeinschaftsorientierten Geist von Bitcore steht.

Insbesondere war die Entwicklung von Bitcore nur möglich, weil Bitcoin die folgenden Merkmale von Open Source, wie von der Open Source Initiative gefordert, erfüllt hat - und die Bitcore Codebasis wiederum unterliegt den gleichen Bedingungen und Freiheitsgraden:

1. Kostenlose Weiterverteilung
2. Einbinden von Quellcode
3. Berechtigung den Code zu kopieren, zu modifizieren und zu veröffentlichen.
4. Integrität des Quellcodes des Autors
5. Keine Diskriminierung von Personen oder Gruppen
6. Keine Diskriminierung von Arbeitsbereichen
7. Anwendbarkeit der Lizenz ohne Notwendigkeit der Ausführung einer anderen Lizenz
8. Lizenz nicht produktspezifisch
9. Keine Einschränkungen anderer Software durch die Lizenz
10. Technologie-Neutralität der Lizenz 

Durch die Einhaltung dieser Standards der Open-Source-Software ermöglicht Bitcore der Open-Source-Community den Zugriff, die Änderung und die Weiterentwicklung Ihres Codes, ohne jegliche Diskriminierung in Bezug auf Identität, Hintergrund, Absicht oder Branche.


## 2.2 Verteilung: Eins-zu-Eins Claiming, Hybrid Fork und Airdrop
Klassische Bitcoin-Forks kopieren die Bitcoin-Blockkette zu einem bestimmten Block und Zeitpunkt. Bitcore hat jedoch einen neuen Coin mit einer leeren Blockchain geschaffen, mit dem ausdrücklichen Ziel, Bitcore von Bitcoin zu trennen und als eigenständige Einheit zu etablieren.

16,2 Millionen Bitcore Coins (BTX) wurden vorab abgebaut (entspricht der Anzahl der vorhandenen Bitcoin zum Zeitpunkt der Erstellung der Bitcore-Blockkette) und waren somit bereit für die Verteilung an die Community.

Die Verteilung von BTX an seine potenzielle Nutzer-Community erfolgte in drei Phasen:
* Eins-zu-Eins Inanspruchnahme (Claiming)
* Hybrid Fork
* Airdrop


### 2.2.1 Eins-zu-Eins Inanspruchnahme (Claiming)
In den ersten sechs Monaten des Bestehens von Bitcore, von April 2017 bis November 2017, konnten Bitcoin (BTC) Besitzer genau so viele Bitcore (BTX) auf der Bitcore-Blockchain in Anspruch nehmen.

Dieses Claiming wurde mit Hilfe einer Datenbank und der Sign-Message-Funktion(vi) von Bitcoin realisiert.

Von 16,2 Millionen vorab geminten BTX wurden in diesem ersten Verteilungsschritt 590.000 BTX abgerufen. Die Möglichkeit zur 1:1 Inanspruchnahme (Claiming) von Bitcore endete am 2. November 2017.


### 2.2.2 Hybrid Fork
Am 2. November 2017 wurde in Blockhöhe #492.820 des Bitcoin-Protokolls eine Momentaufnahme (Snapshot) der Bitcoin-Blockkette erstellt. Die Verteilung der restlichen 15,8 Millionen vorab geminten BTX wurde in einer Weise fortgesetzt, die sich von der 1:1-Inanspruchnahme in der ersten Phase unterschied.

Alle Adressen auf der Bitcore-Blockkette, deren entsprechende Adressen auf der Bitcoin-Blockchain einen Wert von mindestens 0,01 BTC aufwiesen, wurden mit 50% des Wertes an BTX gefüllt - bezogen auf den Wert der BTC in der jeweiligen Adresse. Die Funding-Ratio betrug also 0,5 BTX bis 1,0 BTC.

In den folgenden Tagen wurden rund 5 Millionen Transaktionen abgewickelt und rund 8 Millionen BTX auf alle berechtigten Adressen verteilt. Dies war nicht nur eine praktische Möglichkeit, BTX zu verteilen, sondern hat auch gezeigt, dass die BTX-Blockchain in der Lage ist, eine große Anzahl von Transaktionen in relativ kurzer Zeit zu verarbeiten.

So wurden etwa 8 Millionen der anfänglich 16 Millionen vorab geminten BTX an die Community verteilt. Von den restlichen 8 Millionen wurden 10% vom Bitcore-Team für die zukünftige technische Entwicklung zurück gehalten.


### 2.2.3 Airdrop
90% der restlichen 8 Millionen BTX wurden schließlich nach einem differenzierten Zeitplan in einer Reihe von wöchentlichen Airdrops verteilt.

Beim ersten Airdrop wurde ein 25%iger Bonus auf das BTX Wallet Guthaben des Benutzers verteilt. Infolgedessen wurden weitere Airdrops nach folgendem Zeitplan durchgeführt (mit Prozentsatz der Wallet Balance des Benutzers):

* + 5% jeden Montag im Januar 2018
* + 6% jeden Montag im Februar 2018
* + 7% jeden Montag im März 2018
* + 8% jeden Montag im April 2018
* + 9% jeden Montag im Mai 2018

Mit dieser letzten Phase wurde die Verteilung von vorab geminten BTX abgeschlossen.


### 2.2.4 Ein Airdrop Beispiel
Ein Beispiel soll den Prozess weiter veranschaulichen:

Alice hält 20 Bitcore (BTX) in ihrer Wallet. Sie hat ihre Wallet für einen Airdrop im Januar registriert, als der Bonusprozentsatz 5% betrug. Sie ist daher berechtigt, 5% ihres gesamten BTX-Guthabens im Januar als Airdrop zu erhalten:

```
20 BTX * 5% = 1 BTX
```
So erhält Alice einen zusätzlichen BTX-Coin und besitzt nach dem Airdrop im Januar insgesamt 21 BTX in ihrer Wallet.


### 2.2.5 Warum ein Hybrid Fork und der Airdrop?
Der entscheidende Unterschied zwischen diesem Modell und dem typischen Hard-Fork Modell ist der folgende: Anstatt eine identische Anzahl aller ausstehenden Coins zu verteilen, die zum Zeitpunkt des Snapshots auf der Blockchain ausgegeben wurden, wurden nur 50% der BTX Coins auf diese Weise verteilt. Die daraus resultierenden 50% wurden nur an aktive BTX-Benutzer verteilt. Auf diese Weise stellte das Bitcore-Team sicher, dass passive Besitzer massiver Bitcoin-Mengen, so genannte "Bitcoin-Wale", nicht automatisch auch zu "Bitcore-Walen" werden und damit das Machtgleichgewicht innerhalb der Bitcore-Community verzerren und das zirkulierende Angebot an Bitcore so begrenzen, dass zukünftige Aktivitäten des Ökosystems beeinträchtigt würden. Stattdessen gelang es dem Bitcore-Team, eine gleichmäßigere Verteilung der Coins zu erreichen als bei früheren Bitcoin-Forks - im Einklang mit den dezentralen und partizipativen Idealen der Bitcore-Community.


## Kein ICO
Als Hybrid-Fork war die Markteinführung von Bitcore nicht durch ein Initial Coin Offering (ICO) realisiert oder finanziert.

Dies war eine bewusste Entscheidung der Bitcore-Community, die darauf abzielte, die Chancengleichheit und Beteiligung potenzieller BTX-Nutzer auf der ganzen Welt zu fördern. Wie Trends und Entwicklungen im Kryptobereich in den letzten Jahren gezeigt haben, ziehen ICOs Spekulanten an, was die Volatilität der zugrunde liegenden Kryptowährung erhöht und deren Alltagstauglichkeit verringert. Darüber hinaus führen ICOs zu einem Zustrom von wohlhabenden Privatinvestoren, die sich den Weg in eine überproportionale Macht und einen Einfluss auf Kryptocommunities "kaufen". Nicht zuletzt gelten für ICOs, deren Teams in verschiedenen Ländern angesiedelt sind, unterschiedliche Rechtsrahmen, und viele von ihnen schließen ausdrücklich die Teilnahme von Bürgern bestimmter Länder an ICOs aus.

Diese willkürlichen Einschränkungen sind für die Bitcore-Community nicht akzeptabel. Wir streben danach, ein nützliches Krypto-Ökosystem zu schaffen, das für alle Interessierten gleichermaßen zugänglich ist, und dies ungeachtet von Standort und Nationalität.

Um so unabhängig wie möglich von lokalen Vorschriften zu sein, haben wir uns für eine gemeinnützige Interessengemeinschaft entschieden. Die Mitgliedschaft im Gründungsteam und die Teilnahme an der Bitcore-Community hängen ausschließlich von den individuellen Fähigkeiten, Interessen und dem Engagement ab, nicht von willkürlichen geografischen Grenzen.
