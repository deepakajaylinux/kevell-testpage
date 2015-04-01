==============
NagiosServer
==============

Zusammenfassung
-----------------------

Nagios ist ein Open-Source-Computersystemüberwachung, Netzwerküberwachung und Infrastruktur-Monitoring-Software-Anwendung. Nagios bietet Monitoring und Alerting Services für Server, Switches, Anwendungen und Dienste. Es warnt den Benutzer, wenn etwas schief geht und warnt sie ein zweites Mal, wenn das Problem behoben wurde.

Nagios, ursprünglich unter dem Namen Nagios erstellt wurde geschrieben und wird derzeit von Ethan Galstad zusammen mit einer Gruppe von Entwicklern, die aktiv die Aufrechterhaltung sowohl der offiziellen und inoffiziellen Plugins erhalten. Nagios wurde ursprünglich entwickelt, um unter Linux laufen, sondern auch läuft gut auf anderen Unix-Varianten. Es ist freie Software unter den Bedingungen der GNU General Public License Version 2, wie von der Free Software Foundation veröffentlicht, lizenziert.

Hilfe Befehl
----------------------

Dieser Befehl hilft, den Einsatz von Nagios Modul zu bestimmen. Der Benutzer wird kommen, um über die andere Art und Weise / Format um dieses Modul ausführen kennen. Dieser Befehl leitet den Anwender, um den Zweck dieses Befehls kennen. Da unten sind die Kommando- und der Screenshot der gleiche.

.. code-block:: bash
        
	        ptconfigure nagios help


Die bildliche Screenshot der obigen Befehl aufgelistet unten,

.. code-block:: bash

 kevell@corp:/# ptconfigure nagiosserver help

 ******************************


  This command is part of Core and provides you with a method by which you can install Nagios.

  NagiosServer, nagios-server, nagiosserver, nagios

        - install
        Installs Nagios Network Monitoring Server
        example: ptconfigure nagios-server install

 ------------------------------
 End Help
 ******************************


Installation
----------------

Dieser Befehl hilft bei der Installation des Nagios-in-System. Die unten angegebenen Befehl wird den Prozess der Installation auszuführen.

.. code-block:: bash
        
	        ptconfigure nagios install

Die bildliche Darstellung der obigen Befehl aufgelistet unten,

.. code-block:: bash


 kevell@corp:/# ptconfigure nagios-server install

 Install Nagios Server? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         Nagios Server!        *
 *******************************

 * Starting nagios3 monitoring daemon nagios3                                                                                  [ OK ] 
 enabling Apache2 config...
 apache2_invoke: Enable module cgi
 * Restarting web server apache2                                                                                                  AH00558:  
 apache2: Could not reliably determine the server's fully qualified domain name, using 127.0.1.1. Set the 'ServerName' directive globally to 
 suppress this message
                                                                                                                               [ OK ]
 apache2_invoke: Enable configuration nagios3
 * Reloading web server apache2                                                                                                        * 
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  libjs-jquery nagios-images nagios3-cgi nagios3-common nagios3-core
 Suggested packages:
  javascript-common
 The following NEW packages will be installed:
  libjs-jquery nagios-images nagios3 nagios3-cgi nagios3-common nagios3-core
 0 upgraded, 6 newly installed, 0 to remove and 250 not upgraded.
 Need to get 3,748 kB of archives.
 After this operation, 12.3 MB of additional disk space will be used.
 Get:1 http://archive.ubuntu.com/ubuntu/ trusty/main libjs-jquery all 1.7.2+dfsg-2ubuntu1 [78.8 kB]
 Get:2 http://archive.ubuntu.com/ubuntu/ trusty/main nagios-images all 0.8 [2,589 kB]
 Get:3 http://archive.ubuntu.com/ubuntu/ trusty/main nagios3-common all 3.5.1-1ubuntu1 [53.7 kB]
 Get:4 http://archive.ubuntu.com/ubuntu/ trusty/main nagios3-cgi amd64 3.5.1-1ubuntu1 [794 kB]
 Get:5 http://archive.ubuntu.com/ubuntu/ trusty/main nagios3-core amd64 3.5.1-1ubuntu1 [231 kB]
 Get:6 http://archive.ubuntu.com/ubuntu/ trusty/main nagios3 amd64 3.5.1-1ubuntu1 [1,528 B]
 Preconfiguring packages ...
 Fetched 3,748 kB in 1min 11s (52.1 kB/s)
 Selecting previously unselected package libjs-jquery.
 (Reading database ... 231932 files and directories currently installed.)
 Preparing to unpack .../libjs-jquery_1.7.2+dfsg-2ubuntu1_all.deb ...
 Unpacking libjs-jquery (1.7.2+dfsg-2ubuntu1) ...
 Selecting previously unselected package nagios-images.
 Preparing to unpack .../nagios-images_0.8_all.deb ...
 Unpacking nagios-images (0.8) ...
 Selecting previously unselected package nagios3-common.
 Preparing to unpack .../nagios3-common_3.5.1-1ubuntu1_all.deb ...
 Unpacking nagios3-common (3.5.1-1ubuntu1) ...
 Selecting previously unselected package nagios3-cgi.
 Preparing to unpack .../nagios3-cgi_3.5.1-1ubuntu1_amd64.deb ...
 Unpacking nagios3-cgi (3.5.1-1ubuntu1) ...
 Selecting previously unselected package nagios3-core.
 Preparing to unpack .../nagios3-core_3.5.1-1ubuntu1_amd64.deb ...
 Unpacking nagios3-core (3.5.1-1ubuntu1) ...
 Selecting previously unselected package nagios3.
 Preparing to unpack .../nagios3_3.5.1-1ubuntu1_amd64.deb ...
 Unpacking nagios3 (3.5.1-1ubuntu1) ...
 Processing triggers for ureadahead (0.100.0-16) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Setting up libjs-jquery (1.7.2+dfsg-2ubuntu1) ...
 Setting up nagios-images (0.8) ...
 Setting up nagios3-common (3.5.1-1ubuntu1) ...
 Setting up nagios3-cgi (3.5.1-1ubuntu1) ...
 Setting up nagios3-core (3.5.1-1ubuntu1) ...
 Setting up nagios3 (3.5.1-1ubuntu1) ...
 [Pharaoh Logging] Adding Package nagios3 from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 NagiosServer: Success
 ------------------------------
 Installer Finished
 ******************************




