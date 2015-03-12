=====================
LighttpdControl
=====================

Zusammenfassung
-----------------------

Lighttpd ist eine sichere, schnell, kompatibel ist, und sehr flexible Web-Server, der für Hochleistungsumgebungen optimiert wurde. Lighttpd, die schnell neu definiert Effizienz eines ptdeploy; wie es soll und für höchste Ansprüche Umgebungen optimiert. Mit einem geringen Speicherbedarf im Vergleich zu anderen Web-Server, ein effektives Management der CPU-Last, und umfassender Funktionsumfang lighttpd ist die perfekte Lösung für jeden Server, der Lastproblemen leidet. Dies ist geeignet, um mit Ubuntu und Cent-OS arbeiten.

Hilfe Befehl
----------------------

Hilfe wird die Information über lighttpd zuzugreifen. Zum schnellen Nachschlagen mit den Hilfebefehle in einer der Versionen von ptdeploy Sie können auch den Befehl Hilfe gebrauchen. Der Befehl help ist ein interner Befehl, und ist im ptdeploy Modul.

.. code-block:: bash
   
	ptdeploy lighttpdcontrol help


Der folgende Screenshot unterstützt den Anwender mit ptdeploy Knechtschaft.

.. code-block:: bash

 kevell@corp:/# ptdeploy LighttpdControl help
 ******************************


  This command is part of Default Modules and handles Lighttpd Server Control Functions.

  LighttpdControl, lighttpdcontrol, lighttpdctl

          - start
          Start the Lighttpd server
          example: ptdeploy lighttpdcontrol start
          example: ptdeploy lighttpdcontrol start --yes

          - stop
          Stop the Lighttpd server
          example: ptdeploy lighttpdcontrol stop
          example: ptdeploy lighttpdcontrol stop --yes

          - restart
          Restart the Lighttpd server
          example: ptdeploy lighttpdcontrol restart
          example: ptdeploy lighttpdcontrol restart --yes

          - reload
          Reloads the Lighttpd server configuration without restarting
          example: ptdeploy lighttpdcontrol reload
          example: ptdeploy lighttpdcontrol reload --yes

 ------------------------------
 End Help
 ******************************


Alternative Parameter
--------------------------------

Vorzugsweise unter Verwendung von Lighttpd kann der Benutzer die folgenden Optionen Anstrengung.

LighttpdControl, lighttpdcontrol, lighttpdctl.

Start
--------

Startoption verwendet, um den lighttpd-Server zu starten. Lighttpdcontrol ist eine interaktive Sitzung, die mit der Option ptdeploy Modul ausgeführt wird. Je nachdem, wie der Server ausgeführt wird, kann der Start-Befehl in einem Skript gespeichert werden, in der Linux-Registrierung.

Der Server kann mit einem einfachen Befehl mit der Option, um wieder eine Verbindung zum Server zu steuern, um weitere Optionen zu erhalten gestartet werden.

.. code-block:: bash
   
	ptdeploy lighttpdcontrol start

Nach der Eingabe des Befehls, erlaubt es dem Benutzer, die lighttpd-Server Funktion zu starten.

Stopp
-------

Dieser Anschlag Option verwendet, um den lighttpd Dienst zu beenden. Insbesondere Ubuntu Linux, ruft der Stopp-Befehl die lighttpd, einen Job, der auf dem System ausgeführt wird, stoppen. Es ist gleichbedeutend mit dem Befehl service Altestelle. Nachfolgend finden Sie eine vollständige Beschreibung der Stoppbefehl.

.. code-block:: bash
   
	ptdeploy lighttpdcontrol stop

Nach Eingang als dem oben genannten Befehl, wird der Dienst die Funktion.

Neustart
------------

Der Begriff bezieht sich auf einen Neustart des Betriebssystems vor einem Warmstart der lighttpd-Server alle Programme zu beenden. Neustart ist manchmal notwendig, von einem Fehler zu erholen, oder neu zu initialisieren Treiber oder Hardwarevorrichtungen. Ein Computerspeicherprogramm normalerweise einen Neustart mit dem folgenden einfachen Befehl auszuführen.

.. code-block:: bash
   
	ptdeploy lighttpdcontrol restart

Nach Eingang als dem oben genannten Befehl, starten der Dienst die lighttpd Service.


Neu Laden
------------

Reload bedeutet, die Dinge ändern sich. Die lighttpd erfährt eine Überarbeitung und eine Reinigung. Es erleichtert die Wiederverwendung von lighttpd und Dienstleistungen. Ohne den Prozess abtöten kann lighttpd neu zu laden. Der folgende Befehl assis der Benutzer neu zu laden. Zusammen mit dem Befehl, wenn der Benutzer den Einsatz ja .. Optionen ohne Fragen zu stellen automatisch kann es funktionieren.

.. code-block:: bash
   
	ptdeploy lighttpdcontrol reload


Vorteile
--------------

* Flexible virtuelles Hosting.
* Unterstützt alle Arten von Modulen.
* Geringes Gewicht (weniger als 1 MB).
* Nicht Groß- und Kleinschreibung.
* Der Benutzer kann nach ihrem Wunsch funktionieren.
* Die Kündigung ist möglich.
* Automatisierung möglich.

