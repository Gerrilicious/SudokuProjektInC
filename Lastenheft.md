1 Zielbestimmung
======
Ein Geschäftsbereich des HHBK Tendo Research Centers entwickelt und vertreibt Computerspiele für Thin Clients (Handys, Handhelds, etc.) unter dem Betriebssystem Linux. Der Schwerpunkt liegt dabei auf der Entwicklung linea¬rer Al¬gorith¬¬men zur Unter¬stützung optimaler Spiel¬stra¬te¬gien. Um zu tes¬ten, ob das Spiel „Sudoku“ erfolg¬reich am Markt plaziert wer¬den kann, wird zunächst die Programmierung eines Pro¬totypens in Auftrag gegeben.
Spielbeschreibung: Sudoku ist ein Zahlenpuzzle. Das Puzzlefeld besteht aus einem Quadrat, das in 3 × 3 Unterquadrate bzw. Blöcke eingeteilt ist. Jedes Unterquadrat ist wieder in 3 × 3 Felder eingeteilt. Das Gesamtquadrat enthält also 81 Felder in 9 Reihen und 9 Spalten.
In einige dieser Felder sind schon zu Beginn Ziffern (1 bis 9) eingetragen. Typischerweise sind 22 bis 36 Felder von 81 möglichen vorgegeben. Das Puzzle muss nun so vervollständigt werden, dass
- in jeder Zeile, 
- in jeder Spalte und 
- in jedem der neun Blöcke jede Ziffer von 1 bis 9 genau einmal auftritt. 
Das Puzzlefeld besteht aus einem Quadrat, das in 3 × 3 Unterquadrate bzw. Blöcke eingeteilt ist. Jedes Unterquadrat ist wieder in 3 × 3 Felder eingeteilt. Das Gesamtquadrat enthält also 81 Felder in 9 Reihen und 9 Spalten.
### 1.1	Musskriterien
- Der Prototyp soll als ANSI C Konsolenanwendung entwickelt werden.
- Es sollen mehrere Spielrunden möglich sein.
- Auswahl verschiedener Schwierigkeitsstufen.
- Führen einer Bestenliste in Abhängigkeit der Schwierigkeitsstufe.
- Anbieten einer Hilfefunktion.
- Anzeige der Spielregeln.
- Verwendung einer SQLite-Datenbank zur Verwaltung der Benutzerdaten und der Bestenliste.
### 1.2	Wunschkriterien
- Dynamische Sudoku Generierung.
- Bestenliste-Report in Bezug auf die gespielte Zeit.
### 1.3	Abgrenzungskriterien
- Das Spiel wird von einem Spieler an einem PC gespielt. Netzwerkfähigkeit ist nicht gefordert!
# 2	Produkteinsatz
### 2.1	Anwendungsbereiche
- Freizeitbereich
- Der Prototype „Sudoku“ dient einerseits zum Testen der eigentlichen Spielstrategie, andererseits zum Ausloten der vom Kunden gewünschten Funktionalität.
### 2.2	Zielgruppen
Zielgruppe sind ausgewählte Testpersonen im Alter zwischen 12 und 99, die strategische Spiele bevorzugen.

3 Produktumgebung
======
### 3.1	Software
### 3.2	Hardware
### 3.3	Orgware
### 3.4	Produktschnittstellen

4 Produktfunktionen
======
### 4.1	Bestenliste
LF0100 Für jede Spielrunde wird die benötigte Zeit gemessen und am Ende einer Spielrunde angezeigt. 
LF0200 In Abhängigkeit des Schwierigkeitsgrads soll eine Bestenliste geführt werden. Der Spieler kann sich auf Wunsch in die Bestenliste eintragen. 
### 4.2	Kandidaten anzeigen (optional)
LF0200w	Der Spieler kann sich für alle noch nicht belegten Felder mögliche Kandidaten anzeigen lassen. Natürlich kann er die Kandidaten auch wieder ausblenden lassen.  	 

### 4.3	Hilfe (optional)
LF0300w	Der Spieler kann für ein Feld Hilfe anfordern. In diesem Fall wird die korrekte Ziffer für dieses Feld automatisch gesetzt.
LF0310w	Die Anzahl der automatisch gesetzten Ziffern wird am Ende einer Spielrunde angezeigt. 
### 4.4	Spielabbruch
LF0400 Der Spieler kann sich die Gesamtlösung des Sudokus anzeigen lassen. Die Spielrunde ist damit automatisch beendet.
LF0410 Eine Spielrunde ist auch beendet, wenn das Sudoku gelöst und alle Felder des Sudokus richtig belegt sind.
### 4.5	Schwierigkeitsstufen
LF0500 Zu Beginn einer Spielrunde kann der Spieler zwischen folgenden Schwierigkeitsstufen für das neue Sudoku wählen: leicht, normal, schwierig. Der Schwierigkeitsgrad wird durch die Anzahl der vorbelegten Felder bestimmt.
### 4.6	Bereitstellung von Sudokus
LF0600 Für jede Schwierigkeitsstufe müssen mindestens 10 Sudokus vorhanden sein, die per Zufallsverfahren vom Programm ausgewählt werden.
LF0610w	Optional: Bereitstellung eines linearen Algorithmus zur dynamischen Generierung von Sudokus.
### 4.7	Bereitstellung der Spielregeln (optional)
  
LF0700w	Der Spieler kann jederzeit die Spielregeln einsehen.

### 4.8	Startbedingungen

