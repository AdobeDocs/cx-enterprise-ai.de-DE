---
description: Durchsuchen Sie die Anwendungsfälle und Beispielaufforderungen des Coworker Chat, sortiert nach Bereichen wie Dateneinblicke, Zielgruppen, Journey und Plattformvorgänge.
title: Anwendungsfälle für den Chat mit Kollegen
product_v2:
  - id: fdae8433-07cd-42e7-acce-738afe63f6bb
feature_v2:
  - id: fdae8433-07cd-42e7-acce-738afe63f6bb
source-git-commit: 83cd3d9dcc9ae0c56e8d63e995b166e8ff0736d9
workflow-type: tm+mt
source-wordcount: 4260
ht-degree: 6%

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
>Siehe auch [KI in AEM - Überblick über die Agentenfunktionen in AEM](https://experienceleague.adobe.com/de/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/overview).

## Markenerlebnis

| Anwendungsfall | Beschreibung | Kenntnisse | Anwendung | Eingabeaufforderungen |
| --- | --- | --- | --- | --- |
| Aktualisieren von AEM-Seiten | Führen Sie Aktionen wie das Aktualisieren, Entfernen, Ersetzen oder Hinzufügen von Inhaltselementen durch, um Erlebnisse genau und aktuell zu halten. Eingaben können natürliche Sprache oder visuelle Anmerkungen wie PDFs oder Screenshots sein. | `aem-sites-pages-update` | Adobe Experience Manager (AEM) - AEM Sites | Aktualisieren Sie auf &lt;URL> die Überschrift zu Hello World<br><br>on &lt;URL> und ändern Sie die Schaltfläche „Take our Coffee Quiz“ in eine ansprechendere Version<br><br>Update &lt;URL> basierend auf dem angehängten <br><br>on &lt;URL> Ich möchte einen neuen Teaser-Abschnitt am Ende der Seite über eine Promotion hinzufügen, die wir im Monat August durchführen, nämlich eine Kaffeemaschine kaufen und zwei Tüten Kaffee kostenlos erhalten. Finde auch Bild von Freunden, die Kaffee trinken und verwende das im Teaser |
| AEM stapelweise aktualisieren | Führen Sie Massenaktionen auf mehreren Seiten gleichzeitig durch, z. B. Entfernen, Ersetzen oder Hinzufügen von Inhaltselementen, um Erlebnisse genau und aktuell zu halten. | `aem-sites-pages-bulkreplace` | Adobe Experience Manager (AEM) - AEM Sites | Aktualisieren Sie auf &lt;aem path> alle Seiten, die die Kopie „MyBarista“ enthalten, auf „BrewPass“. |
| Wechseln von Figma zu visuellem Inhaltsfragment | Importieren Sie Designs direkt aus Figma in Adobe Experience Manager mit natürlicher Sprache. Die SKILL erstellt automatisch das erforderliche Inhaltsmodell, Inhaltsfragment, Assets und Visualisierungsvorlage, sodass Business-Anwender innerhalb von Minuten ohne manuelle Einrichtung vom Design zum Web-fähigen Inhalt wechseln können. | `aem-sites-visualcontentfragments-create` | Adobe Experience Manager (AEM) - AEM Sites | Import aus &lt;FIGMA_URL> |

| Anwendungsfall | Beschreibung | Kenntnisse | Anwendung | Eingabeaufforderungen |
| --- | --- | --- | --- | --- |
| Formular erstellen | Generieren eines neuen adaptiven Formulars aus einer Nur-Sprache-Beschreibung, einer angehängten Kurzbeschreibung, einem Bild oder einer PDF | `aem-forms-adaptiveform-create` | Adobe Experience Manager (AEM) - AEM Forms | „Erstellen eines Onboarding-Formulars für Mitarbeiter“<br><br>„Erstellen eines Formulars mithilfe der angehängten Kurzbeschreibung (Bild oder PDF)“<br><br>„Erstellen eines adaptiven Formulars vom Typ &lt;form>&quot; |
| Formular bearbeiten/aktualisieren | Ändern eines vorhandenen Formulars - Hinzufügen/Bearbeiten von Feldern, Anpassen des einfachen Layouts, Konfigurieren von Übermittlungsaktionen oder Anwenden von Änderungen aus einem angehängten Richtliniendokument | `aem-forms-adaptiveform-edit` | Adobe Experience Manager (AEM) - AEM Forms | „Feld „Mittleren Namen hinzufügen“ unter dem Feld „Vorname“<br><br>„Felder „Vorname“ und „Nachname“ in ein 2-spaltiges Layout einfügen, 50/50“<br><br>„Konfigurieren des Formulars, um Daten an einen REST-Endpunkt zu senden“<br><br>„Aktualisieren Sie dieses Formular, sodass es dem angehängten Dokument mit Richtlinien entspricht“<br><br>„Feld &lt;Name des Felds> hinzufügen“ unter &lt;vorhandenes Feld>&quot; |
| Geschäftslogik hinzufügen | Erstellen Sie einfache Regeln, z. B. das Anzeigen oder Ausblenden eines Felds basierend auf dem Wert eines anderen Felds | `aem-forms-adaptiveform-edit` | Adobe Experience Manager (AEM) - AEM Forms | „Das Feld „Firma“ nur anzeigen, wenn „Mitarbeiter“ „Auftragnehmer“ <br><br>„Das Feld &lt;field> nur anzeigen, wenn &lt;other field> &lt;value> ist“ |
| Formular einschließen | Platzieren eines bestehenden oder neu erstellten Formulars auf einer vorgesehenen AEM Sites-Seite (nur für Edge Delivery Services-Seiten unterstützt) | `aem-forms-adaptiveform-embed` | Adobe Experience Manager (AEM) - AEM Forms | „Formular auf der Homepage unserer Website einbetten“<br><br>„Formular auf &lt;Seitenpfad> einbetten“ |

**Verwandte Informationen**

* [Agentenfunktionen in AEM: Markenerlebnis - Erlebnisproduktion - Sites](https://experienceleague.adobe.com/de/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/brand-experience/experience-production/use-cases#use-cases-sites)

* [Agentenfunktionen in AEM: Markenerlebnis - Erlebnisproduktion - Forms](https://experienceleague.adobe.com/de/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/brand-experience/experience-production/use-cases#use-cases-forms)

### Entwicklung

| Anwendungsfall | Beschreibung | Kenntnisse | Anwendung | Eingabeaufforderungen |
| --- | --- | --- | --- | --- |
| Verwalten von Cloud Manager-Pipelines | Erstellen, Ausführen und Überwachen von AEM Cloud Manager-Pipelines, einschließlich Protokollen, Artefakten, Variablen und Einstellungen | `cloud-manager-pipeline-management` | Adobe Experience Manager (AEM) | „Pipelines für Programm 12345 auflisten“<br><br>„Was ist der Status meiner letzten Pipeline?“ |
| Verwalten von Cloud Manager-Umgebungen | Erstellen, Konfigurieren und Verwalten von AEM Cloud Manager-Umgebungen, einschließlich RDEs, Umgebungsvariablen, Protokollen und Backups | `cloud-manager-environment-management` | Adobe Experience Manager (AEM) | „Meine Umgebungen für Programm 12345 auflisten“<br><br>„RDE zurücksetzen“ |
| Verwalten von Cloud Manager-Programmen | Auflisten, Überprüfen und Löschen von AEM Cloud Manager-Programmen, einschließlich ihrer Pipelines und Umgebungen | `cloud-manager-program-management` | Adobe Experience Manager (AEM) | „Meine Cloud Manager-Programme auflisten“<br><br>„Details zu 12345 abrufen“ |
| Verwalten von Zeitplänen für die Aktualisierung von AEM-Versionen | Konfigurieren Sie die täglichen Ruhezeiten und Freie Zeiträume für die automatisierte Wartung und sehen Sie sich die globalen Fenster zum Einfrieren von Code in Adobe an | `cloud-manager-release-management` | Adobe Experience Manager (AEM) | „Was ist mein aktuelles Fenster für die Ruhezeiten?“<br><br>„Planen Sie einen Zeitraum ohne Updates vom 20. Dezember bis zum 2. Januar“ |

**Verwandte Informationen**

* [Agentenfunktionen in AEM: Markenerlebnis - Entwicklung](https://experienceleague.adobe.com/de/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/brand-experience/development/use-cases)

### Einstieg

| Anwendungsfall | Beschreibung | Kenntnisse | Anwendung | Eingabeaufforderungen |
| --- | --- | --- | --- | --- |
| Geführtes End-to-End-Onboarding | Orchestriert den gesamten Onboarding-Lebenszyklus, die Repository-Auswahl, die Zuweisung zum Ordner, Tags, Metadaten, Import und Suche, wenn Sie die benötigten Onboarding-Aufgaben nicht kennen. | `aem-onboarding-workflow` | Adobe Experience Manager (AEM) - AEM Assets | „Begleiten Sie unser Team beim AEM Assets<br><br>„Begleiten Sie mich beim AEM DAM-Onboarding“ |
| Entwerfen und Erstellen von Ordnerhierarchien | Empfiehlt und erstellt skalierbare Ordnerstrukturen in AEM Assets (unter `/content/dam`) basierend auf Geschäftsanforderungen oder CSV-Eingaben. | `aem-folder-management` | Adobe Experience Manager (AEM) - AEM Assets | „Eine Ordnerstruktur für unsere Lifestyle-Marketing-Assets empfehlen“<br><br>„Erstellen von Ordnern basierend auf dieser CSV-Datei“ |
| Entwerfen und Erstellen von Tags | Entwirft und erstellt kontrollierte Tag-Vokabeln unter `/content/cq:tags` - Namespaces, hierarchische Tags und Batch-Tag-Vorgänge. | `aem-tag-taxonomy` | Adobe Experience Manager (AEM) - AEM Assets | „Entwerfen Sie eine Tag-Taxonomie mit Namespaces für unsere Produktkategorien“<br><br>„Importieren Sie Tags aus dieser CSV-Datei“<br><br>„Erstellen Sie diese hierarchischen Tags in AEM&quot; |
| Erstellen und Zuweisen von Metadatenformularen | Entwirft und erstellt benutzerdefinierte Metadatenformulare, die die Autoren der Inhaltserstellungs-Benutzeroberfläche aus einer CSV-Datei, Tabelle, einem Anforderungsdokument oder einer Beschreibung verwenden, und weist sie dann optional Ordnern zu. | `aem-metadata-form` | Adobe Experience Manager (AEM) - AEM Assets | „Erstellen eines Metadatenformulars aus dieser Feldliste“<br><br>„Zuweisen dieses Formulars zum `campaigns`&quot; |

**Verwandte Informationen**

* [Agenturfunktionen in AEM: Markenerlebnis - Onboarding](https://experienceleague.adobe.com/de/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/brand-experience/onboarding/use-cases)

## Inhaltsratgeber

### Content Discovery

| Anwendungsfall | Beschreibung | Kenntnisse | Anwendung | Eingabeaufforderungen |
| --- | --- | --- | --- | --- |
| Nach semantischem Design suchen | Finden Sie Assets nach Konzept, Stimmung oder visuellem Design mithilfe von KI-gestütztem semantischen Abgleich. | `aem-assets-discovery` | Adobe Experience Manager (AEM) - AEM Assets | „Finde mir Bilder vom Morgen-Kaffee-Lifestyle“ |
| Nach benutzerdefinierten Metadaten suchen | Filtern von Assets nach benutzerdefinierten Metadatenfeldern (z. B. Kaffeemischung, Marke, Röststufe). | `aem-assets-discovery` | Adobe Experience Manager (AEM) - AEM Assets | „Assets suchen, bei denen `Coffee Blend` `Morning Muse` ist“<br><br>„Assets abrufen, deren Lizenz nicht abgelaufen ist“<br><br>„Assets suchen, bei denen der Kampagnenname nicht festgelegt ist (die Eigenschaft muss für entsprechende Ergebnisse indiziert werden).“ |
| Nach Genehmigungsstatus suchen | Filtern Sie Assets nach dem Genehmigungsstatus. Beispielsweise den Status „Genehmigt“, „In Überprüfung“, „Abgelehnt“ oder „Fehlend“. | `aem-assets-discovery` | Adobe Experience Manager (AEM) - AEM Assets | „Anzeigen aller genehmigten Assets im Ordner &quot;`Campaign`&quot; |
| Nach Ordner/Pfad suchen | Identifizieren von Assets durch Interpretieren natürlicher Sprachaufforderungen, die auf Ordnernamen in AEM verweisen. Sie können den Ordner einfach in der Eingabeaufforderung erwähnen, ohne manuell durch das Repository zu navigieren, was die Anzahl der Klicks, die zum Auffinden des richtigen Inhalts erforderlich sind, erheblich reduziert. | `aem-assets-discovery` | Adobe Experience Manager (AEM) - AEM Assets | „Gibt es SVGs im Ordner `WKND`?<br><br>„Nach dem 1. November 2025 geänderte Assets in Ordner `WKND` anzeigen“ |

**Verwandte Informationen**

* [Agentenfunktionen in AEM: Content Advisor - Content Discovery](https://experienceleague.adobe.com/de/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/content-advisor/discovery/use-cases)

### Inhaltsoptimierung

| Anwendungsfall | Beschreibung | Kenntnisse | Anwendung | Eingabeaufforderungen |
| --- | --- | --- | --- | --- |
| Erstellung hochauflösender Ausgabedarstellungen und kanaloptimierte Ausgabedarstellungen | Generieren neuer Ausgabedarstellungen eines Assets mit einer festgelegten Auflösung und Qualitätsstufe, sodass kanalbereite Varianten ohne manuelle Bearbeitung einfach vorbereitet werden können. Sie können auch Ausgabedarstellungen erstellen, die auf plattformspezifische Anforderungen zugeschnitten sind, z. B. Instagram-Stories, um sicherzustellen, dass Assets automatisch Format-, Übersetzungs- und Qualitätsrichtlinien erfüllen. | `aem-assets-content-optimisation` | Adobe Experience Manager (AEM) - AEM Assets | „Erstellen einer `2000px` Ausgabedarstellung wie `JPEG` mit `80% quality`&quot;<br><br>„Erstellen einer Ausgabedarstellung für eine Instagram-Story“ |
| Markenüberlagerungen und Composite-Generierung | Wenden Sie Werbe-Grafiken, -Überlagerungen oder -Abzeichen auf vorhandene Assets mit präziser Platzierung an, um die schnelle Erstellung von kampagnenbereiten Composites zu unterstützen. | `aem-assets-content-optimisation` | Adobe Experience Manager (AEM) - AEM Assets | „Überlagern Sie das Bild mit `30%` Rabattgrafiken über dem Werbebanner und platzieren Sie es `100px` von der Mitte.“ |
| Bildverbesserungen, Anpassungen der Hintergrundfarbe, Ausrichtungstransformationen | Wenden Sie visuelle Verbesserungen an (Scharfzeichnen von Bildern), ersetzen Sie Hintergrundfarben und führen Sie Ausrichtungstransformationen durch. | `aem-assets-content-optimisation` | Adobe Experience Manager (AEM) - AEM Assets | „Hintergrundfarbe des `PNG` ändern zu `#ff8932`&quot;<br><br>„Bild scharfzeichnen“<br><br>„Bild horizontal spiegeln“ |

**Verwandte Informationen**

* [Agentenfunktionen in AEM: Inhaltsberater - Inhaltsoptimierung](https://experienceleague.adobe.com/de/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/content-advisor/content-optimization/use-cases)

## Marken-Governance

| Anwendungsfall | Beschreibung | Skills | Anwendung | Eingabeaufforderungen |
| --- | --- | --- | --- | --- |
| Richtlinie und Segmentsuche | Abrufen detaillierter Markenrichtlinien nach Segment, Markt oder Kategorie | enterprise-context | Adobe Experience Manager (AEM) | „Was sind die Klangfarben-Richtlinien für diese Marke?“<br>„Listen Sie die in der vertikalen Konsistenzprüfung verwendeten Anspruchskategorien auf.“ |
| Bewerten von Inhalten anhand der Markenrichtlinien | Bewerten einer veröffentlichten/erstellten Seite, eines Textblocks oder eines Bildes anhand konfigurierter Markenüberprüfungen | aem-governance | Adobe Experience Manager (AEM) | „Bewerten Sie diese Landingpage anhand der SecurBank-Richtlinien<br>„Besteht dieser Slogan unsere Sprachabfrage?“ |
| Debuggen von AEM-Berechtigungen | Debuggen/Verstehen von Berechtigungsrichtlinien, ACLs und Vererbungsregeln. | aem-governance | Adobe Experience Manager (AEM) | „Warum kann der Hauptadministrator `/content/folder/us` auf `https://author/` schreiben?“<br>„Warum kann der Beispielautor `/content/dam` auf `https://author` nicht schreiben?“ |

**Verwandte Informationen**

* [Agentenfunktionen in AEM: Markenverwaltung](https://experienceleague.adobe.com/de/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/brand-governance/use-cases)

## Dateneinblicke

| Anwendungsfall | Beschreibung | Skills | Anwendung | Eingabeaufforderungen |
| --- | --- | --- | --- | --- |
| [Abrufen von CJA-Berichten und -Metriken](data-insights/analytics-chat.md) | Abfragen von CJA in Echtzeit, um Metriken, Dimensionen, Segmente und Datenansichten abzurufen | `cja` | Customer Journey Analytics (CJA) | „Anzeigen der Seitenansichten für die letzten 30 Tage“ <br> „Auflisten der wichtigsten Segmente in der Stammdatenansicht“ |
| Vergleichsanalyse | Vergleichen von Metriken über Kanäle, Zeiträume oder Segmente hinweg nebeneinander | `cja-root-cause-analysis`, `cja`, `dx-api`, `knowledge-graph` | Customer Journey Analytics (CJA) | „Umsatz nach Kanal und Monat vergleichen“ <br> „Wie sieht die Konversion von Mobilgeräten und Desktops in diesem Quartal aus?“ |
| Kampagnenleistung | Messen Sie, wie Kampagnen, Kanäle und Web-Eigenschaften über einen bestimmten Zeitraum ausgeführt wurden. | `cja`, `dx-api`, `knowledge-graph` | | „Wie haben sich unsere Acrobat-Web-Kampagnen im letzten Monat entwickelt?“ |
| Funnel-Analyse | Mehrstufige Konversionstrichter mit Abbruch in jeder Phase | `cja` | Customer Journey Analytics (CJA) | „Führen Sie mich durch den Checkout funnel&quot; <br> „Konversions-funnel von PDP zum Kauf anzeigen“ |
| Prognose | Zukünftige Metrikwerte des Projekts basierend auf historischen CJA-Daten | `cja` | Customer Journey Analytics (CJA) | „Prognostizierte Sitzungen für die nächsten 30 Tage“ <br> „Sind wir auf dem besten Weg, unser Umsatzziel zu erreichen?“ |
| [Ursachenanalyse](data-insights/root-cause-analysis.md) | Finden Sie heraus, warum sich eine Metrik geändert hat: Diagnostizieren von Abfällen, Spitzen und Anomalien | `cja-root-cause-analysis` | Customer Journey Analytics (CJA) | „Warum sind die Konversionen letzte Woche zurückgegangen?“ <br> „Was verursachte die Umsatzspitze am 15. Januar?“ |
| Zusammenfassung für Führungskräfte und KPI-Zusammenfassung | Erstellung von einsatzbereiten Leistungszusammenfassungen für Stakeholder, präskriptiven Empfehlungen und Folienübersichten | `cja-executive-summary`, `cja-bacom-anomaly-tracker-v2`, `cja-cno-weekly-pulse`, `cja-reporting`, `cja`, `dx-api` | Customer Journey Analytics (CJA) | „Gib mir eine Zusammenfassung des letzten Monats“ <br> „Erstellen eines Folien-Decks aus den Daten dieses Quartals“ |
| [AA ↔ CJA-Datenvalidierung](data-insights/data-validation-aa-cja.md) | Vergleichen, Überprüfen und Abstimmung von Daten zwischen Adobe Analytics und Customer Journey Analytics, insbesondere beim Upgrade von Adobe Analytics auf Customer Journey Analytics | `aa-cja-validation`, `cja`, `dx-api` | ADOBE ANALYTICS + CJA | „Meine AA Report Suite mit meiner CJA-Datenansicht vergleichen“ <br> „Seitenansichten zwischen AA und CJA validieren“ |
| Operative Zeitreihen- und Kausalanalyse | Abfragen und Analysieren historischer Zeitreihendaten für Zielgruppen, Datensätze und Journey mit kausaler Attribution | `operational-stats-causal-analysis` | Alle infrage kommenden Anträge | „Trends bei der Zielgruppengröße in den letzten 90 Tagen anzeigen“ <br> „Warum hat die Anzahl meiner Datensatzzeilen am 3. März angezogen?“ |
| Erstellen benutzerdefinierter CJA-Kenntnisse | Verwandeln Sie analytische Muster in wiederverwendbare, wiederholbare Fähigkeiten, die sitzungsübergreifend bestehen bleiben | `cja-skill-creator` | Customer Journey Analytics (CJA) | „Diese wöchentliche Umsatzanalyse in wiederverwendbare Kenntnisse umwandeln“ <br> „Als Kenntnisse für monatliches funnel-Reporting speichern“ |

## Zielgruppen

| Anwendungsfall | Beschreibung | Skills | Anwendung | Eingabeaufforderungen |
| --- | --- | --- | --- | --- |
| [Zielgruppen aus natürlicher Sprache erstellen](audiences/create-audience-from-natural-language.md) | Orchestrieren der schrittweisen Zielgruppenerstellung mit Benutzergenehmigung in jeder Phase | `audience-creation-flow` | Real-Time CDP (RTCDP) | „Erstellen Sie eine Zielgruppe von Benutzern, die in den letzten 30 Tagen gekauft haben“ <br> „Erstellen Sie ein Segment für hochwertige Mitglieder des Treueprogramms in Kalifornien“ |
| Erstellen von PQL-Definitionen | Zusammenstellen von Zielgruppendefinitionen aus XDM-Eigenschaften, Verhaltensereignissen oder vorhandenen Zielgruppen; Unterstützung von Aggregation und Zeitfenstern | `segment-definition-assembly` | Real-Time CDP (RTCDP) | „Erstellen Sie eine PQL für Personen, die mehr als 3 Produkte angesehen, aber nicht gekauft haben“ <br> „Hinzufügen eines 7-Tage-Zeitfensters zu meiner Veranstaltungsbedingung“ |
| Zielgruppen suchen und finden | Zielgruppen nach ID, Name und semantischer Suche suchen, Duplikate erkennen und Überschneidungen analysieren | `audience-search` | Real-Time CDP (RTCDP) | „Alle Loyalitäts-Zielgruppen suchen“ <br> „Gibt es ein Duplikat meines Segments „Holiday Shoppers“?“ |
| Zielgruppengröße schätzen | Schätzen der Profilreichweite für einen PQL-Ausdruck mithilfe der Adobe Experience Platform-Vorschau-API mit Abfrage | `audience-size-estimate` | Real-Time CDP (RTCDP) | „Wie groß ist diese Zielgruppe?“ <br> „Geschätzte Reichweite für diesen PQL-Ausdruck“ |
| Audience-Größe - Wasserfall | Unterprädikate für eine PQL erstellen und zeigen, wie jede Bedingung zur endgültigen Zielgruppengröße beiträgt | `audience-size-waterfall` | Real-Time CDP (RTCDP) | „Show me the waterfall for this PQL&quot; <br> „Aufschlüsselung, wie die einzelnen Bedingungen die Zielgruppe reduzieren“ |
| XDM-Felder für das Targeting entdecken | Suchen Sie Felder nach Name, Beschreibung oder Datenwert; sehen Sie, wo sie sich befinden und wo sie bereits verwendet werden | `field-discovery` | Real-Time CDP (RTCDP) | „Welche Felder kann ich verwenden, um Kundinnen und Kunden von Treueprogrammen anzusprechen?“ <br> „Suchen von Feldern im Zusammenhang mit dem Kaufverlauf“ |
| Veröffentlichen/Speichern von Zielgruppen | Beibehalten von Zielgruppendefinitionen im Segmentierungs-Service von Experience Platform mit Benennungskonventionen und Kompatibilitätsprüfungen | `audience-publish` | Real-Time CDP (RTCDP) | „Als Entwurf speichern“ <br> „Zielgruppe mit dem Namen „Frühlingsverkaufskäufer“ veröffentlichen“ |

## Journeys

| Anwendungsfall | Beschreibung | Skills | Anwendung | Eingabeaufforderungen |
| --- | --- | --- | --- | --- |
| [Erschaffe Journey aus natürlicher Sprache](journeys/create-journey-from-natural-language.md) | Orchestrieren der Journey-Erstellung in AJO über eine Textaufforderung oder ein hochgeladenes Bild/Flussdiagramm | `journey-create` | Adobe Journey Optimizer (AJO) | „Erstellen Sie eine Begrüßungs-Journey, die nach der Anmeldung eine E-Mail sendet, 3 Tage wartet und dann eine Folgenachricht sendet“ <br> „Erstellen Sie eine Journey aus diesem hochgeladenen Flussdiagrammbild“ |
| Journey-Konflikte analysieren | Erkennung von Zielgruppenüberschneidungen, Terminkollisionen und Deduplizierungsproblemen zwischen aktiven Journeys | `journey-analyze-conflict` | Adobe Journey Optimizer (AJO) | „Steht mein Journey bei Warenkorbabbruch in Konflikt mit anderen Journey?“ <br> „Prüfen Sie, ob sich die Zielgruppen meiner aktiven Journey überschneiden.“ |
| Analysieren von Journey-Fallout | Identifizieren Sie, wo und warum Kunden während eines Journey abbrechen, und erkennen Sie Verhaltensmuster, die zu einer Abmeldung führen | `journey-analyze-fallout` | Adobe Journey Optimizer (AJO) | „Wo kommen die Leute auf meiner Re-Engagement-Journey hin?“ <br> „Welche Knoten in Journey X haben den höchsten Fallout?“ |
| Analysieren von Fehlern bei benutzerdefinierten Aktionen | Ermitteln Sie, wann benutzerdefinierte Aktionen fehlschlagen oder Fehlerquoten innerhalb eines Journey in die Höhe schießen, und diagnostizieren Sie die Grundursachen, bevor Fehler in umfassendere Unterbrechungen übergehen. | `journey-analyze-custom-action` | Adobe Journey Optimizer (AJO) | „Warum schlagen benutzerdefinierte Aktionen in meiner Treue-Anmelde-Journey fehl?“ <br> „Fehlerrate für benutzerdefinierte Aktion „ExternalPush“ in meiner Begrüßungs-Journey anzeigen.“ |
| [Erstellen, Bearbeiten und Verwalten von Herausforderungen im Zusammenhang mit der Treue](journeys/create-loyalty-challenge.md) | Vereinfachen und Beschleunigen der Verwaltung von Treueprogrammen | `loyalty` | Adobe Journey Optimizer (AJO) | „Erstellen Sie eine Herausforderung, die Mitglieder dazu ermutigt, ein neues saisonales Getränk auszuprobieren“ <br> „Herausforderungen bezüglich der Treue mit den höchsten Abbruchraten für Mitglieder zeigen“. |

## Grundlegende Elemente

| Anwendungsfall | Beschreibung | Skills | Anwendung | Eingabeaufforderungen |
| --- | --- | --- | --- | --- |
| Produktkenntnisse und Dokumentation | Antworten auf Fragen zu Anleitungen, Konzepten, Fehlerbehebung und Best Practices aus offiziellen Adobe-Dokumenten | `product-knowledge` | Alle infrage kommenden Anträge | „Wie richte ich ein Streaming-Ziel ein?“ <br> „Was ist der Unterschied zwischen Batch- und Streaming-Segmentierung?“ |
| Abfragen von Experience Platform-/Journey Optimizer-Entitäten | Dient als primärer Einstiegspunkt für Fragen zu Ihren Platform-Entitäten; Route zu KG, Felderkennung oder APIs nach Bedarf | `operational-insights` | Alle infrage kommenden Anträge | „Wie viele Datensätze habe ich?“ <br> „Alle aktiven Journey anzeigen“ <br> „Meine Ziele auflisten“ |
| Abfragen von Wissensdiagrammen | Aggregierte Zählungen, entitätsübergreifende Joins, Beziehungssuchen und Metadatenexploration über einzelne SQL-Abfragen | `knowledge-graph` | Alle infrage kommenden Anträge | „Welche Zielgruppen verwenden diesen Datensatz?“ <br> „Anzeigen von Beziehungen zwischen Schemas und Datensätzen“ |
| API-Vorgänge für Experience Platform/Journey Optimizer/Customer Journey Analytics | Bereitstellen eines direkten API-Gateways für Mutationen, Echtzeit-Statusprüfungen und Entitätstypen, die nicht im Wissensdiagramm enthalten sind | `cxo-api` | Alle infrage kommenden Anträge | „Datensatz X löschen“ <br> „Status meines Batch-Erfassungsvorgangs überprüfen“ |
| Auflösung und Verknüpfung von Entitäten | Verwenden Sie die semantische und lexikalische Suche, um Entitätsbezeichnungen in tatsächliche Experience Platform-Entitäten aufzulösen und XDM-Felder zu erkennen | `entity-linking` | Adobe Experience Platform | „Auflösen von „Holiday Shoppers“ in eine tatsächliche Zielgruppe“ <br> „Felder für „Mich finden“ im Zusammenhang mit dem Kaufverlauf“ |
| Benutzerdefinierte Fähigkeiten verwalten | Speichern, Ändern oder Löschen von benutzereigenen wiederverwendbaren Fähigkeiten, die sitzungsübergreifend bestehen bleiben | `manage-skill` | Alle infrage kommenden Anträge | „Diesen Workflow als Qualifikation speichern“ <br> „Meine wöchentlichen Berichtsqualifikationen löschen“ <br> „Diese Qualifikation wiederverwendbar machen“ |
| Überwachen von Streaming-Kapazität und Sicherheitslücken | Überprüfen Sie die aktuelle und frühere Streaming-Nutzung, -Kapazität und den Status der Unterbrechung in allen Sandboxes | `observability-streaming-capacity`, `observability-streaming-usage`, `observability-capacity-breaches` | Adobe Experience Platform | „Wie hoch ist meine aktuelle Streaming-Kapazität in meiner aktuellen Sandbox?“ <br> „Überschreitet meine aktuelle Sandbox in der letzten Woche die Kapazitätsbeschränkungen?“ |
| [Anzeigen der Ergebnisse der Konsistenzprüfungen](https://experienceleague.adobe.com/de/docs/experience-platform/run-and-operate/health-checks/overview) | Zeigen Sie die neueste Bewertung der Konsistenzprüfung für Ihre Sandbox an, führen Sie eine Fehlerprüfung durch und sehen Sie sich die betroffenen Entitäten an | `rao-view-latest-health-checks-assessment` | Adobe Experience Platform | „Was ist los in meiner Sandbox?“ <br> „Erzählen Sie mir von meiner neuesten Bewertung der Konsistenzprüfung“ <br> „Was sind die Probleme bei der benutzerdefinierten Namespace-Beschreibungsüberprüfung?“ |
| Beheben von Problemen mit Konsistenzprüfungen | Beheben Sie gekennzeichnete Identity-Namespaces, Zusammenführungsrichtlinien und Schemaprobleme direkt im Chat mit Ihrer Genehmigung, bevor Änderungen vorgenommen werden | `rao-remediate-identity-namespace-description`, `rao-remediate-merge-policy-duplicate-name`, `rao-remediate-missing-audit-field-group`, `rao-remediate-default-merge-policy-naming` | Adobe Experience Platform | „Identity-Namespace-Beschreibungen korrigieren“ <br> „Doppelte Zusammenführungsrichtlinien-Namen korrigieren“ <br> „Fehlende Überwachungsfeldgruppe in Schemas beheben“ <br> „Standardbenennung der Zusammenführungsrichtlinie korrigieren“ |

## Sandbox-Werkzeuge

| Anwendungsfall | Beschreibung | Skills | Anwendung | Eingabeaufforderungen |
| --- | --- | --- | --- | --- |
| [Objekte über Sandboxes hinweg verschieben](/help/agents/sandbox-tooling.md) | Nahtlose Migration von Schemas, Zielgruppen und anderen Objektkonfigurationen über Sandboxes hinweg, wobei Abhängigkeiten automatisch aufgelöst werden | `sandbox-tooling-workflow` | Adobe Experience Platform | „Verschieben des Schemas Luma Loyalty Members Platinum von der aktuellen Sandbox in die Produktions-Sandbox“ <br> „Heraufstufen der Zielgruppe der US-Gold-Loyalty Members zur Staging-Umgebung“ |

## Warnhinweise für Kunden

| Anwendungsfall | Beschreibung | Skills | Anwendung | Eingabeaufforderungen |
| --- | --- | --- | --- | --- |
| Verwalten von Warnhinweis-Abonnements | Anzeigen und Verwalten von Warnhinweis-Abonnements über Konversationen in natürlicher Sprache. | `alerts-subscribe` | Adobe Experience Platform | „Welche Warnhinweise habe ich abonniert?“<br><br>„Melde mich für diesen Warnhinweis an.“<br><br>„Entfernen Sie mein Abonnement für diesen Warnhinweis.“ |
| Warnungsaktivität überprüfen | Überprüfen des aktuellen Warnhinweisstatus und der historischen Warnhinweisaktivität für einen bestimmten Zeitraum. | `alerts-list` | Adobe Experience Platform | „Was ist in den letzten 24 Stunden passiert?“<br><br>„Welche Warnhinweise wurden in den letzten 24 Stunden ausgelöst?“<br><br>„Anzeigen aktiver Warnhinweise aus den letzten sieben Tagen.“ |
| Identifizieren von Mustern wiederkehrender Warnhinweise | Analysieren Sie den Warnhinweisverlauf, um häufig ausgelöste Warnhinweistypen und operative Trends zu identifizieren. | `alerts-list` | Adobe Experience Platform | „Zeigen Sie mir die drei am häufigsten ausgelösten Warnhinweistypen.“<br><br>„Welche Warnhinweistypen traten in diesem Monat am häufigsten auf?“<br><br>„Welche Warnhinweismuster sehen Sie in den letzten sieben Tagen?“ |
| Konzentration auf Themen mit hoher Priorität | Filtern Sie die Warnungsaktivität nach Schweregrad, um Ermittlungsaktivitäten zu priorisieren. | `alerts-list` | Adobe Experience Platform | „Nur Warnhinweise mit hohem Schweregrad anzeigen.“<br><br>„Welche kritischen Warnhinweise wurden diese Woche ausgelöst?“<br><br>„Anzeigen kritischer Warnhinweise aus den letzten 30 Tagen.“ |
| Verstehen des Auswirkungsradius von Warnhinweisen | Identifizieren Sie die Objekte, die am meisten von Warnhinweisen betroffen sind, und bestimmen Sie, wo die Ermittlung beginnen soll. | `alerts-list` | Adobe Experience Platform | „Was sind die fünf am stärksten betroffenen Objekte?“<br><br>„Welche Objekte sind den Warnhinweisen mit dem höchsten Schweregrad zugeordnet?“ |
| Verbinden von Warnhinweistypen mit betroffenen Objekten | Analysieren Sie die Beziehungen zwischen Warnhinweistypen und betroffenen Ressourcen. | `alerts-list` | Adobe Experience Platform | „Welche Warnhinweistypen haben sich am häufigsten auf diesen Datensatz ausgewirkt?“<br><br>„Zeigt die Beziehung zwischen Warnhinweistypen und betroffenen Objekten.“<br><br>„Welcher Warnhinweistyp hat das am häufigsten betroffene Objekt am häufigsten betroffen?“ |
| Fokus auf meine Warnhinweise | Analysieren Sie Warnhinweise, die Sie abonniert haben und für die Überwachung verantwortlich sind. | `alerts-list` | Adobe Experience Platform | „Zeigen Sie mir die Warnhinweise mit hohem Schweregrad, die ich abonniert habe.“<br><br>„Welche Warnhinweise aus meinen Warnhinweisen wurden diese Woche ausgelöst?“<br><br>„Erfordert eine meiner abonnierten Warnhinweise Aufmerksamkeit?“ |

## Workflow und Planung

| Anwendungsfall | Beschreibung | Skills | Anwendung | Eingabeaufforderungen |
| --- | --- | --- | --- | --- |
| Verwalten von Planning Workspace | Erstellen und entwickeln Sie Workfront Planning-Arbeitsbereiche, Abschnitte, Datensatztypen und Felder, um Programme zu organisieren und die Arbeit zu verfolgen | `manage-workfront-planning`, `wf-planning-solution-architect` | Workfront-Planung | „Erstellen Sie einen Arbeitsbereich mit dem Namen MKG Hub und richten Sie Datensatztypen ein, um Programme nach Region zu verfolgen“ <br> „Richten Sie die Datensatztypen und Beziehungen ein, die zum Tracking von MKG-Programmen über Kanäle und Regionen hinweg erforderlich sind“ |
| Verwalten von Planungsdatensätzen | Erstellen und Aktualisieren von Planungsdatensätzen (Kampagnen, Briefs) und deren Feldwerten in einem Arbeitsbereich | `manage-workfront-planning` | Workfront-Planung | „Erstellen Sie einen Überblick für die Herbst-Brand Launch-Kampagne mit den Zielen, der Zielgruppe und den wichtigsten Botschaften“ <br> „Aktualisieren Sie den Herbst-Brand Launch-Überblick mit dem Budget und den primären Kanälen“ |
| Erstellen und Verwalten von Projekten | Projekte starten und strukturieren: Vorlagen anwenden, Prioritäten und Budgets festlegen, Aufgaben sequenzieren, Phasen und Abhängigkeiten hinzufügen und Personen oder Rollen zuweisen | `manage-workfront-workflow` | Workfront-Workflow | „Erstellen Sie eine Frühjahrskampagne, legen Sie ihr eine hohe Priorität mit einem Budget von 200.000 Dollar fest und sequenzieren Sie die Aufgaben“ <br> „Erstellen Sie einen Workfront-Projektplan mit dem Namen [Projektname] aus [Projektvorlage]&quot; <br> „Erstellen Sie einen Projektplan für den Herbststart: Social-Media-Kampagne mit Aufgaben für Konzeption, Design, Kopie und Überprüfung“ <br> „Fügen Sie eine neue E-Mail-Marketing-Aufgabe hinzu und weisen Sie sie Rachel Smith zu“ |
| Beschleunigen von Überprüfungen und Genehmigungen | Mehrstufige Validierungen einrichten, Validierungsvorlagen anwenden, Genehmigende Personen hinzufügen/entfernen, Erinnerungen senden und Massenaktualisierungen durchführen | `manage-workfront-workflow` | Workfront-Workflow | „Erstellen Sie eine mehrstufige Genehmigung (Kopie, Entwurf, legal) und erinnern Sie alle, die dies nicht genehmigt haben“ <br> „Entfernen Sie Chris Smith aus allen offenen Genehmigungen und ersetzen Sie durch Jane Francis“ |
| Aufgaben- und Arbeitsstatus aktualisieren | Aufgaben als abgeschlossen markieren, Prozent abgeschlossen aktualisieren und Arbeit schließen | `manage-workfront-workflow` | Workfront-Workflow | „Meine Aufgabe ‚Schlüsselgrafik erstellen‘ bei Herbststart als abgeschlossen markieren“ <br> „Meine Aufgabe ‚Kopie für Herbststart‘ bei 100 % schließen“ |
| Erkenntnisse zur Oberflächenarbeit | Stellen Sie Sondierungsfragen, um eine gefährdete Arbeit, nicht zugewiesene Aufgaben, offene Probleme und den Status in allen Projekten zu finden | `query-workfront` | Workfront-Workflow | „Ermitteln Sie noch nicht abgeschlossene Aufgaben für aktuelle Projekte, die niemandem zugewiesen sind und diese Woche fällig sind“ <br> „Wie viele offene Probleme gibt es in allen aktuellen Projekten?“ |
| Zusammenfassung der Projekte und Aufgaben | Listen, Tabellen und Anzahl von Projekten, Aufgaben, Problemen und Zuweisungen abrufen | `query-workfront` | Workfront-Workflow | „Zeigen Sie mir eine Tabelle mit den startbereiten Aufgaben mit dem Projektnamen, dem Fälligkeitsdatum der Aufgabe und dem zugewiesenen Benutzer“ <br> „Erhalten Sie mir alle Aufgaben zugewiesen [Benutzername]&quot; |
| Genehmigungen und Portfoliostatus nachverfolgen | Überprüfen Sie den Status Ihrer Genehmigungen und aggregieren Sie unvollständige Arbeiten nach Portfolio. | `query-workfront` | Workfront-Workflow | „Status meiner Genehmigungen anzeigen“ <br> „Tabelle mit unvollständigen Problemen anzeigen, die Teil des [Portfolio-Namensportfolios sind]&quot; |

## Experimentieren und Optimieren

| Domain | Anwendungsfall | Beschreibung | Skills | Anwendung | Eingabeaufforderungen |
| --- | --- | --- | --- | --- | --- |
| **Experimentieren und Optimieren** | Zielentitäten durchsuchen und suchen | Identifizieren, Überprüfen, Suchen und Auflisten von Target-Entitäten: Aktivitäten (A/B, XT, AP, Automatische Zuordnung, MVT), Zielgruppen und Angebote. Beginnen Sie hier mit Ihrer Entdeckung. | `target-browse` | Adobe Target | „Alle aktiven A/B-Aktivitäten anzeigen“<br>„Welche Zielgruppen habe ich?“<br>„Aktivität suchen \&lt;Name oder ID>&quot; |
| **Experimentieren und Optimieren, Zielgruppenanalyse, Content Performance Intelligence** | Bericht über die Aktivitätsleistung | Berichte zu Leistung und Aufträgen für alle Aktivitätstypen (einschließlich Recommendations): Konversionssteigerung, Umsatz und Bestellungen. | `target-analyze` | Adobe Target | „Wie entwickelt sich die Aktivität \&lt;name/id>?“<br>„Konversionssteigerung und -umsatz anzeigen für \&lt;activity>&quot;<br>„Welche Aktivitäten haben im letzten Monat die meisten Bestellungen verursacht?“ |
| **Experimentieren und Optimieren, Zielgruppen-Management** | Erstellen von Aktivitäten, Angeboten und Audiences | Erstellen und konfigurieren Sie Aktivitäten, Angebote (HTML/JSON/Redirect), Zielgruppen und Antwort-Token. Die zentrale Authoring-Fähigkeit. | `target-design` | Adobe Target | „Erstellen einer A/B-Aktivität mit Targeting \&lt;audience>&quot;<br>„Erstellen eines JSON-Angebots für \&lt;Anwendungsfall>&quot;<br>„Hinzufügen eines Antwort-Tokens für \&lt;attribute>&quot; |
| **Experimentieren und Optimieren, Inhaltserstellung** | Aktivitäten des Typs Visuelles Erstellen (WYSIWYG) | Authoring in Visual Experience Composer: Erstellen und Bearbeiten von visuellen A/B- und XT-Aktivitäten für eine Live Page-URL mithilfe von Änderungen an der CSS-Auswahl. | `target-vec` | Adobe Target | „Erstellen eines visuellen A/B-Tests auf \&lt;Seiten-URL>&quot;<br>„Ändern Sie die Hero-Überschrift auf \&lt;Seiten-URL> in \&lt;Text>&quot;<br>„Einrichten einer XT-Aktivität mit visuellen Bearbeitungen auf \&lt;Seiten-URL>&quot; |
| **Experimentieren und Optimieren** | Empfehlungen durchsuchen und überprüfen | Schreibgeschütztes Durchsuchen und Überprüfen von Kriterien, Sammlungen, Designs, Promotions, Ausschlüssen, Katalogen und Feeds; umfasst Bereinigungsratschläge und Katalogattribut-Intelligenz. | `target-recs` | Adobe Target | „Anzeigen meiner Recommendations-Kriterien und -Sammlungen“<br>„Überprüfen des Designs für \&lt;recs activity>&quot;<br>„Überprüfen meiner Katalog-Feeds und -Ausschlüsse“ |
| **Experimentieren und Optimieren** | Fehlerbehebung bei Recommendations | Schreibgeschützte Fehlerbehebung für Recs-Probleme wie „Ergebnisse nicht bereit“, leere Ergebnisse und fehlgeschlagene Recs. | `target-recs-diagnose` | Adobe Target | „Warum sind meine Empfehlungsergebnisse nicht bereit?“<br>„Meine Recs werden leer zurückgegeben, was ist los?“<br>„Diagnose, warum \&lt;recs activity> fehlschlägt“ |
| **Experimentieren und Optimieren** | Empfehlungen erstellen und automatisieren | Recs-Authoring: Erstellen, Aktualisieren und Löschen von Kriterien, Sammlungen, Designs, Ausschlüssen, Promotions und Feeds; Erstellen von Recs-Aktivitäten sowie Massen-/Automatisierungsfunktionen für viele Aktivitäten. | `target-recs-design` | Adobe Target | „Erstellen eines &#39;kürzlich angezeigten&#39; Kriteriums“<br>„Erstellen einer Recommendations -Aktivität mit \&lt;criteria>&quot;<br>„Massenaktualisierung des Designs für alle meine Recs-Aktivitäten“ |
| **Experimentieren und Optimieren** | Experimente durchsuchen und nachschlagen | Allgemeines Durchsuchen und Suchen in allen Experimenten: Auflisten, Anzeigen und Abrufen von Ergebnissen und Einblicken. | `experiment-explorer` | Experimentation Accelerator | „Show me my experiments“<br>„List active experiments“<br>„Show results for \&lt;experiment>&quot;<br>„What insights does \&lt;experiment> have?“ |
| **Experimentieren und Optimieren, Zielgruppenanalyse, Content Performance Intelligence** | Analyse und Entscheidung über Experimente | Geführte Synthese und Entscheidungsunterstützung für alle Experimente: Konsistenzprüfungen, Schiffsentscheidungen und Zusammenfassungen für Führungskräfte. | `experiment-analysis` | Experimentation Accelerator | „Wie laufen meine Experimente?“<br>„Sollte ich ausliefern \&lt;experiment>?“<br>„Ist mein Experiment gesund?“<br>„Schreiben Sie eine Zusammenfassung unserer Experimente“ |
| **Experimentieren und Optimieren** | Entwerfen und Planen von Experimenten | Zukunftsweisendes Design und Planung von Experimenten: Was als Nächstes getestet werden soll, wie ein Test entworfen wird und wie eine Roadmap erstellt wird. | `experiment-strategist` | Experimentation Accelerator | „Was soll ich als Nächstes testen?“<br>„Helfen Sie mir beim Entwerfen eines Experiments für \&lt;goal>&quot;<br>„Mein Experiment ist fehlgeschlagen, was kommt als Nächstes?“<br>„Erstellen einer Test-Roadmap“ |
| **Experimentieren und Optimieren; Customer &amp; Account Journey Intelligence** | Wissen suchen und Daten aufnehmen | Abrufen und Suchen von Experimentkontextinformationen oder Aufnehmen externer CSV-Daten zur Analyse. | `experiment-knowledge-base` | Experimentation Accelerator | „Was wissen wir über das Experiment \&lt;name>?“<br>„Haben wir diese Hypothese bereits getestet?“<br>„Laden Sie eine CSV-Datei hoch und analysieren Sie diese Datei“ |
