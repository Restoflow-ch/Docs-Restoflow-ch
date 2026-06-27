---
description: >-
  Erfahren Sie mit unserem, wie Sie den Auftragsdruck für Windows-Geräte einrichten und konfigurieren
  Drucksoftware
---

# Drucken für Windows einrichten

Unser System ermöglicht Ihnen den manuellen und automatischen Ausdruck neuer Bestellungen. In dieser Anleitung erfahren Sie, wie Sie den Auftragsdruck einrichten und Probleme beheben.

|| Gerne richten wir Ihren Drucker auch aus der Ferne für Sie ein. Wir wissen, dass dies ein Schritt ist, der viele Leute zum Stolpern bringen kann, da jeder Drucker ein bisschen anders ist. Bitte kontaktieren Sie uns, wenn Sie Hilfe benötigen

Für Schritt-für-Schritt-Anleitungen nach Druckmethode.  Bitte verwenden Sie die folgenden Anweisungen.  Es ist erwähnenswert, dass wir für die meisten Situationen die Verwendung der Windows Shared Printing-Methode empfehlen;

{% content-ref url="understanding-printing/printing-api-key.md" %}
[printing-api-key.md](understanding-printing/printing-api-key.md)
{% endcontent-ref %}

{% content-ref url="understanding-printing/printing-windows-shared-printing.md" %}
[printing-windows-shared-printing.md](understanding-printing/printing-windows-shared-printing.md)
{% endcontent-ref %}

{% content-ref url="understanding-printing/printing-windows-network-printing.md" %}
[printing-windows-network-printing.md](understanding-printing/printing-windows-network-printing.md)
{% endcontent-ref %}

## Anforderungen

