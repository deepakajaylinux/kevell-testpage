=============
PharaohTools
=============

Zusammenfassung
------------------------

Die Pharao-Tool Modul unterstützt in der Installierung ptdeploy, pttest, Jrush, Erzeugung ptvirtualize Berichte. Es ermöglicht den Benutzern, die Verfügbarkeit, bevor Anlagen zu gewährleisten. Nur fehlende Module gezielt eingebaut werden.

Hilfe Befehl
---------------------

Der Befehl help führt den Anwender dazu, wie Sie den Einsatz dieser speziellen Modul unter ptvirtualize machen.

Es machen sie zudem Kenntnis von den Optionen, die zu diesem speziellen Modul durchgeführt werden können.

Es listet outs die alternativen Parameter zusammen mit der Syntax für die Installation der Pharao-Tools.

Der Befehl für die Verwendung der Hilfe-Option ist unten dargestellt,

.. code-block:: bash

	ptvirtualize pharaoh-tools help


Der Screenshot siehe unten gibt Ihnen eine bildliche Darstellung über die Nutzung der Befehl help.

.. code-block:: bash


Installation
--------------

Die Pharao Werkzeugmodul dient als kürzere Route, die Installation von ptdeploy, pttest, Jrush umhüllt. Wenn eines bestimmten Moduls ist unter den drei fehlt, wird der spezifische Modul alleine installiert werden, ein zusätzlicher Vorteil ist. Die sicherzustellen Verfahren spielt eine wichtige Rolle in erregenden Daten bezüglich der Verfügbarkeit von Modulen.

Der Befehl für die Installation unter dem Pharao Werkzeug verwendet wird unten gegeben,

.. code-block:: bash

	ptvirtualize pharaoh-tools install

Nach der Eingabe des Befehls vor, beginnt der Installationsvorgang ausführen und geht auf folgende Weise ab in der Tabelle dargestellt,

.. cssclass:: table-bordered


 +------------------------------+------------------------------+------------------------------------------------------------+
 | Parameters                   | Erhältlich Eingabeoptionen   | Kommentar                                                  |
 +==============================+==============================+============================================================+
 |Install Pharaoh Tools? (Y/N)  | Y(Yes)                       | Wenn der Benutzer Wunsch, mit Installation fortzusetzen,   |
 |                              |                              | können sie Eingang als Y                                   |
 +------------------------------+------------------------------+------------------------------------------------------------+
 |Install Pharaoh Tools? (Y/N)  | N(No)                        | Wenn der Benutzer wünschen, um die Installation zu         |
 |                              |                              | beenden, sie einfach mit N verlassen können|               |
 +------------------------------+------------------------------+------------------------------------------------------------+


 



Bei der Installation des Pharao Werkzeug die folgenden Schritte erfolgt:

Dafür Sorgen
-----------------

* Der Pharao-Tool sorgt für die zur Verfügung stehenden Module.
* Während die Gewährleistung, es wird nicht zu den Versionen überprüfen.

ptdeploy
------------------

* Das Modul ptdeploy meldet sich als angebracht, für den Fall der Existenz.
* Es überprüft auch die Version für ptdeploy Modul.
* Wenn die ptdeploy Modul ist in der Maschine nicht zur Verfügung, so wird automatisch ptdeploy fortschreiten, um zu installieren.

pttest
------------------

* Nach einer Installation ptdeploy wird dadurch sichergestellt, das pttest Moduls.
* Das Modul pttest sich als installiert berichtet, für den Fall der Existenz.
* Wenn die pttest Modul ist in der Maschine nicht zur Verfügung, pttest dann automatisch fortschreiten, um zu installieren.

Jrush
--------

* Nach einer Installation pttest wird dadurch sichergestellt, das Jrush Moduls.
* Das Modul Jrush meldet sich als angebracht, für den Fall der Existenz.
* Wenn die Jrush Modul ist in der Maschine nicht zur Verfügung, so wird automatisch Jrush fortschreiten, um zu installieren.
* Wenn alle drei Module sind bereits vorhanden, dann wird es außergewöhnliche Meldung wie im Screenshot unten angegeben,


PayPal-Logo
-------------------------

Während der Installation von ptdeploy, pttest, Jrush die folgenden Optionen werden als Eingabe durch den Benutzer erforderlich. Wir wollen sehen, über die zusätzlichen Optionen, die von den Benutzern festgelegt werden können, wenn sie wollen, ist vertreten in tabellarischer Form wie unten dargestellt.

.. cssclass:: table-bordered

 +------------------------+--------------------------------------+---------------+-------------------------------------------------+
 | Parameters             | Weg                                  | Option        | Comment                                         |
 +========================+======================================+===============+=================================================+
 |Program data            | “/opt/pttest(corresponding module)”  | Yes           | Wenn der Benutzer die Installation mit dem      | 
 |directory (Default)     |                                      |               | Programmdatenverzeichnis fortfahren möchten,e   |
 |                        |                                      |               | eingeben kann als Ja                            |
 +------------------------+--------------------------------------+---------------+-------------------------------------------------+
 |Program data directory  | User specific                        | No(End        | Wenn der Benutzer mit ihren eigenen             |
 |                        |                                      | Schrägstrich) | Programmdatenverzeichnis fortfahren möchten,    |
 |                        |                                      |               | Standardprogramm Testamentsvollstreckerkönnen n |
 |                        |                                      |               | sie Ort besitzen.                               |
 +------------------------+--------------------------------------+---------------+-------------------------------------------------+
 |Program executor        | “/usr/bin”                           | Yes           | Wenn der Benutzer die Installation mit dem      | 
 |directory (Default)     |                                      |               | Standardprogramm Testamentsvollstrecker         |
 |                        |                                      |               | Verzeichnis gehen sie eingeben kann als Ja      |
 +------------------------+--------------------------------------+---------------+-------------------------------------------------+
 |Program executor        | User specific                        | No(End        | Wenn der Benutzer mit ihren eigenen             |
 |directory               |                                      | Schrägstrich) | Programmausführungs Verzeichnis fortfahren      |
 |                        |                                      |               | möchten, können sie Eingang als N, und in die   |
 |                        |                                      |               | Hand geben sie Ort besitzen.|                   |
 +------------------------+--------------------------------------+---------------+-------------------------------------------------+


Während der Installation wird die Lage von git clone angeben, zeigt die Anzahl der Objekte, Aufnahme von Gegenständen, die Lösung Deltas, Konnektivität.

Der folgende Screenshot erklärt grafisch über den Prozess der Installation des Pharao Werkzeug beteiligt.


.. code-block:: bash

Vorteile
-----------

* Es ermöglicht den Nutzern, vor der Installation zu gewährleisten.
* Bei einem bestimmten Modul fehlt, kann der Nutzer gehen, dass bestimmte Modul alleine zu installieren.
* Der Benutzer kann seine eigenen Pfad oder Speicherort für die Programmdatenverzeichnis und Vollstrecker Verzeichnis angeben.
* Wenn ein bestimmtes Modul in der Maschine bereits vorhanden ist, wird das Installationswerkzeug eine Ausnahmemeldung werfen, da es bereits
  installiert.
* Es vermeidet ein unerwünschtes Überschreiben von Modulen, daher ist es Zeitersparnis.

