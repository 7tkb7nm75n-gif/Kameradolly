# Technische Spezifikation – Entwurf 0.1

Stand: 06.11.2026. Status: vorläufige Entwicklungsanforderungen.

**Statuskonvention:** „bestätigt“ bezeichnet einen Auftrag aus dem vorhandenen Nutzerkontext; „Entwurfsziel“ einen hier formulierten technischen Vorschlag; „offen“ eine noch zu treffende Entscheidung. Kein Entwurfsziel ist bereits ein Prüfergebnis.

## 1. Grundlage und Systemgrenze

Bestätigt sind die Entwicklung eines 3D-Druck-Kameradollys und die Dokumentation der Baugruppen Schiene, Wagen, Antrieb und Kameraaufnahme. Noch nicht entschieden ist, welche Bauteile gedruckt und welche zugekauft werden.

Ein älterer Assistentenentwurf bezog sich auf einen Tischdolly. Dessen vorgeschlagene Maße, Rollen und Lastangaben sind nicht als Nutzerfreigaben belegt und werden hier nicht übernommen. Das frühere ZIP wurde für diesen Stand nicht inhaltlich verifiziert oder importiert.

## 2. Noch benötigte Auslegungsdaten

| Kennung | Größe / Entscheidung | Einheit bzw. Beschreibung | Status / benötigt vor |
| --- | --- | --- | --- |
| P-01 | Nutzlast | kg; Kamera, Objektiv, Kopf, Adapter und Zubehör zusammen | offen / Dimensionierung |
| P-02 | Lage des Lastschwerpunkts | mm relativ zur Aufnahme; auch ungünstige Kamerastellung | offen / Stabilitätsauslegung |
| P-03 | Nutzbarer Fahrweg | mm; von der gesamten Schienenlänge unterscheiden | offen / Schienenlayout |
| P-04 | Einsatzlage und Abstützung | horizontal, geneigt oder vertikal; Auflagepunkte | offen / Lastfälle und Führung |
| P-05 | Druckverfahren und Drucker | Bauraum X/Y/Z in mm; verfügbarer Prozess | offen / Teileaufteilung |
| P-06 | Druckmaterial | konkretes Material und Einsatzbedingungen | offen / Bauteilauslegung und Druckprofil |
| P-07 | Bedienung / Antrieb | manuell oder motorisiert; gewünschter Aufnahmebetrieb | offen / Antriebskonzept |
| P-08 | Fahrverhalten | Geschwindigkeit, Gleichmäßigkeit und ggf. Positioniergenauigkeit | offen / Antriebs- und Prüfauslegung |
| P-09 | Kameraanschluss | tatsächlich vorhandener Kopf, Platte oder Anschluss samt Maßen | offen / Aufnahmegeometrie |
| P-10 | Budget / vorhandene Teile | verfügbare Schienen, Lager, Befestiger, Motoren usw. | offen / Teileauswahl |

Es werden keine Zahlenwerte als Ersatz für fehlende Eingangsdaten eingesetzt.

## 3. Gemeinsame Arbeitskonventionen

Vorgeschlagene Konvention für neue Modelle: Längen in mm, Massen in kg; X entlang der Fahrt, Y quer zur Schiene, Z zur Kamera hin. Ursprung und Bezugsebenen werden mit dem ersten Layout eindeutig im CAD dokumentiert. Gewinde werden erst anhand des realen Gegenstücks spezifiziert; ein Durchmesser allein genügt dafür nicht.

Die tragende Verbindungskette lautet: Abstützung → Schiene → Führung → Wagen → Kameraaufnahme → Kamerasystem. Ein Antrieb wirkt zwischen feststehender Struktur und Wagen.

## 4. Schiene

**Funktion:** Den Wagen über den nutzbaren Fahrweg führen und Lasten an die Abstützung weitergeben.

**Entwurfsziele:**

- Führung, Abstützung und Endanschläge als zusammengehöriges System auslegen.
- Wagenbewegung über den gesamten Fahrweg ermöglichen; Baulänge für Wagen, Anschläge und gegebenenfalls Antrieb berücksichtigen.
- Bei einer geteilten Schiene die Ausrichtung und den Übergang an Verbindungsstellen prüfen.
- Führung und Lagerung passend zu Nutzlast, Schwerpunkt und Einsatzlage auswählen.

**Offen:** Profil bzw. Führungssystem, Werkstoff, Länge, Teilung, Auflageabstand, Anschlussmaße und zulässige Durchbiegung.

**Schnittstellen:** S-01 zum Wagen; S-02 zur Abstützung; S-03 zu Anschlägen und gegebenenfalls Antrieb.

**Späterer Nachweis:** Nutzbarer Fahrweg und Schienenverformung unter vereinbarter Prüflast messen; Übergänge gegebenenfalls mitprüfen.

## 5. Wagen

