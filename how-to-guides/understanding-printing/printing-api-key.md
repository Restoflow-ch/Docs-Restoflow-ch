---
description: >-
  So richten Sie Ihren API-Schlüssel ein.  Dies dient der Anbindung Ihres Online-Drucks
  Konfiguration für Ihre PushPrinter-Anwendung und Ihren Belegdrucker.
---

# Drucken – API-Schlüssel

1\. Melden Sie sich bei Ihrem Restoflow-Konto unter [admin.restoflow.ch](https://admin.restoflow.ch/login?redirect=%2F) an und gehen Sie zu Einstellungen>System>Belegdruck>Drucker erstellen.

![](../../.gitbook/assets/1-create-printer.png)

2\. Benennen Sie den Drucker, idealerweise verwenden Sie denselben Namen wie die Einstellungen in PushPrinter, um Verwirrung zu vermeiden. Wir empfehlen außerdem, „Bestellungen automatisch drucken“ und „Buchungen automatisch drucken“ zu aktivieren.

![](<../../.gitbook/assets/untitled (2).png>)

3\. Wählen Sie nun „Druckereinstellungen“ und stellen Sie sicher, dass;

* „Druckmethode“ – ist auf ESCPOS eingestellt
* „ESCPOS-Drucktyp“ – ist auf „ESCPOS-Bild“ eingestellt.

{% hint style="warning" %}
**HINWEIS** – Falls Ihr Drucker keinen Bilddrucker unterstützt (nicht richtig oder sehr langsam druckt), ändern Sie dies bitte in „ESCPOS-Text nur“.
{% endhint %}

![](<../../.gitbook/assets/untitled-1 (2).png>)

4\. Scrollen Sie auf dem Bildschirm nach unten und klicken Sie auf die Schaltfläche „Speichern“.

5\. Markieren Sie dann den API-Schlüssel, klicken Sie mit der rechten Maustaste und kopieren Sie ihn in die Zwischenablage.

![](<../../.gitbook/assets/untitled-2 (3).png>)

6\. Fügen Sie den API-Schlüssel in das entsprechende API-Feld in PushPrinter ein.



Für weitere Unterstützung können Sie uns gerne [kontaktieren](https://restoflow.ch/contact).
