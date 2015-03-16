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
 Y
 *******************************
 *        Pharaoh Tools        *
 *         !!Java JDK!!        *
 *******************************
 Enter Java Install Directory (no trailing slash):

 Creating /tmp/ptconfigure-temp-script-37090112192.sh
 chmod 755 /tmp/ptconfigure-temp-script-37090112192.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-37090112192.sh Permissions
 Executing /tmp/ptconfigure-temp-script-37090112192.sh
 --2015-03-16 15:52:21--  https://bitbucket.org/phpengine/cleo-jdk-64/get/6c383e2868bd.zip
 Resolving bitbucket.org (bitbucket.org)... 131.103.20.167, 131.103.20.168
 Connecting to bitbucket.org (bitbucket.org)|131.103.20.167|:443... connected.
 HTTP request sent, awaiting response... 200 OK
 Length: unspecified [application/zip]
 Saving to: ‘6c383e2868bd.zip’

    [          <=>                                                                                          ] 2,06,54,011 2.98KB/s   in 12m 14s

 2015-03-16 16:04:59 (27.5 KB/s) - ‘6c383e2868bd.zip’ saved [20654011]

 /tmp/oraclejdk: Scheme missing.
 FINISHED --2015-03-16 16:04:59--
 Total wall clock time: 12m 39s
 Downloaded: 1 files, 20M in 12m 14s (27.5 KB/s)
  End-of-central-directory signature not found.  Either this file is not
  a zipfile, or it constitutes one disk of a multi-part archive.  In the
  latter case the central directory and zipfile comment will be found on
  the last disk(s) of this archive.
 unzip:  cannot find zipfile directory in one of /tmp/oraclejdk.zip or
        /tmp/oraclejdk.zip.zip, and cannot find /tmp/oraclejdk.zip.ZIP, period.
 /tmp/ptconfigure-temp-script-37090112192.sh: 6: cd: can't cd to /tmp/oraclejdk
 mv: cannot stat ‘/tmp/oraclejdk/phpengine-cleo-jdk-64-6c383e2868bd/jdk-7u60-linux-x64.tar.gz’: No such file or directory
 tar: jdk-7u60-linux-x64.tar.gz: Cannot open: No such file or directory
 tar: Error is not recoverable: exiting now
 mkdir: missing operand
 Try 'mkdir --help' for more information.
 cp: missing destination file operand after ‘/tmp/oraclejdk/jdk1.7.0_60/*’
 Try 'cp --help' for more information.
 chmod: missing operand after ‘a+x’
 Try 'chmod --help' for more information.
 update-alternatives: error: alternative path /bin/java doesn't exist
 update-alternatives: error: alternative path /bin/javac doesn't exist
 update-alternatives: error: alternative path /bin/javaws doesn't exist
 update-alternatives: error: alternative /bin/java for java not registered; not setting
 update-alternatives: error: alternative /bin/javac for javac not registered; not setting
 update-alternatives: error: alternative /bin/javaws for javaws not registered; not setting
 Archive:  /tmp/oraclejdk.zip
 Temp File /tmp/ptconfigure-temp-script-37090112192.sh Removed
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
