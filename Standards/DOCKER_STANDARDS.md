---
title: "Docker- und Containerstandards"
schema_version: "1.0"
version: "0.1.0"
last_updated: "2026-11-13T18:34:46Z"
tier: 3
ai_usage: "allowed"
status: "draft"
---

# Docker- und Containerstandards

Die Standards gelten für Docker und vergleichbare OCI-kompatible Werkzeuge. Dieses Repository liefert Methodik, keine konkrete Deploymentkonfiguration.

## Images und Build

- Minimale, vertrauenswürdige Basisimages und nachvollziehbare Versionsbindung verwenden.
- Für reproduzierbare Freigaben Image-Digests dokumentieren; Aktualisierungen regelmäßig prüfen.
- Multi-Stage-Builds einsetzen, wenn sie Laufzeitumfang reduzieren.
- Keine Secrets in Buildkontext, Image-Layern, Build-Argumenten oder Repositorydateien.
- Lizenzen und Schwachstellen vor Freigabe prüfen.

## Laufzeit

- Möglichst unprivilegiert und ohne Root ausführen.
- Fähigkeiten, Dateisystemschreibzugriffe und Netzwerkzugriffe minimieren.
- Keine Docker-Sockets oder Hostverzeichnisse pauschal einbinden.
- Ressourcenlimits, Healthchecks und kontrolliertes Beenden berücksichtigen.
- Konfiguration von Images trennen; Secrets nur über geeignete Laufzeitmechanismen bereitstellen.

## Betrieb

Persistente Daten, Migrationen, Backup, Restore und Rollback projektspezifisch dokumentieren. Logs an Standardausgabe ohne vertrauliche Werte liefern. Interne Adressen und konkrete Betriebsdetails ausschließlich im dafür klassifizierten privaten Bereich pflegen.
