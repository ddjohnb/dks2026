# DKS 2026 — Grußtext-Netzwerk

Interaktive Visualisierung der Grußtext-Verbindungen des Abiturjahrgangs 2026 der Dreikönigsschule Dresden.

**→ [Zur Visualisierung](https://github.com/ddjohnb/dks2026)**

---

## Was zeigt das Diagramm?

Ein sogenannter **Force-Directed Graph** (gerichteter Netzwerkgraph): Jeder Punkt steht für eine Person des Jahrgangs, jede Linie für einen Grußtext.

| Farbe | Bedeutung |
|-------|-----------|
| 🟡 **Gold** | Gegenseitig — beide haben sich gegenseitig einen Grußtext geschrieben |
| 🟢 **Grün mit Pfeil** | Einseitig — der Pfeil zeigt, wer den Grußtext bekommt |

Die **Größe eines Punktes** wächst mit der Anzahl der Grüße, die jemand bekommt.

## Bedienung

- **Hover** über einen Namen → hebt alle Verbindungen dieser Person hervor
- **Klick** → fixiert die Hervorhebung
- **Ziehen** → verschiebt einzelne Knoten
- **↺ Neu ordnen** → startet die Simulation neu
- **↓ SVG** → exportiert das Diagramm als druckbare Vektorgrafik

## Daten

69 Personen · 158 Verbindungen

Die Daten sind direkt in der HTML-Datei eingebettet. Um die Daten zu aktualisieren, kann über den Upload-Bereich auf der Seite eine neue CSV-Datei geladen werden:

```
von,an
Anna Müller,Ben Schmidt
Ben Schmidt,Clara Weber
...
```

## Technik

Die gesamte Visualisierung besteht aus einer einzigen HTML-Datei (`index.html`) ohne externe Abhängigkeiten. Die Schriftart (Cocomat Pro) und alle Daten sind direkt eingebettet — die Seite funktioniert vollständig offline.

Das Layout wird durch eine **Force-Directed Simulation** berechnet: Knoten stoßen sich gegenseitig ab, Kanten ziehen sie zusammen, bis das System ein Gleichgewicht findet.

---

*Dreikönigsschule Dresden · Abitur 2026*
