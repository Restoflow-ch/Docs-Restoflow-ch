---
description: >-
  Vollständige Anleitung zum Hinzufügen eines Bluetooth-, WLAN- oder Netzwerkdruckers zu Android für
  Automatischer Auftragsdruck mit Restoflow.
---

# So richten Sie einen Drucker auf Android ein

Durch die Einrichtung eines **Druckers auf Android** können Restaurants, Cafés und Unternehmen **Bestellbelege automatisch** direkt von ihrem **Android-Gerät** ausdrucken. Unabhängig davon, ob Sie einen Bluetooth-, Wi-F&#x69;**- oder Netzwerkdrucker** verwenden, führt Sie diese Anleitung durch die Konfiguration der **Android-Druckeinstellungen** für eine reibungslose Auftragsabwicklung.

Mit Restoflow können Sie:\
✅ **Bestellungen automatisch drucken** mit einem Android-kompatiblen Belegdrucker.\
✅ **Verbinden Sie einen Drucker über **Bluetooth oder WLAN** mit Android.\
✅ **Drucken Sie von Android auf einen Netzwerkdrucker** mit einer festen IP-Adresse.\
✅ **Aktivieren Sie Cloud-Druck für Android**, um das Remote-Drucken zu vereinfachen.\
✅ **Richten Sie das automatische Drucken für Android ein**, um die Auftragsabwicklung zu optimieren.

Diese Anleitung hilft Ihnen, **einen Drucker zu Android hinzuzufügen**, **Android-Druckereinstellungen** zu konfigurieren und etwaige Druckprobleme zu beheben.

