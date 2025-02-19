# Tag 8 – Schleifen

## Lernziele

- Grundverständnis von Schleifen: Verstehen, was Schleifen sind und wozu sie verwendet werden.
- Arten von Schleifen: Kennenlernen der verschiedenen Arten von Schleifen in JavaScript (`for`, `while`, `do...while`).
- Schleifensteuerung: Wissen, wie man Schleifen startet, kontrolliert und beendet.
- Verschachtelte Schleifen: Verstehen, wie verschachtelte Schleifen funktionieren und angewendet werden.
- Effiziente Nutzung: Lernen, wie man Schleifen effizient und performant einsetzt.

## Inhalte

### Einführung in Schleifen

- Was ist eine Schleife?
- Vorteile der Verwendung von Schleifen

### `for`Schleife

Struktur und Syntax der `for`Schleife.
        
```jsx
for (let i = 0; i < 5; i++) {
	console.log(i);
}
```
        
### `while`Schleife

Struktur und Syntax der `while`Schleife.
        
```jsx
let i = 0;while (i < 5) {
	console.log(i);  i++;
}
```
        
### `do...while`Schleife

Struktur und Syntax der `do...while`Schleife
        
```jsx
let i = 0;

do {
console.log(i);  i++;
} while (i < 5);
```
        
### Schleifensteuerung

Verwendung von `break` und `continue`
        
```jsx
for (let i = 0; i < 5; i++) {
	if (i === 3) {
		break;
	}
  console.log(i);
}
        
for (let i = 0; i < 5; i++) {
	if (i === 3) {
		continue;
	}
  console.log(i);
}
```
        
### Verschachtelte Schleifen
Erklärung und Beispiele für verschachtelte Schleifen
    
```jsx
for (let i = 0; i < 3; i++) {
  for (let j = 0; j < 3; j++) {
	  console.log(`i = ${i}, j = ${j}`);
  }
}
```
        
### Effiziente Nutzung von Schleifen

#### Tipps zur Optimierung der Leistung von Schleifen
#### Vermeidung von Endlosschleifen

## 📌 1. Stunde – Einführung in Schleifen (60 min)

### Lernziele der ersten Stunde:

- ✅ Verstehen, was Schleifen sind und warum sie wichtig sind
- ✅ Erkennen, welche Probleme Schleifen lösen
- ✅ Einführung in verschiedene Schleifenarten
- ✅ Grundlegende Syntax und erste praktische Beispiele

### 🕑 1. Einführung (15 min) – Warum brauchen wir Schleifen?

**❓ Problemstellung: Wie wiederholen wir Anweisungen ohne Schleifen?**
Nehmen wir an, wir wollen die Zahlen 1 bis 5 ausgeben.
Ohne Schleife:

```
console.log(1);
console.log(2);
console.log(3);
console.log(4);
console.log(5);
```

👉 Fragen an die Klasse:

1. Was fällt an diesem Code auf?
2. Was wäre, wenn wir die Zahlen von 1 bis 100 ausgeben wollten?

➡ Antwort: Viel redundanter Code, schwer wartbar und nicht flexibel.

### 🕑 2. Einführung in das Konzept von Schleifen (10 min)

**📌 Was ist eine Schleife?**

Eine Schleife ist eine wiederholende Code-Struktur, die eine Bedingung überprüft und eine Anweisung mehrfach ausführt.

**💡 Alltagsszenario:**

- Eine Ampel schaltet in einem festen Rhythmus (Rot → Grün → Gelb → Rot).
- Ein Roboter schraubt in einer Fließbandproduktion immer wieder Schrauben fest.

**📌 Vorteile von Schleifen:**
1. Reduzierung von Code-Wiederholungen
2. Erhöhte Flexibilität – Der Code funktioniert für beliebige Wertebereiche
3. Automatisierung von Aufgaben

### 🕑 3. Erste Begegnung mit Schleifen (15 min) – Einführung in for-Schleife

#### 🖥 Die for-Schleife – unsere erste Schleife

**📌 Grundstruktur:**

```
for (Startwert; Bedingung; Änderung) {
  // Code, der wiederholt wird
}
```

**💡 Beispiel: Zahlen von 1 bis 5 ausgeben:**

```
for (let i = 1; i <= 5; i++) {
  console.log(i);
}
```

**👉 Erklärung Schritt für Schritt:**

1. `let i = 1;` → Initialisiert die Zählvariable i mit 1.
2. `i <= 5;` → Bedingung: Solange i kleiner oder gleich 5 ist, läuft die Schleife.
3. `i++` → Erhöht `i` um 1 nach jedem Durchlauf.
4. `console.log(i)`; → Gibt `i` bei jedem Schleifendurchlauf aus.

