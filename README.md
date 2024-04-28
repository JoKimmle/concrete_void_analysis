# concrete_void_analysis
## *automatisierte Betonporenerkennung - deutsches Menü*

*kleines Programm mit grafischer Benutzeroberfläche zum Erkennen von Poren in Sichtbeton und Bestimmen von Porenflächenanteil*

Auf diesem Repository liegt der Python Quellcode und die daraus resultierende EXE-Datei (siehe Release im linken Menüband).


## App Übersicht
<img width="1270" alt="image" src="https://github.com/JoKimmle/concrete_void_analysis/assets/64778275/d247551a-b481-4013-b0b4-1c967f9adf8e">
Links das Menüfenster, rechts die Ausgabe des Bildes mit eingezeichneten Poren und dem berechnetten Flächenanteil oben links im Bild.


## Installation der Exe-Datei:

*Alternativ kann auch das Pythonscript (Quellcode) gestartet werden -> Python-Entwicklungsumgebung benötigt.*

In der rechten Seitenleiste von Github auf dieser Seite befindet sich unter der Überschrift "Release" der "Initial Release" mit grünem Label: "Latest", auf diesen Klicken, oder alternativ auf diesen [Link](https://github.com/JoKimmle/concrete_void_analysis/releases/tag/v1.0.0) klicken.
Dort dann die erste Datei auswählen: "poren_analyse.exe" - der Download beginnt automatisch.


Bevor das Programm geladen werden kann muss der Windows defender für .exe Dateien deaktiviert werden (etwas sketchy).

Dazu diesen Schritten folgen:
1. Wählen Sie Start aus und öffnen Sie Einstellungen. Wählen Sie unter Datenschutz und Sicherheit die OptionViren- und Bedrohungsschutz.
2. Wählen Sie unter Einstellungen für den Viren- und Bedrohungsschutz die Option Einstellungen verwalten und dann unter Ausschlüsse Ausschlüsse hinzufügen oder entfernen.
(Quelle zu Schritt 1 und 2: https://support.microsoft.com/de-de/windows/hinzufügen-eines-ausschlusses-zu-windows-sicherheit-811816c0-4dfd-af4a-47e4-c301afe13b26)
3. Dann Ausschlüsse hinzufügen, Dateityp, und dann “exe” eintragen.



Dann die EXE-Datei in den Programm Ordner abspeichern, oder wo immer das Programm gespeichert werden soll.

Durch doppelklicken wird das Programm ausgeführt. Da ich kein verifizierter Entwickler bin, schaltet sich Microsoft Defender ein und warnt dass das Programm gefährlich sein kann.
Klicke auf “Mehr Information” um im Anschluss “Trotzdem Ausführen” auszuwählen.

Das Programm startet innerhalb weniger Sekunden.


## Bedienungsanleitung:

Das Programm wird von oben nach unten bedient. 

Erst wählt man ein Bild aus welches verarbeitet werden soll in dem auf “Bild auswählen” gedrückt wird. Ein Dialog öffnet sich um eine Datei auszuwählen die auf dem Computer gespeichert ist.
Wichtig: Nur Bilder vom Beton importieren (kein Meterstab, Pflanzen, etc im Bild), Bilder daher zuschneiden!

Dann wird ein Speicherort für das verarbeitete Bild festgelegt. Hier werden die ausgewerteten Bilder abgespeichert. Auch hier öffnet sich ein Systemdialog zur Auswahl des Ordners.

Nun kann am Schieberegler der grau-Grenzwert (Threshold) eingestellt werden. Je kleiner dieser Wert desto dunkler müssen die Poren sein und desto weniger werden erkannt.

Jetzt können kleine Poren herausgefiltert werden in dem der erste Hacken in der Checkbox gesetzt wird. Je nach dem was gewünscht ist können damit Poren unterhalb einer gewissen Größe aus der Berechnung ausgegrenzt werden (-> aktiv: kleinerer Porenanteil).

Die Porenkanten können mit der nächsten Checkbox geglättet werden, das erhöht besonders bei kleinen erkannten Poren die erkannte Fläche. Die erkannte Porenkontur wird dabei aber schöner.

Im letzten Schritt kann ganz unten auf “Berechnen…” geklickt werden, nun wird auf basis der festgelegten Parameter das Bild berechnet, abgespeichert und automatisch geöffnet und angezeigt.

Einzelne Parameter können danach angepasst werden und durch erneutes klicken von “Berechnen…” ausgegeben werden.


