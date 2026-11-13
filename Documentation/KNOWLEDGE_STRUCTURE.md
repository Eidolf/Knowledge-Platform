---
title: "Wissensstruktur"
schema_version: "1.0"
version: "0.1.0"
last_updated: "2026-11-13T18:34:46Z"
tier: 3
ai_usage: "allowed"
status: "draft"
---

# Wissensstruktur

## Trennung der Ebenen

| Ebene | Maßgebliche Quelle | Abgeleitete Ansichten |
| --- | --- | --- |
| Methodik | Knowledge-Platform | Explizit geladener generischer KI-Kontext |
| Projektwissen | ER-KnowledgeBase/Projects | Human, Portfolio, Roadmaps, AI |
| Designregeln | ER-DesignSystem | Projektspezifische Themes und Komponenten |
| Interne Infrastruktur | ER-Private | Keine automatisch erzeugten KI-Ansichten |
| Implementierung | Jeweiliges Quellrepository | Verifizierte Projektbeschreibungen |

## Projektwissen

README ist Einstieg, VISION beschreibt das Warum, ROADMAP die Reihenfolge, ARCHITECTURE das System, BACKLOG konkrete Arbeit und DECISIONS getroffene Entscheidungen. Projektübergreifende Entscheidungen liegen im zentralen Entscheidungsbereich; lokale Entscheidungen bleiben beim Projekt.

## Quellen und Synchronisation

Menschliche Übersichten und KI-Kontexte sind Navigation und Ableitung, keine konkurrierenden Primärquellen. Projektänderungen lösen die Prüfung betroffener Ansichten aus. Quellen ohne überprüften Stand werden ausdrücklich als nicht verifiziert markiert.

## Informationsfluss

Methodik darf in Projekten angewendet werden. Projekterkenntnisse dürfen nur anonymisiert und geprüft zur generischen Methodik werden. Infrastrukturinformationen fließen nicht automatisch in Projektkataloge oder KI-Kontexte. Tier-4-Darstellung hebt keinen Schutz auf.

## Skalierung

Kunden- und Unternehmenswissen bei Bedarf in getrennten privaten Wissensrepositories nach demselben Muster organisieren. Zugriffsgrenzen durch Repository- und Kontorechte umsetzen, nicht nur durch Ordner oder Metadaten.
