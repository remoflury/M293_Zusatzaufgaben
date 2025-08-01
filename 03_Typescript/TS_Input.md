# Typescript Input

## Hintergrund
Javascript ist eine beliebte Programmiersprache. Wie Sie wissen, hat Javascript verschiedene Datentypen. JS ist jedoch loosely typed.
Was heisst das? Nehmen wir folgendes Beispiel:

```JS
let age = 24;
```

Der Type des Variable age ist number. Nun ist es in Javascript möglich, diese Variable mit einem komplett anderen Datentyp zu überschreiben:

```JS
let age = 24;
age = "Ich bin keine Numer";
```

Das ist valider JS-Code. Je grösser der Code wird, desto schwieriger wird es für Entwickler:innen den Überblick über alle Variablen zu halten. 
So kann es schnell geschehen, dass man Variablen mit einem anderen Datentyp überschreibt, ohne dass man es merkt. Erst wenn der Code ausgeführt wird, kommt es (eventuell) zu einem Fehler.

Typescript (TS) soll genau das verhindern. Es sollte schon während der Entwicklung anzeigen, ob Fehler passieren:
 
 ```TS
let age = 24;
age = "Ich bin keine Numer"; // Error: Type 'string' is not assignable to type 'number'.
```

## Typen deklarieren
In TypeScript können (und sollten) die Typen von Variablen, Funktionen und Parametern explizit angegeben werden.
Dadurch weiss der Editor bzw. Compiler bereits zur Entwicklungszeit, welcher Typ erwartet wird.

### Beispiele
```TS
let age: number = 24;
let name: string = "Anna";
let isOnline: boolean = true;
```

Auch Objects und Arrays lassen sich so typisieren:
```TS
let scores: number[] = [10, 20, 30];

let user: { name: string; age: number } = {
  name: "Jonas",
  age: 30,
};
```

Funktionen können ebenfalls so typisiert werden:
```TS
const greet = (name: string) => {
  console.log("Hallo " + name);
}
```

Diese Typisierung sorgt dafür, dass nur gültige Werte verwendet werden können – noch bevor der Code ausgeführt wird.


## Implicit vs Explicit
TypeScript ist „smart“ genug, um viele Typen automatisch zu erkennen. Das nennt man **implizite** Typisierung.

```TS
const city = "Zürich"; // TypeScript erkennt automatisch: string
```

Wenn der Typ jedoch bewusst festgelegt werden soll (z. B. zur Dokumentation oder zur Klarheit), spricht man von **expliziter** Typisierung:
```TS
let city: string = "Zürich";
```

Manchmal ist explizite Typisierung auch nötig – etwa bei leeren Arrays oder null-Werten, bei denen TypeScript nicht automatisch erraten kann, was später kommt.


## Eigene Types
In grösseren Programmen werden oft dieselben Strukturen mehrfach verwendet – zum Beispiel Informationen über Benutzer:innen, Produkte oder Artikel.
Damit man diese Strukturen nicht immer wieder neu schreiben muss, kann man in TypeScript eigene Typen definieren.

Das macht den Code übersichtlicher, einheitlicher und wartbarer.

### Beispiel mit Objekt
Nehmen wir an, wir arbeiten mit User-Objekten:

```TS
let user: { name: string; age: number } = {
  name: "Luca",
  age: 25,
};
```

Wenn wir viele solche Objekte brauchen, ist es mühsam, diese Schreibweise jedes Mal zu wiederholen.
Stattdessen definieren wir einen eigenen Typ:
```TS
type User = {
  name: string;
  age: number;
};

let user: User = {
  name: "Luca",
  age: 25,
};
```

Nun können wir den neuen Typ überall verwenden:
```TS
let user1: User = { name: "Luca", age: 25 };
let user2: User = { name: "Stephanie" }; // Error: Property 'age' is missing in type '{ name: string; }' but required in type 'User'.
```