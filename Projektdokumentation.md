# Projekt-Dokumentation



Filip Mitrovic, Lennard Bühler, Raul Gilardoni und Filip Kritzner

| Datum | Version | Zusammenfassung                                              |
| ----- | ------- | ------------------------------------------------------------ |
|   15.09.2023    | 0.0.1   | Die Gruppe hat sich intensiv mit Unity auseinandergesetzt, sowohl durch YouTube-Tutorials als auch mithilfe von Online-Ressourcen, und bereits einige Funktionen erfolgreich implementiert.|
|  22.09.2023  | 0.0.2   | Die Gruppe hat mit Unity experimentiert, um zu erkunden, welche Möglichkeiten es bietet, und zusätzliche kleine Funktionen in das Spiel integriert.                                   |
|  27.10.2023  | 0.0.3   | Die Gruppe hat grosse Fortschritte beim Spiel gemacht.                                |
|  03.11.2023  | 1.0.0   | Spiel ist fertig und spielbar.                           |

## 1 Informieren

### 1.1 Ihr Projekt

In unserem Unity-Spiel handelt es sich um ein Run-and-Shoot-Spiel, bei dem der Spieler von einem Zombie gejagt wird und versuchen muss, ihm zu entkommen. Auf dem Weg begegnen dem Spieler 
kontinuierlich lebende Kugeln, die zerstört werden müssen. Durch das Zerstören dieser Kugeln wird die Waffenstärke des Spielers erhöht, was das Zerstören der Kugeln beschleunigt. Wir wollen außerdem
auch Animationen und Soundeffekte hinzufügen, 
um das Spielerlebnis zu verbessern. Das Spiel ist in 3D gestaltet und endet mit einem Endboss-Kampf, den der Spieler besiegen muss, um die Runde zu gewinnen.




### 1.2 User Stories

| US-№ | Verbindlichkeit | Typ  | Beschreibung                       |
| ---- | --------------- | ---- | ---------------------------------- |
| 1    |       muss         |   funktional   | Als Spieler möchte ich in der Lage sein, mich zu bewegen, um dem Zombie zu entkommen. |
| 2  |          muss       |  funktional    |   Als Spieler möchte ich die Fähigkeit haben, meine Waffe abzufeuern, um die Kugeln zu zerstören.                                 |
|3|          kann       |   funktional   |   Als Spieler möchte ich die Option haben, die Schwierigkeit des Spiels auszuwählen, um die Herausforderung anzupassen.                                   |
|  4 |          muss       |  funktional    |    Als Spieler möchte ich, dass die Waffe an Stärke gewinnt, wenn ich Kugeln zerstöre, damit ich den Endboss umbringen kann und die Runde gewinne.                             |
| 5  |          kann       |  funktional    |     Als Spieler möchte ich die Möglichkeit haben, meine Waffe zu verbessern, um die Kugeln schneller zu zerstören.                           |
| 6 |          kann       |    funktional  |    Als Spieler möchte ich Animationen für Bewegungen und Aktionen im Spiel haben, um die Immersion zu steigern.                             |
| 7  |          kann       |  funktional    |      Als Spieler möchte ich Soundeffekte im Spiel haben, um die Spielatmosphäre zu verbessern.                               |
| 8  |          kann       |  funktional    |     Als Spieler möchte ich visuelle Effekte im Spiel haben, um die Spielszenen dynamischer zu gestalten.                             |
| 9 |          muss       |   funktional   |      Als Spieler möchte ich das Spiel in 3D erleben, um ein immersiveres Spielerlebnis zu haben.                              |
| 10 |          muss       |   funktional   |   Als Spieler möchte ich einen Endboss-Gegner am Ende des Spiels besiegen müssen, um die Runde zu gewinnen.                           |
| 11 |          kann       |   funktional   |   Als Spieler möchte ich Belohnungen für das Zerstören von Kugeln erhalten, um meine Spielfortschritte zu steigern. (Sowie Münzen erhalten)                                 |
| 12 |       kann         |   funktional   |  Als Spieler möchte ich verschiedene Spielmodi zur Auswahl haben, um das Spiel abwechslungsreicher zu gestalten.  |
|13  |kann|funktional|Als Spieler möchte ich, dass sich die Umgebung im Spiel verändert, um unterschiedliche Herausforderungen und Strategien zu bieten. |



