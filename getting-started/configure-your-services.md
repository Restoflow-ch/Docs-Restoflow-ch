---
description: >-
  Ihre Restaurantdienstleistungen stellen die verschiedenen Bestellarten dar, die Sie annehmen. Sicht
  In unserem Video erhalten Sie eine ausführliche Erklärung aller verfügbaren Einstellungen.
---

# Konfigurieren Sie Ihre Dienste

{% embed url="https://youtu.be/EUW9nZVAE68" %}
Video-Tutorial zu Dienstleistungen
{% endembed %}

Derzeit sind 4 Dienste verfügbar. Sie sind:

* Selbstabholung – Bestellungen, die von Kunden im Geschäft zum Mitnehmen abgeholt werden
* Lieferung – Bestellungen, die an die Adresse des Kunden geliefert werden
* Dine-in – Bestellungen, die von Kunden aufgegeben werden, die derzeit in Ihrem Geschäft sitzen
* Tischreservierung – eine Reservierung für einen späteren Zeitpunkt

## So konfigurieren Sie Ihre Dienste

1. Besuchen Sie Ihr Restaurant-Dashboard und gehen Sie zur Einstellungsseite
2. Wählen Sie den Reiter „Dienste“ und bearbeiten Sie Ihre Einstellungen nach Bedarf

## Dienste aktivieren und deaktivieren

Sie können Dienste nach Bedarf aktivieren oder deaktivieren. Gehen Sie zu den gewünschten Diensteinstellungen und schalten Sie einfach den Schalter „Aktiviert“ um, um ihn zu aktivieren oder zu deaktivieren.

{% hint style="info" %}
Sie müssen mindestens einen Dienst aktiviert haben
{% endhint %}

## Servicehinweise

Sie können für jeden Service benutzerdefinierte Notizen hinzufügen, die dem Kunden bei Auswahl angezeigt werden. Nützlich, wenn Sie Ihrem Kunden eine wichtige Botschaft übermitteln müssen

## Bestellzeiten

Erst wenn Ihr Shop geöffnet ist, kann ein Kunde eine sofort fällige Bestellung aufgeben. Bestellungen für einen späteren Zeitpunkt müssen innerhalb Ihrer Öffnungszeiten geplant werden. Daher werden die Bestellzeiten größtenteils durch die Öffnungszeiten Ihres Geschäfts bestimmt. Von dort aus verfügt jeder Dienst über seine eigenen separaten Auftragszeiteinstellungen, die Ihnen eine detailliertere Kontrolle ermöglichen.

### Bestellzeiten aktivieren und deaktivieren

Unter der Registerkarte „Bestellzeiten“ in den Serviceeinstellungen können Sie sowohl sofortige als auch geplante Bestellungen aktivieren und deaktivieren.

### Versatz erster Ordnung

Dies ist der Zeitraum von der Eröffnung Ihres Shops bis zur Annahme der ersten Bestellung. Wenn beispielsweise der Versatz der ersten Bestellung auf 30 Minuten eingestellt ist und Ihr Geschäft um 9:00 Uhr öffnet, kann die erste Bestellung um 9:30 Uhr aufgegeben oder geplant werden.

### Versatz der letzten Bestellung

Dies ist der Zeitraum von der Schließung Ihres Geschäfts bis zur Annahme der letzten Bestellung. Wenn der Versatz der letzten Bestellung beispielsweise auf 30 Minuten eingestellt ist und Ihr Geschäft um 21:00 Uhr schließt, kann die letzte Bestellung um 20:30 Uhr aufgegeben oder geplant werden.

### Auftragsversatz

Der normale Bestellversatz gilt nur für geplante Bestellungen zu einem späteren Zeitpunkt. Dies ist der Zeitraum, ab dem eine geplante Bestellung aufgegeben werden kann. Es dient beispielsweise dazu, Kunden daran zu hindern, ihre Bestellung in den nächsten 10 Minuten einzuplanen, anstatt nur zu verlangen, dass sie so schnell wie möglich fällig ist.

Wenn Ihr Bestellversatz beispielsweise 30 Minuten beträgt und die aktuelle Zeit 18:00 Uhr ist, ist der nächste Zeitpunkt, an dem ein Kunde eine Bestellung planen kann, 19:00 Uhr. Wenn sie es vor 19:00 Uhr möchten, können sie stattdessen einfach so schnell wie möglich bestellen. Wenn der Bestellversatz 15 Minuten betrug, kann der Kunde für 18:30 Uhr bestellen.

Der Auftragsversatz dient auch als Cut-Off-Punkt, um Ihnen Zeit zu geben, den Auftragsplan einzuhalten. Wenn es beispielsweise 18:00 Uhr ist und Ihr Bestellversatz 30 Minuten beträgt. Wenn der Kunde eine Bestellung für 19:00 Uhr plant, muss er die Bestellung vor 18:30 Uhr aufgeben. Damit haben Sie 30 Minuten Zeit, um die geplante Zeit einzuhalten.

