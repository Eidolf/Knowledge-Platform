---
title: "Dokumentationsstandards"
schema_version: "1.0"
version: "0.1.0"
last_updated: "2026-11-13T18:34:46Z"
tier: 3
ai_usage: "allowed"
status: "draft"
---

# Dokumentationsstandards

## Format

UTF-8-Markdown mit YAML-Frontmatter verwenden. YAML ist hier ausschließlich offenes Metadatenformat innerhalb der Markdown-Datei. Wesentliche Inhalte dürfen weder proprietäre Renderer noch Plugins erfordern.

```yaml
---
title: "Dokumenttitel"
schema_version: "1.0"
version: "0.1.0"
last_updated: "2026-11-13T18:34:46Z"
tier: 2
ai_usage: "selective"
status: "draft"
---
```

| Feld | Bedeutung |
| --- | --- |
| `title` | Menschlich lesbarer Titel |
| `schema_version` | Version des Metadatenschemas, hier `1.0` |
| `version` | Dokumentversion als MAJOR.MINOR.PATCH |
| `last_updated` | Letzte tatsächliche Inhaltsänderung, ISO 8601 in UTC |
| `tier` | Ganzzahl von 1 bis 5; Tier-0-Inhalte sind verboten |
| `ai_usage` | `allowed`, `selective` oder `prohibited` |
| `status` | `draft`, `active`, `template`, `deprecated` oder `archived` |
| `source_tiers` | Pflicht bei Tier 4: Liste der Quell-Tiers |

`allowed` gilt für generische Tier-3-Methodik oder freigegebene öffentliche Informationen, nicht als Override für geschützte Quellen. Optionale Felder wie `owner` oder `review_due` dürfen bei tatsächlicher Kenntnis ergänzt werden; keine erfundenen Zuständigkeiten.

## Aufbau und Pflege

- Genau eine H1-Überschrift; danach logisch gegliederte Abschnitte.
- Zweck, aktuellen Status, belastbare Quellen und offene Fragen sichtbar trennen.
- Relative Markdown-Links für lokale Quellen verwenden.
- Keine leeren Dateien; unbekannte Inhalte als `Offen` oder `Nicht verifiziert` kennzeichnen.
- Version bei Inhaltsänderung erhöhen; Datum gleichzeitig aktualisieren.
- PATCH für Klarstellungen, MINOR für kompatible Ergänzungen, MAJOR für inkompatible Regeländerungen.
- Bei Kopien von Vorlagen Klassifizierung, Titel, Status und Änderungszeit neu setzen.
- ADR-Entscheidungsstatus separat vom Dokumentstatus führen.
- Keine Geheimnisse und keine ungeprüften KI-Ausgaben als Fakten aufnehmen.

## Ansichten und Archivierung

Menschliche Übersichten und KI-Kontexte verlinken ihre maßgeblichen Quellen. Nach Änderungen Zusammenfassungen auf Konsistenz prüfen. Veraltete Inhalte als `deprecated` oder `archived` markieren und Nachfolger verlinken; Historie nicht still überschreiben.
