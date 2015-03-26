===============
Jasmine
===============

Zusammenfassung
-------------------

Jasmin ist ein Verhalten driven Development-Framework zum Testen von JavaScript-Code.  Jasmin ist eine schen testing Framework für Javascript.  Es ist nicht auf Browser, DOM oder eine JavaScript-Framework angewiesen. Es ist deshalb geeignet für Webseiten, Node.js-Projekte, oder irgendwo, dass JavaScript ausgeführt werden.

Hilfe Befehl
--------------

Dieser Befehl hilft, um die Verwendung von Jasmin-Modul zu bestimmen. Es listet die alternative Ausgabeparameter von Jasmin. Es beschreibt auch die Syntax für Jasmine Modul funktionieren. Der Help-Befehl für Jasmine wird gezeigt wie unten beschrieben.

.. code-block:: bash

        ptconfigure Jasmine  help

Die bildliche Darstellung der oben genannte Befehl ist im folgenden aufgeführt,

.. code-block:: bash

 kevell@corp:/# ptconfigure Jasmine help
 ******************************


  This command allows you to install Jasmine from a GC Repo.

  Jasmine

        - install
        Installs the latest GC Repo version of Jasmine.
        example: ptconfigure Jasmine install

 ------------------------------
 End Help
 ******************************


Installation
---------------

Für Jasmin-Modul zu installieren, auf dem Terminal verwendete Befehl ist im folgenden aufgeführt,

.. code-block:: bash

        ptconfigure Jasmine install

Der obige Befehl soll die neueste Version von Jasmin und deren Abhängigkeiten installieren

Die bildliche Darstellung der oben genannte Befehl ist im folgenden aufgeführt,

.. code-block:: bash

 kevell@corp:/# ptconfigure jasmine install
 Install Jasmine? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         Jasmine        *
 *******************************
 Creating /tmp/ptconfigure-temp-script-79546324044.sh
 chmod 755 /tmp/ptconfigure-temp-script-79546324044.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-79546324044.sh Permissions
 Executing /tmp/ptconfigure-temp-script-79546324044.sh
 Cloning into 'jasmine'...
 remote: Counting objects: 12178, done.
 remote: Total 12178 (delta 0), reused 0 (delta 0), pack-reused 12178
 Receiving objects: 100% (12178/12178), 6.60 MiB | 8.00 KiB/s, done.
 Resolving deltas: 100% (7866/7866), done.
 Checking connectivity... done.
 Archive:  jasmine-standalone-2.0.0.zip
  inflating: MIT.LICENSE             
  inflating: lib/jasmine-2.0.0/jasmine_favicon.png  
  inflating: lib/jasmine-2.0.0/jasmine.js  
  inflating: lib/jasmine-2.0.0/jasmine-html.js  
  inflating: lib/jasmine-2.0.0/jasmine.css  
  inflating: lib/jasmine-2.0.0/console.js  
  inflating: lib/jasmine-2.0.0/boot.js  
  inflating: SpecRunner.html         
  inflating: src/Player.js           
  inflating: src/Song.js             
  inflating: spec/PlayerSpec.js      
  inflating: spec/SpecHelper.js      
 Temp File /tmp/ptconfigure-temp-script-79546324044.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 Jasmine: Success
 ------------------------------
 Installer Finished
 ******************************


Goals
-----------

* Es sollten Tests bewährte fördern 
* sollte es beginnen mit einfachen 
* es sollte sich leicht mit kontinuierlichen Build-Systeme integrieren




