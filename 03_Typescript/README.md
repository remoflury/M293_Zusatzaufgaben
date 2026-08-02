# Typescript

## 1. Theorie
Lesen Sie sich in [Typescript](TS_Input.md) ein um ein Grundverständnis zu erhalten.

## 2. Aufgaben lösen
Da Typescript zuerst noch kompiliert werden muss, eignet sich ein Playground (keine Installation notwendig).
Lösen Sie die Aufgaben [hier](https://www.typescriptlang.org/play/).
Mit Klick auf "Run" wird der Code ausgeführt. Verwenden Sie console.log(...), um Ihre Ergebnisse sichtbar zu machen.
Wenn möglich, nutzen Sie die explizite Typisierung.
Recherchieren Sie selbstständig wo nötig.

### Aufgabe 1: Implizite Typisierung
Erstellen Sie eine Variable mit dem Namen `firstName` und speichern Sie darin Ihren eigenen Vornamen.
Lassen Sie TypeScript automatisch den Typ erkennen (implizit).
Geben Sie den Wert in der Konsole aus.

### Aufgabe 2: Explizite Typisierung
Erstellen Sie eine Variable `year` mit einem passenden expliziten Typ und speichern Sie das aktuelle Jahr darin.
Erstellen Sie eine weitere Variable `school` mit einem weiteren passenden expliziten Typ.
Geben Sie beide Variablen in der Konsole aus.

### Aufgabe 3: Typisierte Funktion
Schreiben Sie eine Funktion `doubleNumber`, die eine Zahl als Parameter entgegennimmt.
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

### Aufgabe 6: Union Types
Definieren Sie eine Variable `status` mit dem Typ `"loading" | "success" | "error"`.
Wechseln Sie zwischen den verschiedenen Werten und geben Sie sie in der Konsole aus.
Versuchen Sie einen ungültigen Wert zuzuweisen und beobachten Sie die TypeScript-Fehlermeldung.

### Aufgabe 7: Funktion mit benutzerdefiniertem Typ
Verwenden Sie den Typ `User` aus Aufgabe 5.
Schreiben Sie eine Funktion `greet`, die ein Objekt vom Typ `User` als Parameter erhält
und in der Konsole "Hallo <Name>" ausgibt.
Rufen Sie die Funktion mit beiden User-Objekten auf.

### Aufgabe 8: Bedingte Logik mit if
Erstellen Sie eine Funktion `isMinor`, die ein Alter als Parameter entgegennimmt.
Wenn die Person mindestens 18 Jahre alt ist, soll "Volljährig" als alert() ausgegeben werden,
sonst "Minderjährig".

### Aufgabe 9: TypeScript-Fehler entdecken
Erstellen Sie eine Funktion `calculateArea`, die Länge und Breite als Parameter nimmt und die Fläche zurückgibt.
Rufen Sie die Funktion mit verschiedenen Datentypen auf (Zahlen, Strings, Booleans).
Beobachten Sie, wie TypeScript Ihnen hilft, Fehler zu finden, bevor der Code läuft.

### Aufgabe 10: Optionale Eigenschaften
Erweitern Sie den `User`-Typ  aus Aufgabe 5 & 7 um eine optionale Eigenschaft `email?: string`.
Erstellen Sie zwei User-Objekte: eines mit und eines ohne E-Mail-Adresse.
Schreiben Sie eine Funktion, die prüft, ob eine E-Mail vorhanden ist, und diese ausgibt.

### Aufgabe 11: Interface vs Type
Definieren Sie ein Interface `Product` mit den Eigenschaften:
- id: number
- name: string
- price: number
- inStock: boolean

Erstellen Sie ein Array von Produkten und eine Funktion, die alle Produkte ausgibt, die auf Lager sind.
Vergleichen Sie die Verwendung von Interface mit dem bisherigen Type.

### Aufgabe 12: Generics entdecken
Schreiben Sie eine generische Funktion `getFirstItem`, die das erste Element eines Arrays zurückgibt.
Testen Sie sie mit Arrays verschiedener Typen (string[], number[], boolean[]).
Beobachten Sie, wie TypeScript den Rückgabetyp automatisch erkennt.

### Aufgabe 13: Type Guards
Erstellen Sie eine Funktion `processValue`, die einen Parameter vom Typ `string | number` nimmt.
Verwenden Sie Type Guards (typeof), um zu prüfen, ob es sich um einen String oder eine Zahl handelt.
Geben Sie entsprechend unterschiedliche Nachrichten aus.

### Aufgabe 14: Readonly und Const
Erstellen Sie ein Objekt mit `readonly` Eigenschaften und versuchen Sie, diese zu ändern.
Verwenden Sie `const` für Arrays und versuchen Sie, Elemente hinzuzufügen oder zu entfernen.
Beobachten Sie die TypeScript-Warnungen und verstehen Sie den Unterschied zwischen `const` und `readonly`.

### Aufgabe 15: Enum verwenden
Definieren Sie ein Enum `Priority` mit den Werten LOW, MEDIUM, HIGH.
Erstellen Sie eine Funktion `getPriorityMessage`, die eine Priorität nimmt und eine entsprechende Nachricht zurückgibt.
Testen Sie alle Prioritätsstufen und geben Sie die Ergebnisse aus.

### Aufgabe 16: TypeScript vs JavaScript
Schreiben Sie dieselbe Funktion einmal in JavaScript und einmal in TypeScript.
Versuchen Sie bewusst Fehler einzubauen (falsche Datentypen, fehlende Parameter).
Lassen Sie beide Versionen laufen und vergleichen Sie die Fehlermeldungen.
Führen Sie ein Gespräch mit Ihrem Sitznachbarn über die Unterschiede.
