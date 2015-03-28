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

 		ptconfigure ApacheServer help

Der Screenshot, wie unten dargestellt, visuell repräsentieren die Verwendung des Befehls-Hilfe unter diesem Modul.

.. code-block:: bash


 kevell@corp:/# ptconfigure ApacheServer help
 ******************************


  This command is part of Core and provides you  with a method by which you can install Apache HTTP Server

  ApacheServer, apache-server, apacheserver

        - install
        Installs Apache HTTP Server
        example: ptconfigure apacheserver install

 ------------------------------
 End Help
 ******************************


Installation
-------------

Es ist einfacher, diese besondere Werkzeug unter ptconfigure, indem Sie einfach mit dem Befehl unten angegeben zu installieren,


.. code-block:: bash

		ptconfigure ApacheServer install


Nachdem er den Befehl oben, wird das Tool fragen, wie

Installieren Sie Apache Server? (Y / N)

wenn Sie einen Eingang als Y geben, wird das Modul erfolgreich installiert.

Der Screenshot unten angegeben erklärt visuell über die Schritte und Befehle beinhaltet in der Installation.


.. code-block:: bash


 kevell@corp:/# ptconfigure ApacheServer install
 Install Apache Server? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         Apache Server!        *
 *******************************
 AH00558: apache2: Could not reliably determine the server's fully qualified domain name, using 127.0.1.1. Set the 'ServerName' directive globally to suppress this message
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following packages were automatically installed and are no longer required:
   php5-cli php5-readline
 Use 'apt-get autoremove' to remove them.
 Suggested packages:
  apache2-doc apache2-suexec-pristine apache2-suexec-custom apache2-utils
 The following NEW packages will be installed:
  apache2
 0 upgraded, 1 newly installed, 0 to remove and 39 not upgraded.
 Need to get 0 B/87.4 kB of archives.
 After this operation, 473 kB of additional disk space will be used.
 Selecting previously unselected package apache2.
 (Reading database ... 193457 files and directories currently installed.)
 Preparing to unpack .../apache2_2.4.7-1ubuntu4.4_amd64.deb ...
 Unpacking apache2 (2.4.7-1ubuntu4.4) ...
 Processing triggers for ureadahead (0.100.0-16) ...
 ureadahead will be reprofiled on next reboot
 Processing triggers for ufw (0.34~rc-0ubuntu2) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Setting up apache2 (2.4.7-1ubuntu4.4) ...
 Enabling module mpm_event.
 Enabling module authz_core.
 Enabling module authz_host.
 Enabling module authn_core.
 Enabling module auth_basic.
 Enabling module access_compat.
 Enabling module authn_file.
 Enabling module authz_user.
 Enabling module alias.
 Enabling module dir.
 Enabling module autoindex.
 Enabling module env.
 Enabling module mime.
 Enabling module negotiation.
 Enabling module setenvif.
 Enabling module filter.
 Enabling module deflate.
 Enabling module status.
 Enabling conf charset.
 Enabling conf localized-error-pages.
 Enabling conf other-vhosts-access-log.
 Enabling conf security.
 Enabling conf serve-cgi-bin.
 Enabling site 000-default.
 * Starting web server apache2
 * 
 Processing triggers for ureadahead (0.100.0-16) ...
 Processing triggers for ufw (0.34~rc-0ubuntu2) ...
 [Pharaoh Logging] Adding Package apache2 from the Packager Apt executed correctly
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

