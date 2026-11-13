---
title: "Repositorykonzept"
schema_version: "1.0"
version: "0.1.0"
last_updated: "2026-11-13T18:34:46Z"
tier: 3
ai_usage: "allowed"
status: "draft"
---

# Repositorykonzept

## Grenzen und Sichtbarkeit

| Repository | Inhalt | Standard | Veröffentlichung |
| --- | --- | --- | --- |
| Knowledge-Platform | Generische Methodik | Tier 3 | Nach Rechte- und Inhaltsprüfung möglich |
| ER-KnowledgeBase | ER-Projektwissen, keine Implementierungen | Tier 2, privat | Nur separat freigegebene Ableitungen |
| ER-DesignSystem | Designregeln und Theme-Vertrag | Tier 3 | Nach Rechte- und Inhaltsprüfung möglich |
| ER-Private | Interne Infrastruktur | Tier 1, privat | Nicht veröffentlichen; NICHT KI-GEEIGNET |

Tier 3 erlaubt KI-Nutzung, ist aber keine automatische öffentliche Veröffentlichung. Alle vier Repositories sind unabhängig; es gibt keine Submodule oder Anbieterbindung. Relative Links zwischen Repositories setzen eine lokale Anordnung als Geschwister voraus. Bei getrenntem Hosting diese Verweise auf die passende, zugriffsgeschützte Quelle übertragen.

## Vollständiger initialer Dateibaum

Die Git-Verwaltungsverzeichnisse sind bewusst nicht dargestellt. Projektnamen sind Strukturbezeichnungen, keine Behauptungen über konkrete Implementierungen.

```text
Knowledge-Platform/
├── README.md
├── AI/
│   ├── MASTER_CONTEXT.md
│   ├── COPILOT_RULES.md
│   └── AI_USAGE_POLICY.md
├── Architecture/
│   ├── ARCHITECTURE_PRINCIPLES.md
│   ├── ADR_TEMPLATE.md
│   └── PROJECT_TEMPLATE.md
├── Security/
│   ├── TIER_MODEL.md
│   ├── DATA_CLASSIFICATION.md
│   └── SECURITY_POLICY.md
├── Standards/
│   ├── CODING_STANDARDS.md
│   ├── DOCUMENTATION_STANDARDS.md
│   ├── GIT_STANDARDS.md
│   └── DOCKER_STANDARDS.md
├── Templates/
│   ├── PROJECT_TEMPLATE.md
│   ├── ROADMAP_TEMPLATE.md
│   └── CHANGELOG_TEMPLATE.md
├── Documentation/
│   ├── KNOWLEDGE_STRUCTURE.md
│   └── REPOSITORY_CONCEPT.md
└── Governance/
    ├── DECISION_PROCESS.md
    └── REVIEW_PROCESS.md

ER-KnowledgeBase/
├── README.md
├── Human/
│   ├── Portfolio.md
│   ├── Projects.md
│   └── Roadmap.md
├── AI/
│   ├── MASTER_CONTEXT.md
│   ├── PROJECT_CATALOG.md
│   ├── PLATFORM_VISION.md
│   └── DESIGN_OVERVIEW.md
├── Projects/
│   ├── ER-Startseite/
│   │   ├── README.md
│   │   ├── VISION.md
│   │   ├── ROADMAP.md
│   │   ├── ARCHITECTURE.md
│   │   ├── BACKLOG.md
│   │   └── DECISIONS.md
│   ├── ER-DMARC-Monitor/
│   │   ├── README.md
│   │   ├── VISION.md
│   │   ├── ROADMAP.md
│   │   ├── ARCHITECTURE.md
│   │   ├── BACKLOG.md
│   │   └── DECISIONS.md
│   ├── ER-PSScripter/
│   │   ├── README.md
│   │   ├── VISION.md
│   │   ├── ROADMAP.md
│   │   ├── ARCHITECTURE.md
│   │   ├── BACKLOG.md
│   │   └── DECISIONS.md
│   ├── ER-AIMusicPage/
│   │   ├── README.md
│   │   ├── VISION.md
│   │   ├── ROADMAP.md
│   │   ├── ARCHITECTURE.md
│   │   ├── BACKLOG.md
│   │   └── DECISIONS.md
│   ├── ER-MusicTagManager/
│   │   ├── README.md
│   │   ├── VISION.md
│   │   ├── ROADMAP.md
│   │   ├── ARCHITECTURE.md
│   │   ├── BACKLOG.md
│   │   └── DECISIONS.md
│   ├── ER-Biometric-Picture/
│   │   ├── README.md
│   │   ├── VISION.md
│   │   ├── ROADMAP.md
│   │   ├── ARCHITECTURE.md
│   │   ├── BACKLOG.md
│   │   └── DECISIONS.md
│   ├── Docker-AntiGravity/
│   │   ├── README.md
│   │   ├── VISION.md
│   │   ├── ROADMAP.md
│   │   ├── ARCHITECTURE.md
│   │   ├── BACKLOG.md
│   │   └── DECISIONS.md
│   ├── hassio-addons/
│   │   ├── README.md
│   │   ├── VISION.md
│   │   ├── ROADMAP.md
│   │   ├── ARCHITECTURE.md
│   │   ├── BACKLOG.md
│   │   └── DECISIONS.md
│   ├── Public-Scripts/
│   │   ├── README.md
│   │   ├── VISION.md
│   │   ├── ROADMAP.md
│   │   ├── ARCHITECTURE.md
│   │   ├── BACKLOG.md
│   │   └── DECISIONS.md
│   └── eidolf.github.io/
│       ├── README.md
│       ├── VISION.md
│       ├── ROADMAP.md
│       ├── ARCHITECTURE.md
│       ├── BACKLOG.md
│       └── DECISIONS.md
├── Roadmaps/
│   └── README.md
├── Decisions/
│   └── README.md
├── Portfolio/
│   └── README.md
└── Prompts/
    └── README.md

ER-DesignSystem/
├── README.md
├── DESIGN_PRINCIPLES.md
├── COMPONENT_GUIDELINES.md
├── THEME_ENGINE.md
└── Themes/
    ├── ER_ENTERPRISE.md
    ├── ER_NEON.md
    └── ER_GLASS.md

ER-Private/
├── README.md
├── Infrastruktur/
│   └── README.md
├── Homelab/
│   └── README.md
├── Domains/
│   └── README.md
├── Exchange/
│   └── README.md
├── Home-Assistant/
│   └── README.md
├── Storage/
│   └── README.md
├── Netzwerk/
│   └── README.md
└── Monitoring/
    └── README.md
```

## Einführung

1. Rollen und Reviewverantwortung benennen.
2. Tier-1- und Tier-2-Remotes ausschließlich privat anlegen.
3. Standardbranch und Zugriffsschutz konfigurieren.
4. Inhalte prüfen und erst danach initial committen beziehungsweise hochladen.
5. KI nur in getrennten, explizit freigegebenen Kontexten betreiben.

Die Initialisierung richtet keine Hostingrechte ein, erstellt keine Remotes und publiziert keine Inhalte. Leere Bereiche werden durch inhaltliche README-Dateien versionierbar, nicht durch proprietäre Platzhalter.
