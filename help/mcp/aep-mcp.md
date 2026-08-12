---
title: Experience Platform-Tools in CX Coworker Gateway
description: Erfahren Sie, welche Adobe Experience Platform-Tools über CX Coworker Gateway verfügbar sind.
source-git-commit: 4bc180a76f3c1095a4d25ed7e07d804e4d5ff1a9
workflow-type: tm+mt
source-wordcount: '1371'
ht-degree: 8%

---


# Adobe Experience Platform-Tools in Adobe CX Coworker Gateway {#aep-mcp}

Sie können die Adobe Experience Platform-Produkt-Tools verwenden, um Schemata, Datensätze, Data Governance-Konfigurationen, Abfrage-Service-Ressourcen und Audit-Ereignisse von einem MCP-kompatiblen Client aus zu untersuchen. Diese Tools sind über das [Adobe CX Coworker Gateway](overview.md) verfügbar, wenn Ihr Unternehmen aktiviert ist und Ihr Benutzerkonto über die erforderlichen Experience Platform-Berechtigungen verfügt.

>[!AVAILABILITY]
>
>Das Experience Platform-Produkt-Tool befindet sich in Beta. Der Zugriff erfolgt nur auf Einladung und erfordert die Aktivierung durch die Adobe-Organisation. Siehe [Zugriff auf CX Coworker Gateway-Tools](access.md).

## Zusammenfassung

| Tool | Beschreibung | Ressource | Funktionen | Status |
| --- | --- | --- | --- | --- |
| `search_allowed_ip_ranges` | Abrufen von IP-Zugriffsbeschränkungen für den Abfrage-Service | Data Distiller-Authentifizierung ・ IP-Bereiche | Liste | Aktiv |
| `search_audit` | Auflisten von Benutzeraktivitäts-Audit-Ereignissen in Experience Platform | Audit-Abfrage ・ Audit-Ereignisse | Liste, Filtern nach Asset-Typ, Aktion, Status, Zeitbereich | Aktiv |
| `search_datasets` | Abfragen von Datensatz- und Batch-Aufnahme-Metadaten | Katalog-API ・ Datensätze, Batches | list, get, filter, list, last, list files | Aktiv |
| `search_class_relations` | Experience Platform Business-Class-Beziehungen durchsuchen | Klassenbeziehungen ・ statischer YAML-Index | Suche nach Token, Multi-Term, teilweise Übereinstimmung | Aktiv |
| `search_data_access` | Auflisten von Dateien aus fehlgeschlagenen Aufnahme-Batches | Datenzugriffs-API ・ Fehlgeschlagene Batches | Auflisten fehlgeschlagener Dateien | Aktiv |
| `search_data_lake` | Überprüfen von Datensatzmetadaten und des Batch-Status | Data Lake API ・ Datensätze, Batches | Abrufen, Abrufen der Größe, Auflisten fehlgeschlagener Batches | Aktiv |
| `search_dule` | Data Governance-Kennzeichnungen, -Richtlinien, -Aktionen abfragen | Data Governance ・ Kennzeichnungen, Richtlinien, Marketing_Aktionen | list, get, list enabled, evaluieren | Aktiv |
| `search_query_service` | SQL-Abfragen, Vorlagen, Zeitpläne, Warnhinweise abfragen | Abfrage-Service ・ Abfragen, Vorlagen, Zeitpläne, Warnhinweise | Auflisten, Abrufen, Filtern, Abrufen von Verbindungsparametern | Aktiv |
| `search_schema_registry` | XDM-Schemata, Feldergruppen, Klassen, Typen von Abfragen | Schemaregistrierung ・ Schemata, Feldergruppen, Klassen, data_types, Deskriptoren | Auflisten, Abrufen, Filtern nach Container | Aktiv |

## Tool-Referenz

### search_allowed_ip_range

**Resource:** Data Distiller Auth ・ IP-Bereiche
**Status:** aktiv

Rufen Sie alle konfigurierten IP-Zugriffsbeschränkungen für den Abfrage-Service in der aktuellen Sandbox ab. Gibt die Organisations-ID und die Liste der zulässigen IP-Bereiche zurück. Nur für Kunden mit dem Add-on Data Distiller verfügbar.

**Funktionen:** Liste der zulässigen IP-Bereiche für den Abfrage-Service

Keine Parameter.

### search_audit

**Ressource:** Audit Query ・ Audit-Ereignisse
**Status:** aktiv

Auflisten von mit Zeitstempel versehenen Aufzeichnungen der Benutzeraktivitäten in allen Experience Platform-Services. Gibt den Aktionstyp, die Benutzer-E-Mail-Adresse, Asset-Informationen und den Ereignisstatus zurück. Verwenden Sie `asset_type` und `action`, um die Ergebnisse einzugrenzen. Standardmäßig werden die letzten 7 Tage verwendet, wenn kein Zeitbereich angegeben ist. Auf die letzten 1.000 Datensätze und Ereignisse der letzten 90 Tage beschränkt.

