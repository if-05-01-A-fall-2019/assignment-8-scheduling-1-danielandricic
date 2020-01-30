# Assignment Scheduling

## 1.Process Selection

Angenommen mein PC schickt eine Anfrage um auf bestimmte Daten von einem Server zugreifen zu können.
Der Prozess welcher den Befehl zum Server blockiert sich, weil der Benutzer nach einem Passwort für die Zugriffsrechte eingeben muss.
Der Scheduler sollte dann unbedingt den Prozess nehmen, der für die Eingabe dieses Programms zuständig ist, zu nehmen.
Sonst müsste der Benutzer warten, bis er das Passwort eingeben und somit würde es auch noch die Benutzer-Erfahrung verschlechtern.

## 2. Minimizing Turn Around Time

Um die angegebene Liste von Prozessen mit der kleinsten Turn Around Time zu bekommen, muss
man die Queue so sortieren das Sie aufsteigend nach der erwarteten Laufzeit sortiert wird.
Lösung: 
| Process | G | B | A | D | C | F | H | E |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
Expected run time (msec) | 2 | 5 | 8 | 12 | 16 | 21 | 34 | 55 
---

## 3.Round Robin Scheduler

Es würde die doppelte Rechenzeit bekommen, da das Prinzip vom Round-Robin eigentlich dafür sorgen sollte, dass jeder Prozess die gleiche Rechenzeit bekommt.
Der Prozess würde 2-mal vom Scheduler dran genommen werden.