**💡 Erwartete Ausgabe:**

```
1  
2  
3  
4  
5  
```

### 🕑 4. Praktische Übung (15 min) – Erste eigene Schleife schreiben

**📌 Aufgabe 1:**

Erstelle eine for-Schleife, die die Quadratzahlen von 1 bis 10 ausgibt.

**💡 Erwartete Ausgabe:**

```
1  
4  
9  
16  
25  
36  
49  
64  
81  
100
```  

**📌 Lösung:**

```
for (let i = 1; i <= 10; i++) {
  console.log(i * i);
}
```

**📌 Aufgabe 2:**

Gib die Zahlen von 10 bis 1 in absteigender Reihenfolge aus.

**💡 Erwartete Ausgabe:**

```
10  
9  
8  
7  
6  
5  
4  
3  
2  
1  
```

**📌 Lösung:**

```
for (let i = 10; i >= 1; i--) {
  console.log(i);
}
```

### 🕑 5. Abschluss & Diskussion (5 min) – Wann ist eine Schleife sinnvoll?

**👉 Diskussionsfragen:**

- In welchen realen Szenarien sind Schleifen hilfreich?
- Welche möglichen Probleme könnten mit Schleifen entstehen?

**📌 Zusammenfassung:**

1. Schleifen automatisieren sich wiederholende Aufgaben.
2. Die for-Schleife eignet sich besonders für feste Wiederholungen.
3. Wir können sie nutzen, um durch Zahlen, Arrays oder andere Datenstrukturen zu iterieren.

## 📌 2. Stunde – Die while- und do...while-Schleifen (60 min)

### Lernziele:

- ✅ Verstehen, wie die while-Schleife funktioniert
- ✅ Verstehen, wie sich die do...while-Schleife von der while-Schleife unterscheidet
- ✅ Erkennen, wann while-Schleifen gegenüber for-Schleifen vorteilhaft sind
- ✅ Erste praktische Übungen mit while und do...while

### 🕑 1. Wiederholung & Motivation (10 min) – Was wissen wir schon über Schleifen?

**📌 Rückblick auf die for-Schleife**

1. Feste Wiederholungsanzahl
2. Besteht aus Startwert, Bedingung und Änderung

### ❓ Problemstellung: Was passiert, wenn wir nicht genau wissen, wie oft eine Schleife durchlaufen werden soll?

**👉 Beispiel:**

- Ein Benutzer soll so lange nach einem Passwort gefragt werden, bis es richtig eingegeben wurde.
- Eine Animation soll so lange laufen, bis ein bestimmtes Ereignis eintritt.

**➡ Lösung? while-Schleife!**

### 🕑 2. Die while-Schleife (15 min) – Einführung & Syntax

**📌 Grundstruktur:**

```
while (Bedingung) {
  // Code, der wiederholt wird
}
```

**👉 Beispiel: Zahlen von 1 bis 5 ausgeben**

```
let i = 1;

while (i <= 5) {
  console.log(i);
  i++; // WICHTIG: Erhöhen der Variable, sonst Endlosschleife!
}
```

**💡 Erklärung Schritt für Schritt:**

1. `let i = 1;` → Startwert der Zählvariable.
2. `while (i <= 5)` → Bedingung: Solange i kleiner oder gleich 5 ist, läuft die Schleife.
3. `console.log(i);` → Gibt i aus.
4. `i++` → Erhöht i um 1 nach jedem Durchlauf.

**💡 Erwartete Ausgabe:**

```
1  
2  
3  
4  
5  
```

### 🕑 3. Praktische Übung 1 (10 min) – Eigene while-Schleifen schreiben

**📌 Aufgabe 1:**

Schreibe eine while-Schleife, die die ungeraden Zahlen von 1 bis 10 ausgibt.

**💡 Erwartete Ausgabe:**

```
1  
3  
5  
7  
9  
```

**📌 Lösung:**

```
let i = 1;

while (i <= 10) {
  console.log(i);
  i += 2; // Erhöht i um 2
}
```

**📌 Aufgabe 2:**

Schreibe eine `while`-Schleife, die einen Countdown von 10 auf 1 ausgibt.

**💡 Erwartete Ausgabe:**

```
10  
9  
8  
7  
6  
5  
4  
3  
2  
1  
```

**📌 Lösung:**

```
let i = 10;

while (i >= 1) {
  console.log(i);
  i--; // Verringert i um 1
}
```

### 🕑 4. Die `do...while`-Schleife (15 min) – Einführung & Unterschied zur `while`-Schleife

