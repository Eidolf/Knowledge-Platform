---
title: "Coding-Standards"
schema_version: "1.0"
version: "0.1.0"
last_updated: "2026-11-13T18:34:46Z"
tier: 3
ai_usage: "allowed"
status: "draft"
---

# Coding-Standards

## Grundregeln

- Bestehende Sprach- und Repositorykonventionen vor neuen Regeln übernehmen.
- Kleine, kohärente Änderungen mit klaren Verantwortlichkeiten erstellen.
- Verständliche Namen, explizite Schnittstellen und vorhandene gemeinsame Hilfsfunktionen verwenden.
- Typsicherheit erhalten; Eingaben an Vertrauensgrenzen validieren.
- Fehler ausdrücklich behandeln; keine stillen Erfolgsersatzwerte.
- Kommentare erklären nicht offensichtliche Entscheidungen, nicht den sichtbaren Code.
- Abhängigkeiten nur begründet und mit Lizenz-, Wartungs- und Sicherheitsprüfung ergänzen.
- Keine Geheimnisse, internen Kennungen oder personenbezogenen Daten in Code und Logs.

## Qualitätssicherung

Geändertes Verhalten durch fokussierte Tests absichern. Vorhandene Formatter, Linter, Typprüfungen und Builds verwenden. Relevante Fehlerfälle und Regressionen prüfen; Prüfergebnisse nachvollziehbar angeben.

## Projektspezifische Ergänzungen

Sprache, Toolchain, konkrete Befehle und Qualitätsgrenzen im Implementierungsrepository festlegen. Diese Methodik schreibt keine bestimmte Sprache, Cloud oder Entwicklungsumgebung vor.
