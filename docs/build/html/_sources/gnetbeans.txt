============
NetBeans
============

Zusammenfassung
------------------------

NetBeans ist eine integrierte Entwicklungsumgebung (IDE) für die Entwicklung vor allem mit Java, aber auch mit anderen Sprachen, insbesondere PHP, C / C ++ und HTML. Es ist auch eine Anwendungsplattform Rahmen für Java-Desktop-Anwendungen und andere.

Die NetBeans IDE ist in Java geschrieben und kann auf Windows, OS X, Linux, Solaris und andere Plattformen, die ein kompatibles JVM ausgeführt NetBeans IDE ist eine Cross-Plattform-IDE mit eingebauter Unterstützung für Java-Programmiersprache.

Die NetBeans-Plattform ermöglicht es Anwendungen, aus einer Reihe von modularen Softwarekomponenten genannt Module entwickelt werden. Anwendungen auf Basis der NetBeans-Plattform (einschließlich der NetBeans IDE selbst) von Drittentwickler erweitert werden.

Hilfe Befehl
----------------------

Diese Funktion dient, um die Verwendung von Netbeans Modul bestimmen. Der Benutzer wird kommen, um über die andere Art und Weise / Format um dieses Modul ausführen kennen. Dieser Befehl leitet den Anwender, um den Zweck dieses Befehls kennen. Da unten sind die Kommando- und der Screenshot der gleiche.

.. code-block:: bash
        
	        ptconfigure Netbeans help


.. code-block:: bash

 kevell@corp:/# ptconfigure netbeans help
 ******************************


  This command allows you to install and uninstall NetBeans - IDE.

  NetBeans, Netbeans, netbeans

        - install
        Installs a version of NetBeans.
        example: ptconfigure netbeans install
	
	- uninstall
        Uninstalls a version of NetBeans.
        example: ptconfigure netbeans uninstall
 ------------------------------
 End Help
 ******************************


Installation
----------------

Dieser Befehl hilft bei der Installation von Netbeans in System. Die unten angegebenen Befehl wird den Prozess der Installation auszuführen.

.. code-block:: bash
        
	        ptconfigure netbeans install


.. code-block:: bash


 kevell@corp:/# ptconfigure netbeans install
 Install NetBeans-8.0? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         !!NetBeans!!        *
 *******************************
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module Java reports itself as Installed
 [Pharaoh Logging] Not installing as already installed

 Enter (1) to Install NetBeans in Silent:
 Enter (2) to install NetBeans in UserFriendly:
 1
 Creating /tmp/ptconfigure-temp-script-53829501149.sh
 chmod 755 /tmp/ptconfigure-temp-script-53829501149.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-53829501149.sh Permissions
 Executing /tmp/ptconfigure-temp-script-53829501149.sh
 --2015-04-01 11:42:15--  http://download.netbeans.org/netbeans/8.0/final/bundles/netbeans-8.0-linux.sh
 Resolving download.netbeans.org (download.netbeans.org)... 137.254.120.26
 Connecting to download.netbeans.org (download.netbeans.org)|137.254.120.26|:80... connected.
 HTTP request sent, awaiting response... 302 Moved Temporarily
 Location: http://dlc-cdn.sun.com/netbeans/8.0/final/bundles/netbeans-8.0-linux.sh [following]
 --2015-04-01 11:42:16--  http://dlc-cdn.sun.com/netbeans/8.0/final/bundles/netbeans-8.0-linux.sh
 Resolving dlc-cdn.sun.com (dlc-cdn.sun.com)... 23.205.118.80, 23.205.118.73
 Connecting to dlc-cdn.sun.com (dlc-cdn.sun.com)|23.205.118.80|:80... connected.
 HTTP request sent, awaiting response... 200 OK
 Length: 212403200 (203M) [application/x-sh]
 Saving to: â€˜netbeans-8.0-linux.shâ€™ 

 100%[===========================================================================================>] 21,24,03,200 78.0KB/s   in 78m 40s

 2015-04-01 13:00:58 (43.9 KB/s) - â€˜netbeans-8.0-linux.shâ€™ saved [212403200/212403200]

 Temp File /tmp/ptconfigure-temp-script-53829501149.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 NetBeans: Success
 ------------------------------
 Installer Finished
 ****************************** 


Deinstallation
-----------------

Dieser Befehl hilft bei der Deinstallation von Netbeans in System . Die unten angegebenen Befehl wird den Prozess der Installation auszuführen.


.. code-block:: bash

	ptconfigure netbeans uninstall

.. code-block:: bash

 kevell@corp:/# ptconfigure netbeans uninstall

 Uninstall NetBeans-8.0? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         !!NetBeans!!        *
 *******************************
 Creating /tmp/ptconfigure-temp-script-80402838784.sh
 chmod 755 /tmp/ptconfigure-temp-script-80402838784.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-80402838784.sh Permissions
 Executing /tmp/ptconfigure-temp-script-80402838784.sh
 Configuring the installer...
 Searching for JVM on the system...
 Extracting installation data...
 Running the installer wizard...
 Temp File /tmp/ptconfigure-temp-script-80402838784.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Uninstaller:
 ------------------------------
 NetBeans: Success
 ------------------------------
 Installer Finished
 ******************************



Options
-----------                               

.. cssclass:: table-bordered

 +-------------------------+----------------------------------------------------+------------+-------------------------------------+
 | Parameter               | Alternative Parameter                              | Option     | Kommentare                          |
 +=========================+====================================================+============+=====================================+
 |ptconfigure Netbeans     | Es gibt drei alternative Parameter, die in der     | Y(Yes)     | System startet Installation         |
 |Install                  | Befehlszeile verwendet werden kann. Netbeans ,     |            |                                     |
 |                         | NetBeans , netbeans Eg: ptconfigure NetBeans       |            |                                     |
 |                         | install, ptconfigure netbeans install              |            |                                     |
 +-------------------------+----------------------------------------------------+------------+-------------------------------------+
 |ptconfigure Netbeans     | Es gibt drei alternative Parameter, die in der     | N(No)      | Das System stoppt den               |
 |Install                  | Befehlszeile verwendet werden kann. Netbeans ,     |            | Installationsprozess                |
 |                         | NetBeans , netbeans Eg: ptconfigure NetBeans       |            |                                     |
 |                         | install, ptconfigure netbeans install|             |            |                                     |
 +-------------------------+----------------------------------------------------+------------+-------------------------------------+


Vorteile
--------------

* Benutzerschnittstellenmanagement (zB Menüs und Symbolleisten)
* Benutzereinstellungen Management
* Speicherverwaltung (Speichern und Laden von Daten jeglicher Art)
* Fenstermanagement
* Wizard Framework (unterstützt Schritt-für-Schritt-Dialoge)
* NetBeans Visual Library
* Integrierte Entwicklungswerkzeuge

