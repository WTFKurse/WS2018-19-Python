# Python3WTF!?

## Willkommen im **(Exzellenz)kurs**

Ay, Ay! :v: Willkommen in unserem Python Kurs im Wintersemester 2018/19. Bevor es losgeht, ein paar Details zu unserem Kurs

* Dienstags, 4. DS
* Ort: APB/E046
* Kursseite: www.python3.wtf

Unser Kurs besteht aus drei Komponenten

<div class="panel color-1">
Präsentation
</div>

<div class="panel color-2">
Skript
</div>

<div class="panel color-3">
Praxisaufgabe
</div>

Sämtliche Slides sowie Praxisaufgaben findest du auf der Kursinternetseite der jeweiligen Kurseinheit zum Download bereit. Das Skript ist separat auf der Webseite erreichbar.

!> Für das Sammeln von Credits ist ein Nutzerkonto auf unserer Kursseite erforderlich. Eine Freischaltung erfolgt über https://python3.wtf/enrollment.

### Kurstutoren

<div class="teacher-list">
	<div class="teacher">
		<div class="avatar">
			![Patrik Phan](_images/teacher_patrik.jpg 'Patrik Phan')
		</div>
		<div class="contact">
			<h4>Patrik Phan</h4>
			patrik@wtfkurse.de
		</div>
	</div>
	<div class="teacher">
		<div class="avatar">
			![Jannusch Bigge](_images/teacher_jannusch.jpg 'Jannsuch Bigge')
		</div>
		<div class="contact">
			<h4>Jannusch Bigge</h4>
			jannusch@wtfkurse.de
		</div>
	</div>
	<div class="teacher">
		<div class="avatar">
			![Kevin Schmid](_images/teacher_kevin.jpg 'Kevin Schmid')
		</div>
		<div class="contact">
			<h4>Kevin Schmid</h4>
			kevin@wtfkurse.de
		</div>
	</div>
</div>

## Grundlagen **Programmierung**

### Grundbegriffe

<div class="column-2">
	<div>
	**Programm**<br>Ein Programm ist eine Vorschrift, nach der Informationen verarbeitet werden. Es besteht aus einer Folge von Vereinbarungen und Anweisungen. Es löst gestellte Aufgaben durch Manipulation von Daten.
	</div>
	<div>
	**Editor**<br>Ein Editor ist eine Software zur Bearbeitung und Eingabe von Programmcode (Quelltext). Er unterscheidet sich von einer komfortablen Textverarbeitung dadurch, dass er keine unsichtbaren Formatierungsanweisungen in den Text einfügt, um ihn Absätze, Listen und Tabellen zu gliedern.
	</div>
	<div>
	**Compiler**<br>Prozessoren des Computers können nur Maschinenbefehle ausführen. Compiler übersetzen den Quellcode bereits vor der Laufzeit des Programms in Maschinenbefehle.
	</div>
	<div>
	**Debugger**<br>helfen dem Programmierer beim Suchen von logischen Fehlern. Man kann Haltepunkte setzen (Breakpoints) um Variablen auf Fehler zu testen.
	</div>
	<div>
	**IDE**<br>Eine IDE ist eine Integrierte Entwicklungsumgebung (Abk. für **I**ntegrated **D**evelopment **E**nvironment) und vereint Editor, Compiler und Debugger unter einer einheitlichen Oberfläche.
	</div>
</div>


### Arten der Programmierung

#### Strukturierte Programmierung

Die strukturierte Programmierung ist die einfachste Art und Weise in der Programmierung. Innerhalb des Programmes geht man von Phasen aus, die abgegrenzt und hierarchisch sequentiell und/oder nebenläufig ausgeführt werden.


Programme werden immer komplexer, Quelltexte füllen hunderte von Seiten (führte zu einer Softwarekrise im Jahr 1970).

?> Wie können Programmerweiterungen, Verbesserungen usw. nachträglich eingebaut werden? Wie werden sie dokumentiert?


