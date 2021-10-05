# M306-Services
---
---

Inhaltsverzeichnis:
-------------------

**1.1. Autoren, Versionierung des Dokumentes**
---
- Autoren: Léon Rezek, Noah Lennemann
- E-Mail: leon.rezek@edu.tbz.ch, noah.lennemann@edu.tbz.ch
- Version: 1.3
---
**1.2. Einführung**
---
   - _**Beschreibung: Welche Funktionen wird der Service erfüllen?**_
---
   - Webmin ist ein Verwaltungstool, um aus der Ferne oder im eigenen Netz mit Hilfe eines Webbrowsers auf verschiedene Server-Prozesse zugriff zu erhalten, die auf einem Unix Rechner laufen. Dazu zählt Hardware sowie Network traffic und Funktionen, um zumbeispiel ein AD-Server oder DHCP zu betreiben.


![grafik](https://user-images.githubusercontent.com/89446419/134141687-fdfecd0b-99fe-498c-a261-ffb6c0af3c83.png)

--- 
   - _**Vorgesehener Zeitaufwand für die Realisierung?**_
---
Die Umsetzung dauert etwa 30 Minuten. 

---
   - _**Stolpersteine?**_
---
Mögliche Stolpersteine können bei der Version des Webmins vorkommen. Allenfalls wurde das GUI verändert, oder Funktionen wurden entfernt/verändert. 
    
    

---
**1.3. Benötigte Hard- und Software**
   - Hardware 

1 x Raspberry PI mindestens PI 4 <br>
1 x Monitor (ist einfacher als verschiedene Viewer bsp. VNC) <br>
1 x SD Karte 8 GB <br>
1 x Netzwerkkabel ca. 1 Meter <br>

---
   - Software 
	
1 x Webmin Version 1.881 <br>
1 x Putty oder VNC Viewer

---
**1.4. Installationsanleitung (Didaktisch reduzierte Anleitung. Lernende sollen eine
     eigene Lösungswege realisieren)**
---

**1. Geben Sie den folgenden Command in die Kommandozeile ein, um die Minimale Version auf Sourge-Forge herunterzuladen und zu installieren:**

![grafik](https://user-images.githubusercontent.com/89446419/135976542-15868acf-0729-4833-9636-141dc78255d3.png)

_Tipp: Falls sie mit diesem Befehl die ausgewählte Version nicht installieren können, haben Sie vielleicht keine Berrechtigung.
Finden Sie heraus wie man mit hilfe eines Befehls, höhere Rechte erhaltet._

Hier finden Sie die einzelnen Versionen:
https://sourceforge.net/projects/webadmin/files/webmin

---

**2. Installation von der minimalen Version.**
![grafik](https://user-images.githubusercontent.com/89446419/135974406-dd5159d5-a97d-4ee2-9f0f-3bb685cc5e0c.png)

Beachten Sie, dass Sie die neuste Version von Webmin nehmen. Indiesem Fall installierten wir die Version 1.881

---
	
**3. Entpacken Sie den installierten Ordner mit Hilfe von Befehl :**
![grafik](https://user-images.githubusercontent.com/89446419/135974445-28d2e969-4645-418f-b13b-3876f8fa2f1c.png)

---
	
**4. Jetzt können sie in das entsprechende Verzeichnis gehen und folgenden Befehl eingeben:**
![grafik](https://user-images.githubusercontent.com/89446419/135974459-30d705f6-8682-4b04-bd7e-3a6fbdcbe514.png)

---
	
**5. Nun sollte folgendes Fenster erscheinen. Danach können sie alles mit der Enter Taste auf Default lassen und am Schluss einen Benutzer mit Passwort 	erstellen**

![grafik](https://user-images.githubusercontent.com/89446419/135974496-805dd2df-d60c-4bc7-b091-bdf156cf5c13.png)
![grafik](https://user-images.githubusercontent.com/89446419/135974526-526295be-cd72-403c-a94f-611e0bb271b5.png)

---
	
**6. Nach der Installation können sie mithilfe des Browsers über die IP-Adresse des Raspberry Pi's auf das Webinterface zugreifen:**
![grafik](https://user-images.githubusercontent.com/89446419/135974550-bd347cea-9ea6-4cc1-98de-18594b0a2e8b.png)

_Die (IP-Adresse):10000_

---
	
**7. Nach der eingabe der IP-Adresse und dem Port: 10000 können sie sich mit dem gesetzten Benutzername und Passwort anmelden**
![grafik](https://user-images.githubusercontent.com/89446419/135974583-a51d3b77-fecc-48e6-87fa-0b418976e6ec.png)

---

**8. Nun haben Sie jetzt die Möglichkeit, neue Module zu installieren oder das System zu verwalten.**

_Tipp: Informieren Sie sich über die Module die für Ihr System sinnvoll sind unter dem Folgendem Link: https://www.webmin.com/standard.html_

![grafik](https://user-images.githubusercontent.com/89446419/135974600-a3b8ece5-b61c-4608-bb98-8ecaf8c26524.png)

---
**1.5. Qualitätskontrolle (Prüfen der Funktionalität mit Ablauf von Kommandos
	und entsprechenden Outputs)**

Nach der Installation der beiden Perl libraries sollte folgenden Output erscheinen, der den Status der Installation anzeigt:

![grafik](https://user-images.githubusercontent.com/89446419/135980857-c84ce78b-b1b0-4a0a-ab3f-2671f8e62502.png)

Testen Sie zudem folgende Commands, um den webminstatus zu überprüfen:

Abfrage des Status von Webmin: sudo service webmin status

Webmin starten: sudo /etc/webmin/start

Webmin stoppen: sudo service webmin stop

Webmin neustarten: sudo service webmin restart

---

**1.6. Error-Handling**

---

**1.7. Quellenverzeichnis**

Webmin Logo: https://user-images.githubusercontent.com/89446419/134141687-fdfecd0b-99fe-498c-a261-ffb6c0af3c83.png

Webmin Software: http://prdownloads.sourceforge.net/webadmin/webmin-1.881-minimal.tar.gz

VNC Viewer: https://www.realvnc.com/de/connect/download/viewer/

Putty: https://www.putty.org/

---

**1.8. OpenSource Lizenz**
- - -
<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/3.0/ch/"><img alt="Creative Commons Lizenzvertrag" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/3.0/ch/88x31.png" /></a><br />Dieses Werk ist lizenziert unter einer <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/3.0/ch/">Creative Commons Namensnennung - Nicht-kommerziell - Weitergabe unter gleichen Bedingungen 3.0 Schweiz Lizenz</a>

 

- - -
