---
title: Data Management Agent für Adobe Experience Platform
description: Erfahren Sie, wie Sie mit dem Data Management Agent in CX Coworker Adobe Experience Platform-Datensätze finden und analysieren und die Data Lake-Aufbewahrungsrichtlinien verwalten können.
source-git-commit: 40f144c7a06592c78dccc6c17f19554b62f667c9
workflow-type: tm+mt
source-wordcount: '1016'
ht-degree: 3%
---
# Data Management Agent

>[!AVAILABILITY]
>
>Der Data Management Agent steht allen Kunden mit Zugriff auf Adobe CX Enterprise Coworker zur Verfügung.

Verwenden Sie den Data Management-Agenten in CX Coworker, um die Data Lake-Aufbewahrung für Ihre Erlebnisereignis-Datensätze zu verstehen und zu verwalten. Da die Anzahl der Erlebnisereignis-Datensätze in Ihrem Adobe Experience Platform Data Lake wächst, kann es länger dauern, bis Abfragen und nachgelagerte Prozesse abgeschlossen sind, während die Aufbewahrungsanforderungen schwieriger zu verwalten sind. Beschreiben Sie in natürlicher Sprache, was Sie erreichen möchten. Der Data Management-Agent findet die relevanten Erlebnisereignis-Datensätze, analysiert, wie aktiv sie verwendet werden, und modelliert, wie viele Daten sich eine vorgeschlagene Aufbewahrungsfrist auswirken würde. Wenn Sie bereit sind zu handeln, hilft Ihnen das beim Festlegen, Ändern oder Entfernen einer Aufbewahrungsrichtlinie und fordert Sie zur Bestätigung auf, bevor sich etwas ändert.

## Was der Data Management Agent tun kann {#what-the-data-management-agent-can-do}

Der Data Management Agent bietet vier Fähigkeiten.

>[!NOTE]
>
>Die Felder Datensätze auflisten, Datensatznutzung analysieren und Datensatzaufbewahrung analysieren sind schreibgeschützt. Nur die Fähigkeit zur Verwaltung der Datensatzaufbewahrung kann eine Data-Lake-Aufbewahrungsrichtlinie ändern. Vor der Anwendung einer Änderung ist eine ausdrückliche Bestätigung erforderlich.

| Skill | Beschreibung |
|---|---|
| **Datensätze auflisten** | Verwenden Sie diese Option, wenn Sie entscheiden, wo eine Aufbewahrungsüberprüfung gestartet werden soll. Listet Ihre Erlebnisereignis-Datensätze mit Speichergröße, Zeilenanzahl, vorhandenen Aufbewahrungseinstellungen und Profilaktivierung auf, damit Sie schnell Datensätze identifizieren können, die für eine Data-Lake-Aufbewahrungsrichtlinie infrage kommen |
| **Analysieren der Datensatznutzung** | Verwenden Sie , bevor Sie entscheiden, ob ein Datensatz ein guter Kandidat für eine Data-Lake-Aufbewahrungsrichtlinie ist. Klassifiziert anhand von Signalen wie „Zuletzt aufgenommen“, „Abfrageaktivität“ und „Nutzung nachgelagerter Anwendungen“, wie aktiv ein bestimmter Datensatz verwendet wird. |
| **Analysieren der Datensatzaufbewahrung** | Verwenden Sie , bevor Sie sich auf eine Aufbewahrungsfrist festlegen. Zeigt die Speichermetriken eines Datensatzes und das Alter seiner Daten an und verwendet diese Altersverteilung dann, um abzuschätzen, wie viele Daten eine potenzielle Aufbewahrungsfrist beibehalten oder entfernen würde. |
| **Verwalten der Datensatzaufbewahrung** | Verwende, wenn du bereit bist zu handeln. Legt eine Data-Lake-Aufbewahrungsrichtlinie für einen Datensatz fest, ändert sie oder entfernt sie, wobei eine Vorschau und Bestätigung der Auswirkungen angezeigt wird, bevor sich etwas ändert. |

## Umfang: Data-Lake-Aufbewahrung im Vergleich zu anderen Data-Management-Tools {#scope}

Verwenden Sie den Data Management-Agenten, wenn Sie Erlebnisereignis-Datensätze suchen und analysieren und eine Data-Lake-Aufbewahrungsrichtlinie festlegen, ändern oder entfernen möchten.

