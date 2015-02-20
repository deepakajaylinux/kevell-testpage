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



Vorteile
------------

* Die in Hilfe und Installation verwendet muss nicht beachtet werden, welche ein zusätzlicher Vorteil ist, während im Vergleich zu anderen 
  Parametern.
* Es ist gut-to-do sowohl Ubuntu und sowie Cent OS.
* Konfigurieren java, javac, javaws kann mit Hilfe der neuen Oracle-Version durchgeführt werden..