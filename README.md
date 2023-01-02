# Über das Dokument
In diesem Repository möchte ich dir die Grundlagen der professionellen Softwareentwicklung erläutern. Im Unterschied zu anderen Dokumenten lege ich hierbei nicht den Fokus darauf mit minimalen Anweisungen Code zu erstellen. Es besteht dabei die Gefahr dass mit gefährlichen Halbwissen schlechte, anfällige Software zu erstellen und zu veröffentlichen. Daher sind einige Kapitel länger als in anderen Dokumenten, geben jedoch einen erweiterten Überblick wie Software professionell entwickelt wird.

**Noch im Aufbau:**

Das Dokument befindet sich noch im Aufbau, ich empfehle daher es noch nicht zu verwenden!

# Aufbau
* Wie entstehen Software-Anwendungen?
* Welche Fähigkeiten und Fertigkeiten benötige ich?
* Welche grundlegenden Konstrukte benötige ich um eine Anwendung zu schreiben?

# Vom Text zur Anwendung. So entstehen Software-Anwendungen
Es gibt verschiedene Möglichkeiten wie eine Software-Anwendung entsteht. Wir möchten uns in diesem Dokument nicht auf der Ebene von Maschinensprachen sondern auf Ebene von Hochsprachen mit diesem Thema befassen. Bei Hochsprachen wird mithilfe einer Programmiersprache Text erstellt der von einem sogenannten Compiler in Maschinencode compiliert wird. Im folgenden Beispiel soll mithilfe einer Zeile Code "Hallo" ausgegeben werden.
```javascript
console.log('Hallo')
```
Dieser Code kann in eine Datei mit der Dateiendung **.js** eingefügt werden. Mithilfe einer Laufzeitumgebung/dem dort vorhandenen Compiler wird aus dieser Codezeile einen Maschinencode (bestehend auf Nullen und Einsen) erzeugt der von der Maschine ausgeführt wird. Bei der Ausführung würde der Text "Hallo" angezeigt werden.

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

Ihr bestellt bei einer Pizzeria eine Pizza. Anhand einer Zubereitungsanweisung (ähnlich wie "Code") wird wird die Pizza in der Küche mit Küchenutensilien zubereitet, jene wären mit einer Entwicklungsumgebung gleichzusetzen. Den Ofen könnte man als Compiler in der Entwicklungsumgebung sehen. Als Ergebnis würde eine Pizza ("Anwendung") herauskommen die übergeben/ausgeliefert wird. Für das Essen der Pizza (gleich zur Nutzung der Anwendung) benötigt ihr ggf. einen Teller/Karton, ggf. noch Besteck was der Laufzeitumgebung entsprechen würde. Ihr würdet sicherlich nicht erwarten dass bei Lieferung einer Pizza der gesamte Pizza-Ofen mitgeliefert wird.

#  Welche Fähigkeiten und Fertigkeiten benötige ich?

Das Erstellen einer Anwendung ist keine Raketenwissenschaft. Die folgenden Fähigkeiten und Fertigkeiten können euch bei der Softwareentwicklung helfen.

## Sprachkenntnisse
Zwar gibt es Anwendungen zu denen ihr Informationen auf Deutsch findet, häufig sind Informationen jedoch auf **englisch** sodass es hilft wenn ihr grundlegende Englisch-Kenntnisse habt.

## Recherche
Ihr müsst nicht Alles im Kopf haben und wissen. Einfache Recherchen, z.B. über eine Suchmaschine, können euch helfen Informationen und Beispiele zu finden. Möchtet ihr wissen wie man in der Programmiersprache Javascript eine Zufallszahl erzeugt könnte eine Suche nach "Javascript generate random number" Informationen dazu liefern. Erhaltet ihr eine Fehlermeldung "ReferenceError: xyz is not defined" kann eine kurze Suche danach vielleicht weiter helfen. Ihr seid vielleicht nicht die ersten Leute die diese Frage/das Problem haben, vielleicht haben sie Andere bereits gestellt und/oder eine Lösung dafür gefunden.

## Nachfragen
Es ist keine Schande nachzufragen wenn etwas unklar ist. Das könnt ihr beispielsweise auf allgemeinen Seiten wie [stackoverflow](https://stackoverflow.com/) nachfragen. In einigen Projekten findet ihr in der Dokumentation oder Hilfeseiten Informationen darüber wo ihr nachfragen könnt.

## Zeit und Geduld
Rom wurde nicht an einem Tag erbaut. Wenn ihr die Möglichkeit habt solltet ihr zu Beginn ausreichend Zeit einplanen und Geduld mitbringen. 

## In Teile zerlegen
Manchmal ist eine Aufgabe als Ganzes zu groß um sie am Stück zu erledigen. Ihr könnt die Aufgabe in Teile zerlegen und so stückchenweise
umsetzen. Mit der Technik **inkrementelle Entwicklung** würdet ihr dabei eine erste Version der Anwendung erstellen die noch nicht den vollen Funktionsumfang beinhaltet und schrittweise die Anwendung um weitere Funktionalität erweitern. Hierbei sollte die Anwendung nicht während der Entwicklung in einem nicht-funktionalen Zustand sein.

# Grundlegende Konstrukte

In diesem Kapitel wollen wir uns einige grundlegende Konstrukte und Konzepte für die Softwareentwicklung ansehen. 

## Vorbereitung
Wenn ihr die folgenden Konstrukte selbst ausprobieren wollt könnt ihr eine Online IDE verwenden um selbst Code zu schreiben und Auszuführen. Zum Beispiel:
* [Playcode](https://playcode.io/)
* [JSFiddle](https://jsfiddle.net/)
* [CodeSandbox](https://codesandbox.io/)
* [JSEditor](https://jseditor.io/)
* [Stackblitz](https://stackblitz.com/)
