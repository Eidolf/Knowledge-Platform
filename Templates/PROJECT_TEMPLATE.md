---
title: "Vorlage: Projektsteckbrief"
schema_version: "1.0"
version: "0.1.0"
last_updated: "2026-11-13T18:34:46Z"
tier: 3
ai_usage: "allowed"
status: "template"
---

# Projektname

> Für ein konkretes Projekt Titel, Datum und Status setzen sowie standardmäßig `tier: 2` und `ai_usage: selective` verwenden.

## Zweck und Nutzen

Problem, Zielgruppe und erwarteten Nutzen beschreiben; unbekannte Angaben als offen markieren.

## Umfang

- Ziele: offen
- Nichtziele: offen
- Verantwortlich: offen
- Implementierungsrepository: nicht verifiziert
- Lebenszyklus: noch zu erheben

## Wissenssatz

Im Projektordner sechs Dokumente anlegen:

| Datei | Inhalt |
| --- | --- |
| README.md | Einstieg, Status und Verweise |
| VISION.md | Problem, Zielbild und Erfolgskriterien |
| ROADMAP.md | Geplante Ergebnisse und Abhängigkeiten |
| ARCHITECTURE.md | Verifizierter Systemkontext und Entwurf |
| BACKLOG.md | Ausführbare Arbeitspakete mit Akzeptanzkriterien |
| DECISIONS.md | Entscheidungsregister und ADR-Verweise |

Die [Architekturvorlage](../Architecture/PROJECT_TEMPLATE.md) ergänzt diesen Steckbrief. Konkrete Implementierungen verbleiben in ihrem Quellrepository.

## Nachweise und Pflege

Quellen, Prüfdaten, Klassifizierung und Reviewbedarf festhalten. Menschliche Übersicht und KI-Katalog nach Änderungen gezielt synchronisieren.
