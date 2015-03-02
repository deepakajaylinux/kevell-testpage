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

 kevell@corp:/# cleopatra nagios help
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
 E: Unable to correct problems, you have held broken packages.
 Reading package lists...
 Building dependency tree...
 Reading state information...
 Some packages could not be installed. This may mean that you have
 requested an impossible situation or if you are using the unstable
 distribution that some required packages have not yet been created
 or been moved out of Incoming.
 The following information may help to resolve the situation:

 The following packages have unmet dependencies:
 nagios3 : Depends: nagios3-core (= 3.2.3-3ubuntu1) but it is not going to be installed
 [Pharaoh Logging] Adding Package nagios3 from the Packager Apt did not execute correctly
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