**Funktion:** Kameraaufnahme tragen und Kräfte sowie Kippmomente in die Führung einleiten.

**Entwurfsziele:**

- Führung mit definierter Einstellung von Spiel bzw. Vorspannung vorsehen, soweit das gewählte System dies benötigt.
- Rückhaltung gegen unbeabsichtigtes Abheben oder Ausfädeln für die gewählte Einsatzlage vorsehen.
- Befestiger, Lager und Einstellstellen für Montage und Wartung zugänglich halten.
- Freigängigkeit einschließlich Kameraüberhang, Kabeln und Antrieb über den ganzen Fahrweg prüfen.

**Offen:** Grundfläche, Lager-/Rollenanordnung, Spurweite, Befestiger, Eigenmasse und Fertigungstoleranzen.

**Schnittstellen:** S-01 zur Schiene; S-04 zum Antrieb; S-05 zur Kameraaufnahme.

**Späterer Nachweis:** Freier Lauf, Spiel, Kippverhalten, Rückhaltung und Verformung mit definierter Ersatzlast prüfen.

## 6. Antrieb

**Funktion:** Die gewünschte Kamerafahrt erzeugen; Halten oder Positionieren nur soweit der spätere Einsatzzweck dies fordert.

**Entwurfsziele:**

- Manuelle und motorisierte Ausführung zunächst als offene Alternativen führen.
- Erforderliche Vorschub- und gegebenenfalls Haltekraft aus Last, Einsatzlage und gemessenem Fahrwiderstand ableiten.
- Bei Motorisierung zusätzlich Übertragung, Versorgung, Bedienung, Kabelführung und Verhalten am Fahrwegende festlegen.
- Mechanische Endanschläge unabhängig von einer möglichen elektronischen Begrenzung berücksichtigen.

**Offen:** Antriebsprinzip, Übertragung, Kraft/Drehmoment, Geschwindigkeit, Steuerung und Stromversorgung. Es ist noch kein Motor oder Riemen ausgewählt.

**Schnittstellen:** S-03 zur festen Struktur; S-04 zum Wagen.

**Späterer Nachweis:** Fahrwiderstand, Anfahren, Stoppen und Gleichmäßigkeit prüfen; bei Motorisierung auch Begrenzung und Verhalten bei Energieausfall passend zur Einsatzlage prüfen.

## 7. Kameraaufnahme

**Funktion:** Das Kamerasystem lösbar und gegen unbeabsichtigtes Lösen gesichert am Wagen befestigen.

**Entwurfsziele:**

- Die tatsächliche Anschlussgeometrie von Kamera, Kopf oder Schnellwechselplatte aufnehmen.
- Verdrehschutz und zugängliche Betätigung vorsehen.
- Schraubenlänge bzw. Einschraubtiefe anhand des realen Gegenstücks festlegen.
- Schwerpunkt und Hebelarme in die Wagen- und Schienenauslegung zurückführen.

**Offen:** Anschlussart einschließlich Gewindespezifikation, Auflagefläche, Befestigungsmittel, Bauhöhe und Verstellbedarf. Es wird kein Standardgewinde vorausgesetzt.

**Schnittstelle:** S-05 zum Wagen; kameraseitiges Gegenstück nach P-09.

**Späterer Nachweis:** Passung, sichere Klemmung, Verdrehung und Freigängigkeit zunächst mit Ersatzlast, danach mit dem realen Kamerasystem prüfen.

## 8. Schnittstellenregister

| ID | Verbindung | Gemeinsam zu dokumentieren |
| --- | --- | --- |
| S-01 | Schiene ↔ Wagen | Führungsgeometrie, Bezugsflächen, Spiel/Vorspannung, Rückhaltung |
| S-02 | Schiene ↔ Abstützung | Auflagepunkte, Lochbild, Befestiger, Lastpfad |
| S-03 | Feste Struktur ↔ Anschläge/Antrieb | Bauraum, Kraftaufnahme, Befestigung |
| S-04 | Antrieb ↔ Wagen | Angriffspunkt, Kraft-/Bewegungsrichtung, Freigängigkeit |
| S-05 | Wagen ↔ Kameraaufnahme | Bezugsebene, Lochbild, Befestiger, Schwerpunktbezug |

Alle Anschlussmaße und Toleranzen sind noch offen. Änderungen an einer Schnittstelle werden in beiden betroffenen Baugruppen und im Entscheidungsprotokoll nachgeführt.

## 9. Freigabe vor dem ersten Belastungsversuch

Vor dem Versuch sind konkrete Prüflast, Prüfdauer und messbare Grenzwerte für Verformung, Spiel, Fahrverhalten und Klemmung festzulegen. Material, Druckparameter, Bauteilrevision und Abstützung gehören zum Prüfling. Vorgehen und Protokoll stehen in [validation/README.md](../validation/README.md).