Wenn sie zu lange brauchen und die Zeit 18:30 Uhr überschreitet, erhalten sie eine Benachrichtigung, die ihnen mitteilt, dass die Bestellung auf „So schnell wie möglich fällig“ anstelle der geplanten Zeit, 19:00 Uhr, geändert wurde.

## Individuelle Servicezeiten

Jeder Dienst kann seine eigenen unabhängigen Betriebszeiten haben. Durch das Festlegen benutzerdefinierter Betriebszeiten für einen bestimmten Dienst werden die für Ihren Geschäftsstandort festgelegten Betriebszeiten außer Kraft gesetzt.

## Geschätzte Wartezeiten und automatische Status

Damit Sie Ihre Bestellungen und Kundenerwartungen besser verwalten können, bieten wir eine optimierte Möglichkeit zur Berechnung von Bestellwartezeiten und zur automatischen Statusaktualisierung. Es gibt 6 Bestellstatus:

* Unbestätigt
* Bestätigt
* Fertig
* Unterwegs (nur Lieferung)
* Abgeschlossen
* Abgesagt

Sowohl geschätzte Wartezeiten als auch automatische Statusaktualisierungen sind mit denselben Zeiteinstellungen verbunden. Dadurch sind Ihre Statusaktualisierungen und Wartezeiten miteinander synchronisiert. Dies vermeidet jegliche Verwirrung beim Kunden. Diese Timing-Einstellungen sind:

| Einstellung (Minuten) | Von Status | Zum Status |
| ---------------------------------- | ----------- | --------- |
| Zeit bis zur Bestätigung | Unbestätigt | Bestätigt |
| Zeit bis zur Fertigstellung | Bestätigt | Bereit |
| Zeit bis zur Route (nur Lieferung) | Bereit | Unterwegs |
| Zeit bis zur Fertigstellung | Bereit | Komplett |

{% hint style="info" %}
* Die Zeit bis zur Bestätigung ist die Zeit zwischen der Auftragserteilung und der Bestätigung. Wenn Sie die Zeit bis zur Bestätigung auf „0“ setzen, erfolgt eine sofortige Auftragsbestätigung. Sie müssen auch den automatischen Status für den bestätigten Status aktivieren.
* Die Zeit bis zur Fertigstellung ist die Zeit, die Sie nach der Bestätigung benötigen, um eine Bestellung vorzubereiten
* Die Zeit bis zum Versandstatus ist praktisch die Zeit zwischen der Vorbereitung einer Bestellung und der Annahme durch den Zustellfahrer.
* Die Zeit bis zum Abschluss ist nützlich, um Bestellungen automatisch als abgeschlossen zu markieren
{% endhint %}

### Geschätzte Wartezeiten

Wie bereits erwähnt, werden die Wartezeiten der Kunden anhand der oben genannten Zeiteinstellungen berechnet.&#x20;

#### Wie die geschätzte Wartezeit für Abhol- oder Essensbestellungen berechnet wird

Bei Abhol- und Speisenbestellungen berechnet sich die geschätzte Wartezeit aus der Berechnung des Kaufs durch Addition der **Zeit bis zur Bestätigung** mit den Werten für die **Zeit bis zur Bereitschaft**. Wenn Ihre **Zeit bis zur Bestätigung** beispielsweise 5 und Ihre **Zeit bis zur Fertigstellung** 20 beträgt, würde der Kunde eine geschätzte Wartezeit von 20 + 5 = 25 Minuten erhalten.

Wenn Sie keinen Wert für die Zeit bis zur Bestätigung oder die Zeit bis zur Bereitschaft hinzugefügt haben, wird die geschätzte Wartezeit nicht berechnet.

#### Wie die geschätzte Wartezeit für Lieferaufträge berechnet wird

Bei Lieferungen wird die Wartezeit berechnet, indem die **Zeit bis zur Bestätigung** + **Zeit bis zur Fertigstellung** + **Zeit bis zur Route** addiert werden. Dann kommt noch die **Fahrzeit** dazu. Die Fahrzeit wird mithilfe eines externen Dienstes ermittelt, der Verkehrsdaten berücksichtigt. Dadurch erhält der Kunde eine äußerst genaue Wartezeit für die Lieferung seiner Bestellung. Vorausgesetzt&#x20;

Wenn Sie keinen Wert für die Zeit bis zur Bestätigung, die Zeit bis zur Bereitstellung oder die Zeit bis zur Route hinzugefügt haben, wird die Lieferzeit nicht berechnet.

### Automatisierte Status