Wenn Sie nicht sicher sind, ob eine Data-Lake-Aufbewahrungsrichtlinie die richtige Option für Ihr Ziel ist, finden Sie unter [Wählen der richtigen Data-Lifecycle-Management-Funktion](https://experienceleague.adobe.com/en/docs/experience-platform/data-lifecycle/choose-a-capability) einen Vergleich der verfügbaren Aufbewahrungs- und Löschoptionen.

Diese Fähigkeiten verwalten nicht die folgenden zugehörigen Funktionen:

- **Richtlinie zur Aufbewahrung von Profilspeichern.** Um zu verwalten, wie lange Erlebnisereignisse im Profilspeicher verbleiben, konfigurieren Sie eine Gültigkeitsrichtlinie für Erlebnisereignisse in profilaktivierten Erlebnisereignis-Datensätzen. Siehe [Ablauf von Erlebnisereignissen](https://experienceleague.adobe.com/de/docs/experience-platform/profile/event-expirations).
- **Ablauf von Daten pseudonymer Profile über Sandbox.** Informationen zum automatischen Löschen pseudonymer Profildaten in einer Sandbox, sobald sie die konfigurierten Bedingungen erfüllen, finden Sie unter [Pseudonyme Profile](https://experienceleague.adobe.com/de/docs/experience-platform/profile/pseudonymous-profiles).
- **Datensatzgültigkeit.** Informationen zum Planen des Löschens eines gesamten Datensatzes für ein künftiges Datum finden Sie unter [Datensatzgültigkeit](https://experienceleague.adobe.com/en/docs/experience-platform/data-lifecycle/ui/dataset-expiration).
- **Datensatz löschen.** Informationen zum Entfernen einzelner Profildatensätze aus Datenschutz- oder Hygienegründen finden Sie unter [Löschen von Datensätzen](https://experienceleague.adobe.com/en/docs/experience-platform/data-lifecycle/ui/record-delete).

## Voraussetzungen {#prerequisites}

Bevor Sie beginnen, stellen Sie Folgendes sicher:

- Zugriff auf Adobe Experience Platform und die Sandbox, die die Datensätze enthält, die Sie überprüfen möchten.
- Die Adobe Experience Platform-Berechtigungen, die für die Datensätze und Aufbewahrungsaktionen erforderlich sind, die Sie verwenden möchten. Der Data Management Agent verwendet Ihre bestehenden Experience Platform-Berechtigungen und gewährt keinen zusätzlichen Zugriff. Informationen zur Funktionsweise von [&#x200B; und Rollen finden &#x200B;](https://experienceleague.adobe.com/de/docs/experience-platform/access-control/home) in der Übersicht zur Zugriffskontrolle .
- Das in CX Coworker installierte Adobe CXO-Plug-in.

Anweisungen zum Installieren von Plug-ins finden Sie im [Handbuch zur Coworker-Benutzeroberfläche](https://experienceleague.adobe.com/en/docs/cx-enterprise-ai/experience-cloud-ai/coworker/chat/ui-guide).

## Verwenden des Daten-Management-Agenten {#use-the-data-management-agent}

Interagieren Sie mit dem Data Management Agent über CX Coworker in natürlicher Sprache. Beschreiben Sie Ihr Ziel und verfeinern Sie dann die Ergebnisse mit Folgefragen.

>[!NOTE]
>
>Bevor Sie beginnen, stellen Sie sicher, dass Sie in der Sandbox arbeiten, die die Datensätze enthält, die Sie überprüfen möchten.

So verwenden Sie den Data Management-Agenten:

1. Navigieren Sie zu **[!UICONTROL CX Coworker]**. Weitere Informationen zum Zugriff finden Sie im [Handbuch zur Coworker-Benutzeroberfläche](https://experienceleague.adobe.com/en/docs/cx-enterprise-ai/experience-cloud-ai/coworker/chat/ui-guide).
1. Geben Sie eine Anforderung ein, die beschreibt, was Sie erreichen möchten.
1. Überprüfen Sie die Ergebnisse und verwenden Sie Folgefragen, um Ihre Untersuchung fortzusetzen.

Wenn eine Anfrage eine Data-Lake-Aufbewahrungsrichtlinie ändert, zeigt der Data Management-Agent die vorgeschlagenen Auswirkungen an und benötigt Ihre Bestätigung, bevor die Änderung angewendet wird.

Einen End-to-End-Workflow zur Identifizierung von Datensätzen, zur Analyse der Auswirkungen auf Nutzung und Aufbewahrung und zur Verwaltung von Data Lake-Aufbewahrungsrichtlinien finden Sie [Verwalten der Data Lake-Aufbewahrung](../coworker/chat/use-cases/data-management/manage-data-lake-retention.md).

## Funktionsweise des Data Management-Agenten {#how-the-data-management-agent-works}

Der Data Management Agent verwendet deterministische Berechnungen, um die Datensatznutzung zu analysieren, sodass dieselben Eingaben dieselbe Nutzungsstufe ergeben. Außerdem berechnet sie die Retentionswirkung programmgesteuert, anstatt sich auf KI-generierte Schätzungen zu verlassen. Die Auswirkungen der Datenspeicherung bleiben Näherungswerte, da sie auf der Altersverteilung der Daten basieren. Der Agent ruft Daten direkt von Adobe Experience Platform-Services ab, um aktuelle Informationen zu Ihren Datensätzen bereitzustellen.

## Einschränkungen {#limitations}

Der Data Management-Agent kann Datensätze identifizieren, die sich gut für eine Data-Lake-Aufbewahrungsrichtlinie eignen, entscheidet jedoch nicht, ob ein Datensatz einen erfordert. Eine Aufbewahrungsrichtlinie wird ohne Ihre ausdrückliche Bestätigung nicht angewendet, geändert oder entfernt.

## Nächste Schritte {#next-steps}

Eine Anleitung zur Verwendung der einzelnen Kenntnisse zum Suchen, Analysieren und Verwalten der Data Lake-Aufbewahrung in Ihren Experience Event-Datensätzen finden Sie [Verwalten der Data Lake-Aufbewahrung](../coworker/chat/use-cases/data-management/manage-data-lake-retention.md).

Weitere Informationen zur Funktionsweise von Data-Lake-Aufbewahrungsrichtlinien in Adobe Experience Platform, einschließlich Aufbewahrungsverhalten und Konfiguration, finden Sie [&#x200B; Handbuch zur Erlebnisereignis-Datensatzaufbewahrung (TTL)](https://experienceleague.adobe.com/en/docs/experience-platform/catalog/datasets/experience-event-dataset-retention-ttl-guide).
