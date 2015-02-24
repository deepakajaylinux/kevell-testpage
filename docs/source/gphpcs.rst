==========
PHPCS
==========

Zusammenfassung
------------------------

Dieses Modul hilft bei der Installation von PHP cs von GC Repo. Bei der Installation, holt dieses Modul die neueste Version. Der Benutzer kann den Speicherort für die Programmdatenverzeichnis und Vollstrecker Verzeichnis angeben. Schließlich Ergebnisse sind klar ausgewiesen.

Hilfe Befehl
-------------

Der Befehl help führt die Benutzer über den Zweck und als auch über die Möglichkeiten, die in der PHP-cs-Modul enthalten sind. Es beschreibt auch die Syntax für die Installation von PHP-cs. Der Befehl help für php cs ist unten angegeben.

.. code-block:: bash

	ptconfigure PHPCS help

Die Syntax für die Deklaration den Befehl help ist nicht case sensitive was ein zusätzlicher Vorteil ist. Der folgende Screenshot visualisieren Sie den Befehl help unter PHPCS.

.. code-block:: bash

 kevell@corp:/# ptconfigure PHPCS help
 ******************************


 This command allows you to install PHPCS from a GC Repo.

 PHPCS
 - install
 Installs the latest version of PHPCS
 example: ptconfigure phpcs install

 ------------------------------
 End Help
 ******************************

Installation
-------------

Installieren des PHP CS ist einfacher, indem Sie den folgenden Befehl ein, wie gezeigt:

.. code-block:: bash
	
	ptconfigure PHPCS install

Nach der Eingabe des Befehls über die folgenden Vorgänge, wie gezeigt in der Tabellenform auf.

.. cssclass:: table-bordered

 +-----------------------+-------------+---------------------------------------------------------------------+
 | Paramaters            | Optionen    |  Kommentare                                                         |
 +=======================+=============+=====================================================================+
 |Install PHP Code       | Y(Yes)      | Wenn der Benutzer wünschen, den Installationsprozess können         |
 |Sniffer ? (Y/N)        |             | sie Eingang als Y. gehen                                            |
 +-----------------------+-------------+---------------------------------------------------------------------+
 |Install PHP Code       | N(No)       | Wenn der Benutzer wünschen, den Installationsprozess können         |
 |Sniffer ? (Y/N)        |             | sie Eingang als N. beenden|                                         |
 +-----------------------+-------------+---------------------------------------------------------------------+


Wenn der Benutzer den Installationsprozeß schreitet die folgenden Vorgänge stattfindet, wie in der Form einer Tabelle.

.. cssclass:: table-bordered

 +-----------------------+--------------------------+--------------+-----------------------------------------------------+
 | Paramaters            | Weg                      | Optionen     | Kommentare                                          |
 +=======================+==========================+==============+=====================================================+
 |Program data           | opt/phpcs (entsprechend  | Yes          | Wenn der Benutzer der Installation fortzufahren     |
 |directory(Default)     | Modul)”                  |              | mit dem Standard-Programm-Datenverzeichnis können   |
 |                       |                          |              | sie Eingang als Ja                                  |
 +-----------------------+--------------------------+--------------+-----------------------------------------------------+
 |Program data directory | User specific            | No(End       | Wenn der Benutzer mit ihren eigenen                 |
 |                       |                          | Slash)       | Programmdatenverzeichnis fortfahren möchten, können |
 |                       |                          |              | sie Eingang als N, und in die Hand geben sie Ort    |
 |                       |                          |              | besitzen.                                           |
 +-----------------------+--------------------------+--------------+-----------------------------------------------------+
 |Program executor       | “/usr/bin”               | Yes          | Wenn der Benutzer die Installation mit dem          |
 |directory (Default)    |                          |              | Standardprogramm Testamentsvollstrecker Verzeichnis | 
 |                       |                          |              | gehen sie eingeben kann als Ja                      |
 +-----------------------+--------------------------+--------------+-----------------------------------------------------+
 |Program executor       | User specific            | No (End      | Wenn der Benutzer mit ihren eigenen                 |
 |directory              |                          | Slash)       | Programmausführungs Verzeichnis fortfahren möchten, |
 |                       |                          |              | können sie Eingang als N, und in die Hand geben     |
 |                       |                          |              | sie Ort besitzen.|                                  |
 +-----------------------+--------------------------+--------------+-----------------------------------------------------+


Nach diesen Verfahren in der Form einer Tabelle, die Ergebnisse deutlich zusammen mit dem Status berichtet. Der folgende Screenshot erklärt grafisch über den Prozess in die Installation von PHPCS beteiligt.

.. code-block:: bash

 Kevell@corp:/# ptconfigure PHPCS install
 Install PHP Code Sniffer ? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         PHP CSniffer        *
 *******************************
 What is the program data directory? Found "/opt/phpcs" - use this? (Enter nothing for yes, no end slash)
 
 What is the program executor directory? Found "/usr/bin" - use this? (Enter nothing for yes, No Trailing Slash)

 git clone 'https://github.com/phpengine/ptconfigure-phpcs.git'  /tmp/phpcs/phpcsCloning into '/tmp/phpcs/phpcs'...
 remote: Counting objects: 862, done.
 remote: Total 862 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (862/862), 491.23 KiB | 64.00 KiB/s, done.
 Resolving deltas: 100% (378/378), done.
 Checking connectivity... done.
 Program Data folder populated
 Program Executor Deleted if existed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 PHPCS: Success
 ------------------------------
 Installer Finished
 ****************************


Vorteile
-----------

* Dieses Modul ermöglicht den Anwender bei der Installation von PHP CS mit der aktualisierten Version.
* Der Benutzer kann seinen eigenen Weg für die Programmdatenverzeichnis und Vollstrecker wählen
* Die Parameter Deklaration der Hilfe verwendet und Anlagen muss nicht beachtet werden, die aufgenommen wird, während Vorteil im Vergleich zu 
  anderen.


