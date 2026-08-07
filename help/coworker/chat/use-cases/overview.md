---
description: Durchsuchen Sie die Anwendungsfälle und Beispielaufforderungen des Coworker Chat, sortiert nach Bereichen wie Dateneinblicke, Zielgruppen, Journey und Plattformvorgänge.
title: Anwendungsfälle
source-git-commit: 5a04f8fea57dcf6e50ca0040aaad904158c6edf7
workflow-type: tm+mt
source-wordcount: '1143'
ht-degree: 4%

---

# Anwendungsszenarien {#use-cases}

Im Folgenden finden Sie Anwendungsfälle und Beispielaufforderungen, die Anwender im Adobe CX Enterprise Coworker Chat verwenden, sortiert nach Arbeitsbereich. Jede Eingabeaufforderung wird so erstellt, dass sie kopiert, mit Ihren eigenen Daten und Kontexten angepasst und durch Konversation verfeinert wird.

## Dateneinblicke

| Anwendungsfall | Beschreibung | Kenntnisse | Anwendung | Eingabeaufforderungen |
| --- | --- | --- | --- | --- |
| Abrufen von CJA-Berichten und -Metriken | Abfragen von CJA in Echtzeit, um Metriken, Dimensionen, Segmente und Datenansichten abzurufen | `cja` | Customer Journey Analytics (CJA) | „Anzeigen von Seitenansichten für die letzten 30 Tage“ ・ „Auflisten der wichtigsten Segmente in der Stammdatenansicht“ |
| Vergleichsanalyse | Vergleichen von Metriken über Kanäle, Zeiträume oder Segmente hinweg nebeneinander | `cja` | Customer Journey Analytics (CJA) | „Umsatz nach Kanal und Monat vergleichen“ ・ „Wie sieht die Konversion von Mobilgeräten und Desktops in diesem Quartal aus?“ |
| Funnel-Analyse | Mehrstufige Konversionstrichter mit Abbruch in jeder Phase | `cja` | Customer Journey Analytics (CJA) | „Führen Sie mich durch den Checkout funnel&quot; ・ „Konversions-funnel von PDP zum Kauf anzeigen“ |
| Prognose | Zukünftige Metrikwerte des Projekts basierend auf historischen CJA-Daten | `cja` | Customer Journey Analytics (CJA) | „Prognosesitzungen für die nächsten 30 Tage“ ・ „Sind wir auf dem richtigen Weg, unser Umsatzziel zu erreichen?“ |
| Ursachenanalyse | Finden Sie heraus, warum sich eine Metrik geändert hat: Diagnostizieren von Abfällen, Spitzen und Anomalien | `cja-root-cause-analysis` | Customer Journey Analytics (CJA) | „Warum sind die Konversionen letzte Woche zurückgegangen?“ ・ „Was verursachte die Umsatzspitze am 15. Januar?“ |
| Zusammenfassung für Führungskräfte und KPI-Zusammenfassung | Erstellung von einsatzbereiten Leistungszusammenfassungen für Stakeholder, präskriptiven Empfehlungen und Folienübersichten | `cja-executive-summary` | Customer Journey Analytics (CJA) | „Ich möchte eine Zusammenfassung des letzten Monats erhalten“ ・ „Erstellen Sie einen Slide-Deck-Entwurf aus den Daten dieses Quartals“ |
| AA ↔ CJA-Datenvalidierung | Vergleichen, Überprüfen und Abstimmung von Daten zwischen Adobe Analytics und Customer Journey Analytics | `aa-cja-validation` | ADOBE ANALYTICS + CJA | „Meine AA Report Suite mit meiner CJA-Datenansicht vergleichen“ ・ „Seitenansichten zwischen AA und CJA validieren“ |
| Operative Zeitreihen- und Kausalanalyse | Abfragen und Analysieren historischer Zeitreihendaten für Zielgruppen, Datensätze und Journey mit kausaler Attribution | `operational-stats-causal-analysis` | Alle infrage kommenden Anträge | „Trends bei der Zielgruppengröße in den letzten 90 Tagen anzeigen“ ・ „Warum hat die Anzahl meiner Datensatzzeilen am 3. März angezogen?“ |
| Erstellen benutzerdefinierter CJA-Kenntnisse | Verwandeln Sie analytische Muster in wiederverwendbare, wiederholbare Fähigkeiten, die sitzungsübergreifend bestehen bleiben | `cja-skill-creator` | Customer Journey Analytics (CJA) | „Diese wöchentliche Umsatzanalyse in wiederverwendbare Kenntnisse umwandeln“ ・ „Als Kenntnisse für monatliches funnel-Reporting speichern“ |