**📌 Unterschied zwischen while und do...while:**

- Eine `while`-Schleife prüft die Bedingung zuerst. Wenn sie `false` ist, wird der Code kein einziges Mal ausgeführt.
- Eine `do...while`-Schleife führt den Code mindestens einmal aus, egal ob die Bedingung zu Beginn `false` ist.

**📌 Grundstruktur:**

```
do {
  // Code, der mindestens einmal ausgeführt wird
} while (Bedingung);
```

**👉 Beispiel: Zahlen von 1 bis 5 ausgeben**

```
let i = 1;

do {
  console.log(i);
  i++;
} while (i <= 5);
```

**💡 Erwartete Ausgabe:**

```
1  
2  
3  
4  
5  
```

**👉 Was passiert, wenn i = 10 ist?**

```
let i = 10;

do {
  console.log(i);
  i++;
} while (i <= 5);
```

**💡 Ausgabe:**
```
10
```

➡ Der Code wird einmal ausgeführt, bevor die Bedingung geprüft wird!

### 🕑 5. Praktische Übung 2 (10 min) – `do...while` in Aktion

**📌 Aufgabe:**

Schreibe eine `do...while`-Schleife, die eine Zahl vom Benutzer abfragt, bis er eine Zahl größer als 10 eingibt.

**📌 Lösung:**

```
let zahl;

do {
  zahl = prompt("Gib eine Zahl größer als 10 ein:");
} while (zahl <= 10);

console.log("Danke! Du hast eine gültige Zahl eingegeben:", zahl);
```

### 🕑 6. Abschluss & Diskussion (10 min) – Wann while statt for nutzen?

**📌 Wann `while` statt `for` verwenden?**

| `for`-Schleife | `while`-Schleife |
|:--|:--|
| Wenn die Anzahl der Durchläufe bekannt ist |	Wenn die Anzahl der Durchläufe unbekannt ist|
| Perfekt für Zähler-basierte Schleifen	| Perfekt für Ereignis-basierte Schleifen |
| Gut für das Iterieren über Arrays	| Gut für Benutzereingaben oder Sensorwerte |

### 📌 Wann do...while statt while nutzen?

Wenn eine Aktion mindestens einmal ausgeführt werden soll
Perfekt für Benutzereingaben oder Menüs

**👉 Diskussionsfragen:**

- Warum kann eine `while`-Schleife eine Endlosschleife verursachen?
	- Eine `while`-Schleife kann eine Endlosschleife verursachen, wenn die Bedingung niemals false wird. Das bedeutet, dass die Schleife unendlich weiterläuft, weil es keinen Mechanismus gibt, sie zu beenden.
-Wie vermeidet man Endlosschleifen?
	- Überprüfe, ob die Bedingung wirklich irgendwann `false` werden kann.
	- Stelle sicher, dass sich Variablen innerhalb der Schleife verändern.
	- Nutze ein break, falls eine maximale Anzahl an Durchläufen sinnvoll ist.
	- Teste den Code mit kleinen Werten, bevor du große Schleifen ausführst.

- Wo habt ihr `while`-Schleifen in realen Anwendungen gesehen?
	- Unbekannte Anzahl an Durchläufen (z. B. Login-Versuche, API-Anfragen, Spielschleifen).
	- Überwachung und Automatisierung (z. B. Server-Status, Bestellverarbeitung).
	- Kontinuierliche Prozesse (z. B. Hintergrundaufgaben, Echtzeit-Updates).
	- Kurz gesagt: `while` ist perfekt, wenn nicht im Voraus bekannt ist, wie oft eine Schleife durchlaufen werden muss! 🚀

**📌 Zusammenfassung:**

- `while`-Schleifen sind gut, wenn wir nicht wissen, wie oft etwas wiederholt werden soll.
- `do...while`-Schleifen garantieren mindestens eine Ausführung.
- Beide können für Benutzerinteraktionen, Sensorwerte oder Event-basierte Programmierung genutzt werden.

## Hier ist die detaillierte Ausarbeitung der **dritten Stunde** deiner Unterrichtseinheit über Schleifen in JavaScript.  

---

## 🕒 Dritte Stunde: Schleifensteuerung mit `break` und `continue`  

### **🎯 Lernziele:**  
- Verstehen**, wie man Schleifen gezielt unterbricht (`break`).  
- Lernen, wie `continue` genutzt wird, um bestimmte Durchläufe zu überspringen.  
- Praktische Anwendung in realistischen Beispielen.  



### 1️⃣ Einführung in die Schleifensteuerung  

Schleifen laufen in der Regel bis zu einer bestimmten Bedingung. Aber was, wenn wir eine Schleife **vorzeitig abbrechen** oder einen **bestimmten Durchlauf überspringen** wollen?  

Dafür gibt es **zwei wichtige Steuerungsanweisungen** in JavaScript:  

| **Anweisung** | **Bedeutung** |
|--------------|--------------|
| `break` | Stoppt die Schleife vollständig. |
| `continue` | Überspringt den aktuellen Durchlauf und springt zur nächsten Iteration. |

---

### 2️⃣ `break`: Eine Schleife vorzeitig beenden  

**🔹 Beispiel 1: `break` in einer `for`-Schleife**  
Sobald die Zahl `5` erreicht wird, soll die Schleife abgebrochen werden.  

```js
for (let i = 1; i <= 10; i++) {
	if (i === 5) {
		console.log("Schleife abgebrochen!");
		break; // Beendet die Schleife, sobald i gleich 5 ist.
	}
	console.log(i);
}
```

🔍 **Erwartete Ausgabe:**  
```
1  
2  
3  
4  
Schleife abgebrochen!
```

✔ **Warum `break` nutzen?**  
- Wenn man nicht unnötig weiter iterieren möchte (z. B. eine **Zahlensuche beenden**, sobald die gewünschte Zahl gefunden wurde).  

**🔹 Beispiel 2: `break` in einer `while`-Schleife**  
Ein Nutzer soll so lange eine Zahl eingeben, bis er `0` eingibt:  

```js
while (true) {  // Endlosschleife!
	let zahl = prompt("Gib eine Zahl ein (0 zum Beenden):");
	if (zahl === "0") {
		console.log("Schleife gestoppt.");
		break;  // Beendet die Schleife
	}
	console.log("Eingegebene Zahl: " + zahl);
}
```

✔ **Typische Anwendung von `break` in `while`-Schleifen:**  
- **Benutzereingaben verarbeiten** (z. B. Abbruchbedingung `0` oder `"exit"`).  
- **Datenbanken durchsuchen** (z. B. Beenden der Suche, wenn ein Treffer gefunden wird).  


### **3️⃣ `continue`: Den aktuellen Durchlauf überspringen**  

 **🔹 Beispiel 1: `continue` in einer `for`-Schleife**  
Gib alle Zahlen von `1` bis `10` aus, aber überspringe `5`:  

```js
for (let i = 1; i <= 10; i++) {
	if (i === 5) {
		continue; // Überspringt nur diesen einen Durchlauf
	}
	console.log(i);
}
```

🔍 **Erwartete Ausgabe:**  
```
1  
2  
3  
4  
6  
7  
8  
9  
10
```
**🚀 Was passiert hier?**  
1. Wenn `i === 5`, wird `continue` ausgeführt.  
2. Der `console.log(i);` wird für `i = 5` **nicht** ausgeführt.  
3. Die Schleife fährt mit `i = 6` fort.  

✔ **Warum `continue` nutzen?**  
- Um **unerwünschte Werte** zu ignorieren (z. B. **Nur gerade Zahlen drucken**, nur bestimmte Benutzergruppen filtern).  


**🔹 Beispiel 2: `continue` in einer `while`-Schleife**  
Gib nur gerade Zahlen zwischen `1` und `10` aus:  

```js
let i = 0;
while (i < 10) {
	i++;
	if (i % 2 !== 0) {
		continue; // Überspringt ungerade Zahlen
	}
	console.log(i);
}
```

🔍 **Erwartete Ausgabe:**  
```
2  
4  
6  
8  
10
```

✔ **Typische Anwendung von `continue` in `while`-Schleifen:**  
- Nur bestimmte Daten verarbeiten (z. B. keine negativen Werte verarbeiten).  
- Bedingungen für die Verarbeitung von Daten definieren (z. B. nur gerade Zahlen verarbeiten).  

---

### 4️⃣ Kombination von `break` und `continue`  

Man kann **`break` und `continue` in einer Schleife kombinieren**, um präzisere Steuerung zu haben.  

**🔹 Beispiel 1: Suche in einem Array mit `break` und `continue`**  
Wir haben eine Liste von Namen. Wir möchten:  
- Nur Namen mit mehr als 5 Buchstaben ausgeben.  
- Falls der Name „Chris“ kommt, die Suche sofort abbrechen.  

```js
const namen = ["Anna", "Robert", "Chris", "Julia", "Tom"];

for (let i = 0; i < namen.length; i++) {
	if (namen[i] === "Chris") {
		console.log("Suche beendet!");
		break; // Stoppt die Schleife
	}

	if (namen[i].length <= 5) {
		continue; // Überspringt Namen mit weniger als 6 Buchstaben
	}

	console.log(namen[i]); // Wird nur ausgeführt, wenn der Name länger als 5 Zeichen ist
}
```

