---
description: Die Beschreibung ist hier zu finden.
title: Starten einer Kampagne
feature_v2: id: fdae8433-07cd-42e7-acce-738afe63f6bb
source-git-commit: 1c4f9585c04eae8693e38541084cead08412d192
workflow-type: tm+mt
source-wordcount: 757
ht-degree: 0%

---

# Starten einer Kampagne {#launch-campaign}

Das Starten einer Kampagne ist die Aktion, mit der sie vom Entwurf zum aktiven Versand verschoben wird. Bevor das Launch-Dialogfeld geöffnet wird, prüft Halo, ob die Kampagne bereit ist, und blockiert den Launch, bis die erforderliche Einrichtung abgeschlossen ist. Das Launch-Dialogfeld zeigt eine Vorschau der E-Mail und der Audience an, ermöglicht es dem Benutzer, den Versandzeitplan inline zu überprüfen oder zu ändern, und meldet, ob der Launch erfolgreich war. Dieser Abschnitt enthält Informationen zum End-to-End-Launch. Die während des Launches angebotenen Zeitplanoptionen finden Sie unter [Planen einer Kampagne](/help/coworker/campaigns/schedule-campaign.md).

## Voraussetzungen

- Die Kampagne muss den Status Entwurf haben. <!-- The Launch action isn't available once a campaign is already live. -->
<!-- - The campaign must pass a readiness check: sending settings configured, at least one test email sent, and a real (non-sample) audience uploaded. -->
- [BENÖTIGT EINGABE - Bestätigung durch einen Techniker: Einige Benutzer sehen möglicherweise ein „In Kürze verfügbar“-Erlebnis anstelle einer echten Launch-Schaltfläche, über die nur die Kampagne heruntergeladen oder eine Korrekturabzugs-E-Mail gesendet werden kann, anstatt die In-App zu starten. Bestätigen, was bestimmt, welches Erlebnis ein bestimmter Benutzer oder eine bestimmte Kampagne erhält.]

## Funktionsweise dieser Funktion

Wenn ein Benutzer eine Kampagne startet, prüft Halo zunächst, ob die Kampagne bereit ist. Wenn ein erforderliches Element fehlt, wird in einem Dialogfeld aufgelistet, was behoben werden muss, bevor der Launch fortgesetzt werden kann. Nach erfolgreicher Validierung zeigt das Launch-Dialogfeld eine Vorschau der E-Mail und der Audience/des Workflows an, ermöglicht es dem Benutzer, den Versandzeitplan zu überprüfen oder zu bearbeiten, ohne den Fluss zu verlassen, und zeigt bei großen Sendungen eine Benachrichtigung über das geschätzte Versandvolumen an. Bei der Bestätigung der Trigger und Halo-Berichten gibt es drei Ergebnisse: Start, bereits gestartet oder fehlgeschlagen.

### Wichtigste Verhaltensweisen

- Der Launch ist nur für Kampagnen mit dem Status Entwurf verfügbar. Eine Kampagne, die bereits live ist, kann nicht erneut gestartet werden.
- Eine Bereitschaftsprüfung wird automatisch ausgeführt, bevor das Launch-Dialogfeld geöffnet wird. Nicht gelöste Probleme blockieren Launch und werden mit einer Möglichkeit zur Lösung jedes Problems aufgelistet.
- Das Launch-Dialogfeld zeigt eine E-Mail-Vorschau (Betreff, Preheader, Absender) und eine Audience-/Workflow-Vorschau.
- Der Versandzeitplan kann im Launch-Dialogfeld überprüft oder geändert werden.
- Bei großen Sendungen zeigt das Dialogfeld die geschätzte Wirkung des Versandvolumens an. [EINGABE ERFORDERLICH - Der genaue Wortlaut dieser Mitteilung war nicht im Code verfügbar]
- Bei Erfolg wird der Status der Kampagne auf „Geplant“ oder „Live“ (je nach ausgewähltem Zeitplan) aktualisiert, und eine Bestätigungsmeldung weist darauf hin, dass Kampagneneinblicke innerhalb von 2 Stunden verfügbar sind.
- Wenn die Kampagne bereits gestartet wurde (z. B. durch einen doppelten Klick), zeigt Halo anstelle eines Fehlers die Meldung „bereits gestartet“ an.
- Wenn der Launch fehlschlägt, wird eine Fehlermeldung angezeigt und die Kampagne verbleibt im Entwurfsmodus. Der/die Benutzende kann es erneut versuchen.
- Nachdem eine Kampagne <!--(see [Stop a live campaign](./stop-live-campaign.md))--> gestoppt wurde, kann sie nicht mehr aus demselben Kampagnendatensatz neu gestartet werden - das Stoppen ist ein separater, permanenter Status.