Automatisierte Status ändern den Status einer Bestellung nach Ablauf einer festgelegten Zeitspanne. Auf diese Weise können Sie beispielsweise Folgendes tun:

* Neue Bestellungen automatisch bestätigen
* Markieren Sie Bestellungen nach einer gewissen Zeit als fertig
* Markieren Sie Bestellungen nach einer bestimmten Zeit als abgeschlossen

Dies ist sehr hilfreich, wenn Sie Ihre Geschäftszeiten gut kennen und den Bestellstatus nicht manuell aktualisieren möchten. Automatische Statusaktualisierungen können auch für jeden Status einzeln aktiviert oder deaktiviert werden. Auf diese Weise können Sie geschätzte Wartezeiten angeben, ohne den Status automatisch zu aktualisieren. Oder Sie können Bestellungen einfach sofort bestätigen und den Rest manuell erledigen.

Damit automatische Statusaktualisierungen funktionieren, müssen Sie sie für einen bestimmten Status aktivieren und sicherstellen, dass die Zeiteinstellungen zu diesem bestimmten Status hinzugefügt werden.

#### So funktionieren automatisierte Status

Statusaktualisierungen hängen von Ihren Timing-Einstellungen, der Art der Bestellung und der Fälligkeitszeit der Bestellung ab. Es lässt sich am besten anhand einer Reihe von Beispielen erklären.

Für die Beispiele gehen wir davon aus, dass unsere Timing-Einstellungen wie folgt sind

* Zeit bis zur Bestätigung – 10 Minuten
* Zeit bis zur Zubereitung: 10 Minuten
* Zeit bis zur Fahrt – 10 Minuten
* Zeit bis zur Fertigstellung: 60 Minuten

#### Beispiele für Abholung und Abendessen

Wenn ein Kunde um 19:00 Uhr eine Bestellung zur Abholung oder zum Abendessen aufgibt, ist diese sofort fällig

| Zeit | Aktion |
| ------ | ------------------------------------------------------------------------------------------------------------------------------------------ |
| 19:00 Uhr | Bestellung wurde aufgegeben, Status unbestätigt |
| 19:10 Uhr | Status auf „Bestätigt“ aktualisiert, da die Zeit bis zur Bestätigung 10 Minuten beträgt |
| 19:20 Uhr | Der Status wurde auf „Bereit“ aktualisiert, da die Zeit bis zur Fertigstellung 10 Minuten beträgt. Dies wäre auch die dem Kunden angezeigte voraussichtliche Bestellbereitschaftszeit. |
| 20:20 Uhr | Status auf „Abgeschlossen“ aktualisiert, da die Zeit bis zum Abschluss 60 Minuten beträgt |

Für den Fall, dass Sie der geschätzten Bestellbereitschaftszeit des Kunden weitere 10 Minuten hinzugefügt haben, sieht es wie folgt aus:

| Zeit | Aktion |
| ------ | ----------------------------------------------------------------------------------------------------------------------- |
| 19:00 Uhr | Bestellung wurde aufgegeben, Status unbestätigt, Sie addieren 10 Minuten zur geschätzten Bereitschaftszeit |
| 19:10 Uhr | Status auf „Bestätigt“ aktualisiert, da die Zeit bis zur Bestätigung 10 Minuten beträgt |
| 19:30 Uhr | Der Status wurde auf „Bereit“ aktualisiert, da die alte Bereitschaftszeit 19:20 Uhr war. Da Sie weitere 10 Minuten hinzugefügt haben, wird daraus 19:30 Uhr |
| 20:30 Uhr | Status auf „Abgeschlossen“ aktualisiert, da die Zeit bis zum Abschluss 60 Minuten beträgt |

Wenn wir keine voraussichtliche Bereitschaftszeit für die Bestellung berechnen können, weil beispielsweise die Zeit bis zur Bestätigung fehlt, würde es wie folgt ablaufen

| Zeit | Aktion |
| ------ | ------------------------------------------------------------------- |
| 19:00 Uhr | Bestellung wurde aufgegeben, Status unbestätigt |
| 19:05 Uhr | Sie aktualisieren den Bestellstatus manuell auf bestätigt |
| 19:15 Uhr | Status auf „Bereit“ aktualisiert, da die Zeit bis zur Fertigstellung 10 Minuten beträgt |
| 20:15 Uhr | Status auf „Abgeschlossen“ aktualisiert, da die Zeit bis zum Abschluss 60 Minuten beträgt |

Wenn ein Kunde um 18:00 Uhr eine Bestellung zur Abholung oder zum Essen aufgibt, die um 19:00 Uhr fällig ist, passiert Folgendes

