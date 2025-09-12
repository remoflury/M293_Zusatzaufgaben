# Typescript

## 1. Theorie
Lesen dich in [Typescript](TS_Input.md) ein um ein Grundverständnis zu erhalten.

## 2. Aufgaben lösen
Da Typescript zuerst noch kompiliert werden muss, eignet sich ein Playground (keine Installation notwendig).
Löse die Aufgaben [hier](https://www.typescriptlang.org/play/).
Mit Klick auf "Run" wird der Code ausgeführt. Verwende console.log(...), um deine Ergebnisse sichtbar zu machen.
Wenn möglich, nutze die explizite Typisierung.
Recherchiere selbstständig wo nötig.

### Aufgabe 1: Implizite Typisierung
Erstelle eine Variable mit dem Namen `firstName` und speichern darin deinen eigenen Vornamen.
Lasse TypeScript automatisch den Typ erkennen (implizit).
Gib den Wert in der Konsole aus.

### Aufgabe 2: Explizite Typisierung
Erstelle eine Variable `year` mit einem passenden expliziten Typ und speichere das aktuelle Jahr darin.
Erstelle eine weitere Variable `school` mit einem weiteren passenden expliziten Typ.
Gib beide Variablen in der Konsole aus.

### Aufgabe 3: Typisierte Funktion
Schreibe eine Funktion `doubleNumber`, die eine Zahl als Parameter entgegennimmt.
und das Doppelte zurückgibt. Verwende dabei explizite Typen für den Parameter und den Rückgabewert.
Rufe die Funktion einmal mit einem Zahlenwert und einmal mit einem anderen Datentyp auf. 

### Aufgabe 4: Arrays mit Typen
Erstelle ein Array `names`, das mehrere Vornamen enthält.
Erstelle eine Funktion, welche eine Nummer als Parameter nimmt und den Namen mit dem Index
der Nummer des Paramters in der console ausspuckt.
Rufe die Funktion zweimal mit unterschiedlichen Index auf.

### Aufgabe 5: Eigener Type
Definiere einen eigenen Typ `User` mit den Eigenschaften:
- name: string
- isOnline: boolean

Erstelle zwei Objekte vom Typ `User` und gebe jeweils den Namen
und den Online-Status in der Konsole aus.

### Aufgabe 6: Union Types
Definiere eine Variable `status` mit dem Typ `"loading" | "success" | "error"`.
Wechsle zwischen den verschiedenen Werten und gib sie in der Konsole aus.
Versuche einen ungültigen Wert zuzuweisen und beobachte die TypeScript-Fehlermeldung.

### Aufgabe 7: Funktion mit benutzerdefiniertem Typ
Verwende den Typ `User` aus Aufgabe 5.
Schreibe eine Funktion `greet`, die ein Objekt vom Typ `User` als Parameter erhält
und in der Konsole "Hallo <Name>" ausgibt.
Rufe die Funktion mit beiden User-Objekten auf.

### Aufgabe 8: Bedingte Logik mit if
Erstelle eine Funktion `isMinor`, die ein Alter als Parameter entgegennimmt.
Wenn die Person mindestens 18 Jahre alt ist, soll "Volljährig" als alert() ausgegeben werden,
sonst "Minderjährig".

### Aufgabe 9: TypeScript-Fehler entdecken
Erstelle eine Funktion `calculateArea`, die Länge und Breite als Parameter nimmt und die Fläche zurückgibt.
Rufe die Funktion mit verschiedenen Datentypen auf (Zahlen, Strings, Booleans).
Beobachte, wie TypeScript dir hilft, Fehler zu finden, bevor der Code läuft.

### Aufgabe 10: Optionale Eigenschaften
Erweitere den `User`-Typ  aus Aufgabe 5 & 7 um eine optionale Eigenschaft `email?: string`.
Erstelle zwei User-Objekte: eines mit und eines ohne E-Mail-Adresse.
Schreibe eine Funktion, die prüft, ob eine E-Mail vorhanden ist, und diese ausgibt.

### Aufgabe 11: Interface vs Type
Definiere ein Interface `Product` mit den Eigenschaften:
- id: number
- name: string
- price: number
- inStock: boolean

Erstelle ein Array von Produkten und eine Funktion, die alle Produkte ausgibt, die auf Lager sind.
Vergleiche die Verwendung von Interface mit dem bisherigen Type.

### Aufgabe 12: Generics entdecken
Schreibe eine generische Funktion `getFirstItem`, die das erste Element eines Arrays zurückgibt.
Teste sie mit Arrays verschiedener Typen (string[], number[], boolean[]).
Beobachte, wie TypeScript den Rückgabetyp automatisch erkennt.

### Aufgabe 13: Type Guards
Erstelle eine Funktion `processValue`, die einen Parameter vom Typ `string | number` nimmt.
Verwende Type Guards (typeof), um zu prüfen, ob es sich um einen String oder eine Zahl handelt.
Gib entsprechend unterschiedliche Nachrichten aus.

### Aufgabe 14: Readonly und Const
Erstelle ein Objekt mit `readonly` Eigenschaften und versuche, diese zu ändern.
Verwende `const` für Arrays und versuche, Elemente hinzuzufügen oder zu entfernen.
Beobachte die TypeScript-Warnungen und verstehe den Unterschied zwischen `const` und `readonly`.

### Aufgabe 15: Enum verwenden
Definiere ein Enum `Priority` mit den Werten LOW, MEDIUM, HIGH.
Erstelle eine Funktion `getPriorityMessage`, die eine Priorität nimmt und eine entsprechende Nachricht zurückgibt.
Teste alle Prioritätsstufen und gib die Ergebnisse aus.

### Aufgabe 16: TypeScript vs JavaScript
Schreibe dieselbe Funktion einmal in JavaScript und einmal in TypeScript.
Versuche bewusst Fehler einzubauen (falsche Datentypen, fehlende Parameter).
Lasse beide Versionen laufen und vergleiche die Fehlermeldungen.
Führe ein Gespräch mit deinem Nachbarn über die Unterschiede.