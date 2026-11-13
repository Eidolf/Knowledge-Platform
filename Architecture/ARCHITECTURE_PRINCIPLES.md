---
title: "Architekturprinzipien"
schema_version: "1.0"
version: "0.1.0"
last_updated: "2026-11-13T18:34:46Z"
tier: 3
ai_usage: "allowed"
status: "draft"
---

# Architekturprinzipien

## Leitlinien

1. **Methodik und Umsetzung trennen:** Standards kennen keine konkreten Hosts, Kunden oder Implementierungsdetails.
2. **Offene Quellenformate:** Markdown und offene, textbasierte Schnittstellen bevorzugen; kein Tool als alleiniger Wissensspeicher.
3. **Eine maßgebliche Quelle:** Fakten einmal pflegen, Ansichten und KI-Zusammenfassungen daraus ableiten und verlinken.
4. **Lose Kopplung:** klare Verantwortungsgrenzen, explizite Verträge und austauschbare Adapter.
5. **Einfachheit:** kleinste tragfähige Lösung statt vorsorglicher Plattformkomplexität.
6. **Security und Privacy by Design:** minimale Rechte, Datenminimierung, Klassifizierung vor Weitergabe.
7. **Verifizierbarkeit:** messbare Qualitätsziele, nachvollziehbare Entscheidungen und reproduzierbare Prüfungen.
8. **Betriebsfähigkeit:** Fehlerzustände, Beobachtbarkeit, Wiederherstellung und Lebenszyklus berücksichtigen.
9. **Zugänglichkeit:** menschliche Lesbarkeit und Barrierefreiheit nicht gegen KI-Optimierung eintauschen.
10. **Portabilität:** Implementierungen dürfen Anbieter nutzen; Kernwissen und Austausch dürfen nicht davon abhängen.

## Anwendung

Trade-offs projektspezifisch dokumentieren. Eine begründete Ausnahme enthält Verantwortliche, Risiko, Gültigkeitsdauer und Reviewtermin. Signifikante Entscheidungen als [ADR](ADR_TEMPLATE.md) festhalten.
