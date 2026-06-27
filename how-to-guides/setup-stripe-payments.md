---
description: >-
  Erfahren Sie, wie Sie Stripe einrichten, unseren empfohlenen Online-Zahlungsanbieter
  Optimierte Einrichtung und Benutzererfahrung
---

# Stripe-Zahlungen einrichten

{% hint style="success" %}
Wir empfehlen jetzt die Verwendung von [stripe+-integrated-zahlungen.md](stripe+-integrated-payments.md "mention")
{% endhint %}

Sie können Kreditkarten online mit [Stripe](https://stripe.com/) akzeptieren. Es wird derzeit in zahlreichen Ländern mit verschiedenen Währungen unterstützt. Wenn Stripe in Ihrem Land nicht unterstützt wird, können Sie Stripe Atlas testen. Nachfolgend finden Sie unsere einfache Anleitung zur Einrichtung von Stripe und zur Verwaltung Ihres Kontos.

## So funktionieren Stripe-Zahlungen

Wenn Stripe aktiviert ist, können Kunden beim Bezahlen zwischen der Online-Zahlungsoption wählen. Wenn ein Kunde „Kreditkarte“ auswählt, wird unten das Feld „Kreditkarte“ angezeigt.

![Stripe payment example](https://storage.crisp.chat/users/helpdesk/website/e903fdb8557a9800/image_16wk7ks.png)

## Verbinden Ihres Stripe-Kontos

1. Erstellen Sie ein Konto auf der Stripe-Website, falls Sie noch keins haben
2. Stellen Sie sicher, dass Sie Ihr Live-Konto und nicht Ihr Testkonto sehen&#x20;
3. Melden Sie sich bei Ihrem Konto-Dashboard an. Gehen Sie in der linken Navigation zu „Entwickler > API-Schlüssel“.
4. Öffnen Sie als Nächstes Ihr Restaurant-Dashboard und navigieren Sie zu „Einstellungen > Zahlungen > Stripe“.
5. Aktivieren Sie Stripe-Zahlungen mit dem Schalter „Aktivieren“.
6. Kopieren Sie den „Publishable Key“ und den „Secret Key“ aus dem Stripe-Dashboard in das Restaurant-Dashboard
7. Legen Sie Ihre Zahlungswährung im Restaurant-Dashboard fest und speichern Sie die Einstellungen

![Stripe API keys](https://storage.crisp.chat/users/helpdesk/website/e903fdb8557a9800/image_4cpfy8.png)

## Zahlungen testen

Wenn Sie eine Testzahlung durchführen möchten, kopieren Sie Ihre Test-API-Schlüssel von Stripe. Sie können dies tun, indem Sie den Schalter „Testdaten anzeigen“ umschalten.

![Stripe test data](https://storage.crisp.chat/users/helpdesk/website/e903fdb8557a9800/image_1bjx53a.png)

Sobald dies erledigt ist, können Sie die Kreditkartennummer „4242 4242 4242 4242“ mit jedem gültigen Ablaufdatum, CVC und Postleitzahl verwenden. Mit dieser Karte können Sie eine Scheinzahlung durchführen.

## Validierung Ihres Stripe-Kontos

Um Online-Zahlungen an Ihre Bank abzuheben, müssen Sie sicherstellen, dass Ihr Stripe-Konto vollständig gültig ist. Bitte stellen Sie sicher, dass Sie alle erforderlichen Validierungen abgeschlossen haben.

## Stripe-Gebühren

Wir sind nicht für die Verwaltung oder Gebühren Ihres Stripe-Kontos verantwortlich. Ihr Stripe-Konto wird einfach mit Ihrem Restoflow-Konto verknüpft, um Gebühren in Ihrem Namen abzuwickeln und das Geld direkt auf Ihr Konto zu überweisen.

Daher ist es wichtig, dass Sie die Gebühren für die Zahlungsabwicklung von Stripe kennen. Mehr können Sie hier lesen [https://stripe.com/pricing](https://stripe.com/pricing). Bitte nehmen Sie sich auch die Zeit, die FAQ und den Support zu lesen, um etwaige Probleme zu klären.

## Stripe-Währungsumrechnungen

Mit Stripe können Sie je nach Land, in dem Sie sich befinden, online verschiedene Währungen akzeptieren. Wenn Ihre Stripe-Währung von der Währung Ihres Shops abweicht, rechnen wir den Bestellbetrag in Ihre Stripe-Standardwährung um und verwenden dabei Echtzeit-Wechselkurse für die Zahlung.

## Rückerstattungen ausstellen

Stripe-Rückerstattungen können über Ihr Bestellverwaltungs-Dashboard oder das Stripe-Dashboard verarbeitet werden. Im Bestellverwaltungs-Dashboard ist die Rückerstattungszahlungsoption im Popup-Fenster mit den Bestelldetails verfügbar. Drücken Sie einfach die Aktionsauswahlleiste und wählen Sie „Stripe-Zahlung erstatten“.





{% hint style="danger" %}
Bitte senden Sie eine E-Mail an [info@restoflow.ch](mailto:info@restoflow.ch) oder nutzen Sie die Chat-Support-Funktion, um Hilfe bei der Aktivierung dieser Funktion zu erhalten.
{% endhint %}
