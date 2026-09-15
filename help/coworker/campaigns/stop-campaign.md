---
description: Die Beschreibung ist hier zu finden.
title: Stoppen einer Kampagne
product_v2:
  - id: fdae8433-07cd-42e7-acce-738afe63f6bb
    internal-label: CX Enterprise Coworker
feature_v2:
  - id: fdae8433-07cd-42e7-acce-738afe63f6bb
    internal-label: CX Enterprise Coworker
source-git-commit: a8859659a5d4d5820d77bf93df62550f10999ea4
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 0%
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
