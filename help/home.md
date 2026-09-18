---
title: KI in CX Enterprise-Anwendungen
description: Erfahren Sie, wie CX Enterprise-Programme generative KI (GenAI), CX Enterprise Coworker, KI-Assistent, agentische KI und MCP-Tools verwenden.
TQID: 'https://experienceleague.adobe.com/heALjEZbowNaygG24oOM2HSlHa9oYVI5ViUNZDr19Ds'
product_v2:
  - id: fdae8433-07cd-42e7-acce-738afe63f6bb
    internal-label: CX Enterprise Coworker
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
  - id: f8a45b24-4be7-4f1b-909b-60d06b483a20
    internal-label: Leader
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: c7d04a2c-412a-4c9d-9d7a-4456eaa5adeb
    internal-label: Governance
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
    internal-label: Security
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
    internal-label: Privacy
source-git-commit: fccf9111460413fe5b89229564a682827152b1ab
workflow-type: tm+mt
source-wordcount: '962'
ht-degree: 2%
---
# KI in CX Enterprise-Anwendungen

In diesem Handbuch werden die KI-Funktionen in Adobe CX Enterprise behandelt: generative KI, CX Enterprise Coworker, KI-Assistent, Agent Orchestrator und MCP.

## KI-Funktionen - Übersicht

Beginnen Sie hier mit einem Überblick darüber, wo und wie KI in CX Enterprise verwendet wird:

- [Über generative KI](./overview/generative-ai.md) beschreibt, welche CX Enterprise-Programme generative KI und den KI-Assistenten unterstützen und wie sie sich vergleichen.
- [Über die agentische KI](./overview/agentic-ai.md) erläutert, wie die agentische KI in bestehenden CX Enterprise-Programmen und KI-First-Programmen funktioniert, und listet die in den einzelnen Programmen verfügbaren Agenten auf.
- [KI-Überwachung](./overview/monitoring.md) umfasst die Dashboards, die die Akzeptanz, Nutzung, Feedback und Nutzung von KI-Krediten durch Agenten verfolgen.
- [Verbrauch von KI](./overview/ai-credit-consumption.md)Guthaben: Erläutert, wie Agentenaufträge KI-Guthaben verwenden, wobei die geschätzten Verbrauchsraten nach Agent und Vorgangstyp aufgeschlüsselt sind.
- [Generative KI-Inhaltstransparenz](./content-transparency.md) erklärt, wie Adobe automatisch C2PA-Metadaten an GenAI-generierte und GenAI-bearbeitete Inhalte in CX Enterprise-Programmen anhängt.
- [CX Enterprise Agent-Tools](https://experienceleague.adobe.com/de/docs/cx-enterprise-agentic-tools/using/overview) Behandeln Sie zusätzliche Agentenkompetenzen und -Tools, die CX Enterprise-Agenten erweitern (Video-Tutorials).

## Coworker

Bei Coworker handelt es sich um eine agentenorientierte Weiterentwicklung des KI-Assistenten, der Kundenerlebnis- und Marketing-Workflows automatisiert, sodass sich Ihr Team auf Geschäftsziele anstatt auf die routinemäßige Ausführung konzentrieren kann. Anstatt eine Frage nach der anderen zu stellen, beschreibt man ein Ziel. Mitarbeiter plant, führt aus, validiert und gibt die abgeschlossene Arbeit zur Genehmigung zurück. Weitere Informationen zu [Adobe for Business](https://business.adobe.com/de/products/cx-enterprise-coworker.html).

Coworker includes:

- **[Coworker Chat](https://experienceleague.adobe.com/de/docs/cx-enterprise-ai/experience-cloud-ai/coworker/chat/overview)**: Eine Gesprächsoberfläche, mit der Sie Ihre Daten untersuchen, Zielgruppen und Journey validieren und mehrstufige Aufgaben in allen CX Enterprise-Anwendungen ausführen können.
- **[Coworker for Teams](https://experienceleague.adobe.com/de/docs/cx-enterprise-ai/experience-cloud-ai/coworker/campaigns/overview)** (früher _Coworker Campaign_): Eine KI-native Anwendung, die Kampagnen-Briefing, Audience-Erstellung, Inhaltserstellung, Journey-Design und Proofing in einem einzigen Gesprächserlebnis zusammenfasst. Es verwendet integrierte Vorlagen, Best Practices und eine Eingabeaufforderung, um kleine, agile Teams bei der schnellen Durchführung von Kampagnen zu unterstützen. Weitere Informationen zu [Adobe for Business](https://business.adobe.com/products/cx-enterprise-coworker/teams.html).
- **Coworker Projects** (in Kürze verfügbar): Ein einheitlicher Arbeitsbereich zur Automatisierung von End-to-End-Orchestrierungs-Workflows für das Kundenerlebnis, der Teams bei der Koordinierung von Aufgaben, Genehmigungen und Ausführungen unterstützt, um Ergebnisse von der Strategie bis zur Bereitstellung zu erzielen. Die Dokumentation für Projekte wird in Kürze verfügbar sein.

Berechtigte Kunden werden schrittweise von KI-Assistent und Experience Platform-Agenten auf den Coworker Chat umgestellt. Lesen Sie [Coworker Trial](./agents/trial.md), um mehr über die Testeignung, die Verwendung von KI-Guthaben und den Zugriff darauf zu erfahren.

Um den Coworker Chat in Aktion zu sehen, gehen Sie durch [Coworker Chat in Playground](./coworker/playground-coworker-chat.md) oder lesen Sie reale Anwendungsfälle wie [Validieren von AA zu CJA-](./coworker/chat/use-cases/data-insights/data-validation-aa-cja.md) und [Analysieren von CJA-Daten](./coworker/chat/use-cases/data-insights/analytics-chat.md).

Eine vollständige Produktdokumentation zu Coworker Chat, Coworker for Teams und Projekten finden Sie unter [Coworker](./coworker/overview.md). Informationen zur Replikation von Sandbox-zu-Sandbox-Objekten finden Sie unter [Sandbox Tooling Agent Skills](./agents/sandbox-tooling.md).

## KI-Assistent

[AI Assistant](./ai-assistant/ai-assistant-ui.md) ist ein konversatives, generatives KI-Tool, das in Adobe Experience Platform-basierten Anwendungen verfügbar ist. Sie können damit Produktkenntnisse erwerben, Probleme beheben, betriebliche Erkenntnisse gewinnen und auf Experience Platform-Agenten zugreifen - alles über eine Vollbild- oder Leistenansichtsoberfläche in natürlicher Sprache.

Informationen zum Navigieren in der Benutzeroberfläche finden Sie im Handbuch [Benutzeroberfläche des KI-Assistenten](./ai-assistant/ai-assistant-ui.md). Beispielaufforderungen nach Agent finden Sie unter [Bibliothek für Eingabeaufforderungen](./ai-assistant/prompt-library.md).

## Agent Orchestrator- und Experience Platform-Agenten

[Agent Orchestrator](./agents/agent-orchestrator.md) ist die Agentenebene, auf der Experience Platform-Agenten basieren. Wenn Sie eine Frage an den KI-Assistenten stellen, plant Agent Orchestrator die Arbeit, ruft die zu ihrer Beantwortung erforderlichen Spezialisten auf und gibt eine einheitliche Antwort zurück - alles unter menschlicher Aufsicht.

Die folgenden Experience Platform-Agenten sind in diesem Handbuch dokumentiert:

- [Audience Agent](./agents/audience.md)
- [Data Insights Agent](./agents/cja-data-insights-agent.md)
- [Experimentation Agent](./agents/agent-experiment.md)
- [Field Discovery Agent](./agents/field-discovery-agent.md)
- [Journey Agent](./agents/ajo-agent.md)
- [Benachrichtigungsagent](./agents/notifications.md)
- [Produktsupport-Agent](./agents/product-support.md)
- [Adobe Marketing Agent for Microsoft 365 Copilot](./agents/ama-ms.md)
- [Daten validieren](./agents/data-validation.md)

Eine vollständige Liste der Agenten, der von ihnen unterstützten Programme und der Eignungsanforderungen finden Sie unter [Agent AI in CX Enterprise](./overview/agentic-ai.md).

## MCP

[Adobe CX Coworker Gateway](./mcp/overview.md) ist der Unified Model Context Protocol (MCP)-Endpunkt für CX Enterprise. Dadurch erhalten MCP-kompatible Clients wie [!DNL Claude], [!DNL ChatGPT] und [!DNL Cursor] eine einzige geregelte Verbindung zu den Produkt-Tools, die Ihr Unternehmen verwenden darf:

- [Real-Time CDP-Tools](./mcp/rtcdp-mcp.md)
- [Experience Platform-Tools](./mcp/aep-mcp.md)
- [Journey Optimizer-Tools](./mcp/ajo-mcp.md)
- [Customer Journey Analytics-Tools](./mcp/cja-mcp.md)
- [Adobe Analytics-Tools](./mcp/analytics-mcp.md)
- [!DNL Workfront] Tools, dokumentiert im [Workfront MCP-Server-Handbuch](https://experienceleague.adobe.com/de/docs/workfront/using/basics/workfront-mcp-server/workfront-mcp-server-overview)
- [!DNL Target] Tools, dokumentiert im [Target MCP Server Guide](https://experienceleague.adobe.com/de/docs/target/using/mcp/target-mcp)

Neu bei CX Coworker Gateway? Siehe [Zugriff auf CX Coworker Gateway-Tools](./mcp/access.md) und [Installieren von CX Coworker Gateway](./mcp/install.md), um eine Verbindung herzustellen. Verwenden Sie nach der Verbindung die [Sitzungskontext-Tools](./mcp/context-tools.md), um die aktive Organisation, Sandbox und Datenansicht festzulegen, bevor Sie die Produkt-Tools aufrufen.

Bevor Sie eines dieser Tools verwenden, lesen Sie [Bevor Sie beginnen](./overview/overview-ai-cxe.md#before-you-begin) für Zugriffsanforderungen sowie Überlegungen zum Datenschutz und zur Sicherheit.

## Best Practices

Befolgen Sie die folgenden Best Practices, um die Erfahrungen Ihres KI-Assistenten oder -Mitarbeiters optimal zu nutzen:

- **Seien Sie spezifisch** in Ihren Eingabeaufforderungen, um zielgerichtete und relevante Erkenntnisse zu erhalten.
- **Überprüfen der Antworten** indem Sie die Zitate der Quelle und die Begründungen lesen.
- **Verwenden Sie die**, um sicherzustellen, dass für Ihre Fragen die relevantesten Datenquellen verwendet werden.
- **Feedback geben**, um die Leistung und Genauigkeit im Laufe der Zeit zu verbessern.
- **Kombinieren Sie** Einblicke aus mehreren Agenten für eine umfassendere Analyse.

## Rechtliche Erwägungen

Der KI-Assistent unterstützt Antworten derzeit nur auf Englisch, und Sprachmodelle machen gelegentlich Fehler. Überprüfen Sie immer die bereitgestellten Informationen und verwenden Sie die in den einzelnen Antworten enthaltenen Begründungsschritte, um zu verstehen, wie sie generiert wurden. Ausführliche Informationen finden Sie im [Haftungsausschluss](./ai-assistant/legal-disclaimer.md).

Adobe fügt auch automatisch C2PA-Metadaten an GenAI-generierte und GenAI-bearbeitete Inhalte in CX Enterprise-Anwendungen an, um generative KI-Transparenzvorschriften zu erfüllen. Weitere Informationen finden Sie [Inhaltstransparenz mit generativer KI](./content-transparency.md).

