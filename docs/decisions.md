# Grundlagen und Entscheidungen

Stand: 06.11.2026. Offene Punkte verhindern die Dokumentation nicht; sie werden vor dem jeweils abhängigen Konstruktionsschritt entschieden.

## Gesicherte Grundlagen

| ID | Grundlage | Herkunft |
| --- | --- | --- |
| G-01 | Ein Kameradolly mit 3D-druckbaren Bauteilen soll konstruiert werden. | Nutzerauftrag zum 3D-Druck-Kameradolly |
| G-02 | Das Startprojekt enthält README, CAD-/Druckstruktur und eine erste Spezifikation für Schiene, Wagen, Antrieb und Kameraaufnahme. | Aktueller Nutzerauftrag |

## Offene Entscheidungen

| ID | Entscheidung | Benötigte Eingabe | Vor diesem Schritt klären |
| --- | --- | --- | --- |
| D-01 | Lastfall | Kamerasystem, Gesamtmasse, Schwerpunkt, Einsatzlage | Tragende Geometrie dimensionieren |
| D-02 | Fahrweg und Abstützung | Nutzbarer Weg, Platz, Unterbau | Schiene und Wagen layouten |
| D-03 | Fertigungsrahmen | Drucker/Verfahren, Bauraum, Material, verfügbare Kaufteile, Budget | Führung wählen und Teile aufteilen |
| D-04 | Führungssystem | D-01 bis D-03 | Schiene/Wagen detaillieren |
| D-05 | Antriebskonzept | Manuell/motorisiert, Aufnahmebetrieb, Fahrverhalten | Antrieb dimensionieren |
| D-06 | Kameraanschluss | Tatsächlicher Kopf/Adapter, Anschlussmaße | Kameraaufnahme detaillieren |
| D-07 | CAD-System | Verfügbares Werkzeug und gewünschtes natives Format | Erstes editierbares Modell anlegen |
| D-08 | Prüfkriterien | Lastfall und geforderte Qualität der Kamerafahrt | Prototyp belasten / freigeben |

## Arbeitskonventionen dieses Startprojekts

Die Dateistruktur, Kennungen und Einheiten sind organisatorische Vorschläge. Sie enthalten keine Festlegung auf eine Schienenart, Rollen, Motoren, Gewinde oder einen Kunststoff. Ein früherer Tischdolly-Vorschlag ist kein freigegebener Schienenentwurf; seine Werte werden nicht stillschweigend übernommen.

## Eintrag für spätere Entscheidungen

Für jede Entscheidung ergänzen: ID, Datum, gewählte Lösung, Grundlage/Messung, betroffene Parameter und Schnittstellen, Modellrevision und noch ausstehender Nachweis. Einen Vorschlag erst nach ausdrücklicher Entscheidung als festgelegt kennzeichnen.
