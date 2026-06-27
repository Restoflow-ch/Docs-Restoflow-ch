---
description: >-
  In diesem Abschnitt erfahren Sie Schritt für Schritt, wie Sie eine einrichten
  Bluetooth-Drucker.
---

# Drucken mit Bluetooth-Drucker einrichten

{% embed url="https://drive.google.com/file/d/1Px4Sn_7b-ftCAfR7CFe87y6WE5F8SAEQ/view?usp=sharing" %}

### Schritt 1: Erstellen Sie eine Druckerkonfiguration

1. Öffnen Sie Ihr [**Restoflow-Dashboard**](https://admin.restoflow.ch).
2. Gehen Sie zu **Einstellungen > Belegdruck > Drucker erstellen**.
3. Füllen Sie aus:
* **Druckername –** z. B. „Android Kitchen Printer“
* **Druckmethode:** Auf _ESCPOS_ einstellen
* **Drucktyp:** Verwenden Sie _ESCPOS Image_ für beste Ergebnisse. (Beachten Sie, dass einige ältere Drucker diese Methode möglicherweise nicht unterstützen und in diesen Fällen ESCPOS Text Only verwendet werden kann.)
* **Papierskalierungsfaktor:** Passen Sie den Wert auf **1,7** an, wenn der Text abgeschnitten ist.
4. Klicken Sie auf **„Speichern“** und kopieren Sie Ihren eindeutigen **API-Schlüssel** (wird später benötigt).

<figure><img src="../../.gitbook/assets/Screenshot 2025-11-30 at 4.24.51 AM.png" alt="" width="375"><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/Screenshot 2025-11-30 at 4.25.20 AM.png" alt="" width="276"><figcaption></figcaption></figure>

### **Schritt 2: PushPrinter auf Android installieren**

1. **Laden Sie PushPrinter** aus dem _Google Play Store_ herunter.
2. Öffnen Sie die App nach der Installation.
3. Drücken Sie auf das **Einstellungssymbol ⚙️** und wählen Sie dann **Standard**.

### **Schritt 3: Einen Drucker auf Android hinzufügen und konfigurieren**

1. Tippen Sie auf **„+“ (Drucker hinzufügen)**, um einen Druckdienst zu konfigurieren.
2. Wählen Sie **Bluetooth** oder **Netzwerk (für IP-Drucker)**:
* Wenn Sie **Bluetooth** verwenden, sucht die App automatisch nach verfügbaren Druckern.
* Stellen Sie sicher, dass Ihr Drucker eingeschaltet ist und sich im Kopplungsmodus befindet.
* Wählen Sie Ihren Drucker aus der Liste aus.
3. Geben Sie den **API-Schlüssel** aus Ihrem Restoflow-Dashboard ein. Den API-Schlüssel finden Sie in den Druckereinstellungen des Restaurants. (Einstellungen > Quittungsdruck)

<figure><img src="../../.gitbook/assets/Screenshot 2025-11-30 at 4.25.31 AM.png" alt="" width="375"><figcaption></figcaption></figure>

4. Geben Sie bei Aufforderung die Standarddrucker-PIN ein (**0000** oder **1234**).
5. Bestätigen Sie, dass der **Druckerstatus in Ihrem Restoflow-Dashboard „Verbunden“** ist.
6. Sobald alle Angaben ausgefüllt sind, überprüfen Sie den Status des Druckers in den Einstellungen Ihres Restaurants. Stellen Sie sicher, dass es als verbunden angezeigt wird.
7. Klicken Sie auf „Testdruck“. Wenn die Einrichtung erfolgreich war, wird ein Testdruck durchgeführt
8. Führen Sie bei Erfolg einen Bestelltest durch

* Gehen Sie zur Bestellseite und führen Sie eine Testbestellung durch
* Aktivieren Sie das automatische Drucken, um das automatische Drucken sicherzustellen





{% hint style="danger" %}
Bitte senden Sie eine E-Mail an [info@restoflow.ch](mailto:info@restoflow.ch) oder nutzen Sie die Chat-Support-Funktion, um Hilfe bei der Verwaltung dieser Funktion zu erhalten.
{% endhint %}
