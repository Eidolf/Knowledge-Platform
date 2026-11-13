---
title: "Tier-Modell"
schema_version: "1.0"
version: "0.1.0"
last_updated: "2026-11-13T18:34:46Z"
tier: 3
ai_usage: "allowed"
status: "draft"
---

# Tier-Modell

Die Tier-Nummer ist keine numerische Berechtigungsrangfolge. Tier 4 beschreibt insbesondere eine Darstellungsform und keine Herabstufung vertraulicher Inhalte.

| Tier | Bezeichnung | Beispiele | Speicherung und KI |
| --- | --- | --- | --- |
| 0 | Geheim | Passwörter, API Keys, Zertifikate, Recovery Codes, SSH Private Keys | Niemals in Git, niemals in KI, niemals in Dokumentation |
| 1 | Interne Infrastruktur | IP-Adressen, Hostnamen, Netzwerkpläne, Exchange-Strukturen, Home-Assistant-Infrastruktur, Monitoring-Systeme | Nur private Repositories; nicht automatisch an KI weitergeben |
| 2 | Projektdetails | Ideen, Architekturentwürfe, technische Konzepte, Backlogs, Roadmaps | Privat speichern; nur selektiv KI bereitstellen |
| 3 | Standards und Methodik | Entwicklungsmethoden, Coding- und Dokumentationsstandards, Architekturprinzipien | Dürfen jeder KI bereitgestellt werden |
| 4 | KI-Kontext | Projektkataloge, Zusammenfassungen, Entwicklungsrichtlinien, Arbeitskontexte | KI-optimierte Dokumente; Quellklassifizierung und Freigabe bleiben wirksam |
| 5 | Öffentliche Informationen | Freigegebene Readmes, Changelogs, Handbücher, Releases | Nach expliziter Prüfung öffentlich |

## Tier 0

Auch Zertifikate werden im Rahmen dieser Plattform pauschal als Tier 0 behandelt. Geheimnisse ausschließlich in einem geeigneten Secret-Management-System verwalten. Weder Werte noch Kopien, Screenshots oder Beispielwerte echter Geheimnisse dokumentieren.

## Mischinhalte und Ableitungen

- Der strengste zutreffende Schutz gilt für das gesamte Dokument.
- Nicht den größten oder kleinsten Zahlenwert zur Schutzentscheidung verwenden.
- Tier-4-Kontexte führen `source_tiers` und `ai_usage`; die Quellrestriktionen bleiben bindend.
- Zusammenfassen, Umbenennen oder Verschieben allein deklassifiziert keine Information.
- Eine separate anonymisierte Ableitung benötigt Inhaltsprüfung und dokumentierte Freigabe.
- Eine README ist nicht automatisch Tier 5. Projekt-Readmes bleiben standardmäßig Tier 2.

## Repositoryzuordnung

Knowledge-Platform und ER-DesignSystem: Tier 3. ER-KnowledgeBase: Tier 2, KI-Ansichten Tier 4 mit Tier-2-Quellen. ER-Private: Tier 1 und ausdrücklich NICHT KI-GEEIGNET. Tier 0 gehört in keines der Repositories.

Details zur Kennzeichnung und Änderung stehen in der [Datenklassifizierung](DATA_CLASSIFICATION.md).
