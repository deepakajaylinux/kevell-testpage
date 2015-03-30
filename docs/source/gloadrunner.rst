==============
Loadrunner
==============

Zusammenfassung
------------------

HP Loadrunner ist ein automatisiertes Performance und Testautomatisierung Produkt von Hewlett-Packard für die Anwendung Lasttests : Prüfung Systemverhalten und die Leistung , bei der Erzeugung der tatsächlichen Belastung . Loadrunner unterstützt verschiedene Entwicklungs-Tools, Technologien und Kommunikationsprotokolle. 

Hilfe Befehl
--------------

 Der Befehl help führt den Anwender über den Zweck und als auch über die Möglichkeiten , die in der Loadrunner Modul enthalten sind. Es beschreibt auch die Syntax für die Installation des Runner Moduls. Der Befehl help für Loadrunner ist wie unten dargestellt.


.. code-block:: bash

	ptconfigure Loadrunner help

Die bildliche Darstellung der obigen Befehl aufgelistet unten ,

.. code-block:: bash

 kevell@corp:/# ptconfigure Loadrunner help 
 ****************************** 


  This command allows you to install HardyCssRegression from a GC Repo. 

  Loadrunner 

        - install 
        Installs the latest GC Repo version of Loadrunner 
        example: ptconfigure Loadrunner install 

 ------------------------------ 
 End Help 
 ******************************   



Installation
--------------

Der Befehl für die Installation der Loadrunner -Modul auf dem Terminal verwendet wird, aufgeführt unten ,

.. code-block:: bash

	ptconfigure loadrunner install 

Die bildliche Darstellung der obigen Befehl aufgelistet unten ,


.. code-block:: bash

 kevell@corp:/# ptconfigure loadrunner install 
 Install Loadrunner? (Y/N) 
 y 
 ******************************* 
 *        Pharaoh Tools        * 
 *         Loadrunner !         * 
 ******************************* 
 Creating /tmp/ptconfigure-temp-script-32374780925.sh 
 chmod 755 /tmp/ptconfigure-temp-script-32374780925.sh 2>/dev/null 
 Changing /tmp/ptconfigure-temp-script-32374780925.sh Permissions 
 Executing /tmp/ptconfigure-temp-script-32374780925.sh 
 mkdir: cannot create directory â€˜loadrunnerâ€™: File exists 
 Cloning into 'loadrunner'... 
 remote: Counting objects: 1284, done. 
 remote: Total 1284 (delta 0), reused 0 (delta 0), pack-reused 1284 
 Receiving objects: 100% (1284/1284), 5.63 MiB | 21.00 KiB/s, done. 
 Resolving deltas: 100% (592/592), done. 
 Checking connectivity... done. 
 Temp File /tmp/ptconfigure-temp-script-32374780925.sh Removed 
 ... All done! 
 ******************************* 
 Thanks for installing , visit www.pharaohtools.com for more 
 ****************************** 


 Single App Installer: 
 -------------------------------------------- 
 Loadrunner: Success 
 ------------------------------ 
 Installer Finished 
 ****************************** 


Vorteile
----------

* Keine Notwendigkeit , um es auf dem Server zu test installieren. Es verwendet native Monitore. Für Ex: Perfmon für Fenster oder rstatd
  Daemon für Unix
* Verwendet ANSI C als Standard- Programmier language1 und andere Sprachen wie Java und VB .
* Ausgezeichnete Überwachung und Analyse -Schnittstelle , wo man Berichte in leicht farbige Diagramme und Grafiken zu verstehen, zu sehen .
  Unterstützt die meisten der protocols2 .
* Macht correlation3 viel einfacher. Wir werden in Zusammenhang mit einer Reihe von Stellen später graben.
* Nizza GUI generierte Skript durch einen einzigen Klick Aufnahme natürlich würden Sie brauchen, um das Skript nach Ihren Bedürfnissen ändern.
