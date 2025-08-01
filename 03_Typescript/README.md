# Typescript

## 1. Theorie
Lesen Sie sich in [Typescript](TS_Input.md) ein um ein Grundverständnis zu erhalten.

## 2. Aufgaben lösen
Da Typescript zuerst noch kompiliert werden muss, eignet sich ein Playground (keine Installation notwendig).
Lösen Sie die Aufgaben [hier](https://www.typescriptlang.org/play/).
Mit Klick auf "Run" wird der Code ausgeführt. Verwenden Sie console.log(...), um Ihre Ergebnisse sichtbar zu machen.
Wenn möglich, nutzen Sie die explizite Typisierung.

### Aufgabe 1: Implizite Typisierung
Erstellen Sie eine Variable mit dem Namen `firstName` und speichern Sie darin Ihren eigenen Vornamen.
Lassen Sie TypeScript automatisch den Typ erkennen (implizit).
Geben Sie den Wert in der Konsole aus.

### Aufgabe 2: Explizite Typisierung
Erstellen Sie eine Variable `year` mit einem passenden expliziten Typ und speichern Sie das aktuelle Jahr darin.
Erstellen Sie eine weitere Variable `school` mit einem weiteren passenden expliziten Typ.
Geben Sie beide Variablen in der Konsole aus.

### Aufgabe 3: Typisierte Funktion
Schreiben Sie eine Funktion `doubleNumber`, die eine Zahl als Parameter entgegennimmt
und das Doppelte zurückgibt. Verwenden Sie dabei explizite Typen für den Parameter und den Rückgabewert.
Rufen Sie die Funktion einmal mit einem Zahlenwert und einmal mit einem anderen Datentyp auf. 

### Aufgabe 4: Arrays mit Typen
Erstellen Sie ein Array `names`, das mehrere Vornamen enthält.
Erstellen Sie eine Funktion, welche eine Nummer als Parameter nimmt und den Namen mit dem Index
der Nummer des Paramters in der console ausspuckt.
Rufen Sie die Funktion zweimal mit unterschiedlichen Index auf.

### Aufgabe 5: Eigener Type
Definieren Sie einen eigenen Typ `User` mit den Eigenschaften:
- name: string
- isOnline: boolean

Erstellen Sie zwei Objekte vom Typ `User` und geben Sie jeweils den Namen
und den Online-Status in der Konsole aus.


### Aufgabe 7: Funktion mit benutzerdefiniertem Typ
Verwenden Sie den Typ `User` aus Aufgabe 6.
Schreiben Sie eine Funktion `greet`, die ein Objekt vom Typ `User` als Parameter erhält
und in der Konsole "Hallo <Name>" ausgibt.
Rufen Sie die Funktion mit beiden User-Objekten auf.


### Aufgabe 8: Bedingte Logik mit if
Erstellen Sie eine Funktion `isMinor`, die ein Alter als Parameter entgegennimmt.
Wenn die Person mindestens 18 Jahre alt ist, soll "Volljährig" als alert() ausgegeben werden,
sonst "Minderjährig".