🔍 **Erwartete Ausgabe:**  
```
Robert  
Suche beendet!
```

✔ **Warum ist das praktisch?**  
- Daten filtern (`continue`), aber gleichzeitig die Suche frühzeitig abbrechen (`break`).  



### 5️⃣ Fazit & Best Practices  

| `break` | `continue` |
|--------------|----------------|
| Beendet die Schleife vollständig. | Überspringt nur den aktuellen Durchlauf. |
| Nützlich, wenn man nicht weiter iterieren will. | Nützlich, wenn bestimmte Werte ignoriert werden sollen. |
| **Typisches Beispiel**: Suche beenden, wenn ein Wert gefunden wurde. | **Typisches Beispiel**: Nur bestimmte Werte in einer Liste ausgeben. |

**🚀 Best Practices für `break` und `continue`**
- Verwende `break`, wenn du sicher weißt, dass keine weiteren Iterationen nötig sind.  
- Nutze `continue`, wenn du bestimmte Werte überspringen willst, aber die Schleife fortsetzen möchtest.  
- Achte darauf, `break` nicht versehentlich in Schleifen zu nutzen, die eigentlich weiterlaufen sollten.  
- Setze `continue` bewusst ein, damit der Code nicht schwer verständlich wird.  



### 📌 Abschlussübung  
**Aufgabe:**
 Schreibe eine `for`-Schleife, die alle Zahlen von `1` bis `20` ausgibt, aber:  
1. `continue` verwendet, um Zahlen, die durch 3 teilbar sind, zu überspringen.  
2. `break` ausführt, wenn die Zahl `15` erreicht ist.  

🎯 **Erwartete Ausgabe:**  

```
1  
2  
4  
5  
7  
8  
10  
11  
13  
14  
```

**Lösung:**

```js
for(let i = 1; i <= 20; i++) {
	if (i >= 15) break;
	if (i % 3 == 0) continue;
	console.log(i);
}
```

**🔹 Warum funktioniert der Code so?**

1. `break` stoppt die Schleife komplett, sobald `i` 15 erreicht.
2. `continue` sorgt dafür, dass Zahlen wie 3, 6, 9, 12 nicht ausgegeben werden.
3. console.log(i) wird nur für die gewünschten Zahlen ausgeführt.

## Hier ist die **vierte Unterrichtsstunde** über **verschachtelte Schleifen** im Detail ausgearbeitet.  

---

## 🕓 Stunde 4: Verschachtelte Schleifen

### 🎯 Lernziele dieser Stunde
- Verstehen, was verschachtelte Schleifen sind und wann sie nützlich sind.  
- Die **Ausführungsreihenfolge** von verschachtelten Schleifen nachvollziehen.  
- Praktische Anwendungsfälle kennenlernen, z. B. für Tabellen oder Muster.  
- Optimierungen und Fallstricke vermeiden.  


### 🔹 1. Was sind verschachtelte Schleifen?
Eine **verschachtelte Schleife** ist eine Schleife, die sich innerhalb einer anderen Schleife befindet.  
Die innere Schleife wird **bei jedem Durchlauf der äußeren Schleife vollständig durchlaufen**.  

**📌 Beispiel 1: Ausgabe eines Zahlenrasters**
```js
for (let i = 1; i <= 3; i++) {  // Äußere Schleife
  for (let j = 1; j <= 3; j++) {  // Innere Schleife
    console.log(`i = ${i}, j = ${j}`);
  }
}
```
🔍 **Erwartete Ausgabe:**
```
i = 1, j = 1
i = 1, j = 2
i = 1, j = 3
i = 2, j = 1
i = 2, j = 2
i = 2, j = 3
i = 3, j = 1
i = 3, j = 2
i = 3, j = 3
```

💡 **Erklärung:**  
- Die **äußere Schleife** läuft von `1` bis `3`.  
- Bei **jedem Durchlauf** der äußeren Schleife startet die **innere Schleife** von `1` bis `3`.  
- Das bedeutet, dass die **innere Schleife 3-mal für jede äußere Iteration durchläuft**, also insgesamt `3 × 3 = 9` Iterationen.


## 🔹 2. Anwendung: Erstellung einer Multiplikationstabelle
Eine häufige Anwendung für verschachtelte Schleifen ist die Erstellung einer **Multiplikationstabelle**.

