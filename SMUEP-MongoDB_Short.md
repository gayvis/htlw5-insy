# SMÜP: MongoDB

1.) Wie kann ich alle Dokumente der Collection dokumente, in denen das Feld a den Wert 2 besitzt und die id unterdrückt wird, ausgeben?

- [x] `db.domumente.find({a:2},{_id: false})`
- [x] `db.domumente.find({a:2},{_id: 0})`

2.) Wie starte ich einen Konfigurations-Server?

- [x] mongod --configsvr

3.) Welche Eigenschaften treffen auf MongoDB zu?

- [x] Eine RDBMS Attribut entspricht einem MongoDB Feld.
- [x] Eine RDBMS Tabelle entspricht einer MongoDB Collection.
- [x] Ein RDBMS Tupel entspricht einem MongoDB Dokument.

4.) Lösche alle Benutzer mit dem Status D

- [x] `db.users.remove({status: "D"})`

5.) Wie starte ich den Serverprozess einer MongoDB?

- [x] mongod

6.) Kreuze die vollständig richtigen Antworten, die für die Konfiguration eines großen DB-Systems mit MongoDB gelten sollen:

- [x] Man verwendet mehrere Shards, die ein ReplicaSet beinhalten sollen
- [x] Es soll mehrere Router geben.
- [x] Ein ConfigServer besteht aus einem ReplicaSet.

7.) Wie funktioniert die Kommunikation bei Verwendung von Sharding?

- [x] Der Router fragt den ConfigServer, welcher Shard die Anfrage bekommt.
- [x] Der Router fasst die Antwort des Shards zusammen.
- [x] Die Anwendung wendet sich an den Router mit der Anfrage.

8.) Welche Eigenschaften treffen auf NoSQL Datenbanken zu?

- [x] Weiche Konsistenz
- [x] Viele gleichrangige Knoten
- [x] schwache Schemarestriktionen
- [x] Hohe Ausfallsicherheit

9.) Kreuze die richtigen Anmerkungen über die interne Arbeitsweise des MongoDB Servers an.

- [x] Die Daten werden defaultmäßig im Sekundenbereich persistiert.
- [x] Die Operationen werden im Journal gespeichert.
- [x] Das Journal wird defaultmäßig im Millisekundenbreich persistiert.

10.) NoSQL Theorie: Kreuze die richtigen Antworten an:

- [x] BASE sagt aus, dass alle Knoten nicht immer denselben konsistenten Datenzustand haben.
- [x] Um mehr Durchsatz bei höherer Verfügbarkeit mit mehr Daten zu erreichen, sollte man zuerst vertikal, dann horizontal skalieren.
- [x] ACID besagt, dass nach einer Transaktion der Zustand der Datenbank immer konsistent sein muss.

11.) Welche Kategorien von NoSQL Datenbanken gibt es?

- [x] Graphen
- [x] Spaltenorientierte
- [x] Dokumentenorientierte
- [x] Key/Value

12.) Kreuze an, was auf den Shard-Schlüssel zutrifft.

- [x] Die Wahl hängt vom Verhältnis der Lese- und Schreiboperationen ab.
- [x] Bei monoton steigenden Werten gibt es keine gute Performance bei Schreiboperationen.
