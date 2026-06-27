---
description: >-
  Erfahren Sie, wie Sie Apple Pay zusammen mit Checkout.com zur Annahme einrichten
  Reibungslose Kreditkartenzahlungen der Kunden über Touch ID und Face ID.
---

# Richten Sie Apple Pay mit Checkout.com ein

![Apple pay allows iOS users to pay using their phone](../.gitbook/assets/apple-pay-final.png)

## So funktioniert Apple Pay

Kunden mit Apple Pay-kompatiblen Geräten können diese Zahlungsmethode nutzen, um den Vorgang der Kreditkartenzahlung zu vereinfachen. Apple Pay macht die manuelle Eingabe der Karteninformationen und Versanddetails überflüssig. Kunden müssen die Zahlung lediglich mittels biometrischer Authentifizierung wie Touch ID autorisieren.

## Anforderungen

Um Apple Pay mit Restoflow zu konfigurieren und zu nutzen, müssen Sie einige Geschäftskonten und Tools wie folgt vorbereiten:

* Ein Checkout.com-Geschäftskonto. Sie können hier eine Anfrage zur Erstellung eines neuen Kontos an Checkout.com senden – [https://www.checkout.com/contact-sales](https://www.checkout.com/contact-sales)
* Ein Apple-Entwicklerkonto; Stellen Sie sicher, dass Sie über die richtige Rolle zum Erstellen von Identifikatoren und Zertifikaten verfügen.
* Eine funktionierende Domäne mit einem gültigen SSL-Zertifikat.
* Zugriff auf das `openssl`-Befehlszeilentool. Mehr über OpenSSL erfahren Sie hier – [openssl.org](https://www.openssl.org/)

## Konfigurieren Sie Apple Pay und Checkout.com

### Erstellen Sie eine Händler-ID im Apple-Entwicklerkonto

1. Melden Sie sich bei Ihrem Apple Developer-Konto an.
2. Erstellen Sie Ihren Händler, indem Sie zu **Zertifikate, IDs und Profile > Identifikatoren** gehen, auf die Plus-Schaltfläche klicken, den Abschnitt **Händler-IDs** auswählen und dann auf **Weiter** klicken. Sie können schnell auf diesen Abschnitt zugreifen, indem Sie auf diese URL zugreifen: [https://developer.apple.com/account/resources/identifiers/merchant/add](https://developer.apple.com/account/resources/identifiers/merchant/add/)&#x20;
3. Wählen Sie eine nützliche Beschreibung für den Händler.
4. Als Händler-ID sollten Sie einen beschreibenden Namen verwenden, der sowohl Ihr Unternehmen als auch die Umgebung angibt, in der Sie ihn verwenden werden, zum Beispiel **merchant.com.mystore.produktion**.

{% embed url="https://www.youtube.com/watch?v=UY23UdJ5uJA" %}
Demo von Checkout.com
{% endembed %}

### Konfigurieren Sie Checkout.com als Zahlungsabwickler

1. Melden Sie sich bei Ihrem **Checkout.com Hub-Konto -** [https://hub.checkout.com](https://hub.checkout.com/) an.
2. Gehen Sie zu **Einstellungen > Apple Pay** und klicken Sie auf **Neues Zertifikat**
3. Klicken Sie auf **Ihre Zertifikatsignierungsanforderung herunterladen**. Sie erhalten eine `.csr`-Datei. Sie sollten diese Datei an einem geeigneten Ort speichern, da Sie sie für Ihr Apple Developer-Konto benötigen.
4. Klicken Sie bis Schritt 3 auf **Weiter** und lassen Sie diese Seite geöffnet.
5. Gehen Sie zurück zu Ihrem Apple Developer-Konto, gehen Sie zum Listenabschnitt „Händler-IDs“ – [https://developer.apple.com/account/resources/identifiers/list/merchant](https://developer.apple.com/account/resources/identifiers/list/merchant) und klicken Sie auf den Händler, den Sie zuvor erstellt haben.
6. Scrollen Sie zum Abschnitt **Apple Pay Merchant Identity Certificate** und klicken Sie auf **Zertifikat erstellen**.
7. Wählen Sie bei der Frage zur Zahlungsabwicklung in China **Nein** und klicken Sie auf **Weiter**.
8. Laden Sie die Datei `.csr` hoch und klicken Sie auf **Weiter**.
9. Klicken Sie auf „Herunterladen“ und speichern Sie die `.cer`-Datei, die Sie erhalten haben.
10. Gehen Sie zurück zu Ihrem Checkout.com Hub-Konto und aktualisieren Sie diese `.cer`-Datei.

{% embed url="https://www.youtube.com/watch?v=jyY789fQoKs" %}
Demo von Checkout.com
{% endembed %}

### Bereiten Sie die Domäne für die Validierung vor

1. Gehen Sie zurück zu Ihrem [Apple-Entwicklerkonto] (https://drive.google.com/drive/u/1/folders/1kZMY4EHyBdbBBc-uwpaAt4sTtEPQSO\_7) und greifen Sie wie in den vorherigen Schritten auf die Händlerseite zu.
2. Klicken Sie im Abschnitt „Händlerdomänen“ auf „Domäne hinzufügen“.
3. Geben Sie die Domain Ihres Unternehmens ein und klicken Sie auf Speichern.
4. Klicken Sie auf „Herunterladen“, um die `.txt`-Datei abzurufen.
5. Sie sollten diese Datei an einem zugänglichen Ort speichern. Der Schritt zur Domänenüberprüfung ist noch nicht abgeschlossen. Wir werden darauf zurückkommen, wenn wir Apple Pay auf dem Restoflow konfigurieren.

### Erstellen Sie Ihre Apple Pay-Zertifikate

1. Greifen Sie auf Ihr Terminal zu und erstellen Sie mit diesem Befehl eine `.csr`- und `.key`-Datei:

    ```
    openssl req -out uploadMe.csr -new -newkey rsa:2048 -nodes -keyout certificate.key
    ```
2. Geben Sie in der Eingabeaufforderung des Terminals Ihre Daten ein. Stellen Sie sicher, dass Sie das Passwort leer lassen. Sie erhalten eine `.csr`- und eine `.key`-Datei.
3. Gehen Sie zurück zu Ihrer Händlerseite im **Apple Developer Account**.
4. Klicken Sie im Abschnitt **Apple Pay Merchant Identity Certificate** auf **Zertifikat erstellen**.
5. Laden Sie die Datei `.csr` hoch, die Sie mit dem obigen Befehl erstellt haben. Es sollte `uploadMe.csr` heißen, wenn Sie einfach den obigen Befehl kopieren.
6. Klicken Sie auf „Weiter“ und dann auf „Herunterladen“, um Ihre `.cer`-Datei zu erhalten. Der Dateiname sollte wahrscheinlich `merchant_id.cer` lauten.
7. Konvertieren Sie die `.cer`-Datei mit dem folgenden Befehl in eine `.pem`-Datei:&#x20;

    ```
    openssl x509 -inform der -in merchant_id.cer -out certificate.pem
    ```

{% embed url="https://youtu.be/yK1DuXqVCEc" %}
Demo von Checkout.com
{% endembed %}

### Zusammenfassung

Nachdem Sie alle oben genannten Schritte durchgeführt haben, sollten Sie Folgendes zur Hand haben:

* Eine Apple-Händler-ID
* Ein konfiguriertes Checkout.com-Konto, das mit Ihrem Apple-Händler verknüpft ist.
* Eine Domain, die mit Ihrem Apple-Händler verknüpft ist und sich vorerst im Status **Ausstehend** befinden sollte.
* Eine `apple-developer-merchantid-domain-association.txt`-Datei, die von Apple bereitgestellt wird, wenn Sie die Domäne hinzufügen.
* Eine `.key`- und `.pem`-Zertifikatsdatei.

## Aktivieren Sie Apple Pay im Restoflow Dashboard

Nachdem wir das Apple Developer Account und Checkout.com konfiguriert haben, müssen wir einige Schritte im Restoflow-Dashboard ausführen, um Apple Pay voll funktionsfähig zu machen.

1. Gehen Sie in Ihrem Restoflow-Dashboard über Ihre Restauranteinstellungen.
2. Klicken Sie auf die Registerkarte **Zahlungen** und dann auf **Zahlungsmethode hinzufügen**.
3. Wählen Sie **Apple Pay (Checkout.com)** in der Zahlungsmethodenliste aus und klicken Sie auf **Methode hinzufügen**.

![Adding Apple Pay (Checkout.com) payment method](../.gitbook/assets/add-apple-pay.png)

### Holen Sie sich Ihre Checkout.com-Schlüssel

1. Gehen Sie zu Ihrem **Checkout.com Hub-Konto** und gehen Sie zu **Einstellungen > Kanäle**.
2. Erstellen Sie bei Bedarf einen neuen Kanal.
3. Greifen Sie auf Ihren Kanal zu. Im Abschnitt **API-Schlüssel** können Sie den **Geheimen Schlüssel** und den **Öffentlichen Schlüssel** kopieren.

![Checkout.com Channel API Keys](../.gitbook/assets/apikeys.png)

### Aktualisieren Sie die Zahlungsmethodeneinstellungen

Als Nächstes müssen Sie die Details der Zahlungsmethode Apple Pay (Checkout.com) aktualisieren. Konkret benötigen wir folgende Felder:

| Einstellungsoption | Beschreibung |
| ------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Geheimer Schlüssel zur Kasse** | Der geheime Schlüssel von Checkout.com |
| **Öffentlicher Schlüssel zur Kasse** | Der öffentliche Schlüssel von Checkout.com |
| **Apple Pay-Händler-ID** | Die Kennung Ihres Apple-Händlers, zum Beispiel **merchant.com.mystore.produktion**.                                                                                                   |
| **Name des Apple Pay-Händlers** | Die Beschreibung Ihres Apple-Händlers finden Sie auf der Händlerseite |
| **Apple Pay Merchant Domain** | Der Domainname, den Sie bei Apple Merchant registriert haben. Sie sollten die Präfixe `https://` und `www.` löschen. Geben Sie beispielsweise `example.com` statt `https://example.com` | ein
| **Apple Pay Merchant Domain Association** | Kopieren Sie den Inhalt der `apple-developer-merchantid-domain-association.txt`-Datei und geben Sie ihn hier ein.                                                                                            |
| **Apple Pay-Händleridentitätszertifikat** | Kopieren Sie den Inhalt der `.pem`-Datei, die Sie in den obigen Schritten erhalten haben.                                                                                                                            |
| **Privater Schlüssel für Apple Pay Merchant Identity** | Kopieren Sie den Inhalt der `.key`-Datei, die Sie in den obigen Schritten erhalten haben.                                                                                                                            |

Klicken Sie auf **Speichern**, um die Einstellungen zu aktualisieren.

### Überprüfen Sie die Domäne

Gehen Sie zurück zu Ihrer Händlerseite in Ihrem **Apple Developer-Konto**. In den Abschnitten **Händlerdomains** sollten Sie sehen, dass sich Ihre Domain derzeit im Status **Ausstehend** befindet. Klicken Sie auf **Verifizieren**. Der Status Ihrer Domain sollte jetzt **Verifiziert** lauten.

## Fehlerbehebung

### Es können keine Änderungen an Apple Pay Merchant vorgenommen werden

![](../.gitbook/assets/warning.png)

Wenn Sie die Warnung zu den Web-Händler-Geschäftsbedingungen der Apple Pay Platform wie im obigen Bild erhalten. Bitten Sie den Inhaber Ihres Apple Developer-Kontos, die Händlerseite zu besuchen, auf den Link in der Warnung zu klicken und die Bedingungen zu akzeptieren. Andernfalls können Sie keine Änderungen am Händler vornehmen, wie z. B. das Hinzufügen von Domains oder das Generieren von Zertifikaten.

### Die Zahlungen können nicht abgeschlossen werden

Sollten Sie bei der Verarbeitung der Zahlungen Fehler erhalten, prüfen Sie bitte noch einmal das Apple Pay-Zertifikat. Sie können versuchen, neue Zertifikate zu generieren und Ihre Zahlungseinstellungen entsprechend zu aktualisieren. Sollte das Problem nach der Änderung der Zertifikate weiterhin bestehen, kontaktieren Sie uns bitte für weitere Unterstützung.