| Zeit | Aktion |
| ------ | ---------------------------------------------------------------------------------- |
| 18:00 Uhr | Bestellung wurde aufgegeben, Status unbestätigt |
| 18:10 Uhr | Status auf „Bestätigt“ aktualisiert, da die Zeit bis zur Bestätigung 10 Minuten beträgt |
| 19:00 Uhr | Der Status wurde auf „Bereit“ aktualisiert, da der Kunde die Bestellung zu diesem Zeitpunkt für | geplant hat
| 20:00 Uhr | Status auf „Abgeschlossen“ aktualisiert, da die Zeit bis zum Abschluss 60 Minuten beträgt |

#### Lieferbeispiele

Für die Lieferbeispiele gehen wir davon aus, dass die Fahrzeit zwischen Ihrem Geschäft und der Lieferadresse 10 Minuten beträgt.

Wenn ein Kunde um 19:00 Uhr einen Lieferauftrag aufgibt, ist dieser sofort fällig

| Zeit | Aktion |
| ------ | ------------------------------------------------------------------------------------------------------------------------------ |
| 19:00 Uhr | Bestellung wurde aufgegeben, Status unbestätigt |
| 19:10 Uhr | Status auf „Bestätigt“ aktualisiert, da die Zeit bis zur Bestätigung 10 Minuten beträgt |
| 19:20 Uhr | Status auf „Bereit“ aktualisiert, da die Zeit bis zur Fertigstellung 10 Minuten beträgt |
| 19:30 Uhr | Der Status wurde auf „Auf Route“ aktualisiert, da die Zeit bis zur Route 10 Minuten beträgt. Dies wird Ihnen auch als Abholzeit des Fahrers | angezeigt
| 19:40 Uhr | Die Bestellung wurde an den Kunden geliefert, da die Fahrzeit 10 Minuten beträgt |
| 20:40 Uhr | Bestellung als abgeschlossen markiert, da die Zeit bis zur Fertigstellung 60 Minuten beträgt |

Wenn wir die voraussichtliche Lieferzeit und die Abholzeit des Fahrers nicht berechnen könnten, beispielsweise wenn die Zeit bis zur Fahrt fehlte, würde Folgendes passieren

| Zeit | Aktion |
| ------ | ------------------------------------------------------------------------------- |
| 19:00 Uhr | Bestellung wurde aufgegeben, Status unbestätigt |
| 19:10 Uhr | Status auf „Bestätigt“ aktualisiert, da die Zeit bis zur Bestätigung 10 Minuten beträgt |
| 19:20 Uhr | Status auf „Bereit“ aktualisiert, da die Zeit bis zur Fertigstellung 10 Minuten beträgt |
| 19:40 Uhr | Sie markieren die Bestellung manuell als unterwegs zur Lieferung |
| 19:50 Uhr | Die Bestellung wurde an den Kunden geliefert, da die Fahrzeit 10 Minuten beträgt |
| 20:50 Uhr | Bestellung als abgeschlossen markiert, da die Zeit bis zur Fertigstellung 60 Minuten beträgt |

Wenn ein Kunde um 18:00 Uhr einen Lieferauftrag aufgibt, der um 19:00 Uhr fällig ist, würde Folgendes passieren

| Zeit | Aktion |
| ------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 18:00 Uhr | Bestellung wurde aufgegeben, Status unbestätigt |
| 18:10 Uhr | Status auf „Bestätigt“ aktualisiert, da die Zeit bis zur Bestätigung 10 Minuten beträgt |
| 18:40 Uhr | Der Status wurde auf „Bereit“ aktualisiert, da die Lieferzeit 10 Minuten und die Zeit bis zum Versand 10 Minuten beträgt. Das bedeutet, dass die Bestellung zu diesem Zeitpunkt fertig sein muss, wenn sie Ihren Kunden um 19:00 Uhr erreichen soll
| 18:50 Uhr | Der Status wurde auf „Unterwegs“ aktualisiert, da die Lieferzeit 10 Minuten beträgt und der Artikel daher zu diesem Zeitpunkt Ihr Geschäft verlassen muss. Dies ist auch die voraussichtliche Abholzeit des Fahrers.                                          |
| 19:00 Uhr | Die Bestellung wurde an den Kunden geliefert |
| 20:00 Uhr | Bestellung als abgeschlossen markiert, da die Zeit bis zur Fertigstellung 60 Minuten beträgt |

Wenn ein Lieferauftrag für einen späteren Zeitpunkt geplant ist, die voraussichtliche Lieferzeit jedoch nicht berechnet werden konnte, wird der Status „Bereit“ und „Auf dem Weg“ nicht automatisch aktualisiert.

{% hint style="info" %}
Wenn Sie jemals Zweifel haben, wie die automatischen Status-Timings für Ihr Szenario funktionieren, denken Sie einfach darüber nach, wie sie logischerweise auf eine Weise funktionieren würden, die für Ihren Kunden und Sie sinnvoll ist. So haben wir es so konzipiert, dass es funktioniert.
{% endhint %}
