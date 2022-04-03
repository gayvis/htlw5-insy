# SMÜP: MongoDB

1.) Wie kann ich alle Dokumente der Collection dokumente, in denen das Feld a den Wert 2 besitzt und die id unterdrückt wird, ausgeben?

- [ ] `db.domumente.count({a:2},{_id: 0})`
- [ ] `db.domumente.find({a,2},{_id: 0})`
- [x] `db.domumente.find({a:2},{_id: false})`
- [ ] `db.domumente.show({a:2},{_id: 0})`
- [x] `db.domumente.find({a:2},{_id: 0})`
- [ ] `db.domumente.db.find({a:2},{_id: 0})`

2.) Wie starte ich einen Konfigurations-Server?

- [ ] mongos --config
- [ ] mongoc --configsvr
- [ ] mongos --configsvr
- [x] mongod --configsvr
- [ ] mongo --config
- [ ] mongod --config
- [ ] mongo --configsrv
- [ ] mongoc --config

3.) Welche Eigenschaften treffen auf MongoDB zu?

- [x] Eine RDBMS Attribut entspricht einem MongoDB Feld.
- [x] Eine RDBMS Tabelle entspricht einer MongoDB Collection.
- [ ] Ein RDBMS Tupel entspricht einem MongoDB Collection.
- [ ] Ein RDBMS Attribut eintspricht einem MongoDB Dokument
- [ ] Eine RDBMS Tabelle entspricht einem MongoDB Dokument.
- [ ] Ein RDBMS Dokument entspricht einem MongoDB Dokument.
- [x] Ein RDBMS Tupel entspricht einem MongoDB Dokument.

4.) Lösche alle Benutzer mit dem Status D

- [ ] `db.users.remove{status = "D"}`
- [ ] `db.users.remove{status {"eq: "D"}}`
- [ ] `db.users.delete{status {$eq: "D"}}`
- [x] `db.users.remove({status: "D"})`
- [ ] `db.users.remove({status is "D"})`
- [ ] `db.users.delete({status: "D"})`

5.) Wie starte ich den Serverprozess einer MongoDB?

- [ ] mongos
- [x] mongod
- [ ] mserver
- [ ] mongoserv
- [ ] server
- [ ] mongo

6.) Kreuze die vollständig richtigen Antworten, die für die Konfiguration eines großen DB-Systems mit MongoDB gelten sollen:

- [x] Man verwendet mehrere Shards, die ein ReplicaSet beinhalten sollen
- [ ] Ein ReplicaSet soll mehrere Shards beinhalten
- [x] Es soll mehrere Router geben.
- [ ] Es soll mehrere Router geben und jeder besteht aus einem ReplicaSet.
- [x] Ein ConfigServer besteht aus einem ReplicaSet.
- [ ] Ein Shard ist eine mongos Instanz.
- [ ] Ein Router soll aus mehreren ReplicaSets bestehen.

7.) Wie funktioniert die Kommunikation bei Verwendung von Sharding?

- [x] Der Router fragt den ConfigServer, welcher Shard die Anfrage bekommt.
- [ ] Der Shard kommuniziert direkt mit der Anwendung.
- [x] Der Router fasst die Antwort des Shards zusammen.
- [ ] Die Anwendung wendet sich an den ConfigServer mit der Anfrage.
- [x] Die Anwendung wendet sich an den Router mit der Anfrage.
- [ ] Der ConfigServer sendet an dne Router, der die Anfrage an den Shard weiterleitet.
- [ ] Der Router bestimmt, welcher Shard die Anfrage bekommt.
- [ ] Der ConfigServer fasst die Antwort zusammen.

8.) Welche Eigenschaften treffen auf NoSQL Datenbanken zu?

- [x] Weiche Konsistenz
- [ ] Ich kann es auf jede Problemstellung bestens anwenden
- [x] Viele gleichrangige Knoten
- [x] schwache Schemarestriktionen
- [x] Hohe Ausfallsicherheit
- [ ] Bedeutet "kein SQL"
- [ ] Alle Knoten haben immer zur selben Zeit die selben Daten.
- [ ] Man braucht sich überhaupt kein Schema zu überlegen.

9.) Kreuze die richtigen Anmerkungen über die interne Arbeitsweise des MongoDB Servers an.

- [x] Die Daten werden defaultmäßig im Sekundenbereich persistiert.
- [x] Die Operationen werden im Journal gespeichert.
- [ ] Das Journal wird in den RAM geschrieben, die Daten direkt auf die Disk.
- [x] Das Journal wird defaultmäßig im Millisekundenbreich persistiert.
- [ ] Das Journal wird direkt auf die Dissk geschrieben.
- [ ] Die Dokumente werden im Journal gespeichert.

10.) NoSQL Theorie: Kreuze die richtigen Antworten an:

- [x] BASE sagt aus, dass alle Knoten nicht immer denselben konsistenten Datenzustand haben.
- [x] Um mehr Durchsatz bei höherer Verfügbarkeit mit mehr Daten zu erreichen, sollte man zuerst vertikal, dann horizontal skalieren.
- [ ] Das CAP Theorem beinhaltet aus Konsistenz, Verfügbarkeit und Ausfalltoleranz. Bei verteilten Systemen mussen alle drei Eigenschaften erfüllt sein.
- [x] ACID besagt, dass nach einer Transaktion der Zustand der Datenbank immer konsistent sein muss.
- [ ] ACID sagt aus, dass nicht immer alle Knoten verfügbar sein müssen.

11.) Welche Kategorien von NoSQL Datenbanken gibt es?

- [x] Graphen
- [ ] Objektorientierte
- [x] Spaltenorientierte
- [ ] Objektrelationale
- [x] Dokumentenorientierte
- [ ] Datenbasierte
- [x] Key/Value
- [ ] Netzwerk

12.) Kreuze an, was auf den Shard-Schlüssel zutrifft.

- [ ] Bei einer Schlüssel-Mischform könnte der erste Teil aus einem Zeitstempel der Erzeugungszeit und der zweite Teil aus dem Usernamen bestehen.
- [x] Die Wahl hängt vom Verhältnis der Lese- und Schreiboperationen ab.
- [ ] Große Teile des Wertebereichs sollen ausgeschöpft werden.
- [x] Bei monoton steigenden Werten gibt es keine gute Performance bei Schreiboperationen.
- [ ] Hashwerte haben bei Bereichsabfragen bessere Performance als monoton steigende Werte.
