=====	
JAVA
=====

Zusammenfassung
--------------------------

Dieses Modul hilft bei der Installation der Version von Oracle Java JDK 1.7. Es wird auch erleichtert die Konfiguration einer java, javac, javaws zusammen mit dem neuen Oracle-Version.

Hilfe Befehl
---------------------

Der Befehl help führt den Anwender über den Zweck und als auch über die Möglichkeiten, die in Java-Modul enthalten sind. Der Befehl help listet einige der alternativen Parameter des Java-Modul. Es beschreibt auch die Syntax für die Installation von Java JDK 1.7. Der Befehl help for Java-Modul wird wie unten dargestellt.

.. code-block:: bash

		ptconfigure Java help

Die Syntax für die Deklaration den Befehl help ist nicht case sensitive was ein zusätzlicher Vorteil ist. Der folgende Screenshot visualisieren Sie den Befehl help unter Java-Modul.

.. code-block:: bash

 kevell@corp:/# ptconfigure java help
 ******************************


 This command allows you to install Java JDK 1.7 .

 Java, java, java17

        - install
        Installs a version of Oracle Java JDK 1.7. It will also configure java,
        javac and javaws to be provided by the new Oracle version.
        example: ptconfigure java17 install

 ------------------------------
 End Help
 ******************************

Installation
----------------

Installation der Oracle-Version von Java JDK 1.7 auf die Benutzer-Maschine kann einfach mit Hilfe des Befehls wie folgt durchgeführt werden

.. code-block:: bash
	
		ptconfigure Java install

Nach der Eingabe des Befehls oben, passiert folgendes Verfahren im Tabellenformat angezeigt.

.. cssclass:: table-bordered

 +---------------------------+---------------------------------------------+-----------+--------------------------------------+
 | Parameters                | Alternative Parameter                       | Optionen  | Kommentare                           |
 +===========================+=============================================+===========+======================================+
 |Install The Oracle Java    | anstelle von Oracle Java JDK 1.7, folgende  | Y(Yes)    | Wenn der Benutzer wünschen, den      |
 |JDK 1.7? (Y/N)             | Alternativen können ebenfalls verwendet     |           | Installationsprozess können sie als  |
 |                           | werden: Java, java, java17                  |           | Eingangs gehen Y.                    |
 +---------------------------+---------------------------------------------+-----------+--------------------------------------+
 |Install The Oracle Java    | anstelle von Oracle Java JDK 1.7, folgende  | N(No)     | Wenn der Benutzer wünschen, den      |
 |JDK 1.7? (Y/N)             | Alternativen können ebenfalls verwendet     |           | Installationsprozess können sie      |
 |                           | werden: Java, java, java17                  |           | Eingabe als beendet N.|              |
 +---------------------------+---------------------------------------------+-----------+--------------------------------------+


.. code-block:: bash

 kevell@corp:/# ptconfigure java17 install
 Install The Oracle Java JDK 1.7? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         !!Java JDK!!        *
 *******************************
 Enter Java Install Directory (no trailing slash):
 /opt
 Creating /tmp/ptconfigure-temp-script-96883431452.sh
 chmod 755 /tmp/ptconfigure-temp-script-96883431452.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-96883431452.sh Permissions
 Executing /tmp/ptconfigure-temp-script-96883431452.sh
 --2015-04-09 16:27:08--  https://bitbucket.org/phpengine/cleo-jdk-64/get/6c383e2868bd.zip
 Resolving bitbucket.org (bitbucket.org)... 131.103.20.168, 131.103.20.167
 Connecting to bitbucket.org (bitbucket.org)|131.103.20.168|:443... connected.
 HTTP request sent, awaiting response... 200 OK
 Length: 141966331 (135M) [application/zip]
 Saving to: Ã¢â‚¬Ëœ/tmp/oraclejdk/6c383e2868bd.zipÃ¢â‚¬â„¢

 100%[====================================================================================================>] 14,19,66,331  110KB/s   in 12m 36s

 2015-04-09 16:39:46 (183 KB/s) - Ã¢â‚¬Ëœ/tmp/oraclejdk/6c383e2868bd.zipÃ¢â‚¬â„¢ saved [141966331/141966331]

 Archive:  /tmp/oraclejdk.zip
 6c383e2868bd47e56385921e11ec155ac54faa13
   creating: /tmp/oraclejdk/phpengine-cleo-jdk-64-6c383e2868bd/
  inflating: /tmp/oraclejdk/phpengine-cleo-jdk-64-6c383e2868bd/jdk-7u60-linux-x64.tar.gz  
 update-alternatives: using /opt/bin/java to provide /usr/bin/java (java) in auto mode
 update-alternatives: using /opt/bin/javac to provide /usr/bin/javac (javac) in auto mode 
 update-alternatives: using /opt/bin/javaws to provide /usr/bin/javaws (javaws) in auto mode
 Temp File /tmp/ptconfigure-temp-script-96883431452.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************

 Single App Installer:
 --------------------------------------------
 Java: Success
 ------------------------------
 Installer Finished
 ******************************


Vorteile
------------

* Die in Hilfe und Installation verwendet muss nicht beachtet werden, welche ein zusätzlicher Vorteil ist, während im Vergleich zu anderen 
  Parametern.
* Es ist gut-to-do sowohl Ubuntu und sowie Cent OS.
* Konfigurieren java, javac, javaws kann mit Hilfe der neuen Oracle-Version durchgeführt werden..