**📌 Beispiel 2: 10er-Multiplikationstabelle**
```js
for (let i = 1; i <= 10; i++) {
  let row = ""; // Hier speichern wir die Zeile als String
  for (let j = 1; j <= 10; j++) {
    row += (i * j).toString().padStart(4, " "); // Formatierung für bessere Lesbarkeit
  }
  console.log(row);
}
```
🔍 **Erwartete Ausgabe:**
```
   1   2   3   4   5   6   7   8   9  10
   2   4   6   8  10  12  14  16  18  20
   3   6   9  12  15  18  21  24  27  30
   ...
```

💡 **Erklärung:**  
- Die äußere Schleife **wechselt die Zeile** (z. B. `i = 1, i = 2, ...` für jede Reihe der Tabelle).  
- Die innere Schleife berechnet **jeden Wert der aktuellen Zeile** (`i * j`).  
- Wir nutzen **`padStart(4, " ")`**, um alle Zahlen **gleichmäßig zu formatieren**.  


### 🔹 3. Zeichnen von Mustern mit verschachtelten Schleifen
Eine kreative Anwendung ist das Zeichnen von **Mustern** in der Konsole.

**📌 Beispiel 3: Ausgabe eines Sternmusters**
```js
for (let i = 1; i <= 5; i++) {
  let stars = "";
  for (let j = 1; j <= i; j++) {
    stars += "* ";
  }
  console.log(stars);
}
```
🔍 **Erwartete Ausgabe:**
```
* 
* * 
* * * 
* * * * 
* * * * * 
```

💡 **Erklärung:**  
- Die äußere Schleife bestimmt die **Anzahl der Zeilen** (`i` läuft von `1` bis `5`).  
- Die innere Schleife fügt **pro Zeile mehr Sterne hinzu** (`j` läuft bis `i`).  
- Ergebnis: Ein **dreieckiges Sternmuster**.

🔹 **Challenge für Schüler:**  
**Wie würde man das Muster umgedreht darstellen?** 🤔


## 🔹 4. Häufige Probleme & Optimierungstipps
**❌ 1. Endlosschleife durch falsche Bedingungen**
Falls eine Schleifenvariable **nicht korrekt verändert** wird, kann die Schleife unendlich lange laufen!

**Fehlerhaftes Beispiel:**  
```js
for (let i = 0; i < 3; i++) {
  for (let j = 0; j < 3; ) { // j wird nie verändert! 😱
    console.log(`i = ${i}, j = ${j}`);
  }
}
```
✅ **Lösung:**  
Stelle sicher, dass `j` **innerhalb der Schleife** verändert wird!
```js
for (let i = 0; i < 3; i++) {
  for (let j = 0; j < 3; j++ ) { // j wird nie verändert! 😱
    console.log(`i = ${i}, j = ${j}`);
  }
}
```
---

### ✅ 2. Performance-Tipp: Innere Schleife abhängig von der äußeren Schleife begrenzen
Falls eine Schleife unnötig oft läuft, kann das **Leistungsprobleme** verursachen.

**Besseres Beispiel:**  
```js
for (let i = 0; i < 5; i++) {
  for (let j = 0; j < i; j++) {  // Reduziert die Anzahl der Durchläufe
    console.log(`i = ${i}, j = ${j}`);
  }
}
```
Hier läuft die innere Schleife **weniger oft** als in einer klassischen `i x j`-Schleife.

---

### 🔹 5. Praxisaufgabe für Schüler (Hands-on)
**📝 Aufgabe: Erstelle eine "Schachbrett"-Tabelle mit # und leerem Feld**

**Anforderung:**  
- Nutze eine verschachtelte Schleife, um eine **8×8 Schachbrett-Darstellung** auszugeben.  
- Nutze `#` für dunkle Felder und `" "` für helle Felder.  
- Tipp: Die Farbe wechselt abwechselnd pro Spalte & Zeile.  

🔹 **Beispielausgabe für ein 8×8-Feld:**
```
# # # # # # # # 
# # # # # # # # 
# # # # # # # # 
# # # # # # # #
```
✅ **Lösungsvorschlag:**
```js
for (let i = 0; i < 8; i++) {
  let row = "";
  for (let j = 0; j < 8; j++) {
    if ((i + j) % 2 === 0) {
      row += "# ";
    } else {
      row += "  ";
    }
  }
  console.log(row);
}
```


### 🚀 Fazit der 4. Stunde
✅ **Heute gelernt:**  
- Was verschachtelte Schleifen sind & wie sie funktionieren.  
- Wie sie für praktische Anwendungen (Multiplikationstabelle, Muster) genutzt werden.  
- Welche Fehler vermieden werden sollten.  
- Wie man sie effizient optimieren kann.  