#### Objektorientierte Programmierung

**Erwartungen an das objektorientierte Paradigma**

* Wiederverwendbarkeit
* Erweiterbarkeit
* Leichte Wartbarkeit

## Einführung in **Python**

### Python Werkzeuge

Um deinen Python Quelltext auszuführen, gibt es zwei verschiedene Wege. Einen einfachen sowie einen etwas komplexeren Weg.

#### mittels einer IDE (einfach)
:one: Der bequemste Weg ist die Ausführung mittels einer IDE. Wir empfehlen für den Einstieg JetBrains PyCharm. Diese wird im Kurs weiter thematisiert.

#### mittels der Konsole (etwas komplizierter)
:one: Zuerst musst du sicher gehen, dass du Python 3 installiert hast und je nach Betriebssystem auch die Umgebungsvariablen korrekt gesetzt sind.

:two: Gehe mittels der Konsole zu dem entsprechendem Pfad in dem du deinen Python Code als **.py**-Datei gespeichert hast.

:three: Gib `python` in die Konsole ein gefolgt von `[Code-Datei].py`.

:four: Das Programm wird nun auf deiner Konsole ausgeführt. In manchen Fälen kann es passieren, dass die Konsole sich sofort nach erreichen des Endes schließt.

<? Um das Problem zu umgehen, füge in deinem Code als letzte Zeile ein `input()` ein. Die Konsole bleibt nun bis zur nächsten Benutzerinteraktion geöffnet.

### Python Eigenschaften

- Keine Semikolons
- Keine geschweiften Klammern für Codeblöcke
- Einrückungen zeigen Codblöcke an
- Funktionsaufrufe mit runden Klammern
- Funktionen werden wie folgt definiert:
`def <funktionsname>([parameterliste, ...]);`
- Variablen mit der Struktur `__name__` sind spezielle Werte

### Python Operatoren

mathematisch:		

	+, -, * , /
vergleichend:		

	<, >, <=, >=, == *(wertgleich)*, is *(Objektgleich)*
logisch:

	or, and, not |
bitweise:

	&, |, <<, >>, ^ *(xor)*, ~ *(invertierend)*
Accessoren

	. *(für mathematische methoden)* , [] *(für Datenstrukturen mit Index)*

### Start eines Programmes
Jedes Python Programm wird von oben nach unten eingelesen. Alle Befehle, die in einem `.py` Skript liegen, werden beim Start des Skriptes über `python` oder beim Einbinden des Skriptes in andere Programme ausgeführt. Man kann diesen Prozess umgehen, in dem man den Startpunkt besonders definiert. Erkennt Python diese, so startet der Programmablauf ab dieser Stelle.

```python
def main():
    foobar

if __name__ == "__main__":
    # Programm startet hier, aber nur,
    # wenn es direkt als Skript ausgeführt wird.
    main()
```
Hier wird als erstes die Funktion `main()` aufgerufen. Man könnte natürlich auch folgendes schreiben:

```python
def main():
    foobar

# Wird beim Start und beim Importieren ausgeführt
main()
```

Doch wenn man aus einem anderen Skript nun die Funktion `main` importieren möchte, würde diese dabei auch ausgeführt werden. Mit der Abfrage `if __name__ == "__main__":` verhindern wir dies. Alles, was hinter dieser `if`-Abfrage steht, wird nun ausschließlich beim Start des Skripts aufgerufen, in dem es geschrieben steht.


###  Input und Output
Kaum ein Programm kommt ohen Input und Output aus, deswegen hat Python dies gleich in der Standart Bibliothek enthalten.

Eingeb:
```python
eingabe = input("Ihre Eingabe?")
```
Zu beachten sind in dieser Zeile vier Komponente:

