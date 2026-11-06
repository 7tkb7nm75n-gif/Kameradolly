# Kameradolly

Startprojekt zur Konstruktion eines Kameradollys mit 3D-druckbaren Bauteilen. Die aktuelle Planung gliedert das System in **Schiene, Wagen, Antrieb und Kameraaufnahme**.

**Stand: 06.11.2026 · Konzeptphase.** Es gibt noch keine geprüften CAD-Modelle, Druckdateien oder bestätigte Tragfähigkeit.

## Ziel und Randbedingungen

- Ein nachvollziehbar konstruiertes System für geführte Kamerafahrten entwickeln.
- CAD-Quellen, Austauschmodelle, Druckdateien und Prüfprotokolle getrennt versionieren.
- Bestätigt sind das 3D-Druck-Projekt und die hier angeforderte Baugruppengliederung.
- Kamera/Nutzlast, Fahrweg, Einbaulage, Drucker, Material, Führung und Antriebsart sind offen. Maße und Kaufteile werden erst nach Klärung der jeweiligen Schnittstellen festgelegt.
- 3D-Druck bedeutet keine Festlegung auf ausschließlich gedruckte Teile. Kaufteile werden bei der Auslegung gesondert erfasst.

## Orientierung

| Pfad | Inhalt |
| --- | --- |
| [docs/technical-specification.md](docs/technical-specification.md) | Vorläufige Anforderungen und Schnittstellen aller vier Baugruppen |
| [docs/decisions.md](docs/decisions.md) | Gesicherte Grundlagen und offene Entscheidungen |
| [docs/workflow.md](docs/workflow.md) | Schrittweise Anleitung vom Lastenblatt bis zum Prototyp |
| [cad/](cad/README.md) | Editierbare CAD-Quellen und Baugruppen |
| [exports/](exports/README.md) | CAD-Austauschdateien, später etwa STEP |
| [printing/](printing/README.md) | Druckteile, Druckprojekte und Einstellungsnachweise |
| [bom/](bom/README.md) | Stückliste für Druck- und Kaufteile |
| [validation/](validation/README.md) | Prüfplan und spätere Messprotokolle |

## So geht es los

1. [Arbeitsanleitung](docs/workflow.md) öffnen und die Eingangsdaten aufnehmen.
2. Mit diesen Daten [offene Entscheidungen](docs/decisions.md) aktualisieren.
3. Schiene und Wagen gemeinsam auslegen; danach Antrieb und Kameraaufnahme anbinden.
4. Zuerst eine Passprobe, dann einen Prototyp bauen und prüfen.

Die Dokumentation ist die Ausgangsbasis. Sie ist noch keine Bau- oder Druckfreigabe.
