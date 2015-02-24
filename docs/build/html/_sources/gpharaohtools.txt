===================
PharaohTools
===================

Zusammenfassung
-----------------------


Die Pharao-Tool Modul unterstützt in der Installierung ptdeploy, pttest, Jrush, Erzeugung ptconfigure Berichte. Es ermöglicht den Benutzern, die Verfügbarkeit, bevor Anlagen zu gewährleisten. Nur fehlende Module gezielt eingebaut werden.

Hilfe Befehl
---------------

Der Befehl help führt den Anwender dazu, wie Sie den Einsatz dieser speziellen Modul unter ptconfigure machen.

Es machen sie zudem Kenntnis von den Optionen, die zu diesem speziellen Modul durchgeführt werden können.

Der Screenshot siehe unten gibt Ihnen eine bildliche Darstellung über die Nutzung der Befehl help

.. code-block:: bash

 kevell@corp:/# ptconfigure PharaohTools help
 ******************************


  This command allows you to install the Pharaoh Tools which are ready. These include
  ptconfigure - this Configuration Management tool, ptdeploy- the Automated Deployment tool,  andpttest, the test configuration and automation tool.

  PharaohTools, pharaohtools, pharaoh-tools

        - install
        Installs the latest version of all of the Pharaoh Tools
        example: ptconfigure pharaoh-tools install

 ------------------------------
 End Help
 ******************************

Installation
----------------

Der Pharao Werkzeugmodul dient als kürzere Route, die Installation von Dapperstrano, Testingamen, Jrush umhüllt. Wenn eines bestimmten Moduls ist unter den drei fehlt, wird der spezifische Modul alleine installiert werden, ein zusätzlicher Vorteil ist. Die sicherzustellen Verfahren spielt eine wichtige Rolle in erregenden Daten bezüglich der Verfügbarkeit von Modulen.

Der Befehl für die Installation unter dem Pharao Werkzeug verwendet wird unten gegeben,

.. code-block:: bash

		ptconfigure pharaoh-tools install


.. cssclass:: table-bordered

 +------------------------------+---------------------------------+-------------------------------------------------+
 | Parameters                   | Verfügbare Eingabemöglichkeiten | Kommentare                                      |
 +==============================+=================================+=================================================+
 |Install Pharaoh Tools? (Y/N)  | Y(Yes)                          | Wenn der Benutzer Wunsch, mit Installation      |
 |                              |                                 | fortzusetzen, können sie Eingang als Y          |
 +------------------------------+---------------------------------+-------------------------------------------------+
 |Install Pharaoh Tools? (Y/N)  | N(No)                           | Wenn der Benutzer wünschen, um die Installation |
 |                              |                                 | zu beenden, sie einfach mit N verlassen können| |
 +------------------------------+---------------------------------+-------------------------------------------------+ 	

Bei der Installation des Pharao Werkzeug die folgenden Schritte erfolgt:


Dafür Sorgen
---------------

* Der Pharao-Tool sorgt für die zur Verfügung stehenden Module.
* Während die Gewährleistung, es wird nicht zu den Versionen überprüfen.

Ptdeploy
-------------

* Das Modul Ptdeploy meldet sich als angebracht, für den Fall der Existenz.
* Es überprüft auch die Version für Ptdeploy Modul.
* Wenn die Ptdeploy Modul ist in der Maschine nicht zur Verfügung, so wird automatisch Ptdeploy fortschreiten, um zu installieren.

Pttest
---------------

* Nach einer Installation Ptdeploy sie gewährleisten die pttest Moduls.
* Das Modul Pttestreports sich als angebracht, für den Fall der Existenz.
* Wenn die Pttest Modul ist in der Maschine nicht zur Verfügung, so wird automatisch Pttest fortschreiten, um zu installieren.


Jrush
---------

* Nach einer Installation pttest wird dadurch sichergestellt, das Jrush Moduls.
* Das Modul Jrush meldet sich als angebracht, für den Fall der Existenz.
* Wenn die Jrush Modul ist in der Maschine nicht zur Verfügung, so wird automatisch Jrush fortschreiten, um zu installieren.


