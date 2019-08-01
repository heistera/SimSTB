﻿# SimSTB - Simulationsumgebung für digitale und analoge Ein- und Ausgänge 

Die Simulationsumgebung SimSTB ist für die Ausbildung im Bereich C/C++-Programmierung geeignet. Sie ist insbesondere
für den Unterricht bei (elektro)technischen Schülern gedacht.

Oft muss ein Programm nicht nur über die Konsole oder eine graphische Oberfläche mit dem Benutzer kommunizieren, 
sondern auch über analoge und digitale Schnittstellen mit einem technischen System.
Die Simulationsumgebung SimSTB erlaubt es, dies für Schulungszwecke auch ohne zusätzliche Hardware 
mittels Simulation durchzuführen.

Durch das Einbinden der Bibliothek simlib stehen dem Schüler vier einfach zu nutzende Funktionen für die digitale und
analoge Ein- und Ausgabe zur Verfügung. Die analogen und digitalen Werte können über eine graphische Oberfläche
bequem überwacht und gesetzt werden.


![Einsatzkontext](/bilder/Einsatzkontext.png)


## Requirements

- Die Java-Laufzeit-Umgebung (JRE) muss installiert sein.
- Die Library ist für das an der Schule im Einsatz befindliche VS C++ 2010 ausgelegt.

## Installation

1. Kontrollieren sie, ob die Java-Laufzeit-Umgebung (JRE) installiert ist.
2. Kopieren Sie das bereitgestellte Simulationsverzeichnis (in GitHub /auslieferung/sim) 
samt Unterverzeichnissen nach „C:\“. Solange Sie nur die Simulationsumgebung nutzen wollen 
und keine Modifikationen an deren Quellcode vornehmen wollen brauchen Sie keine weiteren Dateien. 
3. Kontrollieren Sie, ob folgende Verzeichnis-Struktur und Dateien vorhanden sind.

```

C:
└── Sim
    ├── anaaus.txt
    ├── anaein.txt
    ├── digaus.txt
    ├── digein.txt
    ├── LICENSE.txt
    ├── README.md
    ├── beispiele
    │   └── beispiel.cpp
    ├── bin
    │   └── SimSTB.exe
    ├── dokumentation
    │   └── SimSTB-Benutzerdokumentation.pdf
    ├── header
    │   └── simulation.h
    └── lib
         └── simlib.lib

```

## Usage

### 1. Simulations Steuerung und Monitor

Mit Hilfe des Programms SimSTB.exe können Sie digitalen und analogen Ein- und Ausgänge überwachen 
und die Eingänge setzen. Die Werte werden im Sekundentakt aktualisiert. Starten können Sie das Programm 
über einen einfachen Doppelklick auf die Exe-Datei.

![SimSTB Benutzeroberfläche](/bilder/SimSTB-GUI.png)

### 2. Erstellung eigener Programme für die Simulationsumgebung SimSTB

Mit Hilfe der vier Funktionen:

- digEin
- digAus
- anaEin
- anaAus

können Sie eigene C++-Programme schreiben. Sie können deren Ausgaben mit der Simulationsumgebung 
überwachen und die Eingänge setzen. 

Um die vier Funktionen zu nutzen, müssen Sie die Header-Datei simulation.h 
in Ihren Quellcode inkludieren und die Bibliothek simlib.lib in Ihr Projekt einbinden.

In der Datei SimSTB-Benutzerdokumentation.pdf finden Sie eine ausführrliche Beschreibung.


## License

[MIT](LICENSE.txt) © [Markus Breuer].
