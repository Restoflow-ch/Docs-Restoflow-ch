---
description: >-
  Erfahren Sie, wie Sie Ihren eigenen benutzerdefinierten Domainnamen mit Ihrem Online-Shop verbinden
  besseres Branding und SEO
---

# Richten Sie eine benutzerdefinierte Domäne ein

## Einrichtungsprozess

1. Sehen Sie im Restaurant-Dashboard „Einstellungen &gt; Website &gt; Domains &gt; Benutzerdefinierte Domain“.
2. Geben Sie Ihren Domainnamen ein und klicken Sie auf Speichern
3. Gehen Sie zu Ihrem Domain-Verwaltungsbereich, in dem Sie Ihre Domain registriert haben
4. Greifen Sie auf Ihre DNS-Einträge zu und fügen Sie die unten aufgeführten DNS-Einträge hinzu
5. Warten Sie nach dem Hinzufügen der DNS-Einträge 10 Minuten, bis sie wirksam werden
6. Klicken Sie dann unter Ihren benutzerdefinierten Domain-Einstellungen auf die Schaltfläche „SSL-Zertifikat generieren“.

Wenn Ihre DNS-Einstellungen wirksam wurden, wird angezeigt, dass das SSL-Zertifikat erfolgreich generiert wurde. Nach der Erstellung ist Ihre Website über Ihren benutzerdefinierten Domainnamen zugänglich. Wenn Sie das Zertifikat nicht generieren können, warten Sie länger, bis Ihre DNS-Einstellungen wirksam werden.

## DNS-Eintrag zum Hinzufügen

| Datensatztyp | Gastgeber | Wert |
| :--- | :--- | :--- |
| Ein Rekord | www / bestellen / irgendetwas | 35.238.2 .132 |

{% hint style="info" %}
Der Hostwert ist die Subdomain Ihrer Domain, die Ihr Kunde besuchen muss, um auf die Website zuzugreifen. Wenn der Hostwert „order“ lautet und Ihre Domain „business.com“ lautet, lautet Ihre Shop-URL „order.business.com“.
{% endhint %}

{% hint style="warning" %}
**Wenn Sie „www“ als Hostwert verwenden, fügen Sie bitte auch den folgenden Eintrag hinzu**
{% endhint %}

| Datensatztyp | Gastgeber | Wert |
| :--- | :--- | :--- |
| Ein Rekord | @ / leer | 35.238.2 .132 |

Wenn Sie dies festlegen, wird sichergestellt, dass jemand, der Ihre Stammdomäne, z. B. example.com, eingibt, zu www.example.com weitergeleitet wird

