---
description: Beschreibung.
title: Grundlegendes zum E-Mail-Editor
source-git-commit: e5992ce91452c98e043e8367d7cc551d6914647b
workflow-type: tm+mt
source-wordcount: '707'
ht-degree: 0%

---

# Grundlegendes zum E-Mail-Editor {#email-editor}

Mit dem E-Mail-Editor können Sie eine von KI generierte E-Mail direkt im Kampagnenboard einschränken. Bearbeiten Sie die Betreffzeile und den Preheader, formatieren Sie Text und Bilder inline oder tauschen Sie sie in einer anderen Vorlage aus. <!-- It's an inline editor over the email's actual HTML, not a drag-and-drop block builder. -->

>[!PREREQUISITES]
>
>Erstellen Sie eine Kampagne mit einer generierten E-Mail.

## Funktionsweise dieser Funktion

Wenn Sie auf eine E-Mail-Karte auf dem Campaign-Board klicken, wird der E-Mail-Editor als Seitenbereich geöffnet. Dort kann der Benutzer den Betreff und den Preheader bearbeiten (mit von KI vorgeschlagenen Alternativen), auf den E-Mail-Textkörper klicken, um Text oder Bilder auszuwählen und zu formatieren, zwischen KI-generierten Varianten wechseln, die HTML-Vorlage austauschen, die Kompatibilität mit dem E-Mail-Client überprüfen und eine Test-E-Mail an den eigenen Posteingang senden. Änderungen werden automatisch gespeichert und frühere Versionen können überprüft und wiederhergestellt werden.

### Wichtigste Verhaltensweisen

- Wenn Sie auf einen Text oder ein Bild im E-Mail-Textkörper klicken, wird dieser ausgewählt und eine unverankerte Formatierungssymbolleiste angezeigt.
- Optionen zur Textformatierung: Fett, Kursiv, Unterstrichen, Schriftart und Schriftgröße.
- Bildoptionen: Ersetzen, Löschen, Verknüpfen, Bearbeiten mit Express, Bild generieren (AI), Hochladen vom Computer.
- Bild-Uploads sind auf 10 MB begrenzt; Bilder über etwa 3 MB werden automatisch komprimiert, wobei ein Qualitätshinweis Bilder unter 3 MB empfiehlt.
- Die Betreff- und Preheader-Felder verfügen jeweils über eine Option „Smart Suggestions“ für KI-generierte Alternativen.
- Changes auto save (on blur, and short after formatting actions) - Ein Statusindikator zeigt Unsaved Changes, Saving…, Saved, AutoSaved oder Cannot save (with a Retry option) an.
- Rückgängig/Wiederholen ist für die aktuelle Bearbeitungssitzung verfügbar.
- Frühere gespeicherte Versionen können über ein Bedienfeld „Versionsverlauf“ in der Vorschau angezeigt und wiederhergestellt werden.
- Wenn mehrere KI-generierte Varianten vorhanden sind, kann der Benutzer über ein Miniaturbild-Bedienfeld zwischen ihnen wechseln.
- Die HTML-Vorlage der E-Mail kann mit &quot;HTML-Vorlage wechseln“ ausgetauscht werden.
- „Test-E-Mail senden“ sendet eine echte Vorschau mithilfe von Beispieldaten an den eigenen Posteingang der Benutzenden. Dies wirkt sich nicht auf das Reporting in Campaign aus.
- In einigen Umgebungen ist eine Kompatibilitätsprüfung des E-Mail-Clients verfügbar, die Gmail, Outlook, Apple Mail, Yahoo Mail, Samsung Email und Thunderbird umfasst. [EINGABE ERFORDERLICH - Dies befindet sich hinter einem Feature Flag. Überprüfen Sie, ob es für die Zielgruppe aktiviert ist, bevor Sie es als allgemein verfügbar dokumentieren]

## Zugriff

1. Öffnen Sie die gewünschte Kampagne und klicken Sie in der E-Mail-Karte auf Editor öffnen .

SCREENSHOT

1. Bearbeiten Sie die Felder **Betreff** und **Preheader** direkt oder klicken Sie **Smart-Vorschläge** neben für KI-generierte Alternativen.
1. Klicken Sie in den E-Mail-Textkörper, um einen Textblock oder ein Bild auszuwählen, und verwenden Sie dann die unverankerte Symbolleiste, die angezeigt wird, um den Text zu formatieren oder das Bild zu verwalten.
1. Verwenden Sie **HTML-Vorlage wechseln** um den E-Mail-Textkörper durch eine andere Vorlage zu ersetzen.
1. Verwenden Sie **Test-E** Mail senden), geben Sie eine Empfängeradresse ein und klicken Sie auf **Senden**, um eine Live-Vorschau an diese Adresse zu senden.
1. Verwenden Sie das Symbol Versionsverlauf , um eine frühere gespeicherte Version in der Vorschau anzuzeigen und wiederherzustellen.
1. Änderungen werden automatisch gespeichert - es ist kein manueller Speicherschritt erforderlich.

### Eingabefelder/Parameter

| Feld | Beschreibung | Erforderlich? |
| --- | --- | --- |
| Betreff | Die Betreffzeile der E-Mail | Nein (kann leer gelassen werden; wird derzeit nicht erzwungen) |
| Preheader | Der Vorschautext wird neben dem Betreff in einem Posteingang angezeigt | Nein |
| E-Mail-Adresse des Empfängers | Senden einer Test-E-Mail | Ja, für Test-E-Mail senden |

## Hinweise zur Benutzeroberfläche

> **Tech Writer Hinweis**: Für Folgendes sind Screenshots erforderlich:

- [ ] Seitenbereich des E-Mail-Editors (Betreff/Preheader-Felder plus E-Mail-Textkörper)
- [ ] Die unverankerte Symbolleiste für die Textauswahl
- [ ] Die unverankerte Symbolleiste für die Bildauswahl
- [ ] Bedienfeld „Miniaturansichten der KI-Variante“
- [ ] Bedienfeld „Versionsverlauf“
- [ ] Dialogfeld &quot;HTML-Vorlage wechseln“
- [ ] Dialogfeld Test-E-Mail senden
- [ ] Die Kompatibilitätsprüfung E-Mail-Client (wenn in der Zielumgebung aktiviert)

## Was diese Funktion nicht tut

- Es handelt sich nicht um einen Drag-and-Drop-Block-Builder - es gibt keine Blockbibliothek. Inhaltsblöcke können nicht hinzugefügt, entfernt oder neu angeordnet werden. Die Bearbeitung erfolgt direkt auf der vorhandenen E-Mail-HTML.
- Das Einfügen von Personalisierungs-/Zusammenführungs-Tags wird derzeit nicht unterstützt.
- Es wird kein Feld für Alternativtext für Bilder bereitgestellt.
- Es werden keine Betreffzeile, kein Preheader oder andere Prüfungen auf Inhaltsebene erzwungen, bevor eine E-Mail als „bereit“ erachtet wird. Die einzigen Prüfungen vor dem Start sind auf Kampagnenebene (Sendeeinrichtung, gesendete Test-E-Mail, eine echte Zielgruppe), nicht auf den E-Mail-Inhalt selbst.
- Das Umschalten der Desktop-/Mobile-Vorschau ist in der standardmäßigen Bearbeitungsansicht von Kampagnen-E-Mails nicht verfügbar. [BENÖTIGT EINGABE zur Bestätigung des Umfangs]
- [EINGABE ERFORDERLICH - Bestätigung durch einen Techniker: Ob der Editor nach der Aktivierung/dem Start einer Kampagne vollständig schreibgeschützt ist (nicht nur das Feld „Absender„)]
