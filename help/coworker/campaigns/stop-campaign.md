---
description: Die Beschreibung ist hier zu finden.
title: Stoppen einer Kampagne
feature_v2: id: fdae8433-07cd-42e7-acce-738afe63f6bb
source-git-commit: 1c4f9585c04eae8693e38541084cead08412d192
workflow-type: tm+mt
source-wordcount: 410
ht-degree: 1%

---

# Stoppen einer Kampagne {#stop-campaign}

Benutzer können jetzt eine Kampagne, die aktiv eine „Live“-Kampagne sendet, direkt über die Seite mit den Kampagnendetails stoppen. Das Stoppen einer Kampagne ist dauerhaft: Empfänger und Empfängerinnen hören sofort auf, die Kampagne zu durchlaufen, und die Kampagne kann danach nicht fortgesetzt oder neu gestartet werden.

## Voraussetzungen

- Die Kampagne muss live (aktiv versendet) sein. Die Stopp-Aktion ist nicht für Kampagnen des Typs Entwurf, geplant oder bereits angehalten verfügbar.
- [EINGABE ERFORDERLICH - Bestätigung durch Techniker: Erfordert das Stoppen einer Kampagne eine bestimmte Rolle oder Berechtigung, oder kann dies irgendein Benutzer mit Kampagnenzugriff tun?]

## Funktionsweise dieser Funktion

Eine Aktion „Kampagne stoppen“ wird in der Kopfzeile „Kampagnendetails“ angezeigt, wenn eine Kampagne live ist. Wenn Sie diese Option auswählen, wird ein Bestätigungsdialogfeld geöffnet, in dem Sie darauf hingewiesen werden, dass die Aktion dauerhaft ist. Bei Bestätigung wird das Backend aufgerufen, um die Kampagne zu stoppen. Bei Erfolg ändert sich der Status der Kampagne in „Gestoppt“ und eine Bestätigungsmeldung wird angezeigt.

### Wichtigste Verhaltensweisen

- Die Aktion Kampagne stoppen wird nur angezeigt, während eine Kampagne live ist (aktiv sendet).
- Anhalten ist dauerhaft: Empfänger hören auf, die Kampagne zu durchlaufen, und sie kann nicht fortgesetzt werden.
- In einem Bestätigungsdialogfeld muss der Benutzer dies explizit bestätigen, bevor die Kampagne gestoppt wird.
- Nach dem Stoppen wird das Status-Badge der Kampagne auf „Gestoppt“ aktualisiert.
- Wenn die Stopp-Anfrage fehlschlägt, wird eine Fehlermeldung angezeigt und die Kampagne bleibt live.

## Verwendung

1. Öffnen Sie eine Kampagne, die derzeit live ist (aktiv sendet).
2. Klicken Sie in der Kopfzeile der Kampagnendetails auf **Kampagne stoppen**.
3. Überprüfen Sie im Bestätigungsdialog die Warnung: „Das Stoppen der Kampagne ist dauerhaft. Alle Empfänger werden nicht mehr weiterentwickelt, und die Kampagne kann nicht fortgesetzt werden.“
4. Klicken Sie zur Bestätigung auf **Stoppen**.
5. Eine „Kampagne gestoppt“. Eine Bestätigungsmeldung wird angezeigt und der Status der Kampagne wird auf „Angehalten“ aktualisiert.

### Eingabefelder/Parameter

Nicht zutreffend : Diese Funktion ist eine einzelne Bestätigungsaktion ohne Eingabefelder.

## Hinweise zur Benutzeroberfläche

> **Tech Writer Hinweis**: Für Folgendes sind Screenshots erforderlich:

- [ ] Die Schaltfläche „Kampagne stoppen“ in der Kopfzeile der Kampagnendetails, angezeigt in einer Live-Kampagne
- [ ] Das Bestätigungsdialogfeld mit der Permanenzwarnung
- [ ] Das Status-Badge „Angehalten“ nach einem erfolgreichen Stopp
- [ ] Die Fehlermeldung, die angezeigt wird, wenn das Anhalten fehlschlägt

## Was diese Funktion nicht tut

- Eine Kampagne wird dadurch nicht vorübergehend angehalten. Es gibt keine Möglichkeit, eine gestoppte Kampagne fortzusetzen. Das Anhalten ist eine unidirektionale Aktion.
- Der Neustart oder Neustart einer gestoppten Kampagne aus demselben Kampagnendatensatz wird nicht unterstützt.
- [EINGABE ERFORDERLICH - Bestätigung mit Techniker: Ist eine separate Pause- und Wiederaufnahmefunktion geplant oder ist Stopp die einzige Aktion zur Statuskontrolle, die in dieser Version bereitgestellt wird?]
