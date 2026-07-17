---
title: Zugriff auf CX Coworker Gateway-Tools
description: Überprüfen Sie die Produktverfügbarkeit, die Aktivierung für das Unternehmen und die Berechtigungen, bevor Sie die Adobe CX Coworker Gateway-Tools verwenden.
source-git-commit: 30f4d593bdec8cb45d10c4c49fac3dce16e8ca03
workflow-type: tm+mt
source-wordcount: '556'
ht-degree: 3%

---

# Zugriff auf CX Coworker Gateway-Tools {#mcp-access}

Adobe CX Enterprise stellt Produkttools über eine einzige MCP bereit. Der Zugriff wird von Produkt-Tools bewertet: Ihr Adobe-Unternehmen muss für die entsprechenden Produkt-Tools aktiviert sein und Ihr Benutzerkonto muss über die erforderlichen Produktberechtigungen verfügen, um die von diesen Tools bereitgestellten Produktdaten anzeigen oder ändern zu können.

>[!IMPORTANT]
>
>Ihr Adobe-Unternehmen muss aktiviert sein, bevor Sie die CX Coworker Gateway-Tools verwenden können. Wenn Ihr Unternehmen noch keinen Zugriff hat, wenden Sie sich an Ihr Adobe Account Team , um die Aktivierung für Ihr Unternehmen anzufordern.

## Zugriffsanforderungen {#mcp-requirements}


| Produkt-Tools | Verfügbarkeit | Zugriffsanforderungen |
| --- | --- | --- |
| Real-Time CDP | Beta | Active Real-Time CDP-Lizenz, Beta-Aktivierung für Ihr Adobe-Unternehmen und Berechtigungen zum Anzeigen der von Ihnen abgefragten Zielgruppen, Ziele, Quellen, Identitäten und Aktivierungsressourcen. |
| Experience Platform | Beta | Aktive Experience Platform-Lizenz, Beta-Aktivierung für Ihr Adobe-Unternehmen und Berechtigungen zum Anzeigen der von Ihnen abgefragten Schemata, Datensätze, Governance, Abfrage-Service, Audit und Sandbox-Ressourcen. |
| Journey Optimizer | Beta | Aktive Journey Optimizer-Lizenz, Beta-Aktivierung für Ihr Adobe-Unternehmen und Berechtigungen zum Anzeigen von Kampagnen und Kanalkonfigurationen. |
| Customer Journey Analytics | Verfügbar | Aktive Customer Journey Analytics-Lizenz und ein Produktprofil, das das Berechtigungselement **MCP-Zugriff** in Adobe Admin Console enthält. Produktberechtigungen steuern weiterhin, auf welche Datenansichten, Komponenten, Berichte, Projekte und Zielgruppen Sie zugreifen oder sie ändern können. |
| Adobe Analytics | Verfügbar | Aktive Adobe Analytics-Lizenz und ein Produktprofil, das das Berechtigungselement **MCP-Zugriff** in Adobe Admin Console enthält. Produktberechtigungen steuern weiterhin, auf welche Report Suites, Komponenten, Berichte, Segmente, Datumsbereiche und Projekte Sie zugreifen oder sie ändern können. |
| Workfront | Vorschau | Aktive Workfront-Lizenz und Aktivierung von Workfront MCP. Siehe die [Workfront MCP-Dokumentation](https://experienceleague.adobe.com/en/docs/workfront/using/basics/workfront-mcp-server/workfront-mcp-server-overview). |


>[!NOTE]
>
>Der MCP zeigt nur die Tools an, zu deren Verwendung Ihr Unternehmen und Ihre Anmeldedaten berechtigt sind. Wenn nach der Anmeldung ein Produkt-Tool fehlt, bestätigen Sie die Produktlizenzierung, die Aktivierung für das Unternehmen und die Benutzerberechtigungen.

## Zugriff anfordern {#mcp-request}

Wenden Sie sich bei Beta- oder Limited-Release-Produkt-Tools an Ihren Adobe-Kundenbetreuer und geben Sie an, welche Adobe for CX Coworker Gateway-Produkt-Tools Sie verwenden möchten. Ihr Ansprechpartner kann die Produktaktivierung koordinieren und bestätigen, wenn Ihr Adobe-Unternehmen bereit ist.

Bitten Sie bei allgemein verfügbaren Produkt-Tools, die das Berechtigungselement **MCP-Zugriff** verwenden, einen System- oder Produktadministrator, Ihr Konto zu einem Produktprofil hinzuzufügen, das MCP-Zugriff enthält.

## Produktinterne Aktivierung {#mcp-product-enablement}

Einige Produkte erfordern zusätzlich zum MCP-Zugriff eine produktinterne Aktivierung oder produktspezifische Berechtigungen. Beispiel:

- Adobe Analytics und Customer Journey Analytics erfordern das Berechtigungselement **MCP** Zugriff) in Adobe Admin Console.
- Workfront MCP-Tools werden in den Workfront-Einstellungen aktiviert.
- Beta-Produkt-Tools erfordern die Aktivierung der Adobe-Organisation, bevor ihre Tools über den MCP angezeigt werden.

Überprüfen Sie die Produktseite für das Produkt-Tool, das Sie für produktspezifische Berechtigungen, Kontextanforderungen und Einschränkungen verwenden möchten.

## Vor der Installation {#mcp-prerequisites}

Bevor Sie Ihren MCP-Client verbinden, überprüfen Sie Folgendes:

- Ihre Adobe-Organisation verfügt über die erforderlichen Produkt-Tools.
- Ihr Benutzerkonto verfügt über die erforderlichen Produktberechtigungen für die Daten und Vorgänge, die Sie verwenden möchten.
- Sie haben Zugriff auf einen unterstützten MCP-Client wie [!DNL Claude], [!DNL ChatGPT], [!DNL Cursor], [!DNL Claude Code], [!DNL Codex] oder [!DNL VS Code].
- Bei einer Unternehmensinstallation können Sie oder ein Kollege Connectoren oder benutzerdefinierte Apps in den Unternehmenseinstellungen Ihres MCP-Clients verwalten.

Weiter: [Installieren Sie Adobe CX Coworker Gateway](install.md).