LF0800 Der Spieler muss sich nicht registrieren oder einloggen, um ein Spiel starten zu können.	

LF0810 Der Spieler muss eingeloggt sein, um sich in die Bestenliste eintragen zu können.



5 Produktdaten
======
### 5.1	Bestenliste
LD0100 Speicherung der Bestenliste in einer SQLite-Datenbank  Datei.

### 5.2	Dokumentationen
LD0210 Anwenderdokumentation im pdf-Format.
	Die Anwenderdokumentation enthält Hinweise zur Installation, die Spielregeln, Spieltipps und einige Spielbeispiele.
LD0220 Feinkonzept im pdf-Format.
LD0230 Das Projekt wird durch eine  Projektpräsentation nach Vorgaben der IHK Düsseldorf ab-geschlossen.
LD0240 Prozessorientierte Projektdokumentation im pdf-Format nach Vorgaben der IHK Düsseldorf. (Erstellung erst nach der Projektwoche)

### 5.3	Quellcode
LD0300 Alle Quellcodedateien incl. Projektdateien.

### 5.4	Lauffähiges Programm
LD0400 Lauffähiger Sudoku-Prototyp als EXE-Datei.

6 Produktleistungen
======
### 6.1	Anforderungen an die Entwicklung des Prototyps
LL0110 Beim Design des Prototyps soll der Schwerpunkt auf wiederverwendbare Software gelegt werden. Aus diesem Grund wird eine modulare und funktionsorientierte Architektur mit sauber definierten Schnittstellen erwartet.
LL0120 100%tige Einhaltung des HHBK Programmierstandards.
### 6.2	Anforderungen an die Anwenderdokumentation („Kundenhandbuch“)
LL0210 Ausführliche Erläuterungen der Spielregeln.
LL0220 Angabe der Zielgruppe mit Begründung der Zielgruppenauswahl.
LL0230 Installationshinweise
LL0240 Beschreibung des Spielverhaltens zur Laufzeit 
LL0250 Beschreibung der Spieloptionen (z.B. Schwierigkeitsgrad)
LL0260 Erläuterungen denkbare Spielstrategien
LL0270 Bekannte Bugs
LL0280 FAQs
### 6.3	Anforderungen an das Feinkonzept („Technische Dokumentation“)
LL0310 Architektur des Quellcodes  Beschreibung der Modulstruktur (Quellcodedateien, Include-Dateien) und Aufteilung der Funktionen auf Module.
LL0320 main()-Funktion  Schnittstellenbeschreibung und Beschreibung des Algorithmus wahlweise als Struktogramm oder PAP.
LL0330 Für jede weitere Funktion  Schnittstellenbeschreibung und Beschreibung des Algorithmus.  Für einige ausgesuchte Funktionen Darstellung als Struktogramm oder PAP (wahlweise).
LL0340 Beschreibung der verwendeten globalen Variablen.
LL0350 Beschreibung der geplanten Testszenarien.
### 6.4	Anforderungen an die Projektdokumentation („IHK-Dokumentation“)
(Diese Dokumentation wird nach der Projektwoche erstellt)
LL0410 Projektziel
LL0420 Projektumfeld (Entwicklungsumgebung, Zielumgebung)
LL0430 Phasenmodell  Formale und inhaltliche Beschreibung der einzelnen Projektphasen, incl. Abweichungen von der geplanten Vorgehensweise. 
LL0440 Projektplan incl. Aufgabenverteilung / Verantwortlichkeiten.
LL0450 Planung der Tests
LL0460 Beschreibung der Projektdurchführung mit Begründungen der Vorgehensweisen, evtl. Erläuterung von möglichen Alternativen.
LL0470 Durchgeführte Tests mit Ergebnissen
LL0480 Zielerreichung  Vergleich des fertigen Produktes mit dem SOLL-Konzept.
LL0490 Zeitlicher Soll-/Ist-Vergleich.
LL0500 Fazit und persönliche Projektreflexion („lessons learned“).


7 Benutzeroberfläche
======

8 Qualitätszielbestimmung
======

9 Globale Testfälle
======

10 Entwicklungs-Umgebung
======

### 10.1 Software
- Betriebssystem Windows 7 oder höher
### 10.2 Hardware
- Standard PC
### 10.3 Orgware
- keine 
### 10.4 Produkt-Schnittstellen
- keine

11 Ergänzungen
======
- Wird der Prototyp als ANSI-C Konsolenanwendung entwickelt, müssen nicht ANSI-C kompatible Funktionen oder Anweisungen in eine eigene Quellcodedatei namens system.c ausgelagert!
- Die Portierung der nicht ANSI-C kompatiblen Funktionen auf Linux erfolgt erst nach erfolgreichem Test des Sudoku-Prototypens.
- Um den Projektfortschritt regelmäßigen Reviews unterziehen zu können, sollte die Planung und der Verlauf des Projektes in einem Projektplaner (z.B. MS Project) erfasst sein.
- Der Projektauftrag wird an kleinere Teams mehrfach vergeben, um zwischen den besten Prototypen wählen zu können. Einem Projektteam sollten nicht mehr als 7 Mitglieder angehören. Die einzelnen Teams sollten so weit möglich „autark“ arbeiten! Ein Austausch von Arbeitsergebnissen ist im Sinne der Konkurrenzsituation nicht erwünscht! Technische Ratschläge und Hilfestellungen unter Kollegen und Kolleginnen sollten allerdings selbstverständlich sein.