Hier ist die **fünfte Unterrichtsstunde** über **effiziente Schleifen und Performance-Optimierung** im Detail ausgearbeitet.  



# 🕓 Stunde 5: Effiziente Nutzung von Schleifen & Vermeidung von Endlosschleifen

### 🎯 Lernziele dieser Stunde

- **Verstehen**, wie Schleifen effizient genutzt werden können.  
- **Lernen**, wie man unnötige Berechnungen vermeidet und die Performance verbessert.  
- **Vermeiden** von Endlosschleifen und ineffizienten Konstruktionen.  
- **Unterschiede zwischen verschiedenen Schleifenarten** in Bezug auf Leistung.  
- **Best Practices** zur Optimierung von Schleifen.  


### 🔹 1. Warum ist die Optimierung von Schleifen wichtig?
Schleifen sind ein leistungsfähiges Werkzeug in JavaScript, aber **ineffiziente Schleifen** können:
- den Code **langsamer** machen,  
- den Browser einfrieren lassen (bei zu vielen Durchläufen),  
- unnötige Berechnungen ausführen.  

**❌ Beispiel für eine ineffiziente Schleife**
```js
for (let i = 0; i < arr.length; i++) { 
	console.log(arr[i]);  
}
```

**Problem:**  
Bei **jedem Durchlauf** wird `arr.length` **neu berechnet**, was bei großen Arrays teuer ist.

✅ **Optimierte Version:**
```js
const length = arr.length;  // Länge nur einmal berechnen
for (let i = 0; i < length; i++) { 
	console.log(arr[i]);  
}
```

📌 **Warum ist das besser?**  
- `arr.length` wird nur **einmal** gespeichert → **schnellere Ausführung!**  


### 🔹 2. Endlosschleifen erkennen & vermeiden
Eine **Endlosschleife** läuft unendlich lange und kann den Browser zum Absturz bringen.  

**❌ Beispiel für eine Endlosschleife mit `while`**
```js
let i = 0;
while (i < 5) {
	console.log(i);
	// i wird NICHT erhöht! Endlosschleife 😱
}
```

✅ **Lösung:**  
```js
let i = 0;
while (i < 5) {
	console.log(i);
	i++;  // i erhöhen, damit die Schleife endet!
}
```

📌 **Regel:**  
Immer sicherstellen, dass die **Schleifenbedingung irgendwann `false` wird**!

---

### 🔹 3. Vergleich: `for` vs. `while` vs. `do...while` – Wann sollte man welche nutzen?

| Schleifenart | Wann verwenden? | Besonderheit |
|-------------|----------------|--------------|
| `for` | Wenn die Anzahl der Durchläufe **bekannt** ist | Ideal für Zählvorgänge |
| `while` | Wenn die Anzahl der Durchläufe **nicht bekannt** ist | Läuft, solange Bedingung `true` ist |
| `do...while` | Wenn der Code **mindestens einmal** ausgeführt werden soll | Erst ausführen, dann Bedingung prüfen |

**📌 Beispiel für eine `do...while`-Schleife**
```js
let i = 10;
do {
	console.log(i);
	i++;
} while (i < 5);
```
**Ausgabe:** `10`  

📌 **Warum?** → Der Code wird **mindestens einmal** ausgeführt, obwohl die Bedingung `false` ist.

### 🔹 4. Best Practices zur Optimierung von Schleifen

#### ✅ 1. Verwenden von `break` und `continue` zur Effizienzsteigerung

**❌ Beispiel ohne `break` (ineffizient)**
```js
for (let i = 0; i < 1000; i++) {
	if (i === 10) {
		console.log("Gefunden!");
	}
}
```
Hier wird **die Schleife bis 1000 durchlaufen**, obwohl das gesuchte Element **bei 10 gefunden wurde**.

✅ **Optimierung mit `break`:**
```js
for (let i = 0; i < 1000; i++) {
	if (i === 10) {
		console.log("Gefunden!");
		break;  // Schleife sofort beenden!
	}
}
```
📌 **Vorteil:** Die Schleife **hört sofort auf**, sobald das Element gefunden wurde.  

#### ✅ 2. Effizientes Traversieren von Arrays

**❌ Klassische `for`-Schleife (bei großen Arrays langsam)**
```js
const numbers = [10, 20, 30, 40, 50];

for (let i = 0; i < numbers.length; i++) {
	console.log(numbers[i]);
}
```
✅ **Bessere Alternativen:**
```js
// 🔹 Mit for...of (lesbarer)
for (const num of numbers) {
	console.log(num);
}

// 🔹 Mit forEach (funktionaler Ansatz)
numbers.forEach(num => console.log(num));
```
📌 **Vorteil:**  
- `for...of` ist **kürzer und lesbarer**.  
- `forEach` ist **sehr klar und funktional**, aber nicht für `break` geeignet.  