* Windows 7/8/10 entweder 32-Bit oder 64-Bit
* Ein Windows-kompatibler Drucker mit installierten Treibern
* Neueste Version von PushPrinter, die [hier] heruntergeladen werden kann (https://pushprinter.com/#windows)

## Einrichtungsprozess

### Überprüfen Sie, ob die Druckertreiber installiert sind und funktionieren

1. Wenn Ihre Treiber erfolgreich installiert wurden, wird Ihr Drucker auf Ihrem PC unter „Systemsteuerung > Hardware und Sound > Geräte und Drucker“ angezeigt.
2. Klicken Sie mit der rechten Maustaste auf Ihren Drucker und wählen Sie „Eigenschaften“
3. Klicken Sie unten links auf „Testseite drucken“.&#x20;
4. Überprüfen Sie, ob die Testseite erfolgreich gedruckt wurde

Wenn dies erfolgreich ist, funktioniert Ihr Drucker einwandfrei. Wenn Sie Ihren Drucker nicht finden können oder er nicht funktioniert, installieren Sie den Treiber erneut.

### Beachten Sie die verfügbaren Papierformate

Dieser Schritt ist bei allen Druckern etwas anders. Einige Drucker verfügen über ein eigenes Konfigurationstool, mit dem Sie die verfügbaren Papierformate anzeigen können.

Standardmäßig finden Sie diese Informationen möglicherweise im Dialogfeld „Eigenschaften“ Ihres Druckers, wie im vorherigen Schritt beschrieben. Manchmal finden Sie dies unter der Registerkarte „Geräteeinstellungen“ in Ihren Druckereigenschaften.

In anderen Fällen können Sie unten im Popup-Fenster mit den Druckereigenschaften „Einstellungen“ und dann unten erneut „Erweitert“ auswählen

Sehen Sie sich das Bild unten an, um zu sehen, wie dies aussehen könnte.

![Printer paper size settings](https://storage.crisp.chat/users/helpdesk/website/e903fdb8557a9800/image_1vcnqy8.png)

Beachten Sie die verfügbaren Papierformate, da Sie wahrscheinlich einige ausprobieren müssen, damit es einwandfrei funktioniert

### Erstellen Sie eine Druckerkonfiguration

1. Besuchen Sie Ihr Restaurant-Dashboard und navigieren Sie zu „Einstellungen > Belegdruck“.
2. Klicken Sie auf die Schaltfläche „Neuer Drucker“ und füllen Sie alle erforderlichen Optionen aus
3. Stellen Sie auf der Registerkarte „Papiereinstellungen“ Ihre Papierbreite und Papierhöhe entsprechend dem größten verfügbaren Papierformat für Ihren Drucker ein, wie im vorherigen Schritt beschrieben. Ausgehend vom Bild oben würden wir eine Breite von „72“ und eine Höhe von „210“ eingeben.
4. Wir empfehlen dringend, mit einer Schriftgröße von „18“ und einem Papierrand von „0“ zu beginnen.
5. Erstellen Sie die Druckkonfiguration. Nach der Erstellung erhalten Sie einen eindeutigen API-Schlüssel, mit dem Sie eine Verbindung herstellen können. Lassen Sie diesen Bildschirm geöffnet, da Sie Ihren API-Schlüssel bald kopieren müssen

![Printer API key](https://storage.crisp.chat/users/helpdesk/website/e903fdb8557a9800/image_bnxer6.png)

|| Die in Ihrer Druckerkonfiguration eingegebenen Papierformate müssen mit Ihren Windows-Papierformateinstellungen übereinstimmen, die in den Druckertreiberoptionen festgelegt sind. Wenn der Ausdruck falsch oder schief ist, müssen Sie die anderen Größen vom größten zum kleinsten testen. Wenn Sie die Größen in der Druckerkonfiguration ändern, stellen Sie sicher, dass Sie diese auch in den Windows-Druckertreibereinstellungen ändern.

### PushPrinter installieren

1. Laden Sie PushPrinter über den folgenden [Link] herunter (https://www.pushprinter.com)
2. Führen Sie das Installationsprogramm aus. Sie erhalten eine Warnung, dass die Anwendung nicht überprüft wurde. Fahren Sie mit der Installation fort
3. Nach erfolgreicher Installation wird PushPrinter automatisch geöffnet

### PushPrinter konfigurieren

1. Das erste, was Sie wahrscheinlich tun möchten, ist, den „Auto Start“-Schalter umzuschalten, damit er eine Verbindung herstellt und startet, wenn Ihr PC gestartet wird.  Aktivieren Sie dies, indem Sie das Zahnrad „Einstellungen“ auswählen und die Schaltfläche „PushPrinter automatisch starten“ aktivieren (Bild 1.1).
2. Klicken Sie oben auf die Registerkarte „Druckersymbol“, um einen Druckdienst zu konfigurieren
3. Klicken Sie auf die Schaltfläche „Drucker erstellen“ (Bild 1.2).
4. Kopieren Sie den API-Schlüssel für den Drucker, den Sie vor zwei Schritten erstellt haben, und fügen Sie ihn ein
5. Legen Sie die Anzahl der zu druckenden Kopien fest und wählen Sie Ihren Drucker aus
6. Drücken Sie die Starttaste und stellen Sie sicher, dass unten „Verbunden“ steht

![Image 1.1 - 'Automatically start PushPrinter' button](../.gitbook/assets/pushprinter-settings.png)

![Image 1.2 - 'Create Printer'](../.gitbook/assets/create-printer-pushprinter.png)

### Testdruck

Besuchen Sie Ihre Bestellseite. Wählen Sie eine Bestellung aus und wählen Sie unter der Aktionsauswahlleiste „Drucken“ aus. Wir empfehlen, sowohl kurze als auch lange Bestellungen auszudrucken, um sicherzustellen, dass nichts vertikal ausgeschnitten wird. Wenn Sie das automatische Drucken für diese Druckkonfiguration aktiviert haben, geben Sie eine Bestellung auf und testen Sie das automatische Drucken

## Fehlerbehebung

#### Kontaktieren Sie uns

Wir haben Hunderte von Druckern erfolgreich eingerichtet. Es besteht eine gute Chance, dass wir Ihnen viele Kopfschmerzen ersparen können. Zögern Sie also nicht, uns zu kontaktieren.

#### Seiten werden abgeschnitten

Reduzieren Sie zunächst entweder Ihre Rand- oder Papierbreitenwerte unter Ihrer Druckerkonfiguration in Ihrem Admin-Dashboard. Sie werden schließlich eine geeignete Breite und einen geeigneten Rand kalibrieren. Sie können die Schriftgröße auch etwas kleiner anpassen. Sie können die richtige Papierbreite in Ihren Windows-Druckereinstellungen ermitteln, wie in der Anleitung oben gezeigt.

#### Das Ende des Kassenbons kommt nicht vollständig heraus

Unter Ihren Windows-Druckereinstellungen. Stellen Sie die Option „Zeile nach dem Drucken einziehen“ auf einen hohen Wert ein, damit der Drucker einige zusätzliche Zeilen durchziehen kann.

#### Ungültiger API-Schlüssel

Der von Ihnen eingegebene API-Schlüssel hat keinen Einfluss auf Ihre Druckkonfigurationen. Überprüfen Sie Ihren API-Schlüssel noch einmal

#### Authentifizierung konnte nicht durchgeführt werden

Überprüfen Sie Ihre Internetverbindung oder versuchen Sie es in Kürze noch einmal

#### Drucker wird in Windows nicht erkannt

Sie müssen den richtigen Treiber für Ihren Drucker finden, sofern dieser für Windows verfügbar ist. Versuchen Sie, den Namen Ihres Druckers zu googeln, gefolgt von den Worten „Windows-Treiber {fügen Sie Ihre Windows-Version ein}“.

#### Das Drucken funktioniert nicht, obwohl alles richtig eingerichtet ist

Bitte stellen Sie sicher, dass Windows Ihren Drucker erkennt. Versuchen Sie, Ihren Drucker oder PC neu zu starten. Versuchen Sie, aus anderen Programmen auf Ihrem PC, beispielsweise Ihrem Browser, auf Ihrem Drucker zu drucken.



{% hint style="info" %}
Starten Sie kostenlos unter [www.restoflow.ch/signup](https://www.restoflow.ch/signup/)
{% endhint %}

