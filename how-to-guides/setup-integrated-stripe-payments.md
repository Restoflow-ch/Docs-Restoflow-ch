---
description: >-
  Erfahren Sie, wie Sie Stripe+-Zahlungen einrichten.  Dies ist unsere empfohlene Lösung für
  Online-Zahlungen aufgrund ihrer optimierten Einrichtung, Benutzererfahrung und Selbstbedienung
  Serviceoptionen in unserem Dashboard.
---

# Richten Sie integrierte Stripe-Zahlungen ein

### Schritte zum Einrichten von Stripe+-Zahlungen:

1. **Anmelden:** Greifen Sie auf Ihr Admin-Dashboard unter [admin.restoflow.ch](https://admin.restoflow.ch) zu.
2. **Navigieren Sie zu Einstellungen:** Gehen Sie zu **Einstellungen > Zahlungen > Zahlungsmethode hinzufügen > Stripe > Methode hinzufügen**.

<figure><img src="../.gitbook/assets/Settings-payments-Stripe.png" alt=""><figcaption><p>Settings > Payments > Add Payment Method > Stripe > Add Method</p></figcaption></figure>

#### Empfohlene Mindesteinstellungen für Stripe:

| Einstellung | Empfehlung | Notizen |
| ------------------------------ | --------------------------- | --------------------------------------------------------------------------------------------------- |
| **Aktiviert** | Auf | Aktiviert die Funktion |
| **Stripe-Geheimschlüssel** | sk\_live |                                                                                                     |
| **Veröffentlichbarer Stripe-Schlüssel** | pk\_live |                                                                                                     |
| **Währung** | AUD – Australischer Dollar – $ | Verwenden Sie Ihre lokale Währung |
| **E-Mail-Empfang deaktivieren** |                             |                                                                                                     |
| **Benutzerdefiniertes Zahlungsformular aktivieren** |                             |                                                                                                     |
| **Layout** | Themen |                                                                                                     |
| **Dienstleistungen** | Etikett | Bezahlen - Online |
| **Lieferetikett** | Etikett drucken | _BEZAHLT - ONLINE_ |
| **Maximaler Bestellwert ($)** | 999 | Legen Sie eine realistische maximale Online-Bestellsumme fest |
| **Mindestbestellwert ($)** | 2 | Die Mindesttransaktion sollte nicht weniger als 2 $ betragen
| **SC-Konto-ID** | ERHALTEN SIE DIESES VOM SUPPORT | Beispielformat – acct\_1A3abABCABCac1aA. Kontaktieren Sie den Chat-/E-Mail-Support, um Ihre SC-Konto-ID zu aktivieren. |

3. **Einstellungen speichern:** Drücken Sie **Speichern**, um die Einstellungen zu übernehmen.
4. **Testen Sie Ihr Setup:** Starten Sie Ihren Shop und geben Sie eine Live-Testbestellung mit Ihrer Karte, Google Pay oder Apple Pay auf.
5. **Unterstützung erhalten:** Bei Problemen oder zur Aktivierung Ihrer SC-Konto-ID senden Sie bitte eine E-Mail an [info@restoflow.ch](mailto:info@restoflow.ch) oder nutzen Sie die Chat-Support-Funktion.<br>







{% hint style="danger" %}
Bitte senden Sie eine E-Mail an [info@restoflow.ch](mailto:info@restoflow.ch) oder nutzen Sie die Chat-Support-Funktion, um Hilfe bei der Aktivierung dieser Funktion zu erhalten.
{% endhint %}

### Sie haben kein Restoflow-Konto?

Besuchen Sie [www.restoflow.ch](https://www.restoflow.ch) und klicken Sie oben rechts auf die Schaltfläche **Anmelden**, um Ihr Konto zu erstellen.

{% content-ref url="using-stripe-integrated.md" %}
[using-stripe-integrated.md](using-stripe-integrated.md)
{% endcontent-ref %}