**Funktionen:** Audit-Ereignisse auflisten, nach Asset-Typ, Aktion, Status, Zeitbereich filtern, paginieren

**Parameter:**

| Parameter | Erforderlich | Beschreibung |
| --- | --- | --- |
| `action` | Nein | Filtern nach Aktionstyp. Allgemeine Werte (durch Kommas getrennt für ODER): `Create`, `Delete`, `Update`, `Enable`, `Disable` |
| `asset_type` | Nein | Filtern nach Asset-Typ. Muss eines der folgenden sein: `Dataset`, `Schema`, `Segment`, `Destination`, `Source Data Flow`, `Merge Policy`, `Identity Namespace`, `Identity Graph`, `Sandbox`, `Role`, `Query`, `Scheduled Query`, `Computed Attribute`, `Class`, `Field Group`, `Data Types`, `Account`, `Product Profile`, `Work Order`, `Query Template`, `Audit Logs`, `Access Control Policy`,,,,, `Datastream`, |
| `status` | Nein | Filtern nach Ereignisstatus. Werte: `Success`, `Failure`, `Allow`, `Deny`. Kommagetrennt für ODER |
| `start_time` | Nein | Frühester Zeitstempel. ISO 8601 UTC mit ms, z. B. `2024-01-15T00:00:00.000Z` |
| `end_time` | Nein | Neuester Zeitstempel. ISO 8601 UTC mit ms |
| `property_filter` | Nein | Roher Filterausdruck, z. B. `action==create`. Bevorzugen Sie die oben genannten dedizierten Parameter |
| `orderby` | Nein | Sortierreihenfolge: `timestamp` (asc) oder `-timestamp` (desc) |
| `limit` | Nein | Maximale Anzahl an Ergebnissen (3-1000, Standard 50) |
| `start` | Nein | Paginierungsversatz. Inkrementieren Sie für jede Seite um den Grenzwert. |
| `query_id` | Nein | Abfrage-ID aus einer vorherigen Antwort, um dieselbe Abfrage zu wiederholen |

### search_datasets

**Resource:** Catalog API ・ Datensätze, Batches
**Status:** aktiv

Einheitliches Dispatch-Tool für den Experience Platform Catalog Service. Abfragen von Datensatzmetadaten (Schemareferenz, Tags, Erstellungsinformationen) oder Batch-Aufnahme-Datensätzen (Status, Metriken, Dateilisten). Verwenden Sie `dataset/list`, um Datensätze zu finden, den Aufnahmezustand zu `batch/list` und bestimmte Batch-Inhalte zu `batch/list_files` oder zu `batch/get_meta_files`. Alle Vorgänge sind schreibgeschützt.

**Funktionen: Datensätze**, Datensatz abrufen, Batches auflisten, Batch abrufen, Letzten Batch pro Datensatz auflisten, Batch-Dateien auflisten, Batch-Metadaten abrufen (Zeilenfehler, Eingabedateien)

**Parameter:**

| Parameter | Erforderlich | Beschreibung |
| --- | --- | --- |
| `entity_type` | Ja | `dataset` oder `batch` |
| `operation` | Ja | `list`, `get`, `list_last`, `list_files`, `get_meta_files`. Gültige Kombinationsfelder: Datensatz → Liste, GET; Batch → alle fünf |
| `resource_id` | Nein | Datensatz- oder Batch-ID. Erforderlich für `dataset/get`, `batch/get`, `batch/list_files`, `batch/get_meta_files` |
| `query_params.limit` | Nein | Max. Ergebnisse pro Seite (max. 100). Gilt für alle Listenvorgänge |
| `query_params.start` | Nein | Paginierungsversatz. Gilt für alle Listenvorgänge |
| `query_params.order_by` | Nein | Sortierrichtung, z. B. `asc:created,updated`. Gilt für alle Listenvorgänge |
| `query_params.properties` | Nein | Zulassungsliste der kommagetrennten Eigenschaft. Gilt für Datensatz/Liste, Datensatz/GET, Batch/Liste, batch/list_last |
| `query_params.name` | Nein | Datensätze nach Namen filtern (nur Datensatz/Liste) |
| `query_params.tags` | Nein | Datensätze nach Tags filtern, z. B. `unifiedProfile:enabled:true` (nur Datensatz/Liste) |
| `query_params.property_filter` | Nein | Regex-Filter für Antwortobjekte (Datensatz/Liste und Batch/Liste) |
| `query_params.status` | Nein | Stapel nach Status filtern: `success`, `failed`, `loading`, `active` (nur Stapel/Liste) |
| `query_params.dataset_id` | Nein | Batches auf einen bestimmten Datensatz beschränken (batch/list und batch/list_last) |
| `query_params.created_after` | Nein | Nach Unix-Zeitstempel erstellte Batches in ms filtern (nur Batch/Liste) |
| `query_params.created_before` | Nein | Batches filtern, die vor dem Unix-Zeitstempel in ms erstellt wurden (nur Batch/Liste) |
| `query_params.last_batch_status` | Nein | Nach letztem Batch-Status filtern (nur batch/list_last) |
| `query_params.aggregate` | Nein | Aggregierte Metriken auf Stammebene zurückgeben (nur Batch/GET) |
| `query_params.path` | Nein | Herunterzuladende Meta-Datei: `row_errors`, `input_files`, `row_errors_sample.json` (nur batch/get_meta_files) |