Wenn alle drei Module sind bereits vorhanden, dann wird es außergewöhnliche Meldung wie im Screenshot unten angegeben,

.. code-block:: bash

 kevell@corp:/# ptconfigure pharaoh-tools install

 Install Pharaoh Tools? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         Pharaoh Tools        *
 *******************************
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module ptdeploy reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module pttest reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module ptconfigure reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module JRush reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************

 Single App Installer:
 --------------------------------------------
 PharaohTools: Success
 ------------------------------
 Installer Finished
 ******************************



PayPal-Logo
-------------------

Während der Installation von Ptdeploy Pttest werden Jrush Sie folgende Optionen bei Eingabe durch den Benutzer erforderlich. Wir wollen sehen, über die zusätzlichen Optionen, die von den Benutzern festgelegt werden können, wenn sie wollen, ist vertreten in tabellarischer Form wie unten dargestellt.

.. cssclass:: table-bordered

 +------------------------------+----------------------------------+-------------------+-------------------------------------------------+
 | Parameter                    | Weg                              | Option            | Bemerkung                                       |
 +==============================+==================================+===================+=================================================+
 |Program data directory        | "/opt/pttest (entsprechendes     | Yes               | Wenn der Benutzer die Installation mit dem      |
 |(Default)                     | Modul)”                          |                   | Standard-Programm-Daten-Verzeichnis gehen sie   |
 |                              |                                  |                   | eingeben kann als Ja                            |
 +------------------------------+----------------------------------+-------------------+-------------------------------------------------+
 |Program data directory        | User specific                    | No(End slash)     | Wenn der Benutzer mit ihren eigenen             |
 |                              |                                  |                   | Programmdatenverzeichnis fortfahren möchten,    |
 |                              |                                  |                   | können sie Eingang als N, und in die Hand geben |
 |                              |                                  |                   | sie Ort besitzen.                               |
 +------------------------------+----------------------------------+-------------------+-------------------------------------------------+
 |Program executor directory    | “/usr/bin”                       | Yes               | Wenn der Benutzer die Installation mit dem      |
 |(Default)                     |                                  |                   | Standardprogramm Testamentsvollstrecker         |
 |                              |                                  |                   | Verzeichnis gehen sie eingeben kann als Ja      |
 +------------------------------+----------------------------------+-------------------+-------------------------------------------------+
 |Program executor directory    | User specific                    | No(End Slash)     | Wenn der Benutzer wünschen, mit ihrem eigenen   |
 |                              |                                  |                   | Programm Testamentsvollstrecker Verzeichnis     |
 |                              |                                  |                   | gehen, können sie Eingang als N, und in die     |
 |                              |                                  |                   | Hand geben sie Ort besitzen|                    |
 +------------------------------+----------------------------------+-------------------+-------------------------------------------------+

Während der Installation wird die Lage von git clone angeben, zeigt die Anzahl der Objekte, Aufnahme von Gegenständen, die Lösung Deltas, Konnektivität.

Der folgende Screenshot erklärt grafisch über den Prozess der Installation des Pharao Werkzeug beteiligt.

.. code-block:: bash

 kevell@corp:/# ptconfigure pharaoh-tools install
 Install Pharaoh Tools? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         Pharaoh Tools        *
 *******************************
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module Ptdeploy reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module pttest reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module ptconfigure reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module JRush reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 PharaohTools: Success
 ------------------------------
 Installer Finished
 ******************************


Vorteile
------------

* Es ermöglicht den Nutzern, vor der Installation zu gewährleisten.
* Bei einem bestimmten Modul fehlt, kann der Nutzer gehen, dass bestimmte Modul alleine zu installieren.
* Der Benutzer kann seine eigenen Pfad oder Speicherort für die Programmdatenverzeichnis und Vollstrecker Verzeichnis angeben.
* Wenn ein bestimmtes Modul in der Maschine bereits vorhanden ist, wird das Installationswerkzeug eine Ausnahmemeldung werfen, da es bereits
  installiert.
