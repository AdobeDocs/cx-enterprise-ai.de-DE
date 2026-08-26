---
title: Transparenz des generativen KI-Inhalts
description: Erfahren Sie, wie Adobe automatisch C2PA-Metadaten an von GenAI generierte und von GenAI bearbeitete Inhalte in Adobe CX Enterprise-Anwendungen anhängt.
feature_v2:
  - id: f84b2906-3ce9-4ef0-86f6-cda249273937
  - id: ec4263d9-bf7c-44c7-b3f1-3e664861c8f2
source-git-commit: 02de82fd17bdf3f806ce120b93cbbd85b50f9b8a
workflow-type: tm+mt
source-wordcount: 1539
ht-degree: 1%

---


# Transparenz des generativen KI-Inhalts

Im August 2026 führt Adobe schrittweise die Unterstützung von C2PA-Metadaten in Adobe Creative Cloud, Adobe Document Cloud, Adobe Firefly und Adobe CX Enterprise-Anwendungen ein.

>[!NOTE]
>
>Nach dem Rollout erhalten zukünftige Workflows, bei denen Inhalte mithilfe von KI erstellt oder bearbeitet werden, automatisch C2PA-Metadaten-Unterstützung.

Auf dieser Seite wird beschrieben, wie Adobe das automatische Anhängen von C2PA-Metadaten an Adobe CX Enterprise-Anwendungen verarbeitet.

Neue Vorschriften verlangen von Anbietern generativer KI-Technologien, dauerhafte, maschinenlesbare Offenlegungen zu unterstützen, die mit durch GenAI generierten und durch GenAI bearbeiteten Inhalts-Workflows verbunden sind, um die Transparenz zu erhöhen.

