---
title: "Datenklassifizierung"
schema_version: "1.0"
version: "0.1.0"
last_updated: "2026-11-13T18:34:46Z"
tier: 3
ai_usage: "allowed"
status: "draft"
---

# Datenklassifizierung

## Pflichtverfahren

1. Inhalt und Quellen vor dem Speichern identifizieren.
2. Nach [Tier-Modell](TIER_MODEL.md) klassifizieren; bei Unsicherheit restriktiv behandeln.
3. Frontmatter setzen und passenden Repositorybereich wählen.
4. Zugriff, KI-Nutzung und Veröffentlichung unabhängig voneinander prüfen.
5. Bei Inhaltsänderung die Klassifizierung erneut bewerten.

## Maschinenlesbare Kennzeichnung

Jedes Markdown-Dokument besitzt `title`, `schema_version`, `version`, `last_updated`, `tier`, `ai_usage` und `status`. Werte und Syntax definiert der [Dokumentationsstandard](../Standards/DOCUMENTATION_STANDARDS.md).

Tier 4 ergänzt `source_tiers` als Liste. `ai_usage: selective` ist keine Freigabe, sondern fordert eine explizite Einzelfreigabe. Tier 1 in ER-Private verlangt `ai_usage: prohibited` und den sichtbaren Hinweis **NICHT KI-GEEIGNET**.

## Umklassifizierung

Die informationsverantwortliche Person prüft vollständigen Inhalt, verlinkte Anhänge und mögliche Rückschlüsse. Freigabe mit Zweck, Umfang, Empfänger und Gültigkeit nachvollziehbar dokumentieren. Unternehmens- und Kundenvorgaben können strengere Regeln setzen.

## Veröffentlichung

Tier 5 wird erst nach Inhalts-, Rechte- und Datenschutzprüfung vergeben. Bereits vorhandene Git-Historie, Branches, Tags und Anhänge vor einem öffentlichen Remote gesondert prüfen. Ein geändertes Frontmatter entfernt keine früher gespeicherten Informationen.