### 1.3 Testfälle

| TC-№ | Ausgangslage | Eingabe | Erwartete Ausgabe |
| ---- | ------------ | ------- | ----------------- |
| 1.1  | Spiel gestartet, Spieler bewegt sich | Spieler bewegt sich in eine Richtung | Spieler bewegt sich in die ausgewählte Richtung. |
| 1.2  | Spiel gestartet, Spieler bewegt sich | Spieler bewegt sich rückwärts | Spieler bewegt sich rückwärts. |
| 2.1  | Spieler im Spiel, Waffe bereit | Spieler feuert Waffe ab | Die Kugel wird abgefeuert und zerstört Hindernisse. |
| 3.1  | Spiel gestartet, Schwierigkeitsauswahl | Spieler wählt leichte Schwierigkeitsstufe | Das Spiel wird einfacher. |
| 3.2  | Spiel gestartet, Schwierigkeitsauswahl | Spieler wählt schwere Schwierigkeitsstufe | Das Spiel wird schwieriger. |
| 4.1  | Spieler zerstört Kugeln | Spieler zerstört eine Kugel | Die Waffe wird stärker. |
| 4.2  | Spieler zerstört Kugeln | Spieler zerstört mehrere Kugeln | Die Waffe wird deutlich stärker. |
| 5.1  | Spieler im Spiel, Verbesserung verfügbar | Spieler verbessert die Waffe | Die Waffe wird schneller. |
| 6.1  | Spieler im Spiel, Animationen aktiviert | Spieler führt eine Bewegung aus | Die Animation der Bewegung wird abgespielt. |
| 7.1  | Spieler im Spiel, Soundeffekte aktiviert | Spieler erzielt Treffer | Ein Soundeffekt wird abgespielt. |
| 8.1  | Spieler im Spiel, visuelle Effekte aktiviert | Spieler erzielt Treffer | Ein visueller Effekt wird angezeigt. |
| 9.1  | Spiel im 3D-Modus gestartet | Spieler bewegt sich im Spiel | Das Spiel wird in 3D dargestellt. |
| 10.1 | Spieler im Endboss-Kampf | Spieler besiegt den Endboss | Die Runde wird gewonnen. |
| 11.1 | Spieler zerstört Kugeln | Spieler erhält Belohnung (Münzen) | Die Belohnung wird dem Spieler gutgeschrieben. |
| 12.1 | Spieler wählt Spielmodus | Spieler wählt einen anderen Spielmodus | Das Spiel wechselt in den ausgewählten Spielmodus. |
| 13.1 | Spieler im Spiel, Umgebung verändert sich | Spieler passt Strategie an | Die Umgebung ändert sich entsprechend. |


### 1.4 Diagramme