1. `eingabe` (Variable)
2. `=` (weist dem Ausdruck links von ihr, den Wert des Ausdrucks rechts von ihr zu)
3.  `input()` (Funktion, welche von der Konsole eine Nutzereingabe entgegennimmt)
4.  `"Ihre Eingabe?"` (String, der als Parameter für die Benutzeranweisung an die  `input()`-Funktion übergeben wurde)

Ausgabe:
```python
print("Dieses Skript ist hilfreich")
```
Es wird die Funktion `print()` aufgerufen, welche als Parameter einen String entgegen nehmen kann. In diesem Fall `Dieses Skript ist hilfreich`, welcher dann auf der Konsole ausgegeben wird.

### Variablentypen
Prinzipiell benötigen Variablen in Python keine Typdekleration. Dies liegt daran, dass während der Laufzeit vorrangig die Typüberprüfung stattfindet. Das Konzept wird auch **dynamische Typisierung** genannt.

Trotzdem sind die Typen sehr wichtig, da Python eine **stark typisierte** Sprache ist. Sprich man muss Variablentypen explizit in andere Typen umwandeln.

| Datentyp                                                                                                                                                                                                                                                                                                                                                                                                                                                   | Beispiel      |Beschreibung | Umwandlung |
|------------------------------------|-------------------|-------------------|-----------|
| Integer | i = 42 | Ganzzahl   | int() |
| Float| f = 4.2 | Gleitkommazahl       | float() |
| Complex | c = 1.5j | komplexe Zahl      | complex('1+2j') |
| Bool | b = True, b = False | boolesche Werte ||
| String | s = "Hello python" | Zeichenkette | str() |
| List | l = ['spam', 1337, 42] | veränderbare Liste ||
| Tupel | t = (21, 'word', 13) | unveränderbare Liste ||
| Dictionary | d = {1:'ham', 2: 'spam'} | assoziatives Array ||
| Set | s = set("Python") | Menge von Elementen ||
| Frozenset | fs = frozenset({1:'spma', 2 : 'ham'}) | unveränderbare Menge ||

#### Strings
Strings (Zeichenketten) sind in jeder Sprache sehr wichtig, da über sie mit dem Nutzer kommuniziert wird. Sie zu beherschen ist deswegen unabdingbar.

- Strings sind in Python nicht veränderbar
- String wird erzeugt mit `''` oder `""v
- Strings sind ab Python3 UTF-8 encoded


Strings können durch Konkatenation verknüpft werden.

```python
'Hallo' + ' ' + 'Python' # => 'Hallo Python'
```
Listen, Tupel etc. von Strings könne mit der Funktion `string.join` verknüpft werden.

```python
' '.join(['Hallo', 'Welt']) #=> 'Hallo Welt'
```


Elemente in Strings werden mit der `format()`-Funktion eingefügt.
```python
'Dies ist ein {} Satz mit {} Worten.'.format('Satz', 8)
```
oder
```python
'Dies ist ein {wort} Satz mit {number} Worten.'.format(wort = 'Satz', number = 8)
```

### JetBrains  als IDE

JetBrains ist ein tschechisches Software-Unternehmen und wurde im Jahr 2000 von den drei Russen gegründet. Das Unternehmen ist seitdem für seine seit 2001 entwickelte Java-Entwicklungsumgebung (IDE) IntelliJ IDEA bekannt.

#### Download

:arrow_down: Für die Programmiersprache Python entwickelte JetBrains die IDE PyCharm. Die Software ist Cross-Plattform kompatibel und somit für die Betriebssysteme macOS, Linux und Windows erhältlich.

https://python3.wtf/pycharm


#### Installation

:arrow_forward: Für die Programmierung von Python werden einige Tools vorausgesetzt:

* für Python 2: Versionen 2.6 und 2.7
* Python 3: ab Version 3.4 bis Version 3.7

Die jeweiligen Tools sind abhängig von der Plattform (Windows, Linux, macOS). Alle Hinweise zur Installation findest du in den Installationshinweisen.

https://python3.wtf/pycharminstall

#### Lizenzierung

:heart: Studierende können über das JetBrains Education Programm sämtliche Software des Herstellers nutzen. JetBrains bietet auch außerhalb von Python interessante Software für den Studienalltag an.

Die Anmeldung als Studierender erfolgt über die Webseite von JetBrains. Dafür ist die Verwendung der E-Mail-Adresse der TU Dresden _(@mailbox.tu-dresden.de)_ notwendig.

https://python3.wtf/jetbrains


### Kontrollstrukturen

Bis zum aktuellen Stand waren die bisher erstellten Programm in ihrer Ablauffolge sehr simpel. Es handelte sich bei den Programmen ausschließlich um Sequenzen von Anweisungen, die nach und nach ausgeführt wurden. Im Prinzip handelte es sich um das EVA-Prinzip.

In vielen Fällen lässt sich die lineare Programmstruktur nicht anwenden, da Anweisungen in eine Abhängigkeit gesetzt werden müssen. Realisiert wird dieser Programmablauf durch Auswahlstrukturen.


#### Einstufige Auswahl

**Bedingung mit einem positiven Zweig**

```python
if Bedingung:
    <Anweisung für ja>
