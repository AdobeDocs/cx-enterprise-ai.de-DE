---
title: SQL-Datenvorbereitung in Coworker
description: Erfahren Sie, wie Sie SQL-Datenvorbereitung in Coworker verwenden, um SQL-Abfragen zu generieren, zu optimieren, zu beheben und zu planen.
source-git-commit: 8e28bb38bd27c1e57ac7c62f74196d146d8519ca
workflow-type: tm+mt
source-wordcount: '1126'
ht-degree: 3%
---
# SQL-Datenvorbereitung in Coworker

Verwenden Sie die SQL-Datenvorbereitung in Coworker, um gängige [Data Distiller](https://experienceleague.adobe.com/de/docs/experience-platform/query/data-distiller/overview)-Aufgaben mit Eingabeaufforderungen in natürlicher Sprache auszuführen. Sie können SQL-Abfragen generieren, eine vorhandene Abfrage beheben oder optimieren, Ergebnisse in der Vorschau anzeigen und Abfragen für die wiederkehrende Ausführung planen.

>[!AVAILABILITY]
>
>Die SQL-Datenvorbereitung in Coworker ist nur in begrenzter Verfügbarkeit verfügbar.

## Voraussetzungen {#prerequisites}

Bevor Sie die SQL-Datenvorbereitung in Coworker verwenden, stellen Sie Folgendes sicher:

- Eine Berechtigung für Data Distiller.
- Zugriff auf Kollegen.

## Erste Schritte {#get-started}

Öffnen Sie zunächst Coworker und geben Sie eine Anforderung in natürlicher Sprache ein, die die gewünschte SQL-Aufgabe oder das gewünschte Ergebnis beschreibt.

Sie können die Datensätze identifizieren, die Sie in Ihrer Anfrage verwenden möchten. Wenn zum Abschließen der Aufgabe zusätzliche Informationen erforderlich sind, kann ein Mitarbeiter weitere Fragen stellen, bevor er fortfährt.

Nachdem ein Mitarbeiter die SQL generiert oder aktualisiert hat, können Sie die Konversation fortsetzen, um eine Vorschau der Ergebnisse anzuzeigen, die Abfrage zu verfeinern, sie zu speichern oder sie für die wiederkehrende Ausführung zu planen.

Eine Anleitung zur Verwendung der Benutzeroberfläche für Kollegen finden Sie im [Handbuch zur Benutzeroberfläche für Kollegen](https://experienceleague.adobe.com/en/docs/coworker/content/chat/ui-guide).

## Unterstützte Funktionen {#supported-capabilities}

Sie können SQL-Datenvorbereitung für die folgenden Aufgaben verwenden:

| Funktion | Beschreibung |
| --- | --- |
| **SQL-Authoring** | Generieren Sie SQL aus einer Beschreibung des Datenvorgangs, den Sie in natürlicher Sprache ausführen möchten. |
| **SQL-Optimierung** | Analysieren Sie eine vorhandene Data Distiller-Abfrage und optimieren Sie sie für die Leistung, während Sie ihre beabsichtigten Ergebnisse beibehalten. |
| **SQL-Fehlerdiagnose und -korrektur** | Diagnostizieren Sie Fehler in einer vorhandenen SQL-Abfrage, erklären Sie die Grundursache und generieren Sie korrigierte SQL. |
| **Abfrageplanung und Warnhinweise** | Speichern und planen Sie Abfragen für die wiederkehrende Ausführung und konfigurieren Sie unterstützte Abfrage-Warnhinweise. |

## SQL-Datenvorbereitung in einer Konversation verwenden {#work-with-sql-data-preparation}

Sie können SQL-Datenvorbereitungs-Funktionen in derselben Coworker-Konversation kombinieren, anstatt sie als separate Workflows zu behandeln.

Sie können zum Beispiel:

1. Beschreiben Sie das gewünschte Ergebnis und generieren Sie SQL.
2. Vorschau von bis zu fünf Zeilen mit Abfrageergebnissen.
3. Verfeinern Sie die Abfrage oder stellen Sie Fragen zur generierten SQL.
4. Speichern Sie die Abfrage.
5. Planen Sie die Abfrage für die wiederkehrende Ausführung und konfigurieren Sie Warnhinweise.

Mitarbeiter können Folgefragen stellen, wenn zusätzliche Informationen erforderlich sind, z. B. um den entsprechenden Datensatz zu identifizieren oder die Zeitzone für einen Zeitplan zu bestätigen.

Eine Abfragevorschau gibt bis zu fünf Zeilen zurück. Informationen zum Ausführen von Abfragen und zum Arbeiten mit Abfragen direkt in Experience Platform finden Sie im [Handbuch zur Benutzeroberfläche des Abfrage-Editors](https://experienceleague.adobe.com/en/docs/experience-platform/query/ui/user-guide).

![Eine Coworker-Antwort zeigt eine fünfzeilige Vorschau der SQL-Abfrageergebnisse und Optionen, um die Abfrage als Vorlage zu speichern oder für die wiederkehrende Ausführung zu planen.](./assets/sql-data-prep/query-preview.png)

### SQL aus natürlicher Sprache generieren {#generate-sql}

Verwenden Sie das SQL-Authoring, wenn Sie das Ergebnis oder die Transformation kennen, die Sie erreichen möchten, aber möchten, dass ein Mitarbeiter die entsprechende SQL generiert.

Um SQL aus den richtigen Daten zu generieren, kann ein Mitarbeiter die betroffenen Datensätze identifizieren und validieren. Wenn Ihre Anfrage nicht genügend Informationen bereitstellt, um den entsprechenden Datensatz zu identifizieren, kann ein Mitarbeiter vor dem Fortfahren Folgefragen stellen.

Beispiel:

> Hallo! Fassen Sie mithilfe von test_luma_web_events_1000 die Kundeninteraktionen nach Ereignistyp zusammen. Ereignistyp, Gesamtzahl der Ereignisse und Unique Customers anzeigen. Gibt eine Zeile pro Ereignistyp zurück und sortiert die Ergebnisse nach Unique Customers von der höchsten zur niedrigsten.

Ein Mitarbeiter gibt die generierte SQL zurück und kann die Abfrage ausführen, um eine Vorschau der Ergebnisse anzuzeigen.

![Coworker-Antwort, die die generierte SQL-Abfrage für die Zusammenfassung der Kundeninteraktion nach Ereignistyp zeigt, gefolgt von einer Tabellenvorschau der Gesamtzahl der Ereignisse und Unique Customers und einer Analyse der Ergebnisse.](./assets/sql-data-prep/authoring-result.png)

Informationen zum Erstellen und Ausführen von Abfragen direkt in Experience Platform finden Sie im [Handbuch zur Benutzeroberfläche des Abfrage-Editors](https://experienceleague.adobe.com/en/docs/experience-platform/query/ui/user-guide).

### Vorhandene SQL optimieren {#optimize-sql}

Verwenden Sie die SQL-Optimierung, wenn Sie bereits über eine Data Distiller-Abfrage verfügen und deren Leistung verbessern möchten, ohne die beabsichtigten Ergebnisse zu ändern.

Sie können einen Mitarbeiter bitten, die Änderungen zu erläutern, die ursprüngliche und die optimierte SQL zu vergleichen und Validierungs- oder Abfrageplaninformationen anzugeben.

Beispiel:

> Optimieren Sie die folgende Abfrage für die Leistung von Data Distiller, während Sie genau dieselben Ergebnisse beibehalten. Erläutern Sie, was Sie geändert haben und warum die optimierte Abfrage logisch äquivalent ist.
>
> ```sql
> SELECT
>         p.customer_id,
>         p.first_name,
>         p.last_name,
>         p.loyalty_status,
>         COUNT(o.order_id) AS total_orders,
>         SUM(CAST(o.order_total AS DOUBLE)) AS total_revenue
> FROM test_luma_profiles_1000 p
> INNER JOIN test_luma_orders_1000 o
>         ON p.customer_id = o.customer_id
> GROUP BY
>         p.customer_id,
>         p.first_name,
>         p.last_name,
>         p.loyalty_status
> ORDER BY total_revenue DESC;
> ```
>
> Senden Sie mir die vollständige Antwort, insbesondere die ursprüngliche SQL, optimierte SQL, Erklärung der Gleichwertigkeit und alle EXPLAIN-/Validierungsergebnisse.

Wenn die bereitgestellte Abfrage bereits optimiert wurde, kann ein Mitarbeiter feststellen, dass keine Änderung erforderlich ist, und seine Bewertung erläutern.

![Antwort des Mitarbeiters, die eine vorhandene SQL-Abfrage zur Optimierung analysiert und erklärt, dass keine Änderungen erforderlich sind, mit Ergebnissen des Abfrageplans und einer Gleichwertigkeitsbewertung.](./assets/sql-data-prep/optimize-query.png)

Die über die SQL-Authoring-Funktion generierte SQL ist bereits optimiert. Es ist nicht erforderlich, neu generierte SQL zur Optimierung separat einzureichen.

Informationen zur SQL-Syntax und zu unterstützten Befehlen finden Sie [SQL-Referenz zum Abfrage-Service](https://experienceleague.adobe.com/en/docs/experience-platform/query/sql/overview).

### SQL-Fehler diagnostizieren und beheben {#diagnose-sql-errors}

Verwenden Sie die SQL-Fehlerdiagnose, wenn eine vorhandene Abfrage fehlschlägt und Sie Hilfe benötigen, um die Ursache zu identifizieren und die SQL zu korrigieren.

Ein Mitarbeiter analysiert die Abfrage, identifiziert die Fehlerursache, erklärt das Problem und liefert korrigierte SQL-Daten.

Beispiel:

> Hallo! Die folgende Abfrage schlägt fehl. Diagnostizieren Sie den Fehler, erklären Sie die Grundursache und stellen Sie eine korrigierte Abfrage bereit:
>
> ```sql
> SELECT
>         o.order_id,
>         o.product_id,
>         p.product_name,
>         o.order_total
> FROM test_luma_orders_1000 o
> JOIN test_luma_product_catalog_1000 p
>         ON o.productid = p.productid;
> ```
>
> Die korrigierte Abfrage sollte die entsprechenden Produkt-ID-Felder aus beiden Datensätzen verwenden.

Nachdem Sie die Abfrage korrigiert haben, können Sie einen Mitarbeiter bitten, sie auszuführen und die Ergebnisse in der Vorschau anzuzeigen.

![Antwort des Mitarbeiters - Diagnose eines SQL-Abfragefehlers, der durch falsche Produkt-ID-Feldnamen verursacht wurde, und Bereitstellung von korrigiertem SQL-Code, der die product_id-Felder verwendet.](./assets/sql-data-prep/diagnose-error.png)

### Abfragen planen und Warnhinweise konfigurieren {#schedule-queries}

Nachdem Sie eine Abfrage generiert, korrigiert oder in der Vorschau angezeigt haben, können Sie die Konversation fortsetzen, um sie zu speichern und für die wiederkehrende Ausführung zu planen.

Beispiel:

> Planen Sie die Ausführung dieser Abfrage jeden Tag um 6:00 Uhr. Warnhinweis konfigurieren, wenn die Abfrage fehlschlägt.

Wenn die erforderlichen Informationen fehlen oder mehrdeutig sind, stellt der Mitarbeiter vor der Erstellung des Zeitplans weitere Fragen. Beispielsweise können Sie aufgefordert werden, die Zeitzone zu bestätigen, die mit der angeforderten Ausführungszeit verbunden ist.

Nachdem Sie die erforderlichen Zeitplandetails bestätigt haben, gibt der Mitarbeiter eine Zusammenfassung der gespeicherten Abfragevorlage, des Zeitplans, der Zeitzone, des Status und der Fehlermeldung zurück.

![Antwort eines Kollegen, die eine geplante SQL-Abfrage bestätigt, einschließlich der gespeicherten Vorlage, des Zeitplans, der Zeitzone, des Enddatums, des Zeitplanstatus und des Fehlerwarnhinweises.](./assets/sql-data-prep/schedule-query.png)

Ausführliche Informationen zu Abfrageplänen, Wiederholungseinstellungen, Ausgabedatensätzen und Warnhinweisen finden Sie unter [Abfragepläne](https://experienceleague.adobe.com/en/docs/experience-platform/query/ui/query-schedules).

## Nächste Schritte {#next-steps}

Weitere Informationen zu den Funktionen von Data Distiller und Query Service, die von der SQL-Datenvorbereitung verwendet werden, finden Sie in der folgenden Dokumentation:

- [Übersicht über Data Distiller](https://experienceleague.adobe.com/de/docs/experience-platform/query/data-distiller/overview)
- [Handbuch zur Benutzeroberfläche des Abfrage-Editors](https://experienceleague.adobe.com/en/docs/experience-platform/query/ui/user-guide)
- [Abfragepläne](https://experienceleague.adobe.com/en/docs/experience-platform/query/ui/query-schedules)
- [SQL-Referenz für Query Service](https://experienceleague.adobe.com/en/docs/experience-platform/query/sql/overview)