## Zugriff

**So starten Sie eine Kampagne:**

1. Klicken Sie in der Kampagne auf **Starten** (angezeigt als „Bereit zum Start“, während Sie sich noch im Entwurf befinden).
2. Wenn etwas fehlt, listet ein Dialogfeld mit dem Titel „Einige Dinge müssen noch beachtet werden“ auf, was abgeschlossen werden muss:
   - **E-Mail-Einstellungen konfigurieren** - Versandparameter (Absender/Domain) wurden noch nicht eingerichtet.
   - **E-Mails nicht getestet** - Senden Sie vor dem Start mindestens eine Test-E-Mail, um die E-Mail zu überprüfen.
   - **Für den Start ist eine echte Zielgruppe erforderlich** - Die Kampagne verwendet weiterhin eine Beispielzielgruppe. Laden Sie eine echte Zielgruppen-CSV hoch.
     Lösen Sie jedes Element auf und versuchen Sie dann erneut, Launch durchzuführen.
3. Sobald die Kampagne die Bereitschaftsprüfung bestanden hat, wird das Launch-Dialogfeld geöffnet, in dem eine Vorschau der E-Mail und der Audience angezeigt wird.
4. Überprüfen Sie den im Dialogfeld angezeigten Zeitplan. Um sie zu ändern, verwenden Sie die Zeitplanoptionen, die unter [Bei Kampagnenstart planen](/help/coworker/campaigns/schedule-campaign.md) beschrieben sind, und speichern Sie dann.
5. Starten bestätigen. Bei Erfolg wird eine Bestätigungsmeldung angezeigt und der Status der Kampagne wird aktualisiert (auf „Geplant“ oder „Live„).

<!-- 
## Input fields / parameters

Not applicable beyond the schedule fields already documented in [Schedule when a campaign launches](/help/coworker/campaigns/schedule-campaign.md) — launching itself doesn't require any additional input. 
-->

## Hinweise zur Benutzeroberfläche

> **Tech Writer Hinweis**: Für Folgendes sind Screenshots erforderlich:

- [ ] Der Einstiegspunkt/die Schaltfläche „Launch“ in der Kopfzeile mit Kampagnendetails
- [ ] Das Dialogfeld Bereitschaft/Validierung, in dem unvollständige Elemente aufgelistet werden
- [ ] Das Launch-Dialogfeld mit der Vorschau der E-Mail + Audience und dem Abschnitt „Zeitplan“
- [ ] Die geschätzte Wirkung des Sendevolumens (für große Zielgruppen)
- [ ] Die Erfolgsbestätigungsmeldung nach dem Start
- [ ] Die Nachricht „Bereits gestartet“
- [ ] Die generische Fehlermeldung bei einem Start

## Was diese Funktion nicht tut

- Es wird keine Kampagne mit einer (nicht realen) Beispielzielgruppe, ungetesteten E-Mails oder nicht konfigurierten Versandeinstellungen gestartet. Alle drei müssen zuerst aufgelöst werden.
- Beim Starten wird kein Zeitplan als Teil derselben Aktion akzeptiert. Der Zeitplan wird separat (im selben Dialogfeld) gespeichert, bevor oder als Teil der Launch-Bestätigung.
- Es unterstützt nicht den Neustart einer gestoppten Kampagne - das Anhalten ist eine dauerhafte <!--(see [Stop a live campaign](./stop-live-campaign.md))-->.
- [EINGABE ERFORDERLICH - Bestätigung durch Techniker/PM: Für einige Benutzende wird Launch möglicherweise durch ein „In Kürze erscheinendes“ Erlebnis ersetzt, das nur Kampagnendownload (PDF/DOCX) oder Testversand per E-Mail bietet, ohne dass ein In-App-Self-Service-Launch durchgeführt werden muss. Bestätigen Sie die Zielgruppe, für die dies gilt, vor der Veröffentlichung, da dadurch die Anleitungsschritte für diese Kohorte geändert werden.]
