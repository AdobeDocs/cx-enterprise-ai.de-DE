---
description: Durchsuchen Sie die Anwendungsfälle und Beispielaufforderungen des Coworker Chat, sortiert nach Bereichen wie Dateneinblicke, Zielgruppen, Journey und Plattformvorgänge.
title: Anwendungsfälle für den Chat mit Kollegen
feature_v2:
  - id: fdae8433-07cd-42e7-acce-738afe63f6bb
source-git-commit: e396bdc6974eb4484049af450f1b3a6b5045311b
workflow-type: tm+mt
source-wordcount: 3050
ht-degree: 7%

---

# Anwendungsfälle für den Chat mit Kollegen{#use-cases}

Mit dem Coworker Chat können Sie Ihre [!DNL Experience Platform]-Daten in natürlicher Sprache abfragen, analysieren und bearbeiten, anstatt mehrere Benutzeroberflächen zu durchsuchen oder Abfragen manuell zu schreiben. Auf dieser Seite werden die Anwendungsfälle katalogisiert, auf die sich die Fachleute am meisten verlassen, sortiert nach Arbeitsbereich: Dateneinblicke, Zielgruppen, Journey, Grundlegende Elemente und Sandbox-Tools. Jeder Eintrag beinhaltet die Qualifikation, die er aufruft, die Anwendungen, mit denen er arbeitet, und Beispielaufforderungen, die Sie kopieren, an Ihre eigenen Daten anpassen und durch Konversation verfeinern können.

>[!NOTE]
>
>Demnächst verfügbar:
>
>Neue AEM-Agentenfunktionen durch CX Enterprise Coworker, die Ihnen helfen, schneller mehr zu erreichen.
>
>Alle berechtigten Kundinnen und Kunden erhalten fortlaufend Zugriff auf die Funktionen der Adobe Experience Manager-Agenten in Coworker.
>
>Siehe auch [KI in AEM - Überblick über die Agentenfunktionen in AEM](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/overview).

## Markenerlebnis

### Anwendungsfälle für die Erlebnisproduktion - Sites

| Anwendungsfall | Beschreibung | Kenntnisse | Anwendung | Eingabeaufforderungen |
| --- | --- | --- | --- | --- |
| Aktualisieren von AEM-Seiten | Führen Sie Aktionen wie das Aktualisieren, Entfernen, Ersetzen oder Hinzufügen von Inhaltselementen durch, um Erlebnisse genau und aktuell zu halten. Eingaben können natürliche Sprache oder visuelle Anmerkungen wie PDFs oder Screenshots sein. | `aem-sites-pages-update` | Adobe Experience Manager (AEM) | Aktualisieren Sie auf &lt;URL> die Überschrift zu Hello World<br><br>on &lt;URL> und ändern Sie die Schaltfläche „Take our Coffee Quiz“ in eine ansprechendere Version<br><br>Update &lt;URL> basierend auf dem angehängten <br><br>on &lt;URL> Ich möchte einen neuen Teaser-Abschnitt am Ende der Seite über eine Promotion hinzufügen, die wir im Monat August durchführen, nämlich eine Kaffeemaschine kaufen und zwei Tüten Kaffee kostenlos erhalten. Finde auch Bild von Freunden, die Kaffee trinken und verwende das im Teaser |
| AEM stapelweise aktualisieren | Führen Sie Massenaktionen auf mehreren Seiten gleichzeitig durch, z. B. Entfernen, Ersetzen oder Hinzufügen von Inhaltselementen, um Erlebnisse genau und aktuell zu halten. | `aem-sites-pages-bulkreplace` | Adobe Experience Manager (AEM) | Aktualisieren Sie auf &lt;aem path> alle Seiten, die die Kopie „MyBarista“ enthalten, auf „BrewPass“. |
| Wechseln von Figma zu visuellem Inhaltsfragment | Importieren Sie Designs direkt aus Figma in Adobe Experience Manager mit natürlicher Sprache. Die SKILL erstellt automatisch das erforderliche Inhaltsmodell, Inhaltsfragment, Assets und Visualisierungsvorlage, sodass Business-Anwender innerhalb von Minuten ohne manuelle Einrichtung vom Design zum Web-fähigen Inhalt wechseln können. | `aem-sites-visualcontentfragments-create` | Adobe Experience Manager (AEM) | Import aus &lt;FIGMA_URL> |

**Verwandte Informationen**

