---
title: "Git-Standards"
schema_version: "1.0"
version: "0.1.0"
last_updated: "2026-11-13T18:34:46Z"
tier: 3
ai_usage: "allowed"
status: "draft"
---

# Git-Standards

## Repositorygrenzen

Vier unabhängige Repositories verwenden, keine ineinander verschachtelten Git-Repositories. Keine Kopie von Infrastrukturwissen in Methodik oder KI-Kontext. Markdown bleibt die maßgebliche Wissensquelle.

## Änderungen

- Kurze, thematisch klare Branches; Änderungen über einen nachvollziehbaren Reviewprozess integrieren.
- Kleine, zusammenhängende Commits mit begründender Nachricht.
- Empfohlenes Nachrichtenschema: `docs: Thema`, `feat: Thema`, `fix: Thema`.
- Keine fremden uncommitteten Änderungen überschreiben.
- Keine Historienumschreibung oder Force-Pushes ohne abgestimmten Anlass.
- Standardbranch schützen, soweit die Hostingplattform dies unterstützt.

## Vor Commit und Push

1. Diff einschließlich neuer Dateien vollständig prüfen.
2. Frontmatter, Links und direkt betroffene Ansichten validieren.
3. Geheimnisse und unzulässige Daten ausschließen; automatisches Scanning ergänzend nutzen.
4. Relevante Tests und Dokumentprüfungen ausführen.
5. Vor Push Remoteziel, Sichtbarkeit und Rechte prüfen.

## Hosting und Wiederherstellung

Git ist herstellerneutral; Remotes können bei unterschiedlichen Anbietern liegen. Private Repositories und geschützte Backups sind für Tier 1 und Tier 2 Pflicht. Git-Historie ersetzt kein überprüftes Backup. Wiederherstellung regelmäßig testen.