Als Tool-Anbieter fügt Adobe mithilfe von Adobe-Technologien (einschließlich unterstützter generativer KI-Modelle von Drittanbietern innerhalb von Adobe-Workflows) automatisch maschinenlesbare C2PA-Metadaten an GenAI-generierte und GenAI-bearbeitete Inhalte an. [Weitere Informationen zu C2PA](https://c2pa.org/).

## Änderungen

Ab August 2026 führt Adobe die Unterstützung von C2PA-Metadaten für Adobe Creative Cloud, Adobe Document Cloud, Adobe Firefly und Adobe CX Enterprise-Anwendungen ein.

Diese Version umfasst:

* Automatisches Anhängen von C2PA-Metadaten an unterstützte GenAI-generierte und GenAI-bearbeitete Inhalte.
* Unterstützung für Inhaltstypen wie Bilder, Video, Audio und Text.
* Beibehaltung von C2PA-Metadaten in allen unterstützten Adobe-Workflows.

Es ist keine zusätzliche Aktion erforderlich, um C2PA-Metadaten an qualifizierte generative KI-Inhalte anzuhängen.

>[!NOTE]
>
>C2PA-Metadaten wirken sich nicht auf die Darstellung Ihrer Inhalte aus. C2PA-Metadaten und sichtbare Wasserzeichen dienen verschiedenen Zwecken. C2PA-Metadaten bieten maschinenlesbare Informationen zur Provenienz, während sichtbare Wasserzeichen für visuelle Offenlegung sorgen. Je nach den geschäftlichen Anforderungen und den rechtlichen Anforderungen der jeweiligen Gerichtsbarkeit können Sie Ihren Inhalten sichtbare Wasserzeichen hinzufügen.

## Welche Details werden als Teil der C2PA-Metadaten hinzugefügt?

Automatisch angehängte C2PA-Metadaten können Informationen enthalten wie:

* Name und Versionsinformationen des verwendeten KI-Systems (z. B. Adobe GenStudio, Adobe Firefly)
* Verwendetes KI-Modell (z. B. Adobe Firefly)
* Nutzung: Ob sie mit GenAI generiert oder bearbeitet wurde
* Zeit und Datum der Inhaltserstellung und/oder -änderung mit generativen KI-Tools
* Eindeutige Kennung (die zur Unterscheidung jeder Verwendung der generativen KI verwendet werden kann)

## C2PA-Metadaten im Content supply chain

C2PA-Metadaten sind so konzipiert, dass sie mit unterstützten Inhalten verknüpft bleiben, während sie zwischen Adobe-Programmen und kompatiblen Drittanbieterplattformen verschoben werden.

Wenn Inhalte veröffentlicht, verteilt oder freigegeben werden, können Plattformen, die C2PA-Metadaten oder zugehörige Provenienztechnologien unterstützen, angehängte Metadaten lesen und Transparenzinformationen für Benutzer anzeigen.

Adobe steuert nicht, wie externe Services C2PA-Metadaten interpretieren, anzeigen oder verwenden, nachdem Inhalte Adobe-Programme verlassen haben. Kunden sollten die Dokumentation zu einzelnen Veröffentlichungsplattformen konsultieren, um zu erfahren, wie C2PA-Metadaten verarbeitet werden.

## Sichtbares Wasserzeichen

Unter bestimmten Umständen und in bestimmten Regionen können Unternehmen sich dafür entscheiden oder dazu verpflichtet sein, von GenAI generierte oder von GenAI bearbeitete Inhalte sichtbar zu identifizieren.

Adobe bietet [Anleitungen](https://helpx.adobe.com/de/creative-cloud/apps/generative-ai/ai-content-watermarks-faq.html) zur Verwendung vorhandener Wasserzeichenfunktionen, die über Adobe-Programme unterstützt werden. Ob ein sichtbares Wasserzeichen erforderlich ist, hängt von den Geschäftsanforderungen eines Unternehmens und den geltenden Gesetzen und Vorschriften in den Rechtssystemen ab, in denen Inhalte veröffentlicht werden.

>[!NOTE]
>
>C2PA-Metadaten und sichtbare Wasserzeichen dienen verschiedenen Zwecken. C2PA-Metadaten bieten maschinenlesbare Informationen zur Provenienz, während sichtbare Wasserzeichen eine visuelle Offenlegung bieten, die Unternehmen anwenden können.

## Verfügbarkeit und Versionen

Diese Funktionen werden während des gesamten **August 2026** in unterstützten Adobe CX Enterprise-Workflows eingeführt.

>[!NOTE]
>
>Nach dem Rollout erhalten zukünftige Workflows, bei denen Inhalte mithilfe von KI erstellt oder bearbeitet werden, automatisch C2PA-Metadaten-Unterstützung.

Die Version umfasst:

### Automatische C2PA-Metadaten

C2PA-Metadaten werden automatisch an unterstützte GenAI-generierte und GenAI-bearbeitete Inhalte angehängt. Diese Funktion ist standardmäßig aktiviert und kann nicht deaktiviert werden.

### Wasserzeichenführung

Adobe bietet [Dokumentation](https://helpx.adobe.com/de/creative-cloud/apps/generative-ai/ai-content-watermarks-faq.html) in der beschrieben wird, wie bestehende Wasserzeichenfunktionen, die in unterstützten Adobe-Anwendungen verfügbar sind, für Organisationen verwendet werden können, die sichtbare Kennzeichnungen anwenden möchten oder müssen.

## Unterstützte Anwendungen in Adobe CX Enterprise {#supported-applications}

Die folgenden Adobe-Programme und -Services bieten zusätzliche Informationen darüber, wie und wann C2PA-Metadaten in bestimmten CX Enterprise-Programmen an qualifizierte Inhalte angehängt werden.

Alle Adobe CX Enterprise-Anwendungen behalten jedoch ggf. vorhandene C2PA-Metadaten bei, da unterstützte Assets durch Adobe-Workflows geleitet werden. Auf diese Weise wird die Integrität der Herkunftsinformationen im gesamten supply chain-Inhalt gewahrt.

>[!NOTE]
>
>Die Versionshinweise oder Anleitungen für jede der unten aufgeführten Anwendungen werden auf Experience League in den jeweiligen Abschnitten der Anwendungsproduktseiten bereitgestellt. Die Tabelle wird mit den Links aktualisiert, sobald sie verfügbar werden. Weitere Informationen finden Sie in den neuesten Produktabschnitten zu Experience League.

| application/solution | Versionshinweise/Anleitungen |
|---|---|
| Adobe Advertising Cloud | |
| Adobe Experience Manager (AEM) | |
| KI-Assistent für die Inhaltserstellung (Funktion in Adobe Journey Optimizer/Adobe Campaign) | <!--[Documentation] (https://experienceleague.adobe.com/de/docs/journey-optimizer-b2b/user/content-management/assets/c2pa-metadata)--> |
| Adobe Journey Optimizer B2B edition | <!--[Documentation] (https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/content-management/assets/content-credentials)--> |
| Adobe Journey Optimizer B2C | |
| Adobe Campaign | |
| Adobe Commerce | |
| GenStudio for Performance Marketing | |
| Adobe Marketo Engage | |
| Adobe Workfront | |
| CX Enterprise Coworker-Kampagnen (ehemals HALO) | <!--[Documentation](https://experienceleague.adobe.com/de/docs/cx-enterprise-ai/experience-cloud-ai/coworker/campaigns/generative-c2pa-metadata)--> |

## Verwandte Links

* [Anleitung für sichtbare Wasserzeichen](https://helpx.adobe.com/de/creative-cloud/apps/generative-ai/ai-content-watermarks-faq.html)
* [Adobe-Prüfung](https://contentauthenticity.adobe.com/inspect)

## Häufig gestellte Fragen

**Welche Adobe-Apps wenden C2PA-Metadaten auf bearbeitete oder erstellte generative KI an?**

Unterstützte Adobe CX Enterprise-Anwendungen fügen automatisch C2PA-Metadaten an qualifizierte, GenAI-generierte und GenAI-bearbeitete Inhalte an. Weitere Informationen zu [&#x200B; CX Enterprise-Anwendungen finden &#x200B;](#supported-applications) im Abschnitt „Unterstützte Anwendungen“.

**Zu welchen Inhaltstypen fügt Adobe C2PA-Metadaten hinzu?**

Im Großen und Ganzen sind Bilder, Audio, Video, Dokumente und Text im Umfang enthalten. Weitere Informationen dazu, wie jede Anwendung C2PA-Metadaten über verschiedene Produkte [&#x200B; Inhaltstypen hinweg unterstützt, finden Sie jedoch in der Dokumentation &#x200B;](#supported-applications) Abschnitt „Unterstützte Anwendungen“.

**Welche Anwendungen in Adobe CX bewahren C2PA-Metadaten während der Bearbeitung und Veröffentlichung auf?**

Alle Adobe CX Enterprise-Anwendungen wurden entwickelt, um C2PA-Metadaten beizubehalten, wenn Inhalte durch kompatible Adobe-Workflows verschoben werden. Die Beibehaltung außerhalb von Adobe-Anwendungen hängt davon ab, ob externe Plattformen C2PA-Metadaten unterstützen.

**Was passiert, wenn mehrere GenAI-generierte Bilder zu einem einzigen Bild kombiniert werden?**

Die resultierenden C2PA-Metadaten hängen von der verwendeten Anwendung und dem verwendeten Workflow ab. Sofern unterstützt, behält Adobe während des gesamten Bearbeitungsprozesses Provenienzinformationen bei. Informationen zum Workflow[spezifischen Verhalten in den einzelnen &#x200B;](#supported-applications-across-adobe-cx-enterprise) finden Sie im Abschnitt „Unterstützte Programme“.

**Was passiert, wenn GenAI-generierte Bilder aus Adobe und Nicht-Adobe-Programmen kombiniert werden?**

Adobe behält C2PA-Metadaten bei, die innerhalb des Workflows verfügbar und unterstützt werden. Adobe aktualisiert die zugrunde liegenden Metadaten gegebenenfalls mit den neuesten Informationen, wenn entsprechende Inhalte (Bild, Audio, Video, Text) in Adobe-Workflows mit GenAI bearbeitet oder erstellt werden. Wenn Sie mehrere Quellen zu einem neuen Asset kombinieren, werden die zugrunde liegenden Metadaten nicht ersetzt oder gehen verloren. Stattdessen erhält das neue Asset seine eigenen C2PA-Metadaten und die Details aus jeder Quelle werden darin gespeichert. Wenn eine Quelle bereits über eigene C2PA-Metadaten verfügte - unabhängig davon, ob sie von einem Adobe oder einem Nicht-Adobe-Tool stammten - bleibt dieser Verlauf mit ihr verknüpft. Das bedeutet, dass das endgültige Asset ein vollständiges Bild trägt: eine eigene Aufzeichnung der Erstellung oder Bearbeitung mit GenAI sowie die individuelle Geschichte jedes Stücks, das darin aufgenommen wurde.

**Hängen GenAI-bearbeitete und GenAI-erstellte Workflows in Adobe CX-Anwendungen automatisch C2PA-Metadaten an?**

Ja. Für unterstützte generative KI-Workflows hängt Adobe automatisch C2PA-Metadaten an, die identifizieren, ob Inhalte von GenAI generiert oder GenAI-bearbeitet wurden, zusammen mit anderen Provenienzinformationen wie Zeitstempeln, KI-Systeminformationen und eindeutigen Kennungen.

**Wie werden C2PA-Metadaten im gesamten supply chain-Inhalt verwaltet?**

C2PA-Metadaten sind dauerhafte Metadaten, die so konzipiert sind, dass sie mit unterstützten Inhalten verknüpft bleiben, während sie zwischen kompatiblen Adobe-Anwendungen und unterstützenden Drittanbieterplattformen wechseln. Externe Dienste bestimmen, wie angehängte Herkunftsinformationen nach der Veröffentlichung angezeigt werden.

**Wie können Unternehmen ihre eigenen authentifizierten Informationen hinzufügen, ohne die Provenienzkette zu unterbrechen?**

Einige Adobe-Programme ermöglichen es Erstellern und Unternehmen, zusätzliche authentifizierte Informationen zu vorhandenen C2PA-Metadaten hinzuzufügen, während die Herkunft beibehalten wird. Die Verfügbarkeit variiert je nach Anwendung.

**Ist es möglich, das automatische Anhängen von C2PA-Metadaten zu deaktivieren?**

Nein. Neue Transparenzgesetze für generative KI schreiben vor, dass Unternehmen, die generative KI-Tools wie Adobe bereitstellen, dauerhafte Metadaten an qualifizierte Inhalte anhängen müssen, die mit generativer KI generiert oder bearbeitet werden. Das automatische Anhängen von C2PA-Metadaten kann nicht deaktiviert werden.

**Was passiert mit Inhalten, die mit generativer KI vor der August-Version erstellt/bearbeitet wurden?**

Für Inhalte, die vor der Version vom August 2026 mit Tools für generative KI erstellt oder bearbeitet wurden, sind keine automatischen C2PA-Metadaten angehängt. In Firefly Web und anderen Apps erstellte Inhalte, auf die zuvor C2PA-Metadaten angewendet wurden, werden jedoch weiterhin angehängt.

**Wie kann ein Kunde überprüfen, ob an Inhalte C2PA-Metadaten angehängt sind?**

Kunden können überprüfen, ob an Inhalte C2PA-Metadaten angehängt sind, indem sie sie auf die Seite [Adobe Inspect](https://contentauthenticity.adobe.com/inspect) hochladen.

**Wie zeigen externe Plattformen C2PA-Metadaten an, sobald Inhalte veröffentlicht oder freigegeben wurden?**

Wenn Inhalte über Veröffentlichungsplattformen, Social-Media-Kanäle, E-Mail-Dienste und andere digitale Ökosysteme hinweg verschoben werden, können nachgelagerte Services, die C2PA-Metadaten unterstützen, oder verwandte Provenienztechnologien angehängte Metadaten lesen und auf Grundlage dieser Informationen Offenlegungen oder Indikatoren anzeigen. Adobe steuert nicht, wie externe Plattformen mit angehängten C2PA-Metadaten verknüpfte Offenlegungen anzeigen, interpretieren oder anwenden. Die neuesten Informationen darüber, wie eine bestimmte Plattform mit Provenienzinformationen umgeht, finden Kunden direkt in den Richtlinien dieser Plattform.

**Erhöhen diese Änderungen die Kosten für Adobe-Produkte oder -Abonnements?**

Nein. C2PA-Metadaten wirken sich nicht auf die Kosten von Adobe-Produkten aus.
