---
title: "Knowledge Platform"
schema_version: "1.0"
version: "0.1.0"
last_updated: "2026-11-13T18:34:46Z"
tier: 3
ai_usage: "allowed"
status: "draft"
---

# Knowledge Platform

Herstellerneutrale, Git-basierte und Markdown-first Wissensplattform für private Projekte, Homelab, Unternehmen und Kunden. Methodik ist generisch; konkrete Implementierungen und vertrauliche Daten bleiben getrennt.

## Einstieg

1. [Repositorykonzept und vollständiger Dateibaum](Documentation/REPOSITORY_CONCEPT.md) lesen.
2. [Tier-Modell](Security/TIER_MODEL.md) und [KI-Richtlinie](AI/AI_USAGE_POLICY.md) anwenden.
3. Projekte mit der [Projektvorlage](Templates/PROJECT_TEMPLATE.md) dokumentieren.
4. Entscheidungen nach dem [Entscheidungsprozess](Governance/DECISION_PROCESS.md) festhalten.

## Bereiche

| Bereich | Zweck |
| --- | --- |
| [AI](AI/MASTER_CONTEXT.md) | Werkzeugunabhängiger Arbeitskontext und KI-Nutzung |
| [Architecture](Architecture/ARCHITECTURE_PRINCIPLES.md) | Architekturprinzipien und Entscheidungsrahmen |
| [Security](Security/SECURITY_POLICY.md) | Klassifizierung, Freigabe und Schutz |
| [Standards](Standards/DOCUMENTATION_STANDARDS.md) | Code, Dokumentation, Git und Container |
| [Templates](Templates/PROJECT_TEMPLATE.md) | Wiederverwendbare Dokumentvorlagen |
| [Documentation](Documentation/KNOWLEDGE_STRUCTURE.md) | Informationsarchitektur |
| [Governance](Governance/REVIEW_PROCESS.md) | Verantwortlichkeiten und Reviews |

## Repositorygrenzen

- **Knowledge-Platform:** ausschließlich Standards und Methodik, standardmäßig Tier 3.
- **ER-KnowledgeBase:** ausschließlich Wissen über konkrete ER-Projekte, standardmäßig privat/Tier 2.
- **ER-DesignSystem:** generische Gestaltungsregeln und Theme-Engine-Vertrag, Tier 3.
- **ER-Private:** interne Infrastruktur, privat/Tier 1 und NICHT KI-GEEIGNET.

Jedes Verzeichnis ist ein eigenständiges lokales Git-Repository. Es werden keine Remotes, Veröffentlichungen oder initialen Commits vorausgesetzt. Vor einem Upload müssen Sichtbarkeit, Inhalte und Zugriffe geprüft werden. Lokales Git setzt keine Hosting-Sichtbarkeit.

## Arbeitsweise

Markdown ist die maßgebliche Quelle. Plattformen wie GitHub Copilot, OpenCode, ChatGPT oder Claude bekommen nur explizit freigegebene, minimale Kontextpakete. Automatische Erkennung bestimmter Dateinamen wird nicht vorausgesetzt. Es gibt keine Abhängigkeit von einem KI-Anbieter, Plugin, Theme oder proprietären Wissensformat.

Diese Erstfassung enthält keine überprüften Implementierungsdetails der genannten Projekte. Status `draft` bedeutet: zur Prüfung, nicht bereits organisatorisch beschlossen.
