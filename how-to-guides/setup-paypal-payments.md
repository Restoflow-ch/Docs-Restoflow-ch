---
description: >-
  Erfahren Sie bei uns, wie Sie Online-Zahlungen mit Ihrem eigenen PayPal-Konto akzeptieren
  einfacher Einrichtungsprozess
---

# PayPal-Zahlungen einrichten

PayPal ist eine der am weitesten verbreiteten Online-Zahlungsmethoden. Restoflow nutzt die REST-Express-Checkout-Zahlungsintegration von PayPal. Dadurch können wir Zahlungen in Ihrem Namen abwickeln, wobei die Gelder direkt auf Ihr Konto überwiesen werden. Bitte beachten Sie, dass PayPal nur in bestimmten Ländern und Währungen verfügbar ist. Sie können sie [hier](https://developer.paypal.com/docs/integration/direct/rest-api-payment-country-currency-support/) sehen.

{% hint style="danger" %}
Wir empfehlen dringend, für Online-Zahlungen Stripe anstelle von PayPal zu verwenden. Nach unserer Erfahrung kommt es bei PayPal gelegentlich zu verschiedenen Serviceproblemen. Sehen Sie sich stattdessen unten den Leitfaden für Stripe-Zahlungen an.
{% endhint %}

{% content-ref url="setup-stripe-payments.md" %}
[setup-stripe-zahlungen.md](setup-stripe-payments.md)
{% endcontent-ref %}

## So funktionieren PayPal-Zahlungen

Sobald PayPal aktiviert ist, steht den Kunden die Option während der Checkout-Phase ihrer Bestellung zur Verfügung. Nach der Auswahl können sie sich entweder bei ihrem PayPal-Konto anmelden, ein Konto erstellen oder ihre Kreditkarte verwenden und als Gast auschecken, um die Zahlung abzuschließen.

## Anforderungen

Um PayPal mit Restoflow nutzen zu können, benötigen Sie ein **vollständig gültiges Geschäftskonto**. Wenn Sie bereits über ein PayPal-Geschäftskonto verfügen, können Sie diesen Schritt überspringen.

Wenn Sie noch keins haben, melden Sie sich unter [https://www.paypal.com/webapps/mpp/account-selection](https://www.paypal.com/webapps/mpp/account-selection) an. Sie können Ihr Privatkonto auch in Ihren Kontoeinstellungen auf ein Geschäftskonto upgraden.

## Verbinden Ihres PayPal-Kontos

#### Erstellen Sie eine REST-API-Anwendung

1. Besuchen Sie [https://developer.paypal.com/developer/applications/](https://developer.paypal.com/developer/applications/)
2. Melden Sie sich über den Login-Button bei Ihrem PayPal-Konto an
3. Scrollen Sie nach der Anmeldung nach unten, bis Sie den Titel „REST API-Apps“ sehen.
4. Klicken Sie auf die Schaltfläche „App erstellen“.
5. Geben Sie Ihren Firmennamen als App-Namen ein und ignorieren Sie das Feld „Sandbox-Entwicklerkonto“.
6. Klicken Sie auf die Schaltfläche „App erstellen“, um diesen Schritt abzuschließen

![PayPal REST apps](https://storage.crisp.chat/users/helpdesk/website/e903fdb8557a9800/image_141scma.png)

#### Kopieren Sie die Anmeldeinformationen der Live-Anwendung

1. Nachdem Sie Ihre Bewerbung erstellt haben, gelangen Sie auf die Seite, auf der Sie Ihre Zugangsdaten kopieren können
2. Wechseln Sie über die Schaltflächen oben rechts von der „Sandbox“- in die „Live“-Ansicht
3. Scrollen Sie nach unten und klicken Sie auf „Anzeigen“ unter dem „Geheimnis“.
4. Sie können nun Ihre „Client-ID“ und „Geheim“-Schlüssel sehen
5. Gehen Sie in einem anderen Fenster zu Ihrem Restaurant-Dashboard und zu „Einstellungen > Zahlungen > PayPal“.
6. Aktivieren Sie PayPal-Zahlungen und geben Sie Ihre „Kunden-ID“ und Ihren „Geheimschlüssel“ aus dem PayPal-Dashboard ein
7. Wählen Sie Ihre Zahlungswährung und speichern Sie das Formular

![PayPal application credentials](https://storage.crisp.chat/users/helpdesk/website/e903fdb8557a9800/image_1g9uc8i.png)

## PayPal-Gebühren

Bitte beachten Sie, dass bei Verwendung von PayPal, wie auch bei anderen Online-Kreditkartenanbietern, für jede Transaktion eine Gebühr erhoben wird. Dies muss selbst über Ihr eigenes PayPal-Konto verwaltet werden, da wir hierfür nicht verantwortlich sind. Die Gebühren für Ihr jeweiliges Land und Ihre Währung können Sie auf der PayPal-Website einsehen.

## Rückerstattungen

Derzeit müssen Rückerstattungen manuell über Ihr PayPal-Konto bearbeitet werden.

\
<br>

{% hint style="danger" %}
Bitte senden Sie eine E-Mail an [info@restoflow.ch](mailto:info@restoflow.ch) oder nutzen Sie die Chat-Support-Funktion, um Hilfe bei der Verwaltung dieser Funktion zu erhalten.
{% endhint %}
