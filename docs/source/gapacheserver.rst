==============
ApacheServer
==============

Zusammenfassung
--------------------

Dieses Modul zielt auf die Installation des Apache-Servers. Ohne jede Anfrage wird automatisch die aktuelle Version des Apache-Server während der Installation zu installieren.

Hilfe Befehl
-----------------

Der Befehl help beschreibt über den Zweck und die Befehle unter dieser Module. Es erklärt auch den Befehl, um die bestimmte Module installiert.


.. code-block:: bash

 		cleopatra ApacheServer help

Der Screenshot, wie unten dargestellt, visuell repräsentieren die Verwendung des Befehls-Hilfe unter diesem Modul.

.. code-block:: bash


 kevell@corp:/# cleopatra ApacheServer help
 ******************************


  This command is part of Core and provides you  with a method by which you can install Apache HTTP Server

  ApacheServer, apache-server, apacheserver

        - install
        Installs Apache HTTP Server
        example: cleopatra apacheserver install

 ------------------------------
 End Help
 ******************************


Installation
-------------

Es ist einfacher, diese besondere Werkzeug unter Kleopatra, indem Sie einfach mit dem Befehl unten angegeben zu installieren,


.. code-block:: bash

		cleopatra ApacheServer install


Nachdem er den Befehl oben, wird das Tool fragen, wie

Installieren Sie Apache Server? (Y / N)

wenn Sie einen Eingang als Y geben, wird das Modul erfolgreich installiert.

Der Screenshot unten angegeben erklärt visuell über die Schritte und Befehle beinhaltet in der Installation.


.. code-block:: bash

 kevell@corp:/# cleopatra apacheserver install
 Install Apache Server? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         Apache Server!        *
 *******************************
 [Pharaoh Logging] Package apache2 from the Packager Apt is already installed, so not installing
 [Pharaoh Logging] Restarting apache2 service
 AH00558: apache2: Could not reliably determine the server's fully qualified domain name, using 127.0.1.1. Set the 'ServerName' directive globally to suppress this message
  * Restarting web server apache2
   ...done.
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 ApacheServer: Success
 ------------------------------
 Installer Finished
 ******************************


Optionen
-----------	

.. cssclass:: table-bordered

 +------------------------------+---------------------------------+--------------+--------------------------------------------+
 | Parameter		        | Alternative Parameter		  | Erforderlich | Kommentar 				      |
 +==============================+=================================+==============+============================================+
 |Install Apache Server? (Y/N)  | Statt ApacheServer , die wir    | Yes		 | Wenn der Benutzer gibt Eingabe wie ja,     |
 |				| verwenden können		  | 		 | wird Installation fortgesetzt	      |
 +------------------------------+---------------------------------+--------------+--------------------------------------------+
 |Install Apache Server? (Y/N)  | Statt ApacheServer , die wir    | No           | Wenn der Benutzer gibt Eingang als nicht,  |
 |                              | verwenden können                |              | wird es bekommen Ausfahrt.|                |
 +------------------------------+---------------------------------+--------------+--------------------------------------------+

Version
-----------

Während das Werkzeug die Bearbeitung wird es greift automatisch den zuletzt aktualisierten Version und macht sie bereit für die Installation zu bekommen.


Vorteile für die Endbenutzer
-----------------------------------

* Diese Module hilft dem Benutzer bei der Installation des Apache-Server. Es vereinfacht die Arbeit der Benutzer bei der Installation des 
  Servers als automatisch überprüfen Sie die aktuelle Version des Apache-Server.
* Es ist wohlhabend in Cent OS und als auch in Ubuntu.
* Die in der Erklärung verwendeten Parameter ist nicht case sensitive, was ein zusätzlicher Vorteil ist.