![924dae60-2eab-43b0-a392-333a483ad6c2](https://github.com/cornhub-57/UnityGame/assets/110892641/c9fa1c00-57be-4414-8faf-e33d15655cb7)


## 2 Planen



| AP-№ | Zuständig          | Beschreibung                                            | Geplante Zeit |
| ---- | ------------------ | ------------------------------------------------------- | ------------- |
| 1.1  | Filip Mitrovic     | Implementierung der Spielerbewegung                    | 60 Min        |
| 1.2  | Raul Gilardoni    | Implementierung der Zombie-Verfolgungslogik            | 60 Min        |
| 1.3  | Filip Mitrovic     | Implementierung der Spieler-Kollisionserkennung        | 60 Min        |
| 2.1  | Raul Gilardoni | Implementierung der Waffensteuerung                | 60 Min        |
| 2.2  | Lennard Bühler | Implementierung des Kugelabfeuerns                 | 60 Min        |
| 2.3  | Lennard Bühler | Implementierung der Kugelzerstörung                | 60 Min        |
| 2.4  | Filip Kritzner | Implementierung der Munitionsverwaltung            | 60 Min        |
| 2.5  | Filip Mitrovic  | Implementierung der Nachlade-Mechanik              | 60 Min        |
| 3.1  | Raul Gilardoni | Implementierung der Waffenstärke-Verbesserung      | 60 Min        |
| 3.2  |  Filip Mitrovic  | Implementierung der Waffenverbesserungsmechanik    | 60 Min        |
| 3.3  | Lennard Bühler | Implementierung von Power-ups                      | 60 Min        |
| 4.1  | Filip Kritzner | Implementierung von Bewegungsanimationen           | 60 Min        |
| 4.2  | Filip Mitrovic  | Implementierung von Aktionsanimationen             | 60 Min        |
| 4.3  | Lennard Bühler | Implementierung von Tod- und Siegesanimationen     | 60 Min        |
| 5.1  | Filip Kritzner | Implementierung von Soundeffekten                 | 60 Min        |
| 5.2  | Filip Kritzner | Implementierung von visuellen Effekten            | 60 Min        |
| 5.3  | Filip Kritzner | Implementierung von Umgebungsgeräuschen           | 60 Min        |
| 6.1  | Raul Gilardoni | Implementierung des 3D-Spielerlebnisses           | 60 Min        |
| 6.2  | Raul Gilardoni | Implementierung von Umgebungsdetails             | 60 Min        |
| 7.1  | Lennard Bühler | Implementierung des Endboss-Gegners               | 60 Min        |
| 7.2  | Filip Kritzner | Implementierung des Endboss-Kampfmechanik          | 60 Min        |
| 8.1  |Lennard Bühler | Implementierung von Belohnungen für Kugelzerstörung| 60 Min        |
| 8.2  | Filip Mitrovic  | Implementierung von Belohnungen für Endboss-Sieg   | 60 Min        |
| 9.1  | Filip Kritzner | Implementierung verschiedener Spielmodi           | 60 Min        |
| 9.2  | Filip Mitrovic | Implementierung von Koop- und Mehrspielermodi     | 60 Min        |
| 10.1 | Lennard Bühler | Implementierung von Umgebungsveränderungen         | 60 Min        |
| 10.2 | Filip Kritzner | Implementierung von Tages- und Nachtzyklus         | 60 Min       |




## 3 Entscheiden

Unsere Gruppe hat sich aus strategischen Gründen für die Entwicklung dieses Spiels und die Nutzung von Unity entschieden. Die Spielidee verspricht ein breites Spielerlebnis, das sowohl Gelegenheitsspieler als auch erfahrene Gamer anspricht.
Unity bietet eine starke Entwickler-Community und vielseitige Plattformunterstützung für die Umsetzung unserer Vision.
Die Effizienz von Unity verkürzt die Entwicklungszeit, während verschiedene Lizenzierungsmodelle unsere Ressourcen schonen.
Diese Entscheidung ermöglicht es uns, ein unterhaltsames Spielprojekt zu realisieren.



## 4 Realisieren

| AP-№ | Datum       | Zuständig        | Geplante Zeit | Tatsächliche Zeit |
| ---- | ----------- | ---------------- | ------------- | ------------------ |
| 1.1  | 22.09.2023  | Filip Mitrovic   | 60 Min        |65 Min|
| 1.2  | 22.09.2023  | Raul Gilardoni   | 60 Min        | 70 Min                 |
| 1.3  | 22.09.2023  | Filip Mitrovic   | 60 Min        |        45 Min          |
| 2.1  | 22.09.2023  | Raul Gilardoni   | 60 Min        |     60 Min             |
| 2.2  | 22.09.2023  | Lennard Bühler   | 60 Min        |      65 Min            |
| 2.3  | 22.09.2023  | Lennard Bühler   | 60 Min        |   55 Min               |
| 2.4  | 22.09.2023  | Filip Kritzner   | 60 Min        |   50 Min               |
| 2.5  | 22.09.2023  | Filip Mitrovic   | 60 Min        |    75 Min              |
| 3.1  | 22.09.2023  | Raul Gilardoni   | 60 Min        |   60 Min               |
| 3.2  | 22.09.2023  | Filip Mitrovic   | 60 Min        |   85 Min               |
| 3.3  | 22.09.2023  | Lennard Bühler   | 60 Min        |   80 Min               |
| 4.1  | 22.09.2023  | Filip Kritzner   | 60 Min        |  40 Min                |
| 4.2  | 22.09.2023  | Filip Mitrovic   | 60 Min        |  45 Min                |
| 4.3  | 22.09.2023  | Lennard Bühler   | 60 Min        |  65 Min                |
| 5.1  | 22.09.2023  | Filip Kritzner   | 60 Min        |  70 Min                |
| 5.2  | 22.09.2023  | Filip Kritzner   | 60 Min        |  50 Min                |
| 5.3  | 22.09.2023  | Filip Kritzner   | 60 Min        |  55 Min                |
| 6.1  | 22.09.2023  | Raul Gilardoni   | 60 Min        |        60 Min          |
| 6.2  | 22.09.2023  | Raul Gilardoni   | 60 Min        |   60 Min               |
| 7.1  | 22.09.2023  | Lennard Bühler   | 60 Min        |   60 Min               |
| 7.2  | 22.09.2023  | Filip Kritzner   | 60 Min        |    75 Min              |
| 8.1  | 22.09.2023  | Lennard Bühler   | 60 Min        |    110 Min              |
| 8.2  | 22.09.2023  | Filip Mitrovic   | 60 Min        |    60 Min              |
| 9.1  | 22.09.2023  | Filip Kritzner   | 60 Min        |  50 Min                |
| 9.2  | 22.09.2023  | Filip Mitrovic   | 60 Min        |  45 Min                |
| 10.1 | 22.09.2023  | Lennard Bühler   | 60 Min        |   50 Min               |
| 10.2 | 22.09.2023  | Filip Kritzner   | 60 Min        |  85 Min                |




## 5 Kontrollieren

### 5.1 Testprotokoll

| TC-№ | Datum       | Resultat       | Tester           |
| ---- | ----------- | -------------- | ---------------- |
| 1.1  | 22.09.2023  | Funktioniert   | Mitrovic+Kritzner |
| 1.2  | 22.09.2023  | Funktioniert   | Mitrovic+Kritzner |
| 2.1  | 22.09.2023  | Funktioniert   | Mitrovic+Kritzner |
| 3.1  | 22.09.2023  | Funktioniert   | Mitrovic+Kritzner |
| 3.2  | 22.09.2023  | Funktioniert   | Mitrovic+Kritzner |
| 4.1  | 22.09.2023  | Funktioniert   | Mitrovic+Kritzner |
| 4.2  | 22.09.2023  | Funktioniert   | Mitrovic+Kritzner |
| 5.1  | 22.09.2023  | Funktioniert   | Mitrovic+Kritzner |
| 6.1  | 22.09.2023  | Funktioniert nicht | Mitrovic+Kritzner |
| 7.1  | 22.09.2023  | Funktioniert   | Mitrovic+Kritzner |
| 8.1  | 22.09.2023  | Funktioniert   | Mitrovic+Kritzner |
| 9.1  | 22.09.2023  | Funktioniert   | Mitrovic+Kritzner |
| 10.1 | 22.09.2023  | Funktioniert   | Mitrovic+Kritzner |
| 11.1 | 22.09.2023  | Funktioniert   | Mitrovic+Kritzner |
| 12.1 | 22.09.2023  | Funktioniert nicht   | Mitrovic+Kritzner |
| 13.1 | 22.09.2023  | Funktioniert nicht   | Mitrovic+Kritzner |

`Fazit:`

Die wichtigsten Teile des Programmes sind mit Erfolg ausgegangen, somit ist unser Programm spielbar. Doch Leider konnten wir wegen geringer Zeit nicht alle unsere Wünsche für das Programm erfüllen.

## 6 Auswerten


