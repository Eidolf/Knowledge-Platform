---
title: "Copilot-Regeln und Werkzeuganbindung"
schema_version: "1.0"
version: "0.1.0"
last_updated: "2026-11-13T18:34:46Z"
tier: 3
ai_usage: "allowed"
status: "draft"
---

# Copilot-Regeln und Werkzeuganbindung

Diese Regeln gelten inhaltlich genauso für OpenCode, ChatGPT, Claude und zukünftige Systeme. Der Dateiname ist eine Orientierung, kein automatisch geladener Anbietermechanismus.

## Einbindung

1. [Masterkontext](MASTER_CONTEXT.md) und [KI-Richtlinie](AI_USAGE_POLICY.md) explizit referenzieren oder als freigegebenes Kontextpaket übergeben.
2. Nur geprüfte Projektzusammenfassungen ergänzen.
3. Werkzeugadapter dürfen auf diese Quellen verweisen; keine getrennte Regelkopie als zweite Wahrheit pflegen.
4. Nach Werkzeugwechsel prüfen, ob Regeln tatsächlich geladen und Zugriffsbeschränkungen wirksam sind.

## Entwicklungsregeln

- Vor Änderungen Ziel, vorhandenen Code und direkte Abhängigkeiten prüfen.
- Repositorystandards und bestehende Tests nutzen.
- Keine Geheimnisse, proprietären Austauschformate oder unnötigen Abhängigkeiten einführen.
- Keine unaufgeforderten großflächigen Refactorings.
- Fehler sichtbar machen; keine scheinbar erfolgreichen Ersatzwerte.
- Geändertes Verhalten testen und direkt betroffene Dokumentation aktualisieren.
- Keine Commits, Pushes, Deployments oder destruktiven Aktionen ohne passenden Auftrag.

## Kontextbegrenzung

Ein Workspace mit ER-Private darf nicht ungeprüft von einem KI-Werkzeug indiziert werden. Ignore-Dateien sind Hilfsmittel, keine Sicherheitsgrenze. Getrennte Workspaces, minimale Dateifreigaben und wirksame Zugriffskontrollen verwenden.
