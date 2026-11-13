---
title: "Sicherheitsrichtlinie"
schema_version: "1.0"
version: "0.1.0"
last_updated: "2026-11-13T18:34:46Z"
tier: 3
ai_usage: "allowed"
status: "draft"
---

# Sicherheitsrichtlinie

## Schutzmaßnahmen

- Tier 0 niemals in Git, Dokumentation oder KI speichern.
- Tier 1 und Tier 2 nur in privaten Repositories mit minimalen Zugriffsrechten verwalten.
- Vor Remoteanlage oder Push Sichtbarkeit und Berechtigungen überprüfen; lokales Git ist keine Zugriffskontrolle.
- Mehrfaktorauthentifizierung, getrennte Konten und regelmäßige Rechteprüfungen einsetzen.
- Verschlüsselte Datenträger und geschützte Backups für vertrauliche Repositories verwenden.
- Keine echten Geheimnisse in Beispielen, Logs, Issues, Bildern oder Testdaten.
- Secret-Scanning vor Push und in CI einsetzen, soweit verfügbar; es ersetzt keine Inhaltsprüfung.
- KI-Werkzeugen keinen pauschalen Zugriff auf ER-Private oder übergeordnete Arbeitsverzeichnisse geben.

## Verantwortung

Repositoryverantwortliche setzen Schutz und Sichtbarkeit um. Informationsverantwortliche klassifizieren und genehmigen Weitergaben. Reviewer prüfen die Einhaltung. Solange Rollen nicht besetzt sind, erfolgen keine externen Freigaben.

## Vorfallbehandlung

1. Weitergabe und betroffene automatisierte Verarbeitung stoppen.
2. Betroffene Geheimnisse unverzüglich widerrufen oder rotieren.
3. Verantwortliche über einen geschützten Kanal informieren, ohne Geheimnisse zu wiederholen.
4. Zugriff und Verbreitung einschließlich KI-Verlauf, Remotes und Backups bewerten.
5. Bereinigung der Git-Historie koordiniert durchführen; Löschen im aktuellen Stand allein reicht nicht.
6. Ursache, Maßnahmen und verifizierte Wiederherstellung ohne sensible Werte dokumentieren.

## Meldung und Review

Keine öffentlichen Issues für vertrauliche Vorfälle verwenden. Ein geschützter Meldeweg muss vor produktiver Nutzung festgelegt werden. Mindestens jährlich und nach Vorfällen oder wesentlichen Änderungen überprüfen.