```

#### Zweistufige Auswahl

**Bedingung mit einem positiven und negativen Zweig**

```python
if Bedingung:
    <Anweisung für ja>
else:
    <Anweisung für nein>
```

#### Mehrstufige Auswahl

**Bedingung mit einem positiven und geschachtelten negativen Zweig**

```python
if Bedingung:
    <Anweisung für ja>
elif Bedinung:
    <Anweisung für ja>
elif Bedinung:
    <Anweisung für ja>
elif Bedinung:
    <Anweisung für ja>
else:
    <Anweisung für nein>
```

### Zyklische Strukturen (Schleifen)

Wird eine Anweisung **mehrmals nacheinander** ausgeführt, so handelt es sich um eine zyklische Wiederholung.

| Typ                | Definition                                                                                                                					 |
|--------------------|-------------------------------------------------------------------------------------------------------------------------------------|
| Feste Schleife     | Besitzen eine festgelegte Anzahl von Schleifendurchläufen.                                                                					 |
| Bedingte Schleifen | Iterieren so lange, bis eine getestete Bedingung wahr wird. Der Test kann am Anfang und Ende der Schleife sein.           					 |
| Endlose Schleife   | Iterieren unendlich lang, bis ein bestimmter Mechanismus sie beendet (Warten auf Eingabe)<br/>Tastenkombination: ```Strg + Pause``` |


#### Merkmale

Bevor eine Schleife ausgelöst wird, muss ein Großteil der Variablen auf einem Anfangswert gesetzt werden.

Diesen **Anfangswert (Vorbedingung)** kann man durch Abfrage von Eingangswerten erhalten oder durch Festlegen von Anfangswerten, die sich später innerhalb der Schleife verändern.


#### for-Schleife

- Es werden die Anzahl der Wiederholungen in einem Zähler festgehalten und bei Erreichen des Zählerendstandes eingestellt.
- Anweisungen werden mindestens einmal ausgeführt, bis zum Erreichen des Endstartes (So lange, bis die Bedingung wahr geworden ist)


```python
for i in range (1, 5) :
    Anweisung1;
    Anweisung2;
    Anweisungn;

```

**Was heißt das?**

| Code            | Erklärung                                            |
|-----------------|------------------------------------------------------|
| ```for i```  	  | Schleifenzähler                                      |
| ```1```   			| Schleife beginnt bei i = 1, Anfangswert ist 1        |
| ```5``` 				| Schleife wird solange ausgeführt, bis i = 5          |


#### while-Schleife

- Bedingung ist oft ein integer-Ausdruck
-	Separater Schleifenzähler erforderlich
-	Startwert muss außerhalb davor deklariert werden


```python
x = 2;

while (x < 15):
	Anweisung1;
	Anweisung2;
	Anweisungn;
```
