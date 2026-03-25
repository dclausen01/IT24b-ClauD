---
url: https://hackmd.io/QRnUzVXISZC28wM5H92xqw
title: 01a - Ergebnisse Von der Sicherheitsrichtlinie zur Schutzbedarfsanalyse
lastSync: 2026-03-24T16:50:09.316Z
---
# Entwicklung einer Sicherheitsrichtlinie (Tim, Mo, Jan, Devin, Kai, Jonas)

Die Entwicklung einer Sicherheitsrichtlinie dient dazu, ein Grundsatzdokument zu erstellen, in dem alle Ziele, Prinzipien und das Niveau der Sicherheit klar festgehalten werden. Es ist also ein Leitfaden für die Sicherheit in Unternehmen, an den sich Mitarbeiter und Führungskräfte gleichermaßen halten müssen. Sie sollte klar verständlich sein damit auch nicht IT-Mitarbeiter keine Schwierigkeiten haben sie zu verstehen. Zusätzlich sollten Mitarbeiter geschult und sensibilisiert werden. Die Sicherheitsrichtlinie sollte auch regelmäßig überprüft und auf dem aktuellen Stand gehalten werden, da es ständig zu neuen Bedrohungen kommt.

Man berücksichtigt dabei unter anderem folgende Punkte:

- Was geschützt werden soll (Daten,Systeme,Prozesse) und was die gesetzlichen Anforderungen sind
- Was sind die Risiken und wie hoch wären die Schäden wenn sie eintreten
- Berücksichtigung der CIA-Triade: Vertraulichkeit, Integrität, Verfügbarkeit
- Wer ist zuständig für die Umsetzung, wer überwacht die Einhaltung?

Typische Bereiche mit denen man sich bei der Erstellung befassen sollte sind z.B.:

- Passwort- und Zugriffsregelungen
- Umgang mit mobilen Geräten & Homeoffice
- E-Mail- und Internetsicherheit
- Datensicherung & Notfallplanung
- Meldewege bei Sicherheitsvorfällen
- Physische Sicherheit (Serverräume, Clean-Desk-Policy)

# Sicherheitskonzept (Ramy, Oliver, Sandro, Pierre)

## Geltungsbereich definieren
•	Welche Standorte, Systeme, Anwendungen und Daten werden erfasst?
•	Wer sind die Verantwortlichen (z. B. ISB, IT-Leitung)?
## Bestandsaufnahme & Schutzbedarf
•	Assets erfassen: Server, Clients, Anwendungen, Datenflüsse, Nutzerrollen.
•	Schutzbedarf bewerten: Vertraulichkeit, Integrität, Verfügbarkeit.
## Risikoanalyse
•	Bedrohungen & Schwachstellen identifizieren (z. B. Malware, Fehlkonfiguration, Ausfall).
•	Bewerten: Eintrittswahrscheinlichkeit und Schadenspotenzial.
## Maßnahmen ableiten & planen
•	Technisch: Firewall, Verschlüsselung, Patchmanagement, MFA.
•	Organisatorisch: Richtlinien, Rollen/Berechtigungen, Schulungen, Notfallkonzept.
•	Priorisieren nach Risiko.
## Dokumentation, Umsetzung & Review
•	Verständlich dokumentieren.
•	Umsetzen mit Zuständigkeiten und Fristen.
•	Regelmäßig prüfen (PDCA-Zyklus, z. B. ISO 27001/BSI-Grundschutz).

# Strukturanalye (Philipp, Jonah, Lars)
• Ziel: Überblick über die gesamte Informations- und IT-Struktur einer Organisation erhalten
• Grundlage für die spätere Schutzbedarfsfeststellung

## Wichtige Schritte der Strukturanalyse:
• Erfassung der Geschäftsprozesse, Anwendungen und Informationen
• Erhebung des Netzplans (Darstellung der Verbindungen zwischen Systemen)
• Erfassung der IT-Systeme und Netzwerke, die Informationen verarbeiten, speichern oder übertragen
• Analyse der räumlichen Gegebenheiten (z. B. Serverräume, Arbeitsplätze, Standorte)

## Ergebnis der Strukturanalyse:
• Strukturierte Übersicht über:
    • Prozesse und Anwendungen
    • IT-Systeme
    • Räume
    • Kommunikationsverbindungen

# Schutzbedarfsfeststellung (Karolin, Semy, Lennart, Lukas)
- Es wird bestimmt, wie wichtig und schützenswert bestimmte Informationen, Systeme oder Daten im Unternehmen sind
- Es wird bewertet, welche Schäden entstehen können falls etwas passiert
- dabei werden drei Punkte besonders beachtet: Vertraulichkeit -> wer darf die Daten sehen?, 
Integrität -> dürfen Daten verändert werden,
Verfügbarkeit -> müssen Daten immer verfügbar sein
- anhand der Bewertung wird entschieden wie stark die Sicherheitsmaßnahmen sein müssen

- Beispiel:
Personalabteilung: 
verarbeitet Mitarbeiterdaten, gehälter und Verträge
Risiko: Datenschutzverletzungen
Schutzbedarf: hoch, da persönliche Daten sehr sensibel sind

IT-Abteilung:
Unternehmenssysteme, Datenbanken, Software
Risiko: Systemausfall oder Hackerangriff
Schutzbedarf: sehr hoch, da das ganze Unternehmen davon abhä