### search_class_relations

**Resource:**-Klassenbeziehungen ・ statischer YAML-Index
**Status:** aktiv

Suchen Sie mithilfe des statischen `class_relations_v1.yaml` nach Experience Platform-Geschäftsklassenbeziehungen nach Namen. Es werden keine Experience Platform-API-Aufrufe durchgeführt. Akzeptiert einen einzelnen Begriff oder kommagetrennte Begriffe. Jeder Begriff wird mit Klassennamen abgeglichen, die einen teilweisen Token-Abgleich verwenden. Gibt übereinstimmende Klassen mit Vorwärtsbeziehungen (worauf jede Klasse verweist) und umgekehrte Beziehungen (welche Klassen darauf zurückverweisen) zurück. Verwenden Sie diese Option, um Entitätsbeziehungen vor dem Erstellen von Abfragen, Datenflüssen oder Schemakompositionen zu verstehen.

**Funktionen:** Suche nach Token, Multi-Term-kommagetrennte Suche, partielle Token-Übereinstimmung, bidirektionale Synonymerweiterung

**Parameter:**

| Parameter | Erforderlich | Beschreibung |
| --- | --- | --- |
| `query` | Ja | Name der Business-Klasse oder Objekttyp, nach dem gesucht werden soll. Unterstützt partielle Token-Übereinstimmungen (`dat` stimmt mit `dataset`, `data_type` usw. überein). Mehrere kommagetrennte Begriffe übergeben, um nach mehreren Klassen gleichzeitig zu suchen (z. B. `dataset, schema`) |
| `n` | Nein | Maximale Anzahl an übereinstimmenden Ergebnissen, die zurückgegeben werden sollen (Standard: 5, min 1) |

### search_data_access

**Resource:** Data Access API ・ Fehlgeschlagene Batches
**Status:** aktiv

Zugreifen auf Dateien aus fehlgeschlagenen Experience Platform-Datenerfassungs-Batches. Verwenden Sie `failed_batch/list_failed`, um die Dateien, die zu einem fehlgeschlagenen Batch gehören, zur Fehlerdiagnose aufzulisten. Erfordert eine Batch-ID für alle Vorgänge. Hinweis: `file/get` und `dataset/preview` sind deaktiviert, da sie tatsächliche Datensatzdaten verfügbar machen. Alle Vorgänge sind schreibgeschützt.

**Funktionen:** Dateien aus einem fehlgeschlagenen Aufnahme-Batch auf

**Parameter:**

| Parameter | Erforderlich | Beschreibung |
| --- | --- | --- |
| `entity_type` | Ja | `failed_batch` - Listet Dateien aus einem fehlgeschlagenen Aufnahme-Batch auf |
| `operation` | Ja | `list_failed` - der einzige unterstützte Vorgang |
| `resource_id` | Ja | Batch-ID des fehlgeschlagenen Batches |
| `query_params.start` | Nein | Paging-Startindex, z. B. `1` |
| `query_params.limit` | Nein | Anzahl der Ergebnisse pro Seite, z. B. `10` |
| `query_params.path` | Nein | Vollständiger Dateinamenfilter, z. B. `profiles.csv` |


### search_data_lake

**Ressource:** Data Lake API ・ Datensätze, Batches
**Status:** aktiv

Überprüfen Sie Datensatz- und Batch-Metadaten aus der Data Lake-Ebene. Verwenden Sie `get` für vollständige Metadaten, `get_size` für Metriken zur Speicher- und Aufnahmegröße und `list_failed`, um Aufnahmefehler innerhalb eines Zeitfensters zu überwachen. Die Standardeinstellung sind die letzten 7 Tage, wenn kein Zeitbereich für `list_failed` angegeben wird. Alle Vorgänge sind schreibgeschützt und erfordern eine Ressourcen-ID.

