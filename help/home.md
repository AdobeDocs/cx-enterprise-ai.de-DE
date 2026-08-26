---
title: KI in CX Enterprise-Anwendungen
description: Erfahren Sie, wie CX Enterprise-Anwendungen generative KI (GenAI), KI-Assistenten, agentische KI, CX Enterprise-Mitarbeiter und MCP-Tools verwenden.
TQID: https://experienceleague.adobe.com/heALjEZbowNaygG24oOM2HSlHa9oYVI5ViUNZDr19Ds
product_v2: id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bdid: f8a45b24-4be7-4f1b-909b-60d06b483a20id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: c7d04a2c-412a-4c9d-9d7a-4456eaa5adebid: d095671a-1355-40aa-8b5f-06c33c68080bid: e1e0219c-f879-479f-8427-888ed2a6e9c2id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: 7668505ba139898a4747e049290e5eaf1e29b9f8
workflow-type: tm+mt
source-wordcount: 969
ht-degree: 3%

---

# KI in CX Enterprise

Dieses Handbuch behandelt die KI-Funktionen in Adobe CX Enterprise: generative KI, KI-Assistent, Agent Orchestrator, Experience Platform-Agenten, CX Enterprise-Mitarbeiter und MCP.

## KI-Funktionen - Übersicht

Beginnen Sie hier mit einem Überblick darüber, wo und wie KI in CX Enterprise verwendet wird:

- [Über generative KI](./overview/generative-ai.md) beschreibt, welche CX Enterprise-Anwendungen generative KI und KI-Assistent unterstützen und wie sie sich vergleichen.
- [Über die agentische KI](./overview/agentic-ai.md) erläutert, wie Experience Platform-Agenten sowohl in bestehenden CX Enterprise-Anwendungen als auch in KI-First-Anwendungen funktionieren, und listet die in den einzelnen Programmen verfügbaren Agenten auf.
- [KI-Überwachung](./overview/monitoring.md) umfasst die Dashboards, die die Akzeptanz, Nutzung, Feedback und Nutzung von KI-Krediten durch Agenten verfolgen.
- [Verbrauch von KI](./overview/ai-credit-consumption.md)Guthaben: Erläutert, wie Agentenaufträge KI-Guthaben verwenden, wobei die geschätzten Verbrauchsraten nach Agent und Vorgangstyp aufgeschlüsselt sind.
- [Generative KI-Inhaltstransparenz](./content-transparency.md) erklärt, wie Adobe automatisch C2PA-Metadaten an GenAI-generierte und GenAI-bearbeitete Inhalte in CX Enterprise-Anwendungen anhängt.
- [CX Enterprise Agent Tools](https://experienceleague.adobe.com/de/docs/cx-enterprise-agentic-tools/using/overview) decken zusätzliche agentische Fähigkeiten und Tools ab, die CX Enterprise Agents erweitern (Video-Tutorials).

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

## Coworker

Bei Coworker handelt es sich um eine agentenorientierte Weiterentwicklung des KI-Assistenten, der Kundenerlebnis- und Marketing-Workflows automatisiert, sodass sich Ihr Team auf Geschäftsziele anstatt auf die routinemäßige Ausführung konzentrieren kann. Anstatt eine Frage nach der anderen zu stellen, beschreibt man ein Ziel. Mitarbeiter plant, führt aus, validiert und gibt die abgeschlossene Arbeit zur Genehmigung zurück. Coworker includes:

- **[Coworker Chat](https://experienceleague.adobe.com/en/docs/cx-enterprise-ai/experience-cloud-ai/coworker/chat/overview)**: Eine Gesprächsoberfläche, mit der Sie Ihre Daten untersuchen, Zielgruppen und Journey validieren und mehrstufige Aufgaben in allen CX Enterprise-Anwendungen ausführen können.
- **[Coworker Campaign](https://experienceleague.adobe.com/en/docs/cx-enterprise-ai/experience-cloud-ai/coworker/campaigns/overview)**: Eine KI-native Anwendung, die Kampagnen-Briefing, Zielgruppenerstellung, Inhaltserstellung, Journey-Design und Proofing in einem einzigen Gesprächserlebnis zusammenfasst. Es verwendet integrierte Vorlagen, Best Practices und eine Eingabeaufforderung, um kleine, agile Teams bei der schnellen Durchführung von Kampagnen zu unterstützen.
- **Coworker Projects** (in Kürze verfügbar): Ein einheitlicher Arbeitsbereich zur Automatisierung von End-to-End-Orchestrierungs-Workflows für das Kundenerlebnis, der Teams bei der Koordinierung von Aufgaben, Genehmigungen und Ausführungen unterstützt, um Ergebnisse von der Strategie bis zur Bereitstellung zu erzielen. Die Dokumentation für Projekte wird in Kürze verfügbar sein.

Berechtigte Kunden werden schrittweise von KI-Assistent und Experience Platform-Agenten auf den Coworker Chat umgestellt. Lesen Sie [Coworker Trial](./agents/trial.md), um mehr über die Testeignung, die Verwendung von KI-Guthaben und den Zugriff darauf zu erfahren.

Um den Coworker Chat in Aktion zu sehen, gehen Sie durch [Coworker Chat in Playground](./coworker/playground-coworker-chat.md) oder lesen Sie reale Anwendungsfälle wie [Validieren von AA zu CJA-](./coworker/chat/use-cases/data-insights/data-validation-aa-cja.md) und [Analysieren von CJA-Daten](./coworker/chat/use-cases/data-insights/analytics-chat.md).

Eine vollständige Produktdokumentation zu Coworker Chat, Kampagnen und Projekten finden Sie unter [Coworker](./coworker/overview.md). Informationen zur Replikation von Sandbox-zu-Sandbox-Objekten finden Sie unter [Sandbox Tooling Agent Skills](./agents/sandbox-tooling.md).

## MCP

[Adobe CX Coworker Gateway](./mcp/overview.md) ist der Unified Model Context Protocol (MCP)-Endpunkt für CX Enterprise. Dadurch erhalten MCP-kompatible Clients wie [!DNL Claude], [!DNL ChatGPT] und [!DNL Cursor] eine einzige geregelte Verbindung zu den Produkt-Tools, die Ihr Unternehmen verwenden darf:

- [Real-Time CDP-Tools](./mcp/rtcdp-mcp.md)
- [Experience Platform-Tools](./mcp/aep-mcp.md)
- [Journey Optimizer-Tools](./mcp/ajo-mcp.md)
- [Customer Journey Analytics-Tools](./mcp/cja-mcp.md)
- [Adobe Analytics-Tools](./mcp/analytics-mcp.md)
- [!DNL Workfront] Tools, dokumentiert im [Workfront MCP-Server-Handbuch](https://experienceleague.adobe.com/en/docs/workfront/using/basics/workfront-mcp-server/workfront-mcp-server-overview)

Neu bei CX Coworker Gateway? Siehe [Zugriff auf CX Coworker Gateway-Tools](./mcp/access.md) und [Installieren von CX Coworker Gateway](./mcp/install.md), um eine Verbindung herzustellen. Verwenden Sie nach der Verbindung die [Sitzungskontext-Tools](./mcp/context-tools.md), um die aktive Organisation, Sandbox und Datenansicht festzulegen, bevor Sie die Produkt-Tools aufrufen.

## Erste Schritte

### Zugriffsanforderungen

Ihr Adobe-Administrator muss Ihnen die entsprechenden Berechtigungen erteilen, bevor Sie den KI-Assistenten und die Experience Platform-Agenten verwenden können. Die Anforderungen variieren je nach Anwendung. Weitere Informationen finden [ unter ](./agents/agent-orchestrator.md#access) im Agent Orchestrator-Handbuch.

### Datenschutz und Sicherheit

KI-Assistent und Experience Platform-Agenten priorisieren Datenschutz, Sicherheit und Governance, einschließlich Sandbox-spezifischer Datenisolierung und Ihrer bestehenden Zugriffssteuerungsrichtlinien. Ausführliche Informationen finden Sie unter [Datenschutz, Sicherheit und Governance im KI-Assistenten](./ai-assistant/privacy.md).

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

