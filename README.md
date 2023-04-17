# pb-classes-pet :fox_face: 

## Pet Toy
Wir programmieren ein kleines "Spielzeug"-Tier

### 1. Pet Klasse
* erstelle eine **Pet** Klasse.
* Der Constructor soll folgende Parameter haben: **name**
* Die Klasse soll zwei weitere Felder haben: **happyness** und **hungry** (Jeweils mit dem Starwert 5)
* schreibe Methoden **addHappyness(value)**, **reduceHappyness(value)**, **addHunger(value)** und **reduceHunger(value)**, die den jeweiligen Wert
in das Objekt schreiben. Dabei sollen die Werte *happyness* und *hunger* nie weniger als 0 oder mehr als 10 sein. 

**Erstelle auch ein Objekt der Klasse Pet zum testen**
### 2. Pet Status
* erstelle ene Methode: **printStatus()**, die eine Meldung auf der Konsole ausgiebt:
    * *"[name] ist [mood] und hat ['hunger'/'keinen Hunger']"*
* Wobei *mood* =
    * wütend (0 <= happyness <= 2)
    * traurig (3 <= happyness <= 5)
    * froh (6 <= happyness <= 8)
    * über glücklich (9 <= happyness <= 10)

### 3. Food
* Erstelle eine Klasse **Food**.
* Die Klasse hat drei Parameter: **name**, **energy**, **sweet**

* erstelle ein paar *Food* Objekte: 
    * Apple (energy: 1, sweet: true)
    * Bread (energy: 3, sweet: false)

### 4. Feed and Play and Sleep
Füge zu der *Pet* Klasse drei neue Methoden hinzu
* **feed(food)**
    * Die Methode **feed** hat ein Parameter **food**, die ein Food Objekt bekommt.
    * Reduziere den Hunger(*hungry*) um den Wert von Energy (*hunger = hunger - energy*)
    * Wenn das Essen nicht Süß ist (*sweet*) ziehe 1 Punkt von *happyness* ab.
    * Gib eine Meldung auf der Konsole aus: *"[pet.name] hat [food.name] gegessen!"*
* **play()**
    * Die Methode **play** hat keine Parameter.
    * Wenn das Pet einen Hunger (*hungry*) von **mehr als 8** hat, brich die Methode ab und gib eine Meldung aus: *"[name] ist zu hungrig zum spielen"
    * Spielen macht das Pet glücklicher (*happyness +2*)
    * Beim Spielen wird das Pet wieder hungrieger (*hunger + 3*)
    * Gib eine Meldung auf der Konsole aus: *"[name] hat gespielt!"*
* **sleep()**
    * Die Methode **sleep** hat keine Parameter.
    * Reduziere *happyness* um 5 und erhöhe *hunger* um 2.
    * gib eine Meldung auf der Konsole aus: *"[name] hat geschlafen!"*

### 5. Action
Lass dein Pet etwas Spielen, Essen und Schlafen. 
Zwischendurch gib auch immer wieder mit printStatus() den status aus um zu sehen, wie es deinem Pet geht.