* [Agentenfunktionen in AEM: Markenerlebnis - Erlebnisproduktion - Sites](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/brand-experience/experience-production/use-cases#use-cases-sites)

### Erlebnisproduktion - Forms-Anwendungsfälle

| Anwendungsfall | Beschreibung | Kenntnisse | Anwendung | Eingabeaufforderungen |
| --- | --- | --- | --- | --- |
| Formular erstellen | Generieren eines neuen adaptiven Formulars aus einer Nur-Sprache-Beschreibung, einer angehängten Kurzbeschreibung, einem Bild oder einer PDF | `aem-forms-adaptiveform-create` | Adobe Experience Manager (AEM) | „Erstellen eines Onboarding-Formulars für Mitarbeiter“<br><br>„Erstellen eines Formulars mithilfe der angehängten Kurzbeschreibung (Bild oder PDF)“<br><br>„Erstellen eines adaptiven Formulars vom Typ &lt;form>&quot; |
| Formular bearbeiten/aktualisieren | Ändern eines vorhandenen Formulars - Hinzufügen/Bearbeiten von Feldern, Anpassen des einfachen Layouts, Konfigurieren von Übermittlungsaktionen oder Anwenden von Änderungen aus einem angehängten Richtliniendokument | `aem-forms-adaptiveform-edit` | Adobe Experience Manager (AEM) | „Feld „Mittleren Namen hinzufügen“ unter dem Feld „Vorname“<br><br>„Felder „Vorname“ und „Nachname“ in ein 2-spaltiges Layout einfügen, 50/50“<br><br>„Konfigurieren des Formulars, um Daten an einen REST-Endpunkt zu senden“<br><br>„Aktualisieren Sie dieses Formular, sodass es dem angehängten Dokument mit Richtlinien entspricht“<br><br>„Feld &lt;Name des Felds> hinzufügen“ unter &lt;vorhandenes Feld>&quot; |
| Geschäftslogik hinzufügen | Erstellen Sie einfache Regeln, z. B. das Anzeigen oder Ausblenden eines Felds basierend auf dem Wert eines anderen Felds | `aem-forms-adaptiveform-edit` | Adobe Experience Manager (AEM) | „Das Feld „Firma“ nur anzeigen, wenn „Mitarbeiter“ „Auftragnehmer“ <br><br>„Das Feld &lt;field> nur anzeigen, wenn &lt;other field> &lt;value> ist“ |
| Formular einschließen | Platzieren eines bestehenden oder neu erstellten Formulars auf einer vorgesehenen AEM Sites-Seite (nur für Edge Delivery Services-Seiten unterstützt) | `aem-forms-adaptiveform-embed` | Adobe Experience Manager (AEM) | „Formular auf der Homepage unserer Website einbetten“<br><br>„Formular auf &lt;Seitenpfad> einbetten“ |

**Verwandte Informationen**

* [Agentenfunktionen in AEM: Markenerlebnis - Erlebnisproduktion - Forms](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/brand-experience/experience-production/use-cases#use-cases-forms)

### Entwicklung

| Anwendungsfall | Beschreibung | Kenntnisse | Anwendung | Eingabeaufforderungen |
| --- | --- | --- | --- | --- |
| Diagnose und Behebung fehlerhafter Cloud Manager-Pipelines | Untersuchen Sie eine fehlgeschlagene Pipeline-Ausführung, identifizieren Sie die Grundursache und generieren Sie eine Korrektur (mit einem Unterschied) zur Überprüfung | `cloud-manager-pipeline-troubleshooting` | Adobe Experience Manager (AEM) | „Warum ist meine Build-Pipeline fehlgeschlagen?“<br><br>„Schlagen Sie eine Fehlerbehebung für meine defekte Produktions-Pipeline vor“ |
| Verwalten von Cloud Manager-Pipelines | Erstellen, Ausführen und Überwachen von AEM Cloud Manager-Pipelines, einschließlich Protokollen, Artefakten, Variablen und Einstellungen | `cloud-manager-pipeline-management` | Adobe Experience Manager (AEM) | „Auflisten von Pipelines für Programm 12345“<br><br>„Warum ist meine Entwicklungs-Pipeline-Ausführung fehlgeschlagen?“ |
| Verwalten von Cloud Manager-Umgebungen | Erstellen, Konfigurieren und Verwalten von AEM Cloud Manager-Umgebungen, einschließlich RDEs, Umgebungsvariablen, Protokollen und Backups | `cloud-manager-environment-management` | Adobe Experience Manager (AEM) | „Meine Umgebungen für Programm 12345 auflisten“<br><br>„RDE zurücksetzen“ |
| Verwalten von Cloud Manager-Programmen | Auflisten, Überprüfen und Löschen von AEM Cloud Manager-Programmen, einschließlich ihrer Pipelines und Umgebungen | `cloud-manager-program-management` | Adobe Experience Manager (AEM) | „Meine Cloud Manager-Programme auflisten“<br><br>„Details zu 12345 abrufen“ |
| Verwalten von Zeitplänen für die Aktualisierung von AEM-Versionen | Konfigurieren Sie die täglichen Ruhezeiten und Freie Zeiträume für die automatisierte Wartung und sehen Sie sich die globalen Fenster zum Einfrieren von Code in Adobe an | `cloud-manager-release-management` | Adobe Experience Manager (AEM) | „Was ist mein aktuelles Fenster für die Ruhezeiten?“<br><br>„Planen Sie einen Zeitraum ohne Updates vom 20. Dezember bis zum 2. Januar“ |

**Verwandte Informationen**

* [Agentenfunktionen in AEM: Markenerlebnis - Entwicklung](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/brand-experience/development/use-cases)

### Onboarding - AEM Assets-Anwendungsfälle

| Anwendungsfall | Beschreibung | Kenntnisse | Anwendung | Eingabeaufforderungen |
| --- | --- | --- | --- | --- |
| Geführtes End-to-End-Onboarding | Orchestriert den gesamten Onboarding-Lebenszyklus, die Repository-Auswahl, die Zuweisung zum Ordner, Tags, Metadaten, Import und Suche, wenn Sie die benötigten Onboarding-Aufgaben nicht kennen. | `aem-onboarding-workflow` | Adobe Experience Manager (AEM) Assets | „Begleiten Sie unser Team beim AEM Assets<br><br>„Begleiten Sie mich beim AEM DAM-Onboarding“ |
| Entwerfen und Erstellen von Ordnerhierarchien | Empfiehlt und erstellt skalierbare Ordnerstrukturen in AEM Assets (unter `/content/dam`) basierend auf Geschäftsanforderungen oder CSV-Eingaben. | `aem-folder-management` | Adobe Experience Manager (AEM) Assets | „Eine Ordnerstruktur für unsere Lifestyle-Marketing-Assets empfehlen“<br><br>„Erstellen von Ordnern basierend auf dieser CSV-Datei“ |
| Entwerfen und Erstellen von Tags | Entwirft und erstellt kontrollierte Tag-Vokabeln unter `/content/cq:tags` - Namespaces, hierarchische Tags und Batch-Tag-Vorgänge. | `aem-tag-taxonomy` | Adobe Experience Manager (AEM) Assets | „Entwerfen Sie eine Tag-Taxonomie mit Namespaces für unsere Produktkategorien“<br><br>„Importieren Sie Tags aus dieser CSV-Datei“<br><br>„Erstellen Sie diese hierarchischen Tags in AEM&quot; |
| Erstellen und Zuweisen von Metadatenformularen | Entwirft und erstellt benutzerdefinierte Metadatenformulare, die die Autoren der Inhaltserstellungs-Benutzeroberfläche aus einer CSV-Datei, Tabelle, einem Anforderungsdokument oder einer Beschreibung verwenden, und weist sie dann optional Ordnern zu. | `aem-metadata-form` | Adobe Experience Manager (AEM) Assets | „Erstellen eines Metadatenformulars aus dieser Feldliste“<br><br>„Zuweisen dieses Formulars zum `campaigns`&quot; |

**Verwandte Informationen**

* [Agenturfunktionen in AEM: Markenerlebnis - Onboarding](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/brand-experience/onboarding/use-cases)

## Content Advisor - AEM Assets-Anwendungsfälle

### Content Discovery

| Anwendungsfall | Beschreibung | Kenntnisse | Anwendung | Eingabeaufforderungen |
| --- | --- | --- | --- | --- |
| Nach semantischem Design suchen | Finden Sie Assets nach Konzept, Stimmung oder visuellem Design mithilfe von KI-gestütztem semantischen Abgleich. | `aem-assets-discovery` | Adobe Experience Manager (AEM) Assets | „Finde mir Bilder vom Morgen-Kaffee-Lifestyle“ |
| Nach benutzerdefinierten Metadaten suchen | Filtern von Assets nach benutzerdefinierten Metadatenfeldern (z. B. Kaffeemischung, Marke, Röststufe). | `aem-assets-discovery` | Adobe Experience Manager (AEM) Assets | „Assets suchen, bei denen `Coffee Blend` `Morning Muse` ist“<br><br>„Assets abrufen, deren Lizenz nicht abgelaufen ist“<br><br>„Assets suchen, bei denen der Kampagnenname nicht festgelegt ist (die Eigenschaft muss für entsprechende Ergebnisse indiziert werden).“ |
| Nach Genehmigungsstatus suchen | Filtern Sie Assets nach dem Genehmigungsstatus. Beispielsweise den Status „Genehmigt“, „In Überprüfung“, „Abgelehnt“ oder „Fehlend“. | `aem-assets-discovery` | Adobe Experience Manager (AEM) Assets | „Anzeigen aller genehmigten Assets im Ordner &quot;`Campaign`&quot; |
| Nach Ordner/Pfad suchen | Identifizieren von Assets durch Interpretieren natürlicher Sprachaufforderungen, die auf Ordnernamen in AEM verweisen. Sie können den Ordner einfach in der Eingabeaufforderung erwähnen, ohne manuell durch das Repository zu navigieren, was die Anzahl der Klicks, die zum Auffinden des richtigen Inhalts erforderlich sind, erheblich reduziert. | `aem-assets-discovery` | Adobe Experience Manager (AEM) Assets | „Gibt es SVGs im Ordner `WKND`?<br><br>„Nach dem 1. November 2025 geänderte Assets in Ordner `WKND` anzeigen“ |

**Verwandte Informationen**

* [Agentenfunktionen in AEM: Content Advisor - Content Discovery](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/content-advisor/discovery/use-cases)

### Inhaltsoptimierung

| Anwendungsfall | Beschreibung | Kenntnisse | Anwendung | Eingabeaufforderungen |
| --- | --- | --- | --- | --- |
| Erstellung hochauflösender Ausgabedarstellungen und kanaloptimierte Ausgabedarstellungen | Generieren neuer Ausgabedarstellungen eines Assets mit einer festgelegten Auflösung und Qualitätsstufe, sodass kanalbereite Varianten ohne manuelle Bearbeitung einfach vorbereitet werden können. Sie können auch Ausgabedarstellungen erstellen, die auf plattformspezifische Anforderungen zugeschnitten sind, z. B. Instagram-Stories, um sicherzustellen, dass Assets automatisch Format-, Übersetzungs- und Qualitätsrichtlinien erfüllen. | `aem-assets-content-optimisation` | Adobe Experience Manager (AEM) Assets | „Erstellen einer `2000px` Ausgabedarstellung wie `JPEG` mit `80% quality`&quot;<br><br>„Erstellen einer Ausgabedarstellung für eine Instagram-Story“ |
| Markenüberlagerungen und Composite-Generierung | Wenden Sie Werbe-Grafiken, -Überlagerungen oder -Abzeichen auf vorhandene Assets mit präziser Platzierung an, um die schnelle Erstellung von kampagnenbereiten Composites zu unterstützen. | `aem-assets-content-optimisation` | Adobe Experience Manager (AEM) Assets | „Überlagern Sie das Bild mit `30%` Rabattgrafiken über dem Werbebanner und platzieren Sie es `100px` von der Mitte.“ |
| Bildverbesserungen, Anpassungen der Hintergrundfarbe, Ausrichtungstransformationen | Wenden Sie visuelle Verbesserungen an (Scharfzeichnen von Bildern), ersetzen Sie Hintergrundfarben und führen Sie Ausrichtungstransformationen durch. | `aem-assets-content-optimisation` | Adobe Experience Manager (AEM) Assets | „Hintergrundfarbe des `PNG` ändern zu `#ff8932`&quot;<br><br>„Bild scharfzeichnen“<br><br>„Bild horizontal spiegeln“ |

**Verwandte Informationen**

* [Agentenfunktionen in AEM: Inhaltsberater - Inhaltsoptimierung](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/content-advisor/content-optimization/use-cases)

## Marken-Governance

| Anwendungsfall | Beschreibung | Skills | Anwendung | Eingabeaufforderungen |
| --- | --- | --- | --- | --- |
| Richtlinie und Segmentsuche | Abrufen detaillierter Markenrichtlinien nach Segment, Markt oder Kategorie | enterprise-context | Adobe Experience Manager (AEM) | „Was sind die Klangfarben-Richtlinien für diese Marke?“<br>„Listen Sie die in der vertikalen Konsistenzprüfung verwendeten Anspruchskategorien auf.“ |
| Bewerten von Inhalten anhand der Markenrichtlinien | Bewerten einer veröffentlichten/erstellten Seite, eines Textblocks oder eines Bildes anhand konfigurierter Markenüberprüfungen | aem-governance | Adobe Experience Manager (AEM) | „Bewerten Sie diese Landingpage anhand der SecurBank-Richtlinien<br>„Besteht dieser Slogan unsere Sprachabfrage?“ |
| Debuggen von AEM-Berechtigungen | Debuggen/Verstehen von Berechtigungsrichtlinien, ACLs und Vererbungsregeln. | aem-governance | Adobe Experience Manager (AEM) | „Warum kann der Hauptadministrator `/content/folder/us` auf `https://author/` schreiben?“<br>„Warum kann der Beispielautor `/content/dam` auf `https://author` nicht schreiben?“ |

**Verwandte Informationen**

* [Agentenfunktionen in AEM: Markenverwaltung](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/brand-governance/use-cases)

## Dateneinblicke

| Anwendungsfall | Beschreibung | Skills | Anwendung | Eingabeaufforderungen |
| --- | --- | --- | --- | --- |
| [Abrufen von CJA-Berichten und -Metriken](data-insights/analytics-chat.md) | Abfragen von CJA in Echtzeit, um Metriken, Dimensionen, Segmente und Datenansichten abzurufen | `cja` | Customer Journey Analytics (CJA) | „Anzeigen von Seitenansichten für die letzten 30 Tage“ ・ „Auflisten der wichtigsten Segmente in der Stammdatenansicht“ |
| Vergleichsanalyse | Vergleichen von Metriken über Kanäle, Zeiträume oder Segmente hinweg nebeneinander | `cja-root-cause-analysis`, `cja`, `dx-api`, `knowledge-graph` | Customer Journey Analytics (CJA) | „Umsatz nach Kanal und Monat vergleichen“ ・ „Wie sieht die Konversion von Mobilgeräten und Desktops in diesem Quartal aus?“ |
| Kampagnenleistung | Messen Sie, wie Kampagnen, Kanäle und Web-Eigenschaften über einen bestimmten Zeitraum ausgeführt wurden. | `cja`, `dx-api`, `knowledge-graph` | | „Wie haben sich unsere Acrobat-Web-Kampagnen im letzten Monat entwickelt?“ |
| Funnel-Analyse | Mehrstufige Konversionstrichter mit Abbruch in jeder Phase | `cja` | Customer Journey Analytics (CJA) | „Führen Sie mich durch den Checkout funnel&quot; ・ „Konversions-funnel von PDP zum Kauf anzeigen“ |
| Prognose | Zukünftige Metrikwerte des Projekts basierend auf historischen CJA-Daten | `cja` | Customer Journey Analytics (CJA) | „Prognosesitzungen für die nächsten 30 Tage“ ・ „Sind wir auf dem richtigen Weg, unser Umsatzziel zu erreichen?“ |
| [Ursachenanalyse](data-insights/root-cause-analysis.md) | Finden Sie heraus, warum sich eine Metrik geändert hat: Diagnostizieren von Abfällen, Spitzen und Anomalien | `cja-root-cause-analysis` | Customer Journey Analytics (CJA) | „Warum sind die Konversionen letzte Woche zurückgegangen?“ ・ „Was verursachte die Umsatzspitze am 15. Januar?“ |
| Zusammenfassung für Führungskräfte und KPI-Zusammenfassung | Erstellung von einsatzbereiten Leistungszusammenfassungen für Stakeholder, präskriptiven Empfehlungen und Folienübersichten | `cja-executive-summary`, `cja-bacom-anomaly-tracker-v2`, `cja-cno-weekly-pulse`, `cja-reporting`, `cja`, `dx-api` | Customer Journey Analytics (CJA) | „Ich möchte eine Zusammenfassung des letzten Monats erhalten“ ・ „Erstellen Sie einen Slide-Deck-Entwurf aus den Daten dieses Quartals“ |
| [AA ↔ CJA-Datenvalidierung](data-insights/data-validation-aa-cja.md) | Vergleichen, Überprüfen und Abstimmung von Daten zwischen Adobe Analytics und Customer Journey Analytics, insbesondere beim Upgrade von Adobe Analytics auf Customer Journey Analytics | `aa-cja-validation`, `cja`, `dx-api` | ADOBE ANALYTICS + CJA | „Meine AA Report Suite mit meiner CJA-Datenansicht vergleichen“ ・ „Seitenansichten zwischen AA und CJA validieren“ |
| Operative Zeitreihen- und Kausalanalyse | Abfragen und Analysieren historischer Zeitreihendaten für Zielgruppen, Datensätze und Journey mit kausaler Attribution | `operational-stats-causal-analysis` | Alle infrage kommenden Anträge | „Trends bei der Zielgruppengröße in den letzten 90 Tagen anzeigen“ ・ „Warum hat die Anzahl meiner Datensatzzeilen am 3. März angezogen?“ |
| Erstellen benutzerdefinierter CJA-Kenntnisse | Verwandeln Sie analytische Muster in wiederverwendbare, wiederholbare Fähigkeiten, die sitzungsübergreifend bestehen bleiben | `cja-skill-creator` | Customer Journey Analytics (CJA) | „Diese wöchentliche Umsatzanalyse in wiederverwendbare Kenntnisse umwandeln“ ・ „Als Kenntnisse für monatliches funnel-Reporting speichern“ |

## Zielgruppen

| Anwendungsfall | Beschreibung | Skills | Anwendung | Eingabeaufforderungen |
| --- | --- | --- | --- | --- |
| [Zielgruppen aus natürlicher Sprache erstellen](audiences/create-audience-from-natural-language.md) | Orchestrieren der schrittweisen Zielgruppenerstellung mit Benutzergenehmigung in jeder Phase | `audience-creation-flow` | Real-Time CDP (RTCDP) | „Erstellen Sie eine Audience von Benutzern, die in den letzten 30 Tagen gekauft haben“ ・ „Erstellen Sie ein Segment für hochwertige Mitglieder des Treueprogramms in Kalifornien“ |
| Erstellen von PQL-Definitionen | Zusammenstellen von Zielgruppendefinitionen aus XDM-Eigenschaften, Verhaltensereignissen oder vorhandenen Zielgruppen; Unterstützung von Aggregation und Zeitfenstern | `segment-definition-assembly` | Real-Time CDP (RTCDP) | „Erstellen Sie eine PQL für Personen, die mehr als 3 Produkte angesehen, aber keinen Kauf getätigt haben“ ・ „Hinzufügen eines 7-Tage-Zeitfensters zu meiner Veranstaltungsbedingung“ |
| Zielgruppen suchen und finden | Zielgruppen nach ID, Name und semantischer Suche suchen, Duplikate erkennen und Überschneidungen analysieren | `audience-search` | Real-Time CDP (RTCDP) | „Alle Loyalitäts-Zielgruppen suchen“ ・ „Gibt es ein Duplikat meines Segments „Holiday Shoppers“?“ |
| Zielgruppengröße schätzen | Schätzen der Profilreichweite für einen PQL-Ausdruck mithilfe der Adobe Experience Platform-Vorschau-API mit Abfrage | `audience-size-estimate` | Real-Time CDP (RTCDP) | „Wie groß ist diese Zielgruppe?“ ・ „Geschätzte Reichweite für diesen PQL-Ausdruck“ |
| Audience-Größe - Wasserfall | Unterprädikate für eine PQL erstellen und zeigen, wie jede Bedingung zur endgültigen Zielgruppengröße beiträgt | `audience-size-waterfall` | Real-Time CDP (RTCDP) | „Show me the waterfall for this PQL&quot; ・ „Aufschlüsselung, wie die einzelnen Bedingungen die Zielgruppe reduzieren“ |
| XDM-Felder für das Targeting entdecken | Suchen Sie Felder nach Name, Beschreibung oder Datenwert; sehen Sie, wo sie sich befinden und wo sie bereits verwendet werden | `field-discovery` | Real-Time CDP (RTCDP) | „Welche Felder kann ich verwenden, um Kundinnen und Kunden von Treueprogrammen anzusprechen?“ ・ „Suchen von Feldern im Zusammenhang mit dem Kaufverlauf“ |
| Veröffentlichen/Speichern von Zielgruppen | Beibehalten von Zielgruppendefinitionen im Segmentierungs-Service von Experience Platform mit Benennungskonventionen und Kompatibilitätsprüfungen | `audience-publish` | Real-Time CDP (RTCDP) | „Als Entwurf speichern“ ・ „Die Zielgruppe mit dem Namen „Frühlingsverkaufskäufer“ veröffentlichen“ |

## Journeys

| Anwendungsfall | Beschreibung | Skills | Anwendung | Eingabeaufforderungen |
| --- | --- | --- | --- | --- |
| [Erschaffe Journey aus natürlicher Sprache](journeys/create-journey-from-natural-language.md) | Orchestrieren der Journey-Erstellung in AJO über eine Textaufforderung oder ein hochgeladenes Bild/Flussdiagramm | `journey-create` | Adobe Journey Optimizer (AJO) | „Erstellen Sie eine Begrüßungs-Journey, die nach der Anmeldung eine E-Mail sendet, 3 Tage wartet und dann eine Folgenachricht sendet“ ・ „Erstellen Sie eine Journey aus diesem hochgeladenen Flussdiagrammbild.“ |
| Journey-Konflikte analysieren | Erkennung von Zielgruppenüberschneidungen, Terminkollisionen und Deduplizierungsproblemen zwischen aktiven Journeys | `journey-analyze-conflict` | Adobe Journey Optimizer (AJO) | „Steht mein Warenkorbabbruch-Journey in Konflikt mit anderen Journey?“ ・ „Prüfen Sie, ob sich die Zielgruppen meiner aktiven Journey überschneiden.“ |
| Analysieren von Journey-Fallout | Identifizieren Sie, wo und warum Kunden während eines Journey abbrechen, und erkennen Sie Verhaltensmuster, die zu einer Abmeldung führen | `journey-analyze-fallout` | Adobe Journey Optimizer (AJO) | „Wo kommen die Leute auf meiner Re-Engagement-Journey vorbei?“ ・ „Welche Knoten in Journey X haben den höchsten Fallout?“ |
| Analysieren von Fehlern bei benutzerdefinierten Aktionen | Ermitteln Sie, wann benutzerdefinierte Aktionen fehlschlagen oder Fehlerquoten innerhalb eines Journey in die Höhe schießen, und diagnostizieren Sie die Grundursachen, bevor Fehler in umfassendere Unterbrechungen übergehen. | `journey-analyze-custom-action` | Adobe Journey Optimizer (AJO) | „Warum schlagen benutzerdefinierte Aktionen in meiner Treue-Anmelde-Journey fehl?“ ・ „Fehlerrate für benutzerdefinierte Aktion „ExternalPush“ auf meiner Begrüßungs-Journey anzeigen.“ |
| [Erstellen, Bearbeiten und Verwalten von Herausforderungen im Zusammenhang mit der Treue](journeys/create-loyalty-challenge.md) | Vereinfachen und Beschleunigen der Verwaltung von Treueprogrammen | `loyalty` | Adobe Journey Optimizer (AJO) | „Erstellen Sie eine Herausforderung, die Mitglieder dazu ermutigt, ein neues saisonales Getränk auszuprobieren“ ・ „Zeigen Sie mir Herausforderungen bezüglich der Treue mit den höchsten Abbruchraten für Mitglieder.“ |

## Grundlegende Elemente

| Anwendungsfall | Beschreibung | Skills | Anwendung | Eingabeaufforderungen |
| --- | --- | --- | --- | --- |
| Produktkenntnisse und Dokumentation | Antworten auf Fragen zu Anleitungen, Konzepten, Fehlerbehebung und Best Practices aus offiziellen Adobe-Dokumenten | `product-knowledge` | Alle infrage kommenden Anträge | „Wie richte ich ein Streaming-Ziel ein?“ ・ „Was ist der Unterschied zwischen Batch- und Streaming-Segmentierung?“ |
| Abfragen von Experience Platform-/Journey Optimizer-Entitäten | Dient als primärer Einstiegspunkt für Fragen zu Ihren Platform-Entitäten; Route zu KG, Felderkennung oder APIs nach Bedarf | `operational-insights` | Alle infrage kommenden Anträge | „Wie viele Datensätze habe ich?“ ・ „Alle aktiven Journey anzeigen“ ・ „Meine Ziele auflisten“ |
| Abfragen von Wissensdiagrammen | Aggregierte Zählungen, entitätsübergreifende Joins, Beziehungssuchen und Metadatenexploration über einzelne SQL-Abfragen | `knowledge-graph` | Alle infrage kommenden Anträge | „Welche Zielgruppen verwenden diesen Datensatz?“ ・ „Anzeigen von Beziehungen zwischen Schemata und Datensätzen“ |
| API-Vorgänge für Experience Platform/Journey Optimizer/Customer Journey Analytics | Bereitstellen eines direkten API-Gateways für Mutationen, Echtzeit-Statusprüfungen und Entitätstypen, die nicht im Wissensdiagramm enthalten sind | `cxo-api` | Alle infrage kommenden Anträge | „Datensatz X löschen“ ・ „Status meines Batch-Erfassungsvorgangs überprüfen“ |
| Auflösung und Verknüpfung von Entitäten | Verwenden Sie die semantische und lexikalische Suche, um Entitätsbezeichnungen in tatsächliche Experience Platform-Entitäten aufzulösen und XDM-Felder zu erkennen | `entity-linking` | Adobe Experience Platform | „Auflösen von „Holiday Shoppers“ in eine tatsächliche Zielgruppe“ ・ „Felder zum Kaufverlauf finden“ |
| Benutzerdefinierte Fähigkeiten verwalten | Speichern, Ändern oder Löschen von benutzereigenen wiederverwendbaren Fähigkeiten, die sitzungsübergreifend bestehen bleiben | `manage-skill` | Alle infrage kommenden Anträge | „Diesen Workflow als Qualifikation speichern“ ・ „Meine wöchentlichen Berichtsqualifikationen löschen“ ・ „Diese Qualifikation wiederverwendbar machen“ |
| Überwachen von Streaming-Kapazität und Sicherheitslücken | Überprüfen Sie die aktuelle und frühere Streaming-Nutzung, -Kapazität und den Status der Unterbrechung in allen Sandboxes | `observability-streaming-capacity`, `observability-streaming-usage`, `observability-capacity-breaches` | Adobe Experience Platform | „Welche aktuelle Streaming-Kapazität habe ich in meiner aktuellen Sandbox?“ ・ „Überschreitet meine aktuelle Sandbox in der letzten Woche die Kapazitätsgrenzen?“ |
| [Anzeigen der Ergebnisse der Konsistenzprüfungen](https://experienceleague.adobe.com/en/docs/experience-platform/run-and-operate/health-checks/overview) | Zeigen Sie die neueste Bewertung der Konsistenzprüfung für Ihre Sandbox an, führen Sie eine Fehlerprüfung durch und sehen Sie sich die betroffenen Entitäten an | `rao-view-latest-health-checks-assessment` | Adobe Experience Platform | „Was stimmt nicht in meiner Sandbox?“ ・ „Erzählen Sie mir von meiner neuesten Bewertung der Konsistenzprüfung“ ・ „Was sind die Probleme bei der benutzerdefinierten Namespace-Beschreibungsüberprüfung?“ |
| Beheben von Problemen mit Konsistenzprüfungen | Beheben Sie gekennzeichnete Identity-Namespaces, Zusammenführungsrichtlinien und Schemaprobleme direkt im Chat mit Ihrer Genehmigung, bevor Änderungen vorgenommen werden | `rao-remediate-identity-namespace-description`, `rao-remediate-merge-policy-duplicate-name`, `rao-remediate-missing-audit-field-group`, `rao-remediate-default-merge-policy-naming` | Adobe Experience Platform | „Identity-Namespace-Beschreibungen beheben“ ・ „Doppelte Zusammenführungsrichtlinien-Namen beheben“ ・ „Beheben von Schemata, denen die Audit-Feldergruppe fehlt“ ・ „Beheben der standardmäßigen Benennung von Zusammenführungsrichtlinien“ |

## Sandbox-Werkzeuge

| Anwendungsfall | Beschreibung | Skills | Anwendung | Eingabeaufforderungen |
| --- | --- | --- | --- | --- |
| [Objekte über Sandboxes hinweg verschieben](/help/agents/sandbox-tooling.md) | Nahtlose Migration von Schemas, Zielgruppen und anderen Objektkonfigurationen über Sandboxes hinweg, wobei Abhängigkeiten automatisch aufgelöst werden | `sandbox-tooling-workflow` | Adobe Experience Platform | „Schema-Luma-Platin-Mitglieder des Treueprogramms aus der aktuellen Sandbox in die Produktions-Sandbox verschieben“ ・ „Die Zielgruppe der US-amerikanischen Mitglieder des Treueprogramms für Gold-Mitglieder zur Staging-Umgebung bewerben“ |
