---
description: Erfahren Sie, wie Coworker Campaign automatisch C2PA-Metadaten (Content Credentials) auf KI-generierten und bearbeiteten Bildern anhängt und beibehält, ohne dass Maßnahmen erforderlich sind.
title: C2PA-Metadaten in Coworker-Kampagnen
hide: true
source-git-commit: 2b75854bde0697971e736bd453a14a4aa44352ed
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 6%

---

# C2PA-Metadaten in Coworker-Kampagnen {#overview}

Im Bereich der generativen KI-Transparenz entstehen neue Gesetze, und Adobe arbeitet daran, die geltenden Anforderungen in allen Rechtssystemen zu erfüllen. [C2PA-Metadaten](https://c2pa.org/) (auch als Content Credentials bezeichnet) sind das Provenienztool, mit dem Adobe die Anforderungen dieser Gesetze erfüllt.

C2PA-Metadaten sind dauerhafte, unsichtbare Metadaten, die aufzeichnen, wie ein Inhaltselement erstellt oder bearbeitet wurde. Wenn Sie ein Bild mit Tools für generative KI in Coworker-Kampagnen generieren oder bearbeiten, werden C2PA-Metadaten automatisch an dieses Bild angehängt. Es ist keine Aktion Ihrerseits erforderlich.

## Aktionen, die C2PA-Metadaten anhängen {#cc-workflows}

In der folgenden Tabelle wird zusammengefasst, wann C2PA-Metadaten angehängt werden, basierend auf der Bildaktion, die bei der Bildgenerierung in Co-Worker-Kampagnen durchgeführt wurde.

| Aktion | Beschreibung | C2PA-Metadaten angehängt? | Anwendungsbeispiel |
| --- | --- | --- | --- |
| **Bild erstellen** | Erstellen Sie ein neues Bild aus einer Textaufforderung oder einem Referenzbild oder generieren Sie ein ähnliches Bild aus einem vorhandenen. | Immer. Das Bild wird durch generative KI generiert, sodass es immer neue C2PA-Metadaten enthält. | Aus einer Textaufforderung, die das gewünschte visuelle Element beschreibt, wird ein Bannerbild für eine E-Mail-Kampagne generiert. |

## Inhaltstypen und ihr Umfang {#cc-content-types}

* **Bilder**: Überdeckt. C2PA-Metadaten werden angehängt, wenn Bilder mit generativer KI generiert werden, und bleiben durch Zuschneiden, Textüberlagerung und Bildüberlagerung erhalten, die von der Bildgenerierung in Coworker-Kampagnen ausgeführt werden.
* **Text**: Nicht zutreffend. Reine Textausgaben der Bildgenerierung in Coworker-Kampagnen, wie z. B. Kopiergenerierung, Übersetzung und Vorschläge für die Markenausrichtung, erfordern keine C2PA-Metadaten.

## Was passiert, wenn Inhalte verschoben werden? {#cc-content-moves}

Coworker Campaign behält Content Credentials bei, das mit unterstützten Bild-Assets verknüpft ist. Wenn ein Bild beim Import in Coworker Campaign Content Credentials enthält, bleiben diese Anmeldedaten erhalten, wenn das Asset in generierten Kampagneninhalten und ausgehenden E-Mail-Erlebnissen verwendet wird.

<!-- Some ways of bringing images into your content, such as extracting an image from a PDF or from an embedded (base64) source, may not preserve the original C2PA metadata. In these cases, no C2PA metadata can be read from the source, and none is created for the result. -->

## Zusätzliche Ressourcen

* [Weitere Informationen zu C2PA-Metadaten](https://helpx.adobe.com/de/firefly/using/content-credentials.html){target="_blank"}

* [Benutzerrichtlinien für die generative KI von Adobe Experience Cloud](https://www.adobe.com/de/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html){target="_blank"}

* [Leitlinien und Einschränkungen](https://experienceleague.adobe.com/de/docs/journey-optimizer/using/content-management/generate-content/gs-generative#generative-guardrails){target="_blank"}