{% hint style="info" %}
Gerne richten wir Ihren Drucker auch aus der Ferne für Sie ein. Wir wissen, dass dieser Schritt viele Menschen zum Stolpern bringen kann, da jeder Drucker anders ist. Bitte [kontaktieren Sie uns](https://www.restoflow.ch) per Live-Chat, wenn Sie Hilfe benötigen.
{% endhint %}

### **Anforderungen**

Bevor Sie beginnen, stellen Sie sicher, dass Sie über Folgendes verfügen:

* **Ein Android-Gerät** (mit **Android 4.1 oder höher**)
* **Ein über Bluetooth oder ein Netzwerk verbundener ESC/POS-Drucker**
* Die **neueste Version von PushPrinter** ([_Hier herunterladen_](https://pushprinter.com/))

## Einrichtungsprozess

### Schritt 1: Erstellen Sie eine Druckerkonfiguration

1. Öffnen Sie Ihr [**Restoflow-Dashboard**](https://admin.restoflow.ch).
2. Gehen Sie zu **Einstellungen > Belegdruck > Drucker erstellen**.
3. Füllen Sie aus:
* **Druckername –** z. B. „Android Kitchen Printer“
* **Druckmethode:** Auf _ESCPOS_ einstellen
* **Drucktyp:** Verwenden Sie _ESCPOS Image_ für beste Ergebnisse. (Beachten Sie, dass einige ältere Drucker diese Methode möglicherweise nicht unterstützen und in diesen Fällen ESCPOS Text Only verwendet werden kann.)
* **Papierskalierungsfaktor:** Passen Sie den Wert auf **1,7** an, wenn der Text abgeschnitten ist.
4. Klicken Sie auf **„Speichern“** und kopieren Sie Ihren eindeutigen **API-Schlüssel** (wird später benötigt).

<figure><img src="../../.gitbook/assets/image (1) (2).png" alt=""><figcaption><p>Step 1, point 2</p></figcaption></figure>

![Printer Settings for Android](../../.gitbook/assets/printer-settings.png)

<figure><img src="../../.gitbook/assets/image (6).png" alt=""><figcaption><p>Image showing example API key from printer settings</p></figcaption></figure>

***

### **Schritt 2: PushPrinter auf Android installieren**

1. **Laden Sie PushPrinter** aus dem _Google Play Store_ herunter.
2. Öffnen Sie die App nach der Installation.
3. Drücken Sie auf das **Einstellungssymbol ⚙️** und wählen Sie dann **Standard**.

***

### **Schritt 3: Einen Drucker auf Android hinzufügen und konfigurieren**

1. Tippen Sie auf **„+“ (Drucker hinzufügen)**, um einen Druckdienst zu konfigurieren.
2. Wählen Sie **Bluetooth** oder **Netzwerk (für IP-Drucker)**:
* Wenn Sie **Bluetooth** verwenden, sucht die App automatisch nach verfügbaren Druckern.
* Stellen Sie sicher, dass Ihr Drucker eingeschaltet ist und sich im Kopplungsmodus befindet.
* Wählen Sie Ihren Drucker aus der Liste aus.
* Wenn Sie ein **Netzwerk (IP-Drucker)** verwenden, wählen Sie **„Netzwerk“** und **geben Sie die IP-Adresse des Druckers manuell ein**.
* Stellen Sie sicher, dass sich der Drucker und das Android-Gerät im selben WLAN-Netzwerk befinden.
3. Geben Sie den **API-Schlüssel** aus Ihrem Restoflow-Dashboard ein. Den API-Schlüssel finden Sie in den Druckereinstellungen des Restaurants. (Einstellungen > Quittungsdruck)
4. Geben Sie bei Aufforderung die Standarddrucker-PIN ein (**0000** oder **1234**).
5. Bestätigen Sie, dass der **Druckerstatus in Ihrem Restoflow-Dashboard „Verbunden“** ist.
6. Sobald alle Angaben ausgefüllt sind, überprüfen Sie den Status des Druckers in den Einstellungen Ihres Restaurants. Stellen Sie sicher, dass es als verbunden angezeigt wird.

<div align="left" data-full-width="true"><figure><img src="../../.gitbook/assets/push3.png" alt="" width="318"><figcaption><p>Drücken Sie oben auf das „+“-Zeichen, um einen Druckdienst zu konfigurieren. Stellen Sie sicher, dass der Drucker eingeschaltet ist.</p></figcaption></figure></div>

<div align="left"><figure><img src="../../.gitbook/assets/image (10).png" alt="" width="210"><figcaption><p>Koppeln Sie das Android-Gerät über Bluetooth mit dem Drucker</p></figcaption></figure></div>

<div align="left"><figure><img src="../../.gitbook/assets/image (11).png" alt="Android-test-print-on-pushprinter" width="204"><figcaption><p>Sobald die Verbindung erfolgreich hergestellt wurde, wird ein Testdruck an den Drucker gesendet.</p></figcaption></figure></div>

<div align="left"><figure><img src="../../.gitbook/assets/image (13).png" alt="" width="208"><figcaption><p>Geben Sie Druckerdetails wie Druckernamen, API-Schlüssel und Anzahl der Kopien ein.</p></figcaption></figure></div>

<div align="left"><figure><img src="../../.gitbook/assets/image (7) (1).png" alt="" width="375"><figcaption><p>Druckerstatus zeigt verbunden an</p></figcaption></figure></div>

***

### **Schritt 4: Testdruck**

1. Besuchen Sie die **Bestellseite** in Restoflow.
2. Wählen Sie eine Bestellung aus und wählen Sie dann **„Drucken“**.\
(Wir empfehlen, sowohl kurze als auch lange Bestellungen auszudrucken, um sicherzustellen, dass nichts vertikal ausgeschnitten wird.)
3. Wenn Sie **automatisches Drucken** aktiviert haben, geben Sie eine Testbestellung auf, um sicherzustellen, dass das automatische Drucken aktiviert ist.

![](<../../.gitbook/assets/image (5) (2).png>)

***

## Fehlerbehebung: Häufige Probleme und Korrekturen

{% hint style="success" %}
**Kontaktieren Sie uns**

Wir haben Hunderte von Druckern erfolgreich eingerichtet; Es besteht eine gute Chance, dass wir Ihnen viele Kopfschmerzen ersparen können. Zögern Sie also nicht, uns per Chat zu kontaktieren (https://www.restoflow.ch).
{% endhint %}

#### **1. Seiten der Quittung sind abgeschnitten**

✅ Stellen Sie den **Papierskalenfaktor** auf **1,7** ein und testen Sie es erneut.

#### **2. Ungültiger API-Schlüssel**

✅ Stellen Sie sicher, dass der **API-Schlüssel** mit dem in Ihren Restoflow-Druckereinstellungen übereinstimmt.

#### **3. Drucker ist angeschlossen, aber es werden keine Ausdrucke erstellt**

✅ Starten Sie das Android-Gerät neu und **stellen Sie sicher, dass Android den Drucker erkennt** in den Bluetooth- oder WLAN-Einstellungen.

#### **4. Der Druckvorgang konnte nicht authentifiziert werden**

✅ Überprüfen Sie Ihre **Internetverbindung** und versuchen Sie es später erneut. Versuchen Sie, Ihr Gerät neu zu starten. Versuchen Sie, mit anderen Computerprogrammen wie Ihrem Browser auf Ihrem Drucker zu drucken.

***

### **Warum Android-Druck für Bestellbelege verwenden?**

📌 **Schnell und zuverlässig:** Belege automatisch ausdrucken, sobald eine Bestellung aufgegeben wird.\
📌 **Funktioniert mit den meisten Druckern:** Unterstützt **ESC/POS-Thermodrucker, Bluetooth-Drucker, WLAN-Drucker und Netzwerkdrucker**.\
📌 **Einfache Einrichtung:** Keine komplizierten Treiber – konfigurieren, verbinden und drucken.\
📌 **Cloud-Druckunterstützung:** Drucken Sie von überall aus, wenn Sie einen **Netzwerkdrucker mit fester IP** verwenden.

{% hint style="info" %}
Starten Sie kostenlos unter [www.restoflow.ch/signup](https://www.restoflow.ch/signup/)
{% endhint %}



