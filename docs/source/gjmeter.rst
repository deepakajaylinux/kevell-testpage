=======
Jmeter
=======

Zusammenfassung
----------------------

Dieses Modul befasst sich mit der Installation der jmeter mit der aktualisierten Version. JMeter kann als Unit-Test-Tool für die JDBC-Datenbankverbindungen, FTP, LDAP, Web-Services, JMS, HTTP, generischen TCP-Verbindungen und OS Mutter Prozessen verwendet werden. Wir wollen sehen, wie dieses Modul hilft dem Anwender bei der Installation und Verwendung des Jmeter.

Hilfe Befehl
---------------------

Der Befehl help führt den Anwender über den Zweck und als auch über die Möglichkeiten, die in der Jmeter Modul enthalten sind. Es listet einige der alternativen Parameter jmeter Modul. Es beschreibt auch die Syntax für die Installation des jmeter Moduls. Der Befehl help für jmeter Modul wird wie unten dargestellt.

.. code-block:: bash

		cleopatra Jmeter help


Die Syntax für die Deklaration den Befehl help ist nicht case sensitive was ein zusätzlicher Vorteil ist. Der folgende Screenshot visualisieren Sie den Befehl help unter Jmeter.

.. code-block:: bash

 kevell@corp:/# cleopatra Jmeter help

 ******************************


  This command allows you to update Jmeter.

  Jmeter, jmeter

        - install
        Installs the latest version of Jmeter
        example: cleopatra jmeter install

 ------------------------------
 End Help
 ******************************

Installation
----------------

Der Befehl zum Installieren der jmeter im Benutzer Maschine verwendet wird unten dargestellt:

.. code-block:: bash

		cleopatra jmeter install

Nach der Eingabe des Befehls oben, passiert folgendes Verfahren im Tabellenformat angezeigt.

.. cssclass:: table-bordered


 +----------------------+-------------------------------------+--------------+----------------------------------------------+
 | Parameters           | Alternative Parameter               | Optionen     | Kommentare                                   |
 +======================+=====================================+==============+==============================================+
 |Install Jmeter? (Y/N) | anstelle von jmeter, wir verwenden  | Y(Yes)       | Wenn der Benutzer wünschen, den              |
 |                      | können, Jmeter also.                |              | Installationsprozess können sie als Eingangs |
 |                      |                                     |              | gehen Y.                                     |
 +----------------------+-------------------------------------+--------------+----------------------------------------------+
 |Install Jmeter? (Y/N) | anstelle von jmeter, wir verwenden  | N(No)        | Wenn der Benutzer wünschen, den              |
 |                      | können, Jmeter also.                |              | Installationsprozess können sie Eingabe als  |
 |                      |                                     |              | beendet N.|                                  |
 +----------------------+-------------------------------------+--------------+----------------------------------------------+


Wenn der Benutzer geht der Installation, während des Prozesses der Anlage wird in den folgenden Listen beschrieben:


* Baut die Abhängigkeitsstruktur.
* Liest den Status Informationen.
* Liste outs die Pakete, die automatisch installiert werden.
* Liste outs die neuen Pakete installieren.
* Details über die Anzahl der Dateien aktualisiert, neu installiert, entfernt und nicht aktualisiert.
* Liest die Paketliste und zeigt die Liste der Verpackung, die bereits installiert sind.


Der folgende Screenshot zeigt bildhaft die oben beschriebene Prozess der Installation.

.. code-block:: bash



Vorteile
------------

* Die in Hilfe und Installation verwendet muss nicht beachtet werden, welche ein zusätzlicher Vorteil ist, während im Vergleich zu anderen 
  Parametern.
* Es ist gut-to-do sowohl Ubuntu und sowie Cent OS.
* Dies wird Modul installiert die Jmeter in aktualisierte Version.
* Wenn das Modul bereits in der Benutzermaschine vorhandene es wird eine Meldung angezeigt werden, da sie bereits vorhanden sind.
* JMeter unterstützt variable Parametrierung, Behauptungen (Antwort Validierung), pro Thema Cookies, Konfigurationsvariablen und eine Vielzahl 
  von Berichte.
* Off-Site-Entwickler können leicht erweitern JMeter mit benutzerdefinierten Plugins.

