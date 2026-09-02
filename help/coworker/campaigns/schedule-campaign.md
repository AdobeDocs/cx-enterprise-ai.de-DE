---
description: Die Beschreibung ist hier zu finden.
title: Planen einer Kampagne
product_v2: id: fdae8433-07cd-42e7-acce-738afe63f6bb
feature_v2: id: fdae8433-07cd-42e7-acce-738afe63f6bb
source-git-commit: a3df1a0f8e1014d95483f977aaa64435c18e6578
workflow-type: tm+mt
source-wordcount: 676
ht-degree: 1%

---

# Planen einer Kampagne {#schedule-campaign}

Beim Starten einer Kampagne können Benutzende jetzt genau auswählen, wann sie ausgeführt wird: sofort, zu einem bestimmten Datum und zu einer bestimmten Uhrzeit in der Zukunft oder nach einem sich wiederholenden (wiederkehrenden) Zeitplan. Benutzer können auch zu einem späteren Zeitpunkt zurückkehren und den Zeitplan einer Kampagne ändern, die bereits gestartet oder geplant wurde.

> **Was hat sich**: Zuvor konnten Kampagnen nur sofort gestartet werden. Diese Version fügt eine einmalige zukünftige Planung, wiederkehrende Zeitpläne und die Möglichkeit hinzu, einen Zeitplan nach dem Start zu bearbeiten.

## Voraussetzungen

- Die Kampagne muss startbereit sein (alle erforderlichen Einstellungen sind abgeschlossen).
- Außer einer Kampagne im Zustand „Starts möglich“ sind keine weiteren Voraussetzungen erforderlich.

## Funktionsweise dieser Funktion

Wenn ein(e) Benutzende(r) eine Kampagne startet, wählt er/sie einen von drei Zeitplanmodi und bestätigt dann. Der ausgewählte Zeitplan bestimmt, wann die Kampagne mit dem Versand beginnt und bei wiederkehrenden Kampagnen wie oft sie sich wiederholt und wann (oder ob) sie endet. Sobald eine Kampagne geplant oder live ist, kann ihr Zeitplan in den Kampagneneinstellungen bearbeitet werden.

### Wichtigste Verhaltensweisen

- Beim Starten sind drei Zeitplanmodi verfügbar **„Jetzt**, **Einmal planen** und **Wiederkehrend**.
- Eine für die Zukunft geplante Kampagne zeigt den Status „Geplant“ an, bis ihre Startzeit eintrifft, und wechselt dann automatisch zu „Live“.
- Eine wiederkehrende Kampagne, die gestartet wurde, zeigt „Live“ zusammen mit einer Zusammenfassung ihrer Wiederholung an (z. B. „Wöchentlich am Di, Do um 9:00 Uhr„).
- Wiederkehrende Kampagnen können so eingestellt werden, dass sie unbegrenzt („nie„) oder bis zu einem bestimmten Enddatum ausgeführt werden. Einmalige und sofortige Kampagnen haben keine Enddatumsoption, da sie einmal ausgeführt werden.
- Benutzer können den Zeitplan einer bereits gestarteten oder geplanten Kampagne bearbeiten, indem sie dieselben Zeitplanoptionen in den Kampagneneinstellungen verwenden.

## Verwendung

**So planen Sie eine Kampagne beim Start:**

1. Klicken Sie in der Kampagne auf **Startbereit**.
2. Wählen Sie im Launch-Dialogfeld die Option Zeitplan aus:
   - **Jetzt** - Die Kampagne wird sofort nach dem Start gesendet.
   - **Einmal planen** - Wählen Sie ein **Startdatum** (Datum und Uhrzeit zusammen).
   - **Wiederkehrend** - Wählen Sie eine **Häufigkeit** (täglich, wöchentlich oder monatlich) und eine Startzeit aus und legen Sie dann das Wiederholungsmuster fest (siehe Felder unten).
3. Wenn Wiederkehrend ausgewählt ist, wählen Sie aus, ob die Kampagne **Nie** oder **An einem Datum** endet, und wählen Sie gegebenenfalls ein Enddatum aus.
4. Bestätigen Sie, dass die Kampagne mit dem ausgewählten Zeitplan gestartet werden soll.

**So bearbeiten Sie einen vorhandenen Zeitplan:**

1. Öffnen Sie die Kampagne und wechseln Sie zu ihren Einstellungen.
2. Suchen Sie den Abschnitt Zeitplan und wählen Sie die aktuelle Zeitplanübersicht aus.
3. Aktualisieren Sie den Zeitplan mithilfe der oben beschriebenen Optionen.
4. Speichern Sie die Änderung.

### Eingabefelder/Parameter

| Feld | Beschreibung | Erforderlich? |
| --- | --- | --- |
| Zeitplanmodus | Auswahl von Jetzt, Zeitplan einmal oder Wiederkehrend | Ja |
| Startdatum | Datum und Uhrzeit des Starts der Kampagne (Zeitplanmodus) | Ja, einmal planen |
| Häufigkeit | Täglich, wöchentlich oder monatlich (wiederkehrender Modus) | Ja, für wiederkehrend |
| Startzeit | Tageszeit, zu der die wiederkehrende Kampagne sendet | Ja, für wiederkehrend |
| Wochentage | An welchen Tagen wird die Kampagne wiederholt? | Ja, für die wöchentliche Häufigkeit |
| Tag des Monats | An welchem Tag des Monats wird die Kampagne wiederholt | Ja, für die monatliche Häufigkeit |
| Kampagne beenden | Nie oder an einem bestimmten Enddatum | Ja, für wiederkehrend |

## Hinweise zur Benutzeroberfläche

> **Tech Writer Hinweis**: Für Folgendes sind Screenshots erforderlich:

- [ ] Das Launch-Dialogfeld mit den Optionen Jetzt / Zeitplan einmal / Wiederkehrend
- [ ] Die Datumsauswahl und die Zeitauswahl für den Zeitplan
- [ ] Die wiederkehrenden Optionen: Häufigkeitsauswahl, Wöchentliche Tag-Umschalter, Monatliches Tag-des-Monats-Raster
- [ ] Die Auswahl „Kampagne beenden“ Niemals/An einem Datum
- [ ] Das Status-Badge „Geplant“ für eine Kampagne, die auf ihren Start wartet
- [ ] Das Status-Badge „Live“ mit einer Wiederholungszusammenfassung (z. B. „Wöchentlich am Dienstag, Do um 9:00 Uhr„)
- [ ] In den Kampagneneinstellungen wird im Bereich Planung der Einstiegspunkt für die Bearbeitung angezeigt

## Was diese Funktion nicht tut

- Es unterstützt keine benutzerdefinierten Wiederholungsintervalle, wie „alle 2 Wochen“ oder „alle 3 Tage“ - nur die standardmäßigen täglichen, wöchentlichen oder monatlichen Häufigkeiten sind verfügbar.
- Relative monatliche Wiederholungen wie „der zweite Montag des Monats“ werden nicht unterstützt. Für „Monatlich“ ist nur eine bestimmte Auswahl von Tagen pro Monat verfügbar.
- Er bietet kein Enddatum für Kampagnen des Typs **Jetzt** oder **Einmal planen** - ein Enddatum ist nur verfügbar, wenn Wiederkehrend ausgewählt ist, da einmalige Kampagnen per Definition nur einmal ausgeführt werden.
