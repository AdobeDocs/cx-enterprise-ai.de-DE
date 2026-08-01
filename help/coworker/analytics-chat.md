---
title: Analysieren von Customer Journey Analytics-Daten mit dem Coworker Chat
description: Erfahren Sie, wie Sie mit dem Adobe CX Enterprise Coworker Chat Customer Journey Analytics-Daten analysieren, Trichter erstellen und herausfinden können, wo Kundinnen und Kunden ihre Journey abgeben.
source-git-commit: 6e3ab12f1d9ec706e745749b7ca47b91a09ff8b3
workflow-type: tm+mt
source-wordcount: '2104'
ht-degree: 5%

---

# Analysieren von Customer Journey Analytics-Daten mit dem Coworker Chat

>[!AVAILABILITY]
>
>Die in diesem Artikel beschriebene Funktion befindet sich in der eingeschränkten Testphase der Veröffentlichung und ist möglicherweise noch nicht in Ihrer Umgebung verfügbar. Dieser Hinweis wird entfernt, wenn die Funktion allgemein verfügbar ist. Informationen zum Customer Journey Analytics-Veröffentlichungsprozess finden Sie unter [Customer Journey Analytics-Funktionsversionen](https://experienceleague.adobe.com/de/docs/analytics-platform/using/releases/latest).

Adobe CX Enterprise Coworker Chat kann erweiterte Datenanalysen durchführen, die zuvor nur in Analysis Workspace möglich waren. Coworker Chat greift auf Daten aus Ihren Customer Journey Analytics-Datenansichten zu, sodass Sie diese Daten untersuchen und Antworten auf Eingabeaufforderungen in natürlicher Sprache erhalten können.

Bevor Sie mit der Analyse beginnen, informieren Sie sich über die Oberfläche und die Konfigurationsoptionen für den Coworker-Chat und stellen Sie dann sicher, dass Coworker mit Customer Journey Analytics und der Datenansicht verbunden ist, die die Daten enthält, die Sie verwenden möchten.

## Erste Schritte mit dem Coworker Chat

### Schnittstellen- und Konfigurationsoptionen

Bevor Sie den Coworker Chat mit Ihren Customer Journey Analytics-Daten verwenden, erfahren Sie, wie Sie sich anmelden und Konfigurationsoptionen für die folgenden Funktionen verwalten:

* Chat-Eingaben

* Unterhaltungen

* Marktplätze

* MCP-Server

* Arbeitsspeicher

* Plug-ins

* Kenntnisse

* Und mehr

Weitere Informationen finden Sie im [Handbuch zur Benutzeroberfläche für den Coworker-Chat](https://experienceleague.adobe.com/de/docs/cx-enterprise-coworker/content/chat/ui-guide).

### Anwendungsbeispiele für Customer Journey Analytics

Sie können Customer Journey Analytics-Anwendungsfälle und Beispielaufforderungen sehen, die Anwender im Adobe CX Enterprise Coworker Chat verwenden. Jede Eingabeaufforderung wird so erstellt, dass sie kopiert, mit Ihren eigenen Daten und Kontexten angepasst und durch Konversation verfeinert wird.

Weitere Informationen finden Sie unter [Anwendungsbeispiele](https://experienceleague.adobe.com/de/docs/cx-enterprise-coworker/content/chat/use-cases).

## Überprüfen, ob der Coworker Chat mit Customer Journey Analytics verbunden ist

1. Stellen Sie im Coworker Chat sicher, dass Coworker mit Customer Journey Analytics verbunden ist:

1. Wählen Sie das MCP-Symbol in der linken Leiste aus und stellen Sie sicher, dass [!UICONTROL **cja-**]) in Ihrer Liste der verbundenen MCP-Server verfügbar ist.

   ![Das hervorgehobene MCP-Symbol in der linken Leiste „Mitarbeiter“](assets/data-validation-aa-cja/coworker-mcp-cja.png)

1. (Bedingt) Wenn [!UICONTROL **cja-mcp**] noch nicht verbunden ist, wählen Sie [!UICONTROL **MCP-Server hinzufügen**], geben Sie cja im Feld [!UICONTROL **Server-Name**] an und wählen Sie es aus, wenn es angezeigt wird. Wählen Sie dann [!UICONTROL **Server hinzufügen**].

## Herstellen einer Verbindung zur rechten Datenansicht

Eine Datenansicht ist ein Container in Customer Journey Analytics, der bestimmt, wie Daten interpretiert werden.

Möglicherweise haben Sie Zugriff auf verschiedene Datenansichten in Customer Journey Analytics, die jeweils unterschiedliche Dimensionen und Metriken enthalten, die Coworker bei der Datenanalyse verwenden kann.

### Festlegen, welche Datenansichten verwendet werden sollen

Teilen Sie Coworker mit, welche Fragen Sie beantwortet haben möchten, und fragen Sie, auf welche Datenansichten Sie Zugriff haben, damit Sie diese Informationen am besten bereitstellen können. Sie können [&#x200B; auch „Ihre Datenansicht als Voreinstellung im Speicher festlegen](#add-a-data-view-preference-in-memory).

**Sie:**

>[!BEGINSHADEBOX]

Ich bin daran interessiert zu erfahren, wo Kunden auf der Kunden-Journey abbrechen. Auf welche Datenansichten in Customer Journey Analytics habe ich Zugriff, die diese Frage für mich beantworten können?

>[!ENDSHADEBOX]

**Chat-Antwort eines Kollegen:**

>[!BEGINSHADEBOX]

Sie haben Zugriff auf drei Datenansichten. Die `Customer lifecycle` Datenansicht enthält die folgenden Dimensionen und Metriken, die am besten für die Beantwortung Ihrer Frage geeignet sind.

>[!ENDSHADEBOX]

**Sie:**

>[!BEGINSHADEBOX]

Toll, verwenden wir diese Datenansicht.

>[!ENDSHADEBOX]

**Chat-Antwort eines Kollegen:**

>[!BEGINSHADEBOX]

Okay, ich werde die `Customer lifecycle` Datenansicht verwenden, um zukünftige Fragen in dieser Chat-Sitzung zu beantworten.

>[!ENDSHADEBOX]

### Hinzufügen einer Datenansichtseinstellung im Speicher

Der Coworker Chat enthält eine Speicherfunktion, mit der Sie Zugriff auf Informationen erhalten, die sich über alle Chats erstrecken. Es empfiehlt sich, die von Ihnen bevorzugten Datenansichten im Arbeitsspeicher des Kollegen als Voreinstellungen hinzuzufügen.

1. Wählen Sie im Coworker Chat in der linken Navigationsleiste das Speichersymbol aus.

1. Geben Sie auf der Speicherseite im Abschnitt „Gespeicherte Voreinstellungen“ eine oder mehrere Datenansichten an, die der Coworker Chat in Ihren Chats verwenden soll.

   ![Speicherabschnitt in der linken Leiste](assets/data-validation-aa-cja/coworker-memory.png)

## Durchführen von Analysen in Customer Journey Analytics

Nachdem ein Mitarbeiter eine Visualisierung erstellt hat, können Sie die Visualisierung in Analysis Workspace in Customer Journey Analytics öffnen, um eine tiefergehende Analyse mit detaillierterer Steuerung zu ermöglichen. Die Visualisierung wird in einem neuen Analysis Workspace-Projekt in Customer Journey Analytics geöffnet.

Öffnen einer Visualisierung in einem neuen Analysis Workspace-Projekt:

1. Wählen Sie [!UICONTROL **Analysieren in CJA**] neben einer Visualisierung aus, die in Coworker erstellt wird.

1. Wenn die Visualisierung in Customer Journey Analytics geöffnet ist, können Sie die Analysis Workspace-Browser-Benutzeroberfläche per Drag-and-Drop verwenden, um Änderungen vorzunehmen, Ihre Analyse weiter zu erstellen, eine Zielgruppe zu erstellen und vieles mehr. Sie können Ihr Workspace-Projekt sogar für jeden freigeben, den Sie auswählen.

   Weitere Informationen zu Analysis Workspace finden Sie unter [Übersicht über Analysis Workspace](https://experienceleague.adobe.com/de/docs/analytics-platform/using/cja-workspace/home).

## Beispiel: Finden Sie heraus, wo Kunden abbrechen

Sie können Coworker Chat bitten, Ihre Daten zu verwenden, um geschäftliche Fragen zu analysieren.

Als Marketing-Manager, Merchandiser oder Wachstumsleiter möchten Sie vielleicht verstehen, wo Kundinnen und Kunden den Weg zum Kauf verlassen, warum sie ihn getan haben und was getan werden kann, um höhere Konversionsraten zu erzielen.

>[!NOTE]
>
>Die folgenden Abbildungen zeigen beispielhafte Daten für einen fiktiven retailer, [!DNL TechPulse Electronics], der verwendet wird, um die Form des Gesprächs zu zeigen.

### Die Arten von Fragen, die Sie stellen können

Sie müssen nicht wissen, was eine „Fallout-Visualisierung“ ist oder welche Metrik in welchen Slot passt. Beschreiben Sie stattdessen das Ergebnis, das Ihnen wichtig ist, in einfacher Sprache:

* „Wo verlieren wir Menschen auf dem Weg zum Kauf?“
* „Was ist meine vollständige Konversion von funnel, von der Produktansicht bis zum Checkout?“
* „Welche Marketing-Kanäle lecken am meisten zwischen Warenkorb und Kauf?“
* „Ist der Warenkorbabbruch auf Mobilgeräten oder Desktop-Computern schlimmer?“
* „Konvertieren Menschen aus Paid Social anders als Menschen aus E-Mails?“

### Das Gespräch

#### &#x200B;1. Beginnen Sie mit der Geschäftsfrage

**Sie:**

>[!BEGINSHADEBOX]

Wo verlieren wir Menschen auf dem Weg zum Kauf?

>[!ENDSHADEBOX]

**Chat-Antwort eines Kollegen:**

Beachten Sie, dass im Coworker Chat die richtige Visualisierung ausgewählt wird, die Touchpoints sequenziert und sogar empfohlene nächste Schritte hinzufügt.

>[!BEGINSHADEBOX]

![funnel-Antwort des Kollegen](assets/data-validation-aa-cja/coworker-funnel-response.png)

Dies ist eine funnel-Frage. Lassen Sie mich die funnel-Konversion ausführen, um zu sehen, wo es auf dem Kaufpfad zu einer Abnahme kommt.

Hier verliert man Menschen:

| Funnel-Schritt | Anzahl | Konvertierung in nächste | Abbruch |
| --- | --- | --- | --- |
| Sessions | 137,476 | 45,0 % Produkt ansehen | 55% verlassen, ohne Produkte zu durchsuchen |
| Produktansichten | 61,845 | 55,0 % In den Warenkorb | 45 % durchsuchen, aber nicht hinzufügen |
| Hinzufügungen zum Warenkorb | 34,045 | 16,4 % Kauf | 83,6 % Warenkorbabbruch |
| Käufe | 5,582 | – | – |

**Die große Erkenntnis: Der zu kaufende Warenkorb ist Ihr größtes Leck**

28.463 Personen fügen Artikel zu ihrem Warenkorb hinzu, schließen den Kauf jedoch nie ab. Dies entspricht einer Abgaberate von 83,6 % bei Warenkorb - dem bei weitem größten Einzelfehler.

Um es in Dollar auszudrücken: Nur 10% mehr dieser Hinzufügungen zum Warenkorb würden etwa 2.846 Käufe hinzufügen. Auf der aktuellen Datenskala ist das potenziell ein erheblicher Umsatz, der noch auf dem Tisch liegt.

**Was dies über Prioritäten sagt:**

| Priorität | Problem | Opportunity-Umfang |
| --- | --- | --- |
| #1 | Warenkorbabbruch bei Kaufabbruch (Rückgang um 83,6 %) | 28.463 verlorene Käufer |
| #2 | Sitzung zur Produktansicht (55 % nie durchsuchen) | 75.631 Sitzungen ohne Produktinteraktion |
| #3 | Produktansicht zum Warenkorb (45 % fügen nicht hinzu) | 27.800 Interessierte, aber unverbindlich |

**Empfohlene nächste Schritte:**

1. Warenkorbabbruch nach Marketing-Kanal aufschlüsseln - Bringen bestimmte Kanäle Low-Intent-Traffic, der zum Warenkorb hinzukommt, aber nie kauft?
1. Betrachten Sie den Warenkorbabbruch nach Gerätetyp - Tötet die Reibung beim mobilen Checkout Konversionen?
1. Ermitteln Sie, welche Produkte am häufigsten aufgegeben werden - Preisproblem? Versand-Überraschung?

**Auf welche davon möchte ich als Nächstes eingehen?** Die Kanalaufschlüsselung würde Ihnen direkt mitteilen, welche Marketing-Aktionen Ihnen „fast-Käufer“ gegenüber tatsächlichen Käufern bringen.

>[!ENDSHADEBOX]

#### &#x200B;2. In das Leck bohren

**Sie:**

>[!BEGINSHADEBOX]

Okay, lassen Sie uns nach Marketing-Kanal aufschlüsseln

>[!ENDSHADEBOX]

**Chat-Antwort eines Kollegen:**

>[!BEGINSHADEBOX]

![funnel-Antwort des Kollegen](assets/data-validation-aa-cja/coworker-funnel-response2.png)

Es gibt eine benutzerdefinierte Dimension **Marketing** Kanal. Lassen Sie mich den funnel daran entnehmen, dann die Konversionsraten pro Kanal berechnen und feststellen, wo jeder Kanal undicht ist.

**Das Urteil: Das Leck ist nicht kanalspezifisch**

Das ist eine wirklich aufschlussreiche Erkenntnis. Hier finden Sie die Aufschlüsselung nach funnel pro Kanal:

| Kanal | Sessions | Zur Produktansicht | Zum Warenkorb hinzufügen | Zu erwerben | Konversion insgesamt | Umsatz/Sitzung |
| --- | --- | --- | --- | --- | --- | --- |
| Paid Search | 43,958 | 45.1% | 54.6% | 16.6% | 4.09% | $499.58 |
| Organische Suche | 31,492 | 44.9% | 54.9% | 16.9% | 4.17% | $494.76 |
| Direkt | 25,661 | 43.6% | 55.4% | 15.8% | 3.82% | $497.29 |
| E-Mail | 17,586 | 45.3% | 55.4% | 16.2% | 4.07% | $501.13 |
| Bezahlte Social Media | 12,684 | 45.4% | 55.7% | 16.0% | 4.03% | $512.17 |
| Anzeige | 6,511 | 45.3% | 55.7% | 16.2% | 4.09% | $501.45 |

**Wichtige Erkenntnisse:**

1. Die Abladung vom Warenkorb zum Kauf ist über alle Kanäle hinweg einheitlich schlecht (83-84 %). Das bedeutet, dass es nicht um die Traffic-Qualität geht - jeder Kanal liefert ähnlich engagierte Besucher. Das Leck liegt in Ihrem Checkout-Erlebnis selbst, nicht in Ihrem Marketing.
1. Kein Kanal ist bei der Konvertierung signifikant besser oder schlechter. Die Gesamtkonversionsraten liegen dicht zwischen 3,8 % und 4,2 %, und der Umsatz pro Sitzung ist nahezu identisch (495 - 512 $).
1. Wo die Auswirkungen auf das Volumen am wichtigsten sind: Die bezahlte Suche verliert die meisten Menschen in absoluten Zahlen (9.015 Warenkorbabbrüche), gefolgt von der organischen Suche (6.449 verloren). Dies sind die größten Chancen in Bezug auf den Wert eines Dollars, da sie den meisten Traffic verursachen.

**Was sagt Ihnen das strategisch**

Die Marketing-Kanäle machen ihren Job - sie alle bringen die Leute dazu sich zu interessieren und fügen zum Warenkorb zu ähnlichen Preisen hinzu. Das Problem liegt im Downstream des Marketings: Ihr Checkout und Zahlungsfluss ist dort, wo das Geld durchsickert.

**Empfohlene nächste Untersuchungen:**

1. Warenkorbabbruch nach Gerätetyp aufschlüsseln - Ist der mobile Checkout defekt oder frustrierend?
1. Sehen Sie, welche Produkte am häufigsten aufgegeben werden - gibt es eine Preis- oder Versandüberraschung an der Kasse?
1. Überprüfen Sie, ob die Kampagne „Holiday_flash_sale“ eine bessere Checkout-Konversion hatte - dringengesteuerte Kampagnen könnten die Checkout-Reibung überwinden.

**Welchen Blickwinkel möchten Sie als Nächstes untersuchen?**

>[!ENDSHADEBOX]

#### &#x200B;3. Weiter untersuchen

**Sie:**

>[!BEGINSHADEBOX]

Interessant. Versuchen wir, nach Gerätetyp aufzuschlüsseln.

>[!ENDSHADEBOX]

**Chat-Antwort eines Kollegen:**

>[!BEGINSHADEBOX]

![funnel-Antwort des Kollegen](assets/data-validation-aa-cja/coworker-funnel-response3.png)

**Gefunden: Der mobile Checkout ist defekt**

Der funnel ist geräteübergreifend bis zum Checkout identisch - dann fällt Mobile von einer Klippe:

| Gerät | Sessions | Zur Produktansicht | Zum Warenkorb hinzufügen | Zu erwerben | Konversion insgesamt |
| --- | --- | --- | --- | --- | --- |
| Desktop | 70,172 | 44.9% | 54.8% | 23.2% | 5.70% |
| Tablet | 14,149 | 44.7% | 55.6% | 14.3% | 3.56% |
| Mobile | 53,449 | 44.9% | 55.3% | 8.1% | 2.02% |

**Die Raucherpistole**

| Metrik | Desktop | Mobile | Lücke |
| --- | --- | --- | --- |
| Warenkorb zur Kaufrate | 23.2% | 8.1% | 15 Prozentpunkte |
| Mobile ist | — | 2,8fach schlechter | — |
| Transaktionsabbrüche | 13,274 | 12,178 | Nahezu das gleiche absolute Volumen |

Das Browsen und Hinzufügen zum Warenkorb funktioniert auf Mobilgeräten einwandfrei (identische Browser-Rate von ~45 %, ~55 % Quote von Hinzufügungen zum Warenkorb). Die Menschen sind gleichermaßen interessiert und engagiert. Aber irgendetwas im mobilen Checkout-Fluss bringt Konversionen zum Erliegen.

**Die Umsatzmöglichkeit**

Wenn die Mobile-Kasse mit derselben Rate wie die Desktop-PCs konvertiert würde, würden Sie ca. 1.991 zusätzliche Käufe erzielen - eine Steigerung des gesamten Kaufvolumens um 35 % durch die Behebung eines Erlebnisses.

**Was passiert wahrscheinlich**

Das Datenmuster (gleiches Engagement, katastrophaler Checkout-Rückgang) ist ein klassisches Signal für:

* Reibungsloser Ablauf von Zahlungsformularen auf kleinen Bildschirmen (Probleme beim automatischen Ausfüllen, Formular-Layout)
* Unerwartete Kosten an der Kasse (Versand, Steuer), die Aufkleber-Schock verursachen
* Gast-Checkout nicht verfügbar oder Anmeldewand auf Mobilgerät
* Seitenladeprobleme oder Zeitüberschreitungsprobleme bei der Zahlungsverarbeitung auf Mobilgeräten

**Empfohlene nächste Schritte:**

1. Aufschlüsselung des Verlassens des Warenkorbs auf Mobilgeräte nach Produktkategorie — Ist es bei teuren Artikeln (was auf Probleme mit dem Vertrauen in den mobilen Zahlungsverkehr hindeutet) schlechter?
1. Sehen Sie, welche Marketing-Kanäle den meisten mobilen Traffic verursachen - geben Sie dafür bezahlte Medienbudgets aus, um Leute in ein kaputtes mobiles funnel zu schicken?
1. Überprüfen Sie, ob ein Seiten- oder Site-Abschnittssignal vorliegt - können wir sehen, welche Checkout-Seiten mobile Benutzer zuletzt aufgerufen haben, bevor sie aufgeben?

**Welche möchten Sie untersuchen, oder reicht dieser Beweis, um ihn zu Ihrem UX- und Checkout-Team zu bringen?**

>[!ENDSHADEBOX]

#### &#x200B;4. Aus ihr eine Entscheidung machen

**Sie:**

>[!BEGINSHADEBOX]

Was soll ich also tun?

>[!ENDSHADEBOX]

**Chat-Antwort eines Kollegen:**

>[!BEGINSHADEBOX]

Basierend auf dem, was die Daten zeigen, würde ich mich hier konzentrieren:

* **Reparieren Sie den mobilen Checkout - es ist kein Kanalproblem.** Jeder Kanal konvertiert Personen zu einem ähnlichen, gesunden Tempo in den Warenkorb, sodass die Anzeigenausgaben überall funktionieren. Der Umsatz geht insbesondere im Mobile-Checkout-Fluss verloren, in den die Fehlerbehebung gehört.
* **Beginnen Sie mit der Zahlung und Formularreibung.** Dies sind die häufigsten Gründe dafür, dass vorsätzliche Mobilkäufer ihren Warenkorb verlassen. Mobile Wallet-Optionen anzubieten und das Formular zu kürzen sind in der Regel die schnellsten Gewinne.
* **Überprüfen Sie nach der Behebung erneut.** Sobald die Checkout-Änderungen versendet werden, sollten Sie überprüfen, ob sich die Warenkorb-Kaufrate von Mobile auf die Desktop-Rate von 23,2 % zubewegt.

Soll ich das als Projekt speichern, damit Sie es verfolgen können, oder einen Warnhinweis einrichten, wenn der Kauf von Mobilgeräten per Warenkorb unter einen Schwellenwert fällt?

>[!ENDSHADEBOX]

### Was gerade passiert ist

Bei vier fremdsprachigen Fragen hat uns die Kollegin geholfen:

* Erstellen Sie eine mehrstufige Konversions-funnel und kennzeichnen Sie „Warenkorb-zu-Kauf“ als größtes Leck
* Marketing-Kanal als Ursache ausschließen - jeder Kanal sickerte fast mit der gleichen Rate durch
* Isolieren Sie das eigentliche Problem der mobilen Kasse und quantifizieren Sie die Fehlerbehebung bei einer Steigerung der Käufe um 35 %.
* Entscheiden Sie sich für eine Lösung, die Ihre Prioritäten setzt: mobiles Bezahlen und Formularkonflikte. Dies entspricht einer Konversionsrate von 23,2 % für Desktop-Computer

<!--

## Example #2: Find which marketing efforts drive revenue

You can ask Coworker Chat to use your data to analyze any business question.

For example, as a marketing manager, demand generation lead, or CMO, you might want to know which marketing efforts actually deserve credit for revenue so you can confidently decide where to put your marketing spend, rather than rewarding whichever channel happened to get the last click.

>[!NOTE]
>
>The figures below are illustrative sample data for a fictional retailer, [!DNL TechPulse Electronics], used to show the shape of the conversation.

### The types of questions you can ask

You don't need to know what an "attribution model" is, or how to configure an Attribution panel. Instead, describe the outcome you care about in plain language:

* "Which channels actually drive our revenue, not just the last click?"
* "If I change how I give credit for a sale, does my best channel change?"
* "Which campaigns start customer journeys versus close them?"
* "Am I over-investing in paid search because it always gets the last click?"
* "What role does email play in conversions it never gets credit for?"

### The conversation

#### 1. Start with the business question

**You:**

>[!BEGINSHADEBOX]

Which marketing channels actually drive our revenue?

>[!ENDSHADEBOX]

**Coworker Chat response:**

Notice that Coworker Chat picks the right analysis, starts with the model most reports default to, and immediately flags what that model can't tell you.

>[!BEGINSHADEBOX]

![Coworker Chat showing attributed revenue by marketing channel under a last-touch model](assets/data-validation-aa-cja/coworker-attribution-response.png)

This is an attribution question — let me attribute revenue to your marketing channels so you can see who's earning it.

I'll start with **last-touch attribution**, since that's what most out-of-the-box reports show. It gives all the credit for a sale to the last channel a person used before purchasing.

| Marketing channel | Attributed revenue (last touch) | Share |
| --- | --- | --- |
| Paid search | $948,000 | 34% |
| Organic search | $614,000 | 22% |
| Direct | $474,000 | 17% |
| Email | $307,000 | 11% |
| Paid social | $251,000 | 9% |
| Display | $195,000 | 7% |

**The headline: paid search looks like your hero**

Under last touch, paid search earns a third of all revenue — more than any other channel. If this were the only view you had, you'd likely pour more budget into paid search.

**One important caveat before you do that**

Last touch only tells you who *closed* the sale. It says nothing about who *started* the journey or *assisted* along the way. A channel that introduces people to your brand weeks before they buy gets zero credit here, even if the purchase never would've happened without it.

To know whether paid search is really driving revenue — or just harvesting demand other channels created — you need to compare attribution models.

**Recommended next step:**

Compare the same channels across first-touch, last-touch, and linear models. If paid search stays on top across all of them, it's a genuine driver. If it shrinks under first touch, it's a closer, not a creator.

**Want me to run that comparison?**

>[!ENDSHADEBOX]

#### 2. Compare attribution models

**You:**

>[!BEGINSHADEBOX]

Yes, compare it across models.

>[!ENDSHADEBOX]

**Coworker Chat response:**

>[!BEGINSHADEBOX]

![Coworker Chat comparing channel revenue share across first-touch, last-touch, and linear attribution models](assets/data-validation-aa-cja/coworker-attribution-response2.png)

Here's each channel's share of revenue under three models. First touch credits the channel that started the journey, last touch credits the one that closed it, and linear splits credit evenly across every touch.

| Marketing channel | First touch | Last touch | Linear |
| --- | --- | --- | --- |
| Paid search | 19% | 34% | 26% |
| Organic search | 20% | 22% | 21% |
| Direct | 9% | 17% | 13% |
| Email | 18% | 11% | 15% |
| Paid social | 21% | 9% | 15% |
| Display | 13% | 7% | 10% |

**The verdict: your "best" channel depends entirely on how you count**

This is the finding that changes budget decisions.

1. **Paid search closes far more than it starts.** It jumps from 19% of first touches to 34% of last touches. That's the signature of a *harvester* — it captures people who are already ready to buy, often after another channel introduced them. Valuable, but it's finishing journeys, not creating them.
1. **Paid social and email are badly undercredited by last touch.** Paid social starts 21% of journeys but gets credit for only 9% of sales. Email starts 18% but closes 11%. These channels are doing the expensive work at the top of the funnel and handing warm prospects to paid search.
1. **Organic search is your steady workhorse.** It sits around 20% across every model — it both starts and closes journeys reliably.

**Why this matters for budget**

If you cut paid social or email based on their weak last-touch numbers, you'd starve the top of your funnel — and paid search would have far fewer ready-to-buy people to close. You'd likely see paid search revenue fall too, even though you didn't touch its budget.

**Recommended next step:**

Look at the campaign level to see exactly which efforts start journeys versus close them. That's where you can act — trimming or protecting specific campaigns rather than whole channels.

**Want me to break this down by campaign?**

>[!ENDSHADEBOX]

#### 3. Keep investigating

**You:**

>[!BEGINSHADEBOX]

Let's break it down by campaign.

>[!ENDSHADEBOX]

**Coworker Chat response:**

>[!BEGINSHADEBOX]

![Coworker Chat showing top campaigns ranked by their role as initiators or closers of customer journeys](assets/data-validation-aa-cja/coworker-attribution-response3.png)

There's a **Campaign Name** dimension. Here are your highest-involvement campaigns, comparing the revenue they start (first touch) against the revenue they close (last touch).

| Campaign | Starts (first touch) | Closes (last touch) | Role |
| --- | --- | --- | --- |
| brand_awareness_q3 | $412,000 | $103,000 | Initiator |
| email_winback | $214,000 | $88,000 | Initiator |
| holiday_flash_sale | $268,000 | $249,000 | All-rounder |
| retargeting_dynamic | $71,000 | $339,000 | Closer |
| branded_search_always_on | $84,000 | $498,000 | Closer / harvester |

**The pattern: some of your "worst" campaigns are actually your best starters**

* **brand_awareness_q3** and **email_winback** start far more revenue than they close. On a last-touch ROI report, these look like underperformers you might cut. In reality, they're filling the top of your funnel — the journeys other campaigns finish.
* **retargeting_dynamic** and **branded_search_always_on** are the opposite. They close a lot but start almost nothing. They're efficient closers, but they can only close demand that already exists. Branded search, in particular, is largely capturing people who were going to search for you by name anyway.
* **holiday_flash_sale** does both — it introduces new shoppers and closes them, which is why urgency-driven promotions often look strong under any model.

**What this tells you strategically**

The campaigns you'd cut first on a last-touch report — the awareness and win-back efforts — are the ones creating the demand your closers depend on. Judge initiators on the journeys they start, and closers on the journeys they finish.

**Recommended next steps:**

1. Protect the initiator campaigns even though their last-touch ROI looks weak — they're feeding the funnel.
1. Right-size the branded search spend — test whether trimming it changes total revenue, since much of that demand may convert anyway.
1. Adopt a balanced model — like linear or a position-based model — as your default reporting view, so no channel gets systematically over- or under-rewarded.

**Want me to save this as a project, or is this enough to take into your budget planning?**

>[!ENDSHADEBOX]

#### 4. Turn it into a decision

**You:**

>[!BEGINSHADEBOX]

So how should I allocate budget?

>[!ENDSHADEBOX]

**Coworker Chat response:**

>[!BEGINSHADEBOX]

Based on what the data shows, here's where I'd focus:

* **Stop judging upper-funnel channels on last touch alone.** Paid social and email start about 20% of your revenue each, but last touch credits them for less than half of that. Protect their budgets — they're creating the demand paid search closes.
* **Treat branded search as a harvester, not a driver.** It closes a lot but starts almost nothing. Test trimming it, since much of that demand may convert through other paths anyway.
* **Make a balanced model your default.** Reporting on linear or a position-based model instead of last touch will stop you from over-rewarding closers and under-funding the channels that start journeys.
* **Re-check after you rebalance.** Watch whether total revenue holds steady as you shift spend toward initiators — that's the signal your funnel is healthier, not just your last-touch report.

Want me to save this as a project so you can track it, or build a calculated metric that reports revenue on a balanced attribution model going forward?

>[!ENDSHADEBOX]

### What just happened

In four plain-language questions, Coworker helped us:

* Attribute revenue to marketing channels and flag that the default last-touch view tells only part of the story
* Compare attribution models and reveal that the "best" channel changes completely depending on how credit is counted
* Discover that paid social and email start far more revenue than they ever get credit for closing
* Identify which campaigns initiate journeys versus close them, and walk away with a budget direction: protect the initiators, right-size the harvesters, and report on a balanced model

-->
