---
title: Journey Optimizer-Tools in CX Coworker Gateway
description: Erfahren Sie, welche Adobe Journey Optimizer-Tools über das CX Coworker Gateway verfügbar sind.
source-git-commit: 4bc180a76f3c1095a4d25ed7e07d804e4d5ff1a9
workflow-type: tm+mt
source-wordcount: '533'
ht-degree: 3%

---

# Adobe Journey Optimizer-Tools in CX Coworker Gateway {#ajo-mcp}

Verwenden Sie die Adobe Journey Optimizer-Produkt-Tools, um Kampagnen und Kanalkonfigurationen von einem MCP-kompatiblen Client aus zu überprüfen. Diese Tools sind über das [CX Coworker Gateway](overview.md) verfügbar, wenn Ihr Unternehmen aktiviert ist und Ihr Benutzerkonto über die erforderlichen Journey Optimizer-Berechtigungen verfügt.

>[!AVAILABILITY]
>
>Die Journey Optimizer-Produkt-Tools befinden sich in Beta. Der Zugriff erfolgt nur auf Einladung und erfordert die Aktivierung durch die Adobe-Organisation. Siehe [Zugriff auf CX Coworker Gateway-Tools](access.md).

## Wichtigste Funktionen {#mcp-capabilities}

Journey Optimizer-Tools bieten eine schreibgeschützte Oberfläche zur Überprüfung der Kampagnen- und Kanalkonfiguration. Sie haben folgende Möglichkeiten:

- Journey Optimizer-Kampagnen auflisten und nach Status filtern.
- Abrufen von Kampagnendetails, einschließlich Zielgruppenbestimmung, Zeitplan, Kanal und Inhaltskonfigurations-Metadaten.
- Listen Sie Kanalkonfigurationen für E-Mail-, SMS-, Push- und WhatsApp-Kanäle auf.
- Überprüfen Sie die Einrichtung von Kampagnen und Kanälen in natürlicher Sprache ohne Navigation durch die Produktbildschirme.

>[!IMPORTANT]
>
>Alle Journey Optimizer-Tools in der aktuellen Beta sind schreibgeschützt. Das Erstellen, Aktualisieren, Löschen, Starten, Beenden oder Veröffentlichen von Kampagnen wird nicht unterstützt.

## Verfügbare Tools {#mcp-tools}

| Tool | Beschreibung |
| --- | --- |
| `ajo_campaign_list` | Durchsuchen Sie Journey Optimizer Marketing-Kampagnen. Unterstützt das Filtern nach Status wie `DRAFT`, `LIVE`, `STOPPED` und `COMPLETED`. |
| `ajo_campaign_get` | Abrufen von Details und Konfiguration für eine bestimmte Kampagne nach ID, einschließlich Zielgruppen-Targeting, Zeitplan, Kanal- und Inhaltseinstellungen und Metadaten. |
| `ajo_channel_configuration_list`, `ajo_channel_configuration_get` | Anzeigen von Oberflächenvorgaben und Branding-Einstellungen für E-Mail-, SMS-, Push- oder [!DNL WhatsApp]. |

## Beispiel-Eingabeaufforderungen {#mcp-use-cases}

| Ziel | Beispiel-Eingabeaufforderung |
| --- | --- |
| Kampagnen-Überblick | „Alle meine Journey Optimizer-Kampagnen anzeigen.“ |
| Statusprüfung | „Welche Kampagnen sind derzeit aktiv?“ |
| Kampagnendetails | „Vollständige Details zu Campaign `[campaign ID]`.“ |
| Zielgruppe und Zielgruppenbestimmung | „Welche Zielgruppe wird in Campaign `[campaign ID]` angesprochen?“ |
| Zeitplan und Zeitplan | „Wann soll Campaign `[campaign ID]` ausgeführt werden?“ |
| Fehlerbehebung | „Überprüfen Sie die Einrichtung von Campaign `[campaign ID]` und markieren Sie mögliche Probleme.“ |
| Kanalkonfiguration | „Welche E-Mail-Kanal-Konfigurationen sind verfügbar?“ |
| Kanalprüfung | „Welche Kanalkonfigurationen fehlen oder sind unvollständig?“ |

## Produktkontext und Berechtigungen {#mcp-context}

Ihr Benutzerkonto muss über die Berechtigung zum Anzeigen der von Ihnen abgefragten Journey Optimizer-Kampagnen und Kanalkonfigurationen verfügen. Der MCP umgeht keine Produktberechtigungen.

Wenn Ihr Unternehmen mehrere Sandboxes verwendet, geben Sie die Sandbox oder den Umgebungskontext in der Eingabeaufforderung an, wenn Sie Ergebnisse aus einer bestimmten Sandbox benötigen.

## Bekannte Einschränkungen {#mcp-limitations}

| Einschränkung | Beschreibung | Problemumgehung |
| --- | --- | --- |
| Schreibgeschützte Oberfläche | Journey Optimizer-Tools machen nur Abrufvorgänge verfügbar. Sie können keine Kampagnen erstellen, aktualisieren, löschen, starten, stoppen oder veröffentlichen. | Verwenden Sie die Journey Optimizer-Benutzeroberfläche oder APIs für Schreibvorgänge. |
| Keine Interaktion oder Leistungsmetriken | Tools geben keine Berichtsdaten wie Impressionen, Clickthrough-Raten, Konversionen oder Versandstatistiken zurück. | Verwenden Sie Journey Optimizer-Reporting, Customer Journey Analytics-Tools oder Adobe Analytics-Tools für Leistungsmetriken. |
| Die Paginierung der Kampagnenliste ist begrenzt | Die Kampagnenauflistung gibt die erste Ergebnisseite mit bis zu 50 alphabetisch sortierten Kampagnen zurück. Versatz- und Grenzwerte werden nicht angewendet. | Wenn die Kampagnen-ID bekannt ist, können Sie `Get Campaign` direkt verwenden. Verwenden Sie die Journey Optimizer-Benutzeroberfläche für das vollständige Durchsuchen und Filtern. |
| Keine Server-seitige Filterung nach Datum, Kanal oder Zeitplan | Die Kampagnenauflistung unterstützt die Statusfilterung, jedoch nicht die Filterung von Veröffentlichungsdatum, Zeitplandatum, Kanal oder Kampagnentyp. | Verwenden Sie die Kampagnenliste der Journey Optimizer-Benutzeroberfläche für die native Datums- und Kanalfilterung. |
| Abruf des Nachrichteninhalts nicht verfügbar | Nachrichten-HTML, Betreffzeilen, Personalisierungs-Token und Angebotsinhalte sind in den aktuellen Tools nicht verfügbar. | Anzeigen des Nachrichteninhalts und der Personalisierung direkt in der Journey Optimizer-Benutzeroberfläche. |