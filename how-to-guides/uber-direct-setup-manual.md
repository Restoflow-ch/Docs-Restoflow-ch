# Uber Direct-Setup-Handbuch

## **Anforderungen**

Um Uber-Lieferungen zu ermöglichen, sollte das Restaurant über Folgendes verfügen:

* Stripe Connect
* Restaurant aus folgenden Ländern:
* Australien
* Neuseeland
* Kanada&#x20;
* USA

## Uber aktivieren

Uber DaaS ist eine zuverlässige und bequeme Möglichkeit, Ihr Essen schnell und effizient zu liefern. So aktivieren Sie es:

1. Klicken Sie im Admin-Dashboard auf Einstellungen > Integrationen, suchen Sie die Uber Delivery Management-Karte und klicken Sie darauf.

<figure><img src="../.gitbook/assets/Screen Shot 2023-05-10 at 9.52.37 AM.png" alt=""><figcaption></figcaption></figure>

2. Ein Popup öffnet sich und füllt die Informationen aus. Klicken Sie auf Speichern.

<figure><img src="../.gitbook/assets/Screen Shot 2023-05-10 at 9.56.08 AM.png" alt=""><figcaption></figcaption></figure>

3. Legen Sie Uber als Standardlieferung fest

Sobald Sie Uber DaaS aktiviert haben, können Sie den Standard-Lieferanbieter unter „Einstellungen“ > „Dienste“ > „Lieferungen“ auswählen (wie im Bild unten gezeigt).

<figure><img src="../.gitbook/assets/Screen Shot 2023-05-10 at 9.47.12 AM.png" alt=""><figcaption></figcaption></figure>

### Hinweise:

* Stellen Sie sicher, dass Ihre Kartendatenquelle Google Maps ist. Gehen Sie zu Einstellungen > System > Standort > Kartendatenquelle.

<figure><img src="../.gitbook/assets/Uber Screenshot 2023-05-09 at 6.38.47 PM.png" alt=""><figcaption></figcaption></figure>

* Die Währung muss mit dem Standort des Landes und der Verfügbarkeit im Uber-Land übereinstimmen. Gehen Sie zu Einstellungen > System > Allgemein > Währung.

<figure><img src="../.gitbook/assets/Uber Screenshot 2023-05-09 at 6.41.14 PM.png" alt=""><figcaption></figcaption></figure>

* Uber benötigt eine gültige Telefonnummer von Ihrem Geschäft (die Landesvorwahl muss vorhanden sein). Gehen Sie zu Einstellungen > System > Standort > Telefonnummer.

<figure><img src="../.gitbook/assets/Uber Screenshot 2023-05-09 at 6.43.23 PM.png" alt=""><figcaption></figcaption></figure>

## Checkout-Details

Sobald ein Kunde eine Bestellung abschließt, wird Uber (sofern im Admin-Dashboard als Standard-Lieferanbieter festgelegt) als Lieferanbieter angezeigt.

<figure><img src="../.gitbook/assets/Screenshot 2023-05-09 at 7.06.03 PM.png" alt=""><figcaption></figcaption></figure>

#### Die Lieferschätzung liefert Folgendes:

**Lieferanbieter** – das ist Uber

**Geschätzte Gebühr** – die Gesamtgebühr

**Tipps** – werden vom Benutzer eingegeben und direkt an den Uber-Fahrer gesendet

**Geschätzte Lieferzeit** – Zeit bis zur Abgabe



#### Die akzeptable Zahlungsmethode ist die folgende:

**Kreditkarte** – sofern aktiviert und mit angegebener Stripe Connect-Konto-ID

**Apple Pay** | **Google Pay (Stripe**)



## Bestellworkflow

Sobald der Kunde die Bestellung aufgegeben hat, wird die Miniaturansicht der Bestellung im Admin-Dashboard durch das Uber-Logo ersetzt (was anzeigt, dass Uber verwendet wird).

#### Bestellung: UNBESTÄTIGT

<figure><img src="../.gitbook/assets/Screenshot 2023-05-09 at 7.44.43 PM.png" alt=""><figcaption></figcaption></figure>

#### Bestellung: BESTÄTIGT

Die Bestellung **SOLLTE** den Status **BESTÄTIGT** erreichen, um die Uber-Lieferanfrage auszulösen.

Sobald die Bestellung auf BESTÄTIGT gesetzt ist, ist die Lieferverfolgungs-URL sowohl im ADMIN als auch im KUNDENbereich verfügbar.

<figure><img src="../.gitbook/assets/Untitled (7).png" alt=""><figcaption><p>Admin Order View</p></figcaption></figure>

<figure><img src="../.gitbook/assets/Untitled (4).png" alt=""><figcaption><p>Customer Order View</p></figcaption></figure>

<figure><img src="../.gitbook/assets/Untitled (5).png" alt=""><figcaption><p>Sample Screenshot of the Tracking URL</p></figcaption></figure>

<figure><img src="../.gitbook/assets/Untitled (6).png" alt=""><figcaption><p>SMS sent by Uber to the recipient.</p></figcaption></figure>

#### Bestellung: FERTIG

<figure><img src="../.gitbook/assets/Untitled (9).png" alt=""><figcaption><p>Customer Order View</p></figcaption></figure>

Es wird erwartet, dass der Fahrer noch auf dem Weg zum Restaurant ist oder im Restaurant wartet.

#### Bestellung: UNTERWEGS

<figure><img src="../.gitbook/assets/Untitled (10).png" alt=""><figcaption><p>Admin Order View</p></figcaption></figure>

#### Bestellung: ABGESAGT

Wenn die Bestellung storniert wird (durch den Kunden oder das Geschäft), wird auch die Uber-Lieferung automatisch storniert





{% hint style="danger" %}
Bitte senden Sie eine E-Mail an [info@restoflow.ch](mailto:info@restoflow.ch) oder nutzen Sie die Chat-Support-Funktion, um Hilfe bei der Aktivierung dieser Funktion zu erhalten.
{% endhint %}