#### ✅ 3. Verschachtelte Schleifen vermeiden, wenn möglich
Wenn möglich, sollte man **doppelte Schleifen vermeiden**, da sie **exponentiell langsamer** sind.

**❌ Ineffiziente doppelte Schleife**
```js
for (let i = 0; i < users.length; i++) {
	for (let j = 0; j < posts.length; j++) {
		if (users[i].id === posts[j].userId) {
			console.log(users[i].name + " hat einen Post geschrieben!");
		}
	}
}
```

✅ **Bessere Lösung mit `Map` für schnelles Lookup:**
```js
const postMap = new Map();
posts.forEach(post => postMap.set(post.userId, post));

users.forEach(user => {
	if (postMap.has(user.id)) {
		console.log(user.name + " hat einen Post geschrieben!");
	}
});
```

📌 **Warum ist das besser?**  
- **Statt `O(n²)`, nur `O(n)` Laufzeit** → 🚀 **wesentlich schneller!**  

### 🔹 5. Praxisaufgabe für Schüler (Hands-on)

**📝 Aufgabe: Filtere Zahlen effizient**

1. Erstelle ein Array mit **100 zufälligen Zahlen** zwischen 1 und 1000.
2. Finde die **ersten 5 Zahlen**, die durch `7` teilbar sind.
3. Nutze eine **effiziente Schleife mit `break`**.

**Beispielcode zum Starten:**
```js
const numbers = Array.from({ length: 100 }, () => Math.floor(Math.random() * 1000) + 1);

const divisibleBySeven = [];
for (let num of numbers) {
	if (num % 7 === 0) {
		divisibleBySeven.push(num);
		if (divisibleBySeven.length === 5) {
			break;  // Sofort beenden, wenn 5 Zahlen gefunden wurden!
		}
	}
}

console.log(divisibleBySeven);
```

📌 **Erwartete Ausgabe:**  
`[14, 49, 77, 700, 203]` (Beispielwerte)


### 🚀 Fazit der 5. Stunde
✅ **Heute gelernt:**  
✔ Warum effiziente Schleifen wichtig sind.  
✔ Wie man Endlosschleifen vermeidet.  
✔ Wann `for`, `while` oder `do...while` am besten genutzt wird.  
✔ Optimierungstipps: `break`, `Map`, `forEach` & Co.  
✔ Praktische Anwendung mit einer effizienten Filterung.  

### 🎯 **Nächster Schritt:**  
👉 **Bonusaufgabe:**  
Hier ist die **Lösung für die Bonusaufgabe**, um den größten gemeinsamen Teiler (**ggT**) zweier Zahlen mithilfe einer Schleife zu berechnen:  


**Lösung mit einer `while`-Schleife (Euklidischer Algorithmus)**
```js
function ggT(a, b) {
	while (b !== 0) {
		let temp = b;
		b = a % b;
		a = temp;
	}
	return a;
}

// Testfälle
console.log(ggT(48, 18)); // ➝ 6
console.log(ggT(101, 103)); // ➝ 1 (weil prim)
console.log(ggT(56, 98)); // ➝ 14
```
📌 **Erklärung:**  
1. Solange `b` nicht `0` ist, wird der Rest `a % b` berechnet.  
2. `a` nimmt den alten Wert von `b` an, `b` den Rest.  
3. Sobald `b === 0`, ist `a` der größte gemeinsame Teiler.  


**Alternative Lösung mit einer `for`-Schleife**
```js
function ggTFor(a, b) {
	let min = Math.min(a, b);
	let result = 1;

	for (let i = 1; i <= min; i++) {
		if (a % i === 0 && b % i === 0) {
			result = i; // ggT aktualisieren
		}
	}
	return result;
}

// Testfälle
console.log(ggTFor(48, 18)); // ➝ 6
console.log(ggTFor(101, 103)); // ➝ 1
console.log(ggTFor(56, 98)); // ➝ 14
```
📌 **Warum ist die `while`-Version besser?**  
✅ **Schneller:** Euklidischer Algorithmus ist `O(log n)`, die `for`-Variante ist `O(n)`.  
✅ **Weniger Iterationen:** Während die `for`-Schleife alle Zahlen bis `min(a, b)` durchgeht, reduziert die `while`-Schleife die Zahlen schnell.  
