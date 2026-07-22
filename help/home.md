---
title: KI in CX Enterprise-Anwendungen
description: Erfahren Sie, wie CX Enterprise-Anwendungen generative KI (GenAI), KI-Assistenten, agentische KI, CX Enterprise-Mitarbeiter und MCP-Tools verwenden.
TQID: https://experienceleague.adobe.com/heALjEZbowNaygG24oOM2HSlHa9oYVI5ViUNZDr19Ds
product_v2:
  - id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: f8a45b24-4be7-4f1b-909b-60d06b483a20
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: c7d04a2c-412a-4c9d-9d7a-4456eaa5adeb
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: d8daade8bb7d0259cd18fe7c8f957955dd97b2a0
workflow-type: tm+mt
source-wordcount: 766
ht-degree: 2%

---

# KI in CX Enterprise

Dieses Handbuch behandelt die KI-Funktionen, die in Adobe CX Enterprise-Anwendungen verfügbar sind: Generative KI und KI-Assistent für Produktkenntnisse und operative Einblicke, Agent Orchestrator und Experience Platform-Agenten für die Automatisierung von Aufträgen, CX Enterprise-Mitarbeiter für ein vollständig konversatives, agentenorientiertes Erlebnis und MCP für die Verbindung Ihrer eigenen KI-Tools mit CX Enterprise-Daten.

## Über KI in CX Enterprise

Beginnen Sie hier mit einem Überblick darüber, wo und wie KI in CX Enterprise verwendet wird:

- [Generative KI](./overview/generative-ai.md) beschreibt, welche CX Enterprise-Anwendungen generative KI und AI Assistant unterstützen und wie sie sich vergleichen.
- [Agentic AI](./overview/agentic-ai.md) erläutert, wie Experience Platform-Agenten sowohl in bestehenden CX Enterprise-Anwendungen als auch in AI-First-Anwendungen funktionieren, und listet die in den einzelnen Programmen verfügbaren Agenten auf.
- [Überwachung der agenten KI](./overview/monitoring.md) umfasst die Dashboards, die die Akzeptanz, Nutzung, Feedback und Nutzung von KI-Krediten durch Agenten verfolgen.
- [Agentenaufträge und KI-](./overview/ai-credit-consumption.md): Erläutert, wie KI-Gutschriften von Agentenaufträgen mit geschätzten Verbrauchsraten nach Agent und Vorgangstyp genutzt werden.

## KI-Assistent

[AI Assistant](./ai-assistant/ai-assistant-ui.md) ist ein konversatives, generatives KI-Tool, das in Adobe Experience Platform-basierten Anwendungen verfügbar ist. Sie können damit Produktkenntnisse erwerben, Probleme beheben, betriebliche Erkenntnisse gewinnen und auf Experience Platform-Agenten zugreifen - alles über eine Vollbild- oder Leistenansichtsoberfläche in natürlicher Sprache.

Lesen Sie das [Handbuch für die Benutzeroberfläche des KI](./ai-assistant/ai-assistant-ui.md)Assistenten, um zu erfahren, wie Sie in der Benutzeroberfläche navigieren, und die [Eingabeaufforderungsbibliothek](./ai-assistant/prompt-library.md), z. B. nach Agent.

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

Eine vollständige Liste der Agenten, der von ihnen unterstützten Programme und der Eignungsanforderungen finden Sie unter [Agent AI in CX Enterprise](./overview/agentic-ai.md).

## CX Enterprise-Mitarbeiter

CX Enterprise Coworker ist eine agentenerste Weiterentwicklung von AI Assistant. Anstatt eine Frage nach der anderen zu stellen, beschreiben Sie ein Ziel in natürlicher Sprache, und ein Mitarbeiter plant die Arbeit, führt sie in Ihrem Adobe und den verbundenen Systemen aus, validiert die Ergebnisse und gibt die fertige Arbeit zur Genehmigung zurück. Coworker includes:

- **Coworker Chat**: Eine Gesprächsoberfläche, mit der Sie Ihre Daten untersuchen, Zielgruppen und Journey validieren und mehrstufige Aufgaben in allen CX Enterprise-Anwendungen ausführen können.
- **Coworker Campaign**: Eine KI-native Anwendung, die Kampagnen-Briefing, Zielgruppenerstellung, Inhaltserstellung, Journey-Design und Proofing in einem einzigen Gesprächserlebnis zusammenfasst.

Berechtigte Kunden werden schrittweise von KI-Assistent und Experience Platform-Agenten auf den Coworker Chat umgestellt. Lesen Sie [CX Enterprise Coworker Trial](./agents/trial.md), um mehr über die Testeignung, die Verwendung von KI-Gutschriften und den Zugriff darauf zu erfahren.

Um den Coworker Chat in Aktion zu sehen, gehen Sie durch [Coworker Chat in Playground](./coworker/playground-coworker-chat.md) oder lesen Sie reale Anwendungsfälle wie [Validieren von AA zu CJA-](./coworker/data-validation-aa-cja.md) und [Abbruch der Konversionsanalyse](./coworker/analytics-chat.md).

## MCP

[Adobe CX Coworker Gateway](./mcp/overview.md) ist der Unified Model Context Protocol (MCP)-Endpunkt für CX Enterprise. Dadurch erhalten MCP-kompatible Clients wie [!DNL Claude], [!DNL ChatGPT] und [!DNL Cursor] eine einzige geregelte Verbindung zu den Produkt-Tools, die Ihr Unternehmen verwenden darf, einschließlich Real-Time CDP, Experience Platform, Journey Optimizer, Customer Journey Analytics und Adobe Analytics.

## Erste Schritte

### Zugriffsanforderungen

Ihr Adobe-Administrator muss Ihnen die entsprechenden Berechtigungen erteilen, bevor Sie den KI-Assistenten und die Experience Platform-Agenten verwenden können. Die Anforderungen variieren je nach Anwendung. Weitere Informationen finden [&#x200B; unter &#x200B;](./agents/agent-orchestrator.md#access) im Agent Orchestrator-Handbuch.

### Datenschutz und Sicherheit

KI-Assistent und Experience Platform-Agenten werden mit Datenschutz, Sicherheit und Governance an vorderster Front erstellt, einschließlich Sandbox-spezifischer Datenisolierung und unter Berücksichtigung Ihrer bestehenden Zugriffssteuerungsrichtlinien. Ausführliche Informationen finden Sie unter [Datenschutz, Sicherheit und Governance im KI-Assistenten](./ai-assistant/privacy.md).

## Best Practices

Befolgen Sie die folgenden Best Practices, um die Erfahrungen Ihres KI-Assistenten oder -Mitarbeiters optimal zu nutzen:

- **Seien Sie spezifisch** in Ihren Eingabeaufforderungen, um zielgerichtete und relevante Erkenntnisse zu erhalten.
- **Überprüfen der Antworten** indem Sie die Zitate der Quelle und die Begründungen lesen.
- **Verwenden Sie die**, um sicherzustellen, dass für Ihre Fragen die relevantesten Datenquellen verwendet werden.
- **Feedback geben**, um die Leistung und Genauigkeit im Laufe der Zeit zu verbessern.
- **Kombinieren Sie** Einblicke aus mehreren Agenten für eine umfassendere Analyse.

## Rechtliche Erwägungen

Der KI-Assistent unterstützt Antworten derzeit nur auf Englisch, und Sprachmodelle können gelegentlich Fehler machen. Überprüfen Sie immer die bereitgestellten Informationen und verwenden Sie die in den einzelnen Antworten enthaltenen Begründungsschritte, um zu verstehen, wie sie generiert wurden. Ausführliche Informationen finden Sie im [Haftungsausschluss](./ai-assistant/legal-disclaimer.md).
