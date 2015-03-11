================
Apache Control
================

Zusammenfassung
-----------------------

Dieses Modul ist eine der Standardmodule , die bei der Handhabung der Kontrollfunktionen des Apache-Server soll. Es ermöglicht und erleichtert die erforderlichen Steuerfunktionen , die in der Apache-Server ausgeführt werden sollen. Lassen Sie uns sehen, die Arbeits- und Zweck der Steuerfunktionen und wie diese im Umgang mit diesen Steuerfunktionen des Apache-Server beteiligten Module.

Hilfe Befehl
---------------------

Der Befehl help dient als kurze Anleitung, die die Benutzer den Umgang und die Nutzung dieser speziellen Modul führt.

Die Syntax für die Hilfebefehl unter der Apache-Steuerung ist unten dargestellt:

.. code-block:: bash

	ptdeploy ApacheControl help

Die Syntax für die Deklaration den Befehl help ist nicht case sensitive was ein zusätzlicher Vorteil ist. Der Befehl help listet auch die alternativen Parameter, die in der Erklärung verwendet werden kann. Der folgende Screenshot visualisieren Sie den Befehl help unter Apache Control.

.. code-block:: bash

 kevell@corp:/# ptdeploy ApacheControl help
 ******************************


  This command is part of Default Modules and handles Apache Server Control Functions.

  ApacheControl, apachecontrol, apachectl

          - start
          Start the Apache server
          example: ptdeploy apachecontrol start
          example: ptdeploy apachecontrol start --yes --guess
          example: ptdeploy apachecontrol start --yes --apache-command="apache2"

          - stop
          Stop the Apache server
          example: ptdeploy apachecontrol stop
          example: ptdeploy apachecontrol stop --yes --guess
          example: ptdeploy apachecontrol stop --yes --apache-command="apache2"

          - restart
          Restart the Apache server
          example: ptdeploy apachecontrol restart
          example: ptdeploy apachecontrol restart --yes --guess
          example: ptdeploy apachecontrol restart --yes --apache-command="apache2"

          - reload
          Reloads the Apache server configuration without restarting
          example: ptdeploy apachecontrol reload
          example: ptdeploy apachecontrol reload --yes --guess
          example: ptdeploy apachecontrol reload --yes --apache-command="apache2"

 ------------------------------
 End Help
 ******************************

Die vier grundlegenden Steuerungsfunktionen in der Apache-Server enthalten sind:

* Beginn
* Stopp
* Neustart
* Neu Laden

Es gibt drei Möglichkeiten der Festlegung einer Steuerfunktionen. Zum Beispiel, wenn wir Start-Funktion ist, kann auf drei verschiedene Weisen, wie durch den Benutzer erforderlich ist, wie weiter unten definiert werden.

.. code-block:: bash
		
	ptdeploy ApacheControl start

or 

.. code-block:: bash

	ptdeploy ApacheControl start --yes --guess

or

.. code-block:: bash

	ptdeploy ApacheControl start --yes --apache-command="apache2"

Lassen Sie uns sehen die Verwendung von drei verschiedenen Syntax erklärt in kommenden Themen.


Alternative Parameter
-------------------------------

Im Folgenden sind die Parameter, die in alternative Erklärungen definiert werden können:

ApacheControl, apachecontrol, apachectl


Start-Funktion
--------------------

Wenn der Benutzer wünschen, den Apache-Steuerfunktion zu starten, kann die folgende Syntax verwenden, wie hier gezeigt:

.. code-block:: bash

	ptdeploy ApacheControl start

(Dies ist der erste Typ von Syntax der Festlegung einer Steuerfunktionen für apche Server)

Nach der Eingabe des Befehls, wie oben, werden die folgenden Schritte durchgeführt:

Schritt 1: Möchten Sie Apache starten? (Y / N).

Der Benutzer muss J oder N angeben

Schritt 2: Was ist der Apache-Service-Name?

(0) apache2

(1) httpd

Der Nutzer sollte, ob 0 oder 1 nach der Anforderung angeben.

Nachdem sie die Eingabe des Apache-Service-Name, wird es startet den Prozess.

Der folgende Screenshot zeigt den Startvorgang bildlich.

.. code-block:: bash

 kevell@corp:/# ptdeploy apachecontrol start
 Do you want to Start Apache? (Y/N)
 y
 What is the apache service name?
 (0) apache2
 (1) httpd
 0
 Starting Apache...
 * Starting web server apache2
 *
 ******************************


 1Apache Controller Finished
 ******************************


Stop-Funktion
------------------

Wenn der Benutzer wünschen, den Apache-Steuerfunktion zu stoppen, kann die folgende Syntax verwenden, wie hier gezeigt:

.. code-block:: bash

	ptdeploy apachecontrol stop --yes --guess

(Dies ist die zweite Art von Syntax der Festlegung einer Steuerfunktionen für Apache-Server)

Die Option Vermutung kann verwendet werden, um ein Standardwerte der bestimmten definierten Funktionen auszuführen.

Für Ubuntu die apche2 ist der Standardwert.

Für Cent OS httpd ist der Standardwert.

Der folgende Screenshot zeigt Sie über die Stopp-Funktion und Zweck der Vermutung Möglichkeiten bildhaft.

.. code-block:: bash

 kevell@corp:/# ptdeploy apachecontrol stop --yes --guess
 Stopping Apache...
 * Stopping web server apache2
 *
 ******************************
 1Apache Controller Finished
 ******************************


Starten Sie eine Funktion
-----------------------

Wenn der Benutzer wünschen, den Apache-Steuerfunktion neu zu starten, kann die folgende Syntax verwenden, wie hier gezeigt:

.. code-block:: bash
	
	ptdeploy apachecontrol restart --yes --apache-command="apache2"

Dies ist die dritte Art von Syntax der Festlegung einer Steuerfunktionen für apche Server)

Der Benutzer kann diese dritte Art von Syntax verwenden, um den Wert des erforderlichen Apache-Befehl angeben. Der Screenshot siehe unten zeigt diese dritte Art von Syntax und Prozess der Neustart einer Funktion bildlich.

.. code-block:: bash

 kevell@corp:/# ptdeploy apachecontrol restart --yes --apache-command="apache2"
 Restarting Apache...
 AH00558: apache2: Could not reliably determine the server's fully qualified domain name, using 127.0.1.1. Set the 'ServerName' directive globa lly to suppress this message
 * Restarting web server apache2
  
  ....done.
 ******************************


 1Apache Controller Finished
 ******************************


Nachladen einer Funktion
----------------------------

Wenn der Benutzer wünschen, den Apache-Steuerfunktion neu zu laden, kann die folgende Syntax verwenden, wie hier gezeigt:

.. code-block:: bash

	ptdeploy apachecontrol reload

or

.. code-block:: bash

	ptdeploy apachecontrol --yes --guess

or

.. code-block:: bash

	ptdeploy apachecontrol --yes --apache-command="apache2"

Der Reload-Funktion führt das erneute Laden der Apache-Server ohne Neustart.

Vorteile
-----------

* Es ist gut, sowohl in Cent-OS und Ubuntu zu tun.
* Die für Erklärungen verwendeten Parameter muss nicht beachtet werden, was ein zusätzlicher Vorteil ist, während im Vergleich zu anderen.
* Es gibt drei verschiedene Syntax zur Deklaration verwendet wird, kann der Benutzer unter ihnen gemäß den Anforderungen zu wählen.
* Die drei verschiedenen Syntax gelten für alle vier Steuerfunktionen Start, Stopp, neu zu starten, neu zu laden.