Optionen
-----------

.. cssclass:: table-bordered

 +----------------------------+-------------------------------------------------+-------------+---------------------------------------+
 | Parameter                  | Alternative Parameter                           | Option      | Kommentare                            |
 +============================+=================================================+=============+=======================================+
 |ptconfigure nagiosserver    | Es gibt vier alternative Parameter, die in der  | Y(Yes)      | System startet Installation           |
 |Install                     | Befehlszeile verwendet werden können.           |             |                                       |
 |                            | NagiosServer, nagios-server, nagiosserver,      |             |                                       |
 |                            | nagios Eg: ptconfigure nagios install/          |             |                                       |
 |                            | ptconfigure nagiosserver install                |             |                                       |
 +----------------------------+-------------------------------------------------+-------------+---------------------------------------+
 |ptconfigure nagiosserver    | Es gibt vier alternative Parameter, die in der  | N(No)       | Das System stoppt den                 |
 |Install                     | Befehlszeile verwendet werden können.           |             | Installationsprozess                  |
 |                            | NagiosServer, nagios-server, nagiosserver,      |             |                                       |
 |                            | nagios Eg: ptconfigure nagios install/          |             |                                       |
 |                            | ptconfigure nagiosserver install|               |             |                                       |
 +----------------------------+-------------------------------------------------+-------------+---------------------------------------+


Vorteile
--------------

* Überwachung von Netzwerkdiensten ( SMTP, POP3, HTTP, NNTP , ICMP, SNMP , FTP, SSH )

* Überwachung von Host-Ressourcen ( Prozessorlast , Plattennutzung , Systemprotokolle ) auf einem Großteil der Netzwerkbetriebssystemen , 
  darunter Microsoft Fenster mit der NSClient ++ Plugin oder Prüfen MK .

* Überwachung der noch etwas wie Sonden ( Temperatur , Alarme, etc. ), Die in der Lage, die gesammelten Daten über ein Netzwerk zu senden sind
  speziell geschrieben Plugins

* Überwachung via remote ausführen Skripte über Nagios Remote- Plugin Executor

* Fernüberwachung über SSH oder SSL- verschlüsselte Tunnel unterstützt.

* Ein einfaches Plugin -Design , die Benutzer auf einfache Weise entwickeln ihre eigene Service-Prüfungen je nach Bedarf , indem sie ihre 
  Werkzeuge der Wahl erlaubt ( Shell-Skripte , C ++, Perl, Ruby , Python, PHP , C # , etc.)

* Die verfügbaren Daten Grafik- Plugins

* Parallel laufende Service- Prüfungen

* Die Fähigkeit, Netzwerk-Host -Hierarchien mit Hosts "Eltern" zu definieren , so dass die Erkennung von und Unterscheidung zwischen Hosts, 
  die unten sind,  oder nicht erreichbar

* Kontakt -Benachrichtigungen, wenn Service- oder Host- Probleme auf, entschlossen zu erhalten (per E- Mail, Pager , SMS, oder jede 
  benutzerdefinierte Methode durch Plugin-System )

* Die Fähigkeit, Event-Handler definieren, die während der Service- oder Host- Veranstaltungen zur proaktiven Problemlösung ausgeführt werden

* Automatische Protokolldatei Dreh

* Unterstützung für Implementieren von redundanten Überwachungs -Hosts

* Ein optionaler Web-Interface für die Anzeige von aktuellen Netzwerkstatus , Benachrichtigungen Problem der Geschichte , Protokolldateien usw.

* Datenspeicherung über Textdateien und nicht -Datenbank
