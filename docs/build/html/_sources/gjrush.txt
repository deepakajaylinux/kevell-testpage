======
Jrush
======

Zusammenfassung
-----------------------

Dieses Modul hilft bei der Installation des jrush auf Ihren Rechner. Es erleichtert auch die Aktualisierung mit einer neuen Version. Lassen Sie uns sehen, wie diese Module hilft bei der Installation eines jrush.

Hilfe Befehl
--------------------

Der Befehl help führt den Anwender über den Zweck und als auch über die Möglichkeiten, die in der Jrush Modul enthalten sind. Es listet einige der alternativen Parameter Jrush Modul. Es beschreibt auch die Syntax für die Installation des Jrush Moduls. Der Befehl help für Jrush Modul wird wie unten dargestellt.

.. code-block:: bash

		ptconfigure JRush help

Die Syntax für die Deklaration den Befehl help ist nicht case sensitive was ein zusätzlicher Vorteil ist. Der folgende Screenshot visualisieren Sie den Befehl help unter JRush.

.. code-block:: bash

 kevell@corp:/# ptconfigure JRush help
 ******************************


  This command allows you to install or Update JRush.

  JRush, jrush, Jrush, jRush

        - install
        Installs the latest version of jRush
        example: ptconfigure jRush install

 ------------------------------
 End Help
 ******************************


Installation
----------------

Der Befehl zum Installieren der JRush zum Benutzer Maschine verwendet wird unten gezeigt.

.. code-block:: bash

		ptconfigure JRush install



Optionen
-------------

Nach der Eingabe des Befehls vor, tritt die folgenden Vorgänge wie im Tabellenformat angezeigt.

.. cssclass:: table-bordered

 +----------------------------+-------------------------------------+-------------+--------------------------------------+
 | Parameters                 | Alternative Parameter               | Option      | Kommentare                           |
 +============================+=====================================+=============+======================================+
 |Install JRush - Joomla      | anstelle von JRush wir verwenden    | Y(Yes)      | Wenn der Benutzer wünschen, den      |
 |Command Line ? (Y/N)        | können : jrush, Jrush, jRush.       |             | Installationsprozess können sie als  |
 |                            |                                     |             | Eingangs gehen Y.                    |
 +----------------------------+-------------------------------------+-------------+--------------------------------------+
 |Install JRush - Joomla      | anstelle von JRush wir verwenden    | N(No)       | Wenn der Benutzer wünschen, den      |
 |Command Line ? (Y/N)        | können : jrush, Jrush, jRush.       |             | Installationsprozess können sie      |
 |                            |                                     |             | Eingabe als beendet N.|              |
 +----------------------------+-------------------------------------+-------------+--------------------------------------+


Wenn der Benutzer den Installationsprozeß schreitet die folgenden Vorgänge stattfindet, wie in der Form einer Tabelle.


.. cssclass:: table-bordered

 +--------------------------------+--------------------------------+---------------+-------------------------------------------------+
 | Parameter                      | Weg                            | Option        | Kommentare                                      |
 +================================+================================+===============+=================================================+
 |Program data directory          | “/opt/jrush (corresponding     | Yes           | Wenn der Benutzer die Installation mit der      |
 |(Default)                       | module)                        |               | Standard-Programmdatenverzeichnis können sie    |
 |                                |                                |               | als Eingangs gehen Yes                          |
 +--------------------------------+--------------------------------+---------------+-------------------------------------------------+
 |Program data directory          | User specific                  | No(End slash) | Wenn der Benutzer wünschen, mit ihrem eigenen   |
 |                                |                                |               | Programm-Daten-Verzeichnis, können sie als      |
 |                                |                                |               | Eingangs gehen N, und in der Hand ihrer eigenen |
 |                                |                                |               | Speicherort angeben                             |
 +--------------------------------+--------------------------------+---------------+-------------------------------------------------+
 |Program executor directory      | “/usr/bin”                     | Yes           | Wenn der Benutzer die Installation mit dem      |
 |(default)                       |                                |               | Standardprogramm Testamentsvollstrecker         |
 |                                |                                |               | Verzeichnis können sie als Eingangs gehen Yes   |
 +--------------------------------+--------------------------------+---------------+-------------------------------------------------+
 |Program executor directory      | User specific                  | No(End slash) | Wenn der Benutzer wünschen, mit ihrem eigenen   |
 |                                |                                |               | Programmausführungsverzeichnis , können sie als |
 |                                |                                |               | Eingangs gehen N, und in die Hand geben sie Ort |
 |                                |                                |               | besitzen.|                                      |
 +--------------------------------+--------------------------------+---------------+-------------------------------------------------+


Während der Installation wird der folgende Prozess:

* Zeigt den Status der Aufnahme von Gegenständen.
* Zeigt den Status der Lösung Deltas.
* Überprüft die Konnektivität.
* Zeigt als Programmdatenordner besiedelt.
* Löscht die Programmverwalter , ob bereits vorhanden.

Schließlich wird die Installation von Jrush abgeschlossen. Der folgende Screenshot zeigt den Prozess der Installation und deinstallieren JRush auf Ihren Rechner:

.. code-block:: bash

 kevell@corp:/# ptconfigure JRush install
 Install JRush - Joomla Command Line ? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         JRush CLI !!        *
 *******************************
 What is the program data directory? Found "/opt/jrush" - use this? (Enter nothing for yes, no end slash)
 
 What is the program executor directory? Found "/usr/bin" - use this? (Enter nothing for yes, No Trailing Slash)

 git clone 'https://github.com/PharaohTools/jrush.git'  /tmp/jrush/jrushCloning into '/tmp/jrush/jrush'...
 remote: Counting objects: 3452, done.
 remote: Total 3452 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (3452/3452), 2.04 MiB | 50.00 KiB/s, done.
 Resolving deltas: 100% (2097/2097), done.
 Checking connectivity... done.
 Program Data folder populated
 Program Executor Deleted if existed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 JRush: Success
 ------------------------------
 Installer Finished
 ******************************


.. code-block:: bash

 kevell@corp:/# ptconfigure jRush uninstall
 Un Install JRush - Joomla Command Line ? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         JRush CLI !!        *
 *******************************
 What is the program data directory? Found "/opt/jrush" - use this? (Enter nothing for yes, no end slash)
 
 What is the program executor directory? Found "/usr/bin" - use this? (Enter nothing for yes, No Trailing Slash)
 
 Program Executor Deleted if existed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Uninstaller:
 ------------------------------
 JRush: Success
 ------------------------------
 Installer Finished
 ******************************



Vorteile
------------

* Dieses Modul erleichtert dem Anwender bei der Installation JRush mit der neuesten Version.
* Der Benutzer kann seinen eigenen Weg für die Programmdatenverzeichnis und Vollstrecker Verzeichnis auszuwählen.
* Die Parameter Deklaration der Hilfe verwendet und Anlagen muss nicht beachtet werden, die aufgenommen wird, während Vorteil im Vergleich zu 
  anderen.
* Es ist gut-to-do in beiden Cent OS und als auch in Ubuntu.
* Die erforderlichen Status eindeutig bei der Installation überwacht.

