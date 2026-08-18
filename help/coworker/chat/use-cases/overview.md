---
description: Durchsuchen Sie die Anwendungsfälle und Beispielaufforderungen des Coworker Chat, sortiert nach Bereichen wie Dateneinblicke, Zielgruppen, Journey und Plattformvorgänge.
title: Anwendungsfälle für den Chat mit Kollegen
feature_v2: id: fdae8433-07cd-42e7-acce-738afe63f6bb
source-git-commit: 9188ccfc1a01288bee775bc82d84c7f252e66615
workflow-type: tm+mt
source-wordcount: 1333
ht-degree: 7%

---

# Anwendungsfälle für den Chat mit Kollegen{#use-cases}

Mit dem Coworker Chat können Sie Ihre [!DNL Experience Platform]-Daten mit natürlicher Sprache abfragen, analysieren und bearbeiten, anstatt mehrere Benutzeroberflächen zu durchsuchen oder Abfragen von Hand zu schreiben. Auf dieser Seite werden die Anwendungsfälle katalogisiert, auf die sich die Fachleute am meisten verlassen, sortiert nach Arbeitsbereich: Dateneinblicke, Zielgruppen, Journey, Grundlegende Elemente und Sandbox-Tools. Jeder Eintrag beinhaltet die Qualifikation, die er aufruft, die Anwendungen, mit denen er arbeitet, und Beispielaufforderungen, die Sie kopieren, an Ihre eigenen Daten anpassen und durch Konversation verfeinern können.

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

## Sandbox-Werkzeuge

| Anwendungsfall | Beschreibung | Skills | Anwendung | Eingabeaufforderungen |
| --- | --- | --- | --- | --- |
| [Objekte über Sandboxes hinweg verschieben](/help/agents/sandbox-tooling.md) | Nahtlose Migration von Schemas, Zielgruppen und anderen Objektkonfigurationen über Sandboxes hinweg, wobei Abhängigkeiten automatisch aufgelöst werden | `sandbox-tooling-workflow` | Adobe Experience Platform | „Schema-Luma-Platin-Mitglieder des Treueprogramms aus der aktuellen Sandbox in die Produktions-Sandbox verschieben“ ・ „Die Zielgruppe der US-amerikanischen Mitglieder des Treueprogramms für Gold-Mitglieder zur Staging-Umgebung bewerben“ |