## Zielgruppen

| Anwendungsfall | Beschreibung | Kenntnisse | Anwendung | Eingabeaufforderungen |
| --- | --- | --- | --- | --- |
| Zielgruppen aus natürlicher Sprache erstellen | Orchestrieren der schrittweisen Zielgruppenerstellung mit Benutzergenehmigung in jeder Phase | `audience-creation-flow` | Real-Time CDP (RTCDP) | „Erstellen Sie eine Audience von Benutzern, die in den letzten 30 Tagen gekauft haben“ ・ „Erstellen Sie ein Segment für hochwertige Mitglieder des Treueprogramms in Kalifornien“ |
| Erstellen von PQL-Definitionen | Zusammenstellen von Zielgruppendefinitionen aus XDM-Eigenschaften, Verhaltensereignissen oder vorhandenen Zielgruppen; Unterstützung von Aggregation und Zeitfenstern | `segment-definition-assembly` | Real-Time CDP (RTCDP) | „Erstellen Sie eine PQL für Personen, die mehr als 3 Produkte angesehen, aber keinen Kauf getätigt haben“ ・ „Hinzufügen eines 7-Tage-Zeitfensters zu meiner Veranstaltungsbedingung“ |
| Zielgruppen suchen und finden | Zielgruppen nach ID, Name und semantischer Suche suchen, Duplikate erkennen und Überschneidungen analysieren | `audience-search` | Real-Time CDP (RTCDP) | „Alle Loyalitäts-Zielgruppen suchen“ ・ „Gibt es ein Duplikat meines Segments „Holiday Shoppers“?“ |
| Zielgruppengröße schätzen | Schätzen der Profilreichweite für einen PQL-Ausdruck mithilfe der Adobe Experience Platform-Vorschau-API mit Abfrage | `audience-size-estimate` | Real-Time CDP (RTCDP) | „Wie groß ist diese Zielgruppe?“ ・ „Geschätzte Reichweite für diesen PQL-Ausdruck“ |
| Audience-Größe - Wasserfall | Unterprädikate für eine PQL erstellen und zeigen, wie jede Bedingung zur endgültigen Zielgruppengröße beiträgt | `audience-size-waterfall` | Real-Time CDP (RTCDP) | „Show me the waterfall for this PQL&quot; ・ „Aufschlüsselung, wie die einzelnen Bedingungen die Zielgruppe reduzieren“ |
| XDM-Felder für das Targeting entdecken | Suchen Sie Felder nach Name, Beschreibung oder Datenwert; sehen Sie, wo sie sich befinden und wo sie bereits verwendet werden | `field-discovery` | Real-Time CDP (RTCDP) | „Welche Felder kann ich verwenden, um Kundinnen und Kunden von Treueprogrammen anzusprechen?“ ・ „Suchen von Feldern im Zusammenhang mit dem Kaufverlauf“ |
| Veröffentlichen/Speichern von Zielgruppen | Beibehalten von Zielgruppendefinitionen im Segmentierungs-Service von Experience Platform mit Benennungskonventionen und Kompatibilitätsprüfungen | `audience-publish` | Real-Time CDP (RTCDP) | „Als Entwurf speichern“ ・ „Die Zielgruppe mit dem Namen „Frühlingsverkaufskäufer“ veröffentlichen“ |

## Journeys

| Anwendungsfall | Beschreibung | Kenntnisse | Anwendung | Eingabeaufforderungen |
| --- | --- | --- | --- | --- |
| Erstellen von Journey aus natürlicher Sprache | Orchestrieren der Journey-Erstellung in AJO über eine Textaufforderung oder ein hochgeladenes Bild/Flussdiagramm | `journey-create` | Adobe Journey Optimizer (AJO) | „Erstellen Sie eine Begrüßungs-Journey, die nach der Anmeldung eine E-Mail sendet, 3 Tage wartet und dann eine Folgenachricht sendet“ ・ „Erstellen Sie eine Journey aus diesem hochgeladenen Flussdiagrammbild.“ |
| Journey-Konflikte analysieren | Erkennung von Zielgruppenüberschneidungen, Terminkollisionen und Deduplizierungsproblemen zwischen aktiven Journeys | `journey-analyze-conflict` | Adobe Journey Optimizer (AJO) | „Steht mein Warenkorbabbruch-Journey in Konflikt mit anderen Journey?“ ・ „Prüfen Sie, ob sich die Zielgruppen meiner aktiven Journey überschneiden.“ |
| Analysieren von Journey-Fallout | Identifizieren Sie, wo und warum Kunden während eines Journey abbrechen, und erkennen Sie Verhaltensmuster, die zu einer Abmeldung führen | `journey-analyze-fallout` | Adobe Journey Optimizer (AJO) | „Wo kommen die Leute auf meiner Re-Engagement-Journey vorbei?“ ・ „Welche Knoten in Journey X haben den höchsten Fallout?“ |
| Analysieren von Fehlern bei benutzerdefinierten Aktionen | Ermitteln Sie, wann benutzerdefinierte Aktionen fehlschlagen oder Fehlerquoten innerhalb eines Journey in die Höhe schießen, und diagnostizieren Sie die Grundursachen, bevor Fehler in umfassendere Unterbrechungen übergehen. | `journey-analyze-custom-action` | Adobe Journey Optimizer (AJO) | „Warum schlagen benutzerdefinierte Aktionen in meiner Treue-Anmelde-Journey fehl?“ ・ „Fehlerrate für benutzerdefinierte Aktion „ExternalPush“ auf meiner Begrüßungs-Journey anzeigen.“ |

