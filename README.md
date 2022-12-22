# Über das Dokument
In diesem Repository möchte ich dir die Grundlagen der professionellen Softwareentwicklung erläutern. Im Unterschied zu anderen Dokumenten lege ich hierbei nicht den Fokus darauf mit minimalen Anweisungen Code zu erstellen. Es besteht dabei die Gefahr dass mit gefährlichen Halbwissen schlechte, anfällige Software zu erstellen und zu veröffentlichen. Daher sind einige Kapitel länger als in anderen Dokumenten, geben jedoch einen erweiterten Überblick wie Software professionell entwickelt wird.

# Aufbau
* Wie entstehen Software-Anwendungen?
* Was ist beim Erstellen von Software wichtig?
* Welche grundlegenden Konstrukte benötige ich um eine Anwendung zu schreiben?

# Vom Text zur Anwendung. So entstehen Software-Anwendungen
Es gibt verschiedene Möglichkeiten wie eine Software-Anwendung entsteht. Wir möchten uns in diesem Dokument nicht auf der Ebene von Maschinensprachen sondern auf Ebene von Hochsprachen mit diesem Thema befassen. Bei Hochsprachen wird mithilfe einer Programmiersprache Text erstellt der von einem sogenannten Compiler in Maschinencode compiliert wird. Im folgenden Beispiel soll mithilfe einer Zeile Code "Hallo" ausgegeben werden.
```javascript
console.log('Hallo')
```
Dieser Code kann in eine Datei mit der Dateiendung **.js** eingefügt werden. Mithilfe einer Laufzeitumgebung/dem dort vorhandenen Compiler wird aus dieser Codezeile einen Maschinencode (bestehen auf Nullen und Einser) erzeugt der von der Maschine ausgeführt wird. Bei der Ausführung würde der Text "Hallo" angezeigt werden.

Wie/Wo die Ausgabe erfolgt unterscheidet sich je nach Anwendung. Einige Beispiele hierzu wären:
* Konsolen-Anwendung: Ausgabe von "Hallo" in der Konsole
* Browser-Anwendung: Ausgabe von "Hallo" in der Entwicklerkonsole, d.h. es ist nicht direkt für den Benutzer sichtbar
* Server-Anwendung: Ausgabe von "Hallo" in der Konsole des Servers.

Ich werde in weiteren Kapiteln näher aus der Thema Ausgabe und Logging eingehen.

## Laufzeitumgebung und Entwicklungsumgebung

Sofern der Code in Textform existiert benötigt ihr eine Laufzeitumgebung damit euer Code ausgeführt wird, er sozusagen "läuft".
Im Vergleich dazu kann eine Entwicklungsumgebung verwendet werden um bei der Arbeit mit dem Code zu unterstützen. Zwar reicht teils auch ein einfacher Texteditor aus, ist jedoch nicht immer so komfortabel wie eine Entwicklungsumgebung. In einer Entwicklungsumgebung können beispielsweise folgende Funktionen  bereitstehen.
* Code-Editor mit Hervorhebung des Codes, Auto-Vervollständigung, Ein-Klick-Ausführung
* Debugger: Schrittweises Ausführen des Codes mit der Möglichkeit an definierten Stellen anzuhalten oder jene zu überspringen.
* Unterstützung bei der Verwaltung mehrerer Versionen

**Tipp:**

Beim Bereitstellen/Ausliefern einer Software solltet ihr dafür sorgen dass klar ist was benötigt wird damit die Software **läuft**. Es ist für den Endnutzer meist nicht notwendig eine Entwicklungsumgebung zu benutzen, die Laufzeitumgebung sollte ausreichen.

**Beispiel:**

Ihr bestellt bei einer Pizzeria eine Pizza. Anhand einer Zubereitungsanweisung (ähnlich wie "Code") wird wird die Pizza in der Küche mit Küchenutensilien zubereitet, jene wären mit einer Entwicklungsumgebung gleichzusetzen. Den Ofen könnte man als Compiler in der Entwicklungsumgebung sehen. Als Ergebnis würde eine Pizza ("Anwendung") herauskommen die übergeben/ausgeliefert wird. Für das Essen der Pizza (gleich zur Nutzung der Anwendung) benötigt ihr ggf. einen Teller/Karton, ggf. noch Besteck was der Laufzeitumgebung entsprechen würde. Ich würdet sicherlich nicht erwarten dass bei Lieferung einer Pizza der gesamte Pizza-Ofen mitgeliefert wird.
