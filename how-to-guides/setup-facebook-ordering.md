---
description: >-
  Durch die Aktivierung der Facebook-Bestellung können Ihre Kunden bei Ihnen bestellen
  Facebook-Seite.
---

# Facebook-Bestellung einrichten

{% hint style="danger" %}
So großartig diese Funktion auch klingt, für die Leute ist es ehrlich gesagt nicht sehr angenehm, über Facebook zu bestellen. Diese Registerkarten sind außerdem nur in Desktop-Versionen von Facebook verfügbar, was sie noch weiter einschränkt. Das bedeutet, dass es für Benutzer auf ihren Mobiltelefonen nicht funktioniert. Facebook führt auch regelmäßig Updates durch und manchmal geht etwas unerwartet kaputt. Daher raten wir insgesamt davon ab, diese Funktion zu verwenden. Eine weitaus zuverlässigere Option ist die einfache Weiterleitung von Personen zu Ihrer Bestelldomäne.
{% endhint %}

Besuchen Sie [https://developers.facebook.com](https://developers.facebook.com). Wenn Sie noch nicht bei Facebook angemeldet sind, können Sie sich mit Ihrem regulären Facebook-Konto anmelden.

Wenn Sie fertig sind, klicken Sie oben rechts auf die Schaltfläche „Meine Apps“ und wählen Sie „Neue App erstellen“.

![](https://storage.crisp.chat/users/helpdesk/website/e903fdb8557a9800/image\_f92n5y.png)

Geben Sie Ihren Firmennamen für Ihren App-Namen zusammen mit Ihrer E-Mail-Adresse ein und klicken Sie auf „Erstellen“.

Nach dem Erstellen der App gelangen Sie zum App-Dashboard. Gehen Sie im linken Menü zu „Einstellungen > Allgemein“

![](https://storage.crisp.chat/users/helpdesk/website/e903fdb8557a9800/image\_wtsxiz.png)

Wählen Sie „Seitenregisterkarte“. Sie müssen nun Ihre Shop-URL unter „URL des sicheren Seiten-Tabs“ und unter „Name des Seiten-Tabs“ eingeben, wie Sie Ihren Seiten-Tab nennen möchten. Ihre Shop-URL kann entweder Ihre Restoflow-Subdomain wie „[https://yourdomain.restoflow.ch](https://yourdomain.restoflow.ch)“ oder Ihr benutzerdefinierter Domainname sein, falls eingerichtet

![](https://storage.crisp.chat/users/helpdesk/website/e903fdb8557a9800/image\_cb565a.png)

Um den Seiten-Tab zu Ihrer Facebook-Seite hinzuzufügen, benötigen Sie Ihre Facebook-App-ID, die Sie auf dem vorherigen Foto oben auf der Seite orange hervorgehoben sehen

Als Nächstes müssen Sie die folgende URL in Ihrem Browser aufrufen und diese durch Ihre Facebook-App-ID und die zuvor eingegebene Store-URL ersetzen

[https://www.facebook.com/dialog/pagetab?app\_id=\{{YOUR\_APP\_ID\}}\&redirect\_uri=\{{IHR\_STORE\_URL\}}](https://www.facebook.com/dialog/pagetab?app\_id=\{{YOUR\_APP\_ID\}}\&redirect\_uri=\{{YOUR\_STORE\_URL\}})

Wenn Sie es richtig gemacht haben, wird auf Facebook eine Seite mit der Aufschrift „Seiten-Tab hinzufügen“ angezeigt und Sie können eine Ihrer Facebook-Seiten auswählen

Wenn Sie es richtig gemacht haben, wird auf Facebook eine Seite mit der Aufschrift „Seiten-Tab hinzufügen“ angezeigt und Sie können eine Ihrer Facebook-Seiten auswählen