**Funktionen:** von Datensatz-/Batch-Metadaten, Abrufen von Metriken zur Speichergröße, Auflisten fehlgeschlagener Batches innerhalb eines Zeitfensters

**Parameter:**

| Parameter | Erforderlich | Beschreibung |
| --- | --- | --- |
| `entity_type` | Ja | `dataset` oder `batch` |
| `operation` | Ja | `get`, `get_size`, `list_failed`. `list_failed` unterstützt nur `batch` Entitätstyp |
| `resource_id` | Ja | Datensatz-ID oder Batch-ID. Für `list_failed`: die Datensatz-ID, auf die Fehler angewendet werden sollen |
| `query_params.created_after` | Nein | Beginn des Zeitfensters. Unix-Zeitstempel in ms |
| `query_params.created_before` | Nein | Ende des Zeitfensters Unix-Zeitstempel in ms |
| `query_params.limit` | Nein | Max. Ergebnisse pro Seite (max. 100) |
| `query_params.order_by` | Nein | Sortierrichtung, z. B. `desc:created` |

### search_dule

**Ressource:** Data Governance ・ Kennzeichnungen, Richtlinien, Marketing_Aktionen
**Status:** aktiv

Fragen Sie die Policy Service-API nach Datennutzungskennzeichnungen, Richtlinien und Marketing-Aktionen ab. Verwenden Sie `marketing_action/evaluate`, um zu testen, ob eine Marketing-Aktion für Daten mit bestimmten Kennzeichnungen gegen Governance-Richtlinien verstößt. Alle Vorgänge sind schreibgeschützt.

**Funktionen:** Auflisten/Abrufen von Datennutzungskennzeichnungen, Auflisten/Abrufen von Richtlinien, Auflisten von aktivierten Richtlinien, Auflisten/Abrufen von Marketing-Aktionen, Auswerten von Marketing-Aktionen anhand von Kennzeichnungen

**Parameter:**

| Parameter | Erforderlich | Beschreibung |
| --- | --- | --- |
| `entity_type` | Ja | `label`, `policy` oder `marketing_action` |
| `operation` | Ja | `list`, `get`, `list_enabled` (nur Richtlinie), `evaluate` (nur Marketing-Aktion). `list_enabled` erfordert keinen Umfang |
| `scope` | Nein | `core` (Adobe-definiert) oder `custom` (org-definiert) Erforderlich für `list`, `get`, `evaluate`; wird nicht für `list_enabled` verwendet |
| `resource_id` | Nein | Name der Kennzeichnung, Richtlinien-ID oder Name der Marketing-Aktion. Erforderlich für `get` und `evaluate` |
| `query_params.dule_labels` | Nein | Kommagetrennte Beschriftungen (z. B. `C1,C3`). Erforderlich für `marketing_action/evaluate`; optionaler Filter für `policy/list` |
| `query_params.limit` | Nein | Max. Ergebnisse |
| `query_params.start` | Nein | Paginierungscursor aus dem `_page.next` einer früheren Antwort |
| `query_params.orderby` | Nein | Kommagetrennte Sortierfelder |
| `query_params.property_filter` | Nein | Filterausdruck, z. B. `name==C1` |
| `query_params.marketing_action` | Nein | Richtlinienliste auf Richtlinien beschränken, die auf diese Marketing-Aktion verweisen (nur Richtlinie/Liste) |
| `query_params.include_draft` | Nein | Richtlinienentwürfe in `marketing_action/evaluate` einschließen (Standard: nur aktivierte Richtlinien) |

### search_query_service

**Ressource:** Query Service ・ Abfragen, Vorlagen, Zeitpläne, Zeitplanausführungen, Verbindungen, Warnhinweis-Abonnements
**Status:** aktiv

Einheitliches Tool für Abfrage-Service-Ressourcen. Auflisten und Abrufen von Ad-hoc-Abfragen, gespeicherten SQL-Vorlagen, geplanten Abfragen und ihren Ausführungen, interaktiven Verbindungsparametern (für PSQL/JDBC-Clients) und Warnhinweis-Abonnements. Für Abfragelisten wird standardmäßig `isService==false,isParentLevel==true`, um internen Traffic herauszufiltern. Alle Vorgänge sind schreibgeschützt.

**Funktionen:** Listen-/Abfragen abrufen, Listen-/GET-Vorlagen, Listen-/GET-Zeitpläne, Listen-/GET-Zeitplanausführungen, Verbindungsparameter abrufen, Abonnements für Warnhinweise auflisten

**Parameter:**

| Parameter | Erforderlich | Beschreibung |
| --- | --- | --- |
| `entity_type` | Ja | `query`, `query_template`, `schedule`, `schedule_run`, `connection`, `alert_subscription` |
| `operation` | Ja | `list`, `get`, `get_connection_params`, `list_by_u...` |
