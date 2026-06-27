---
description: Anleitung zum Drucken mit einem Netzwerkdrucker
---

# Drucken – Windows-Netzwerkdruck

## **Netzwerkdruck**

1. Bitte gehen Sie zur Windows-Systemsteuerung

![](<../../.gitbook/assets/untitled (1).png>)

2\. Öffnen Sie Geräte und Drucker

![](../../.gitbook/assets/untitled-1.png)

3\. Klicken Sie mit der rechten Maustaste und wählen Sie „Druckereigenschaften“.

![](<../../.gitbook/assets/untitled-2 (5).png>)

4\. Wenn Ihr Drucker nicht angezeigt wird, verwenden Sie diese Anweisungen, um ihn einzurichten [Druckereinrichtung](printing-add-a-printer-to-windows.md).

5\. Um zu testen, ob der Drucker funktioniert, klicken Sie bitte auf Testseite drucken

![](<../../.gitbook/assets/untitled-3 (1).png>)

6\. Wenn die Testseite nicht gedruckt wird. Anschließend schließen Sie den Drucker bitte korrekt an und installieren ihn. Bitte lesen Sie: [Druckereinrichtung](https://www.notion.so/restoflowwiki/Printing-Add-a-printer-18689e4654fe4978b20aeb82b581d81e).

7\. Öffnen Sie die Programmanwendung PushPrinter für Windows

8\. Gehen Sie zum Zahnrad „Einstellungen“ und wählen Sie das Standardanbieterprofil aus der Dropdown-Liste aus.

![](<../../.gitbook/assets/untitled-4 (2).png>)

9\. Aktivieren Sie „PushPrinter automatisch starten“. (Dadurch kann die Anwendung automatisch gestartet werden, wenn Ihr Computer zurückgesetzt wird.)

10\. Drücken Sie die Druckertaste

![](../../.gitbook/assets/untitled-6.png)

11\. Erstellen Sie über die Schaltfläche „Drucker erstellen“ einen Drucker

![](<../../.gitbook/assets/untitled-7 (4).png>)

12\. Fügen Sie Einstellungen einschließlich API-Schlüssel vom gerade erstellten Drucker hinzu.

{% hint style="info" %}
**Für einen Netzwerkdrucker:**&#x20;

* Benennen Sie den Drucker.&#x20;
* API-Drucker hinzufügen (zu finden in den Druckereinstellungen des Shops),&#x20;
* Anzahl der Kopien festlegen&#x20;
* Fügen Sie die IP-Adresse des Druckers hinzu und stellen Sie den Port auf 9100 ein.
{% endhint %}

![](<../../.gitbook/assets/untitled-8 (3).png>)

{% hint style="danger" %}
**HINWEIS:**

**Druckername** – Dies ist der Name, den der Drucker in Restoflow anzeigt.

**API-Schlüssel** – Dieser muss aus den Druckereinstellungen in Restoflow kopiert werden.

**Anzahl der Kopien** – Hiermit wird bestimmt, wie viele Kopien gedruckt werden.

**Drucktyp** – Damit dies funktioniert, muss dieser auf Windows Shared Printer (ESCPOS) eingestellt sein.

**Windows-Freigabedruckername** – Dieser muss GENAU mit dem zuvor hinzugefügten Freigabedruckernamen übereinstimmen. Leer- und Sonderzeichen sollten Sie vermeiden.
{% endhint %}

13\. Testdruck

14\. Drucker erstellen

15\. Gehen Sie in Ihr Geschäft und geben Sie eine Testbestellung auf.



Für weitere Unterstützung können Sie uns gerne [kontaktieren](https://restoflow.ch/contact).
