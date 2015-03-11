============
Cucumber
============

Zusammenfassung
-------------------------

Dieses Modul unterstützt den Benutzer zu initialisieren und ausführen, die Gurke Testsuite. Sehen wir, wie zu initialisieren und die Gurke Testsuite in der bevorstehenden Themen durchführen.

Hilfe Befehl
--------------------

Der Befehl help führt den Anwender in Bezug auf den Zweck und die Möglichkeiten im Rahmen eines Moduls. Es listet einige der alternativen Parameter, die in der Erklärung verwendet. Es beschreibt die Syntax für zu initialisieren und die Gurke unter der pttest auszuführen. Der Befehl, um Hilfe erklärt verwendet wird nachfolgend dargestellt:

.. code-block:: bash

	pttest cucumber help

Der folgende Screenshot zeigt bildhaft über die Arbeit der Befehl help.

.. code-block:: bash

 kevell@corp:/# pttest cucumber help
 ******************************


  This command allows you to initialize a Cucumber test suite.

  Cucumber, cucumber

        - init, initialize
        Initialises the Cucumber test suite of this project
        example: pttest cucumber init
        example: pttest cucumber initialize

        - execute
        Executes the Cucumber test suite of this project
        example: pttest cucumber execute

 ------------------------------
 End Help
 ******************************

Wie Gurke initialisieren
-----------------------------------

Der Befehl für die Initialisierung der Gurke unter pttest verwendet wird angezeigt:

.. code-block:: bash

	pttest cucumber init

or 

.. code-block:: bash

	pttest cucumber initialize

Nach der Eingabe des Befehls über das Verfahren der initialize auftritt, wie in der Tabelle unten dargestellt.

.. cssclass:: table-bordered

 +-----------------------+----------------------------------+----------+------------------------------------------------------+
 | Parameters            | Alternative parameters           | Options  | Kommentare                                           |
 +=======================+==================================+==========+======================================================+
 |Initialize Cucumber?   | Statt Gurke, können wir auch     | Y(Yes)   | Wenn der Benutzer wünschen, den init sie eingeben    |
 |(Y/N)                  | mit Gurke.                       |          | können, wie Y. gehen                                 |
 +-----------------------+----------------------------------+----------+------------------------------------------------------+
 |Initialize Cucumber?   | Statt Gurke, können wir auch     | N(No)    | Wenn der Benutzer wünschen, den init-Prozess können  |
 |(Y/N)                  | mit Gurke.                       |          | sie Eingang als N. beenden|                          |
 +-----------------------+----------------------------------+----------+------------------------------------------------------+

Schließlich wird die pttest Gurke wird initialisiert, wie im folgenden Screenshot gezeigt.

.. code-block:: bash


 kevell@corp:/# pttest cucumber init
 Initialize Cucumber? (Y/N) 
 Y
 *******************************
 *   Golden Contact Computing  *
 *          Cucumber         *
 *******************************
 Creating /tmp/ptconfigure-temp-script-81470621814.sh
 chmod 755 /tmp/ptconfigure-temp-script-81470621814.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-81470621814.sh Permissions
 Executing /tmp/ptconfigure-temp-script-81470621814.sh
 Temp File /tmp/ptconfigure-temp-script-81470621814.sh Removed
 Creating /tmp/ptconfigure-temp-script-65310697385.sh
 chmod 755 /tmp/ptconfigure-temp-script-65310697385.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-65310697385.sh Permissions
 Executing /tmp/ptconfigure-temp-script-65310697385.sh
 Temp File /tmp/ptconfigure-temp-script-65310697385.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.gcsoftshop.co.uk for more
 ******************************


 Single App Installer:
 --------------------------------------------


 Cucumber: Success

 ------------------------------
 Installer Finished
 ******************************

Wie man die Gurke ausführen
----------------------------------------

Der Befehl für die Ausführung der Gurke unter pttest verwendet wird angezeigt:

.. code-block:: bash

	pttest cucumber execute

Nach der Eingabe des Befehls vor, tritt der Prozess der Ausführung wie in der Tabelle unten dargestellt.

.. cssclass:: table-bordered

 +-----------------------+-----------------------------+--------------+------------------------------------------------+
 | Parameters            | Alternative parameters      | Options      | Kommentare                                     |
 +=======================+=============================+==============+================================================+
 |Execute Cucumber?      | Statt Gurke, können wir     | Y(Yes)       | Wenn der Benutzer wünschen, die Ausführung     |
 |(Y/N)                  | auch mit Gurke.             |              | können sie Eingang als Y. gehen                |
 +-----------------------+-----------------------------+--------------+------------------------------------------------+
 |Execute Cucumber?      | Statt Gurke, können wir     | N(No)        | Wenn der Benutzer wünschen, den                |
 |(Y/N)                  | auch mit Gurke.             |              | Ausführungsprozess können sie Eingang          |
 |                       |                             |              | als N. beenden|                                |
 +-----------------------+-----------------------------+--------------+------------------------------------------------+

Wenn der Benutzer die Ausführung gehen, wird der Prozess der Ausführung auftreten, wie in der folgenden Abbildung dargestellt.

Vorteile
------------


* Es ist gut-to-do in beiden Cent OS und als auch in Ubuntu.
* Die in der Erklärung verwendet muss nicht beachtet werden, welche ein zusätzlicher Vorteil ist, während im Vergleich zu anderen Parametern.
* Dieser Gurken erlaubt den Benutzern, zu initialisieren und die Gurke Testsuite auszuführen.