## Grundlegende Elemente

| Anwendungsfall | Beschreibung | Kenntnisse | Anwendung | Eingabeaufforderungen |
| --- | --- | --- | --- | --- |
| Produktkenntnisse und Dokumentation | Antworten auf Fragen zu Anleitungen, Konzepten, Fehlerbehebung und Best Practices aus offiziellen Adobe-Dokumenten | `product-knowledge` | Alle infrage kommenden Anträge | „Wie richte ich ein Streaming-Ziel ein?“ ・ „Was ist der Unterschied zwischen Batch- und Streaming-Segmentierung?“ |
| Abfragen von Experience Platform-/Journey Optimizer-Entitäten | Dient als primärer Einstiegspunkt für Fragen zu Ihren Platform-Entitäten; Route zu KG, Felderkennung oder APIs nach Bedarf | `operational-insights` | Alle infrage kommenden Anträge | „Wie viele Datensätze habe ich?“ ・ „Alle aktiven Journey anzeigen“ ・ „Meine Ziele auflisten“ |
| Abfragen von Wissensdiagrammen | Aggregierte Zählungen, entitätsübergreifende Joins, Beziehungssuchen und Metadatenexploration über einzelne SQL-Abfragen | `knowledge-graph` | Alle infrage kommenden Anträge | „Welche Zielgruppen verwenden diesen Datensatz?“ ・ „Anzeigen von Beziehungen zwischen Schemata und Datensätzen“ |
| API-Vorgänge für Experience Platform/Journey Optimizer/Customer Journey Analytics | Bereitstellen eines direkten API-Gateways für Mutationen, Echtzeit-Statusprüfungen und Entitätstypen, die nicht im Wissensdiagramm enthalten sind | `cxo-api` | Alle infrage kommenden Anträge | „Datensatz X löschen“ ・ „Status meines Batch-Erfassungsvorgangs überprüfen“ |
| Auflösung und Verknüpfung von Entitäten | Verwenden Sie die semantische und lexikalische Suche, um Entitätsbezeichnungen in tatsächliche Experience Platform-Entitäten aufzulösen und XDM-Felder zu erkennen | `entity-linking` | Adobe Experience Platform | „Auflösen von „Holiday Shoppers“ in eine tatsächliche Zielgruppe“ ・ „Felder zum Kaufverlauf finden“ |
| Benutzerdefinierte Fähigkeiten verwalten | Speichern, Ändern oder Löschen von benutzereigenen wiederverwendbaren Fähigkeiten, die sitzungsübergreifend bestehen bleiben | `manage-skill` | Alle infrage kommenden Anträge | „Diesen Workflow als Qualifikation speichern“ ・ „Meine wöchentlichen Berichtsqualifikationen löschen“ ・ „Diese Qualifikation wiederverwendbar machen“ |

## Sandbox-Werkzeuge

| Anwendungsfall | Beschreibung | Kenntnisse | Anwendung | Eingabeaufforderungen |
| --- | --- | --- | --- | --- |
| Verschieben von Metadatenobjekten über Sandboxes hinweg | Nahtlose Migration von Schemas, Zielgruppen und anderen Objektkonfigurationen über Sandboxes hinweg, wobei Abhängigkeiten automatisch aufgelöst werden | `sandbox-tooling-workflow` | Adobe Experience Platform | „Schema-Luma-Platin-Mitglieder des Treueprogramms aus der aktuellen Sandbox in die Produktions-Sandbox verschieben“ ・ „Die Zielgruppe der US-amerikanischen Mitglieder des Treueprogramms für Gold-Mitglieder zur Staging-Umgebung bewerben“ |
