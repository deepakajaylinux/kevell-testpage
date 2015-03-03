==========
PHPUnit
==========

Zusammenfassung
-------------------------

Dieses Modul ermöglicht den Benutzern, PHPUnit aus einer GC Repo installieren. PHP Unit Testing Framework ist ein Unit Testing Framework, die Entwicklern ermöglicht, Fehler zu entdecken und damit zur Senkung der Kosten bei der Entwicklung von PHP-Software verbunden. Die PHP-Unit Testing Framework-generiert Berichte im XML-, XHTML- oder ASCII. Lassen Sie uns sehen, wie funktioniert das Modul hilft bei der Installation eines PHP-Einheit.

Hilfe Befehl
--------------------

Der Befehl help führt die Benutzer über den Zweck und als auch über die Möglichkeiten, die in der PHP-Modul-Einheit enthalten sind. Es beschreibt auch die Syntax für die Installation von PHP-Einheit. Der Befehl help für PHP Einheit Modul wird wie unten dargestellt.

.. code-block:: bash

		ptconfigure PHPUnit help

Die Syntax für die Deklaration den Befehl help ist nicht case sensitive was ein zusätzlicher Vorteil ist. Der folgende Screenshot visualisieren Sie den Befehl help unter PHP Einheit.

.. code-block:: bash

 kevell@corp:/# ptconfigure PHPUnit help
 ******************************

  This command allows you to install PHPUnit from a GC Repo.

  PHPUnit

        - install
        Installs the latest GC Repo version of PHPUnit
        example: ptconfigure phpunit install

 ------------------------------
 End Help
 ******************************

Installation
---------------

Der Befehl zum Installieren der PHP Einheit zum Benutzer Maschine verwendet wird unten gezeigt.

.. code-block:: bash

		ptconfigure PHPUnit install

Nach der Eingabe des Befehls vor, tritt die folgenden Vorgänge wie im Tabellenformat angezeigt.

.. cssclass:: table-bordered

 +---------------------------+-------------+---------------------------------------------------------+
 | Parameters                | Optionen    | Kommentare                                              |
 +===========================+=============+=========================================================+
 |Install PHPUnit? (Y/N)     | Y(Yes)      | Wenn der Benutzer wünschen, den Installationsprozess    |
 |                           |             | können sie Eingang als Y. gehen                         |
 +---------------------------+-------------+---------------------------------------------------------+
 |Install PHPUnit? (Y/N)     | N(No)       | Wenn der Benutzer wünschen, den Installationsprozess    |
 |                           |             | können sie Eingang als N. beenden|                      |
 +---------------------------+-------------+---------------------------------------------------------+


Wenn der Benutzer den Installationsprozeß schreitet die folgenden Vorgänge stattfindet, wie in der Form einer Tabelle.


.. cssclass:: table-bordered
  
 +-------------------------+-------------------------+---------------+-------------------------------------------------------------+
 | Parameters              | Weg                     | Optionen      | Kommentare                                                  |
 +=========================+=========================+===============+=============================================================+
 |Program data directory   | “/opt/phpunit           | Yes           | Wenn der Benutzer die Installation mit dem Standard-        |
 |                         | (entsprechend Modul) "  |               | Programm-Daten-Verzeichnis gehen sie eingeben kann als Ja   |
 +-------------------------+-------------------------+---------------+-------------------------------------------------------------+
 |Program data directory   | User specific           | No(End        | Wenn der Benutzer wünschen, mit ihrem eigenen Programm-     |
 |                         |                         | Schrägstrich) | Daten-Verzeichnis gehen, können diese Eingabe als N, und in |
 |                         |                         |               | die Hand geben den eigenen Standort                         |
 +-------------------------+-------------------------+---------------+-------------------------------------------------------------+
 |Program executor         | “/usr/bin”              | Yes           | Wenn der Benutzer die Installation mit dem Standardprogramm |
 |directory (default)      |                         |               | Testamentsvollstrecker Verzeichnis gehen sie eingeben kann  |
 |                         |                         |               | als Ja                                                      |
 +-------------------------+-------------------------+---------------+-------------------------------------------------------------+
 |Program executor         | User specific           | No(End        | Wenn der Benutzer mit ihren eigenen Programmausführungs     |
 |directory                |                         | Schrägstrich) | Verzeichnis fortfahren möchten, können sie Eingang als N,   |
 |                         |                         |               | und in die Hand geben sie Ort besitzen.|                    |
 +-------------------------+-------------------------+---------------+-------------------------------------------------------------+


Schließlich wird die Montage der PHP-Einheit abgeschlossen ist. Der folgende Screenshot zeigt visuell über den Prozess der Installation.

.. code-block:: bash

 kevell@corp:/# ptconfigure phpunit install
 Install PHP Unit ? (Y/N)
 Y
 *******************************
 *        Pharaoh Tools        *
 *          PHP Unit !         *
 *******************************
 What is the program data directory? Found "/opt/phpunit" - use this? (Enter nothing for yes, no end slash)

 What is the program executor directory? Found "/usr/bin" - use this? (Enter nothing for yes, No Trailing Slash)

 git clone -b 3.5 'https://github.com/sebastianbergmann/phpunit.git'  /tmp/phpunit/phpunitCloning into '/tmp/phpunit/phpunit'...

 remote: Counting objects: 50529, done.
 Receiving objects:  71% (35876/50529), 12.02 MiB | 41.00 KiB/s
 Receiving objects:  95% (48003/50529), 16.82 MiB | 38.00 KiB/s
 Receiving objects:  95% (48254/50529), 16.86 MiB | 40.00 KiB/s
 Receiving objects:  96% (48508/50529), 16.95 MiB | 43.00 KiB/s



 remote: Total 50529 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (50529/50529), 17.91 MiB | 36.00 KiB/s, done.
 Resolving deltas: 100% (26834/26834), done.
 Checking connectivity... done.
 git clone -b 1.0 'https://github.com/sebastianbergmann/dbunit.git'  /tmp/phpunit/dbunitCloning into '/tmp/phpunit/dbunit'...
 remote: Counting objects: 4596, done.
 remote: Total 4596 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (4596/4596), 1.04 MiB | 31.00 KiB/s, done.
 Resolving deltas: 100% (3183/3183), done.
 Checking connectivity... done.
 git clone -b 1.2 'https://github.com/sebastianbergmann/php-file-iterator.git'  /tmp/phpunit/php-file-iteratorCloning into '/tmp/phpunit/php-file-iterator'...
 remote: Counting objects: 453, done.
 remote: Total 453 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (453/453), 60.66 KiB | 16.00 KiB/s, done.
 Resolving deltas: 100% (188/188), done.
 Checking connectivity... done.
 git clone -b 1.0 'https://github.com/sebastianbergmann/php-code-coverage.git'  /tmp/phpunit/php-code-coverageCloning into '/tmp/phpunit/php-code-coverage'...
 remote: Counting objects: 7650, done.
 remote: Total 7650 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (7650/7650), 2.77 MiB | 17.00 KiB/s, done.
 Resolving deltas: 100% (3671/3671), done.
 Checking connectivity... done.
 git clone -b 1.0 'https://github.com/sebastianbergmann/php-token-stream.git'  /tmp/phpunit/php-token-streamCloning into '/tmp/phpunit/php-token-stream'...
 remote: Counting objects: 1234, done.
 remote: Total 1234 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (1234/1234), 201.76 KiB | 41.00 KiB/s, done.
 Resolving deltas: 100% (565/565), done.
 Checking connectivity... done.
 git clone -b 1.0 'https://github.com/sebastianbergmann/phpunit-mock-objects.git'  /tmp/phpunit/phpunit-mock-objectsCloning into '/tmp/phpunit/phpunit-mock-objects'...
 remote: Counting objects: 4703, done.
 remote: Total 4703 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (4703/4703), 837.24 KiB | 104.00 KiB/s, done.
 Resolving deltas: 100% (2910/2910), done.
 Checking connectivity... done.
 git clone -b 1.0 'https://github.com/sebastianbergmann/phpunit-selenium.git'  /tmp/phpunit/phpunit-seleniumCloning into '/tmp/phpunit/phpunit-selenium'...
 remote: Counting objects: 8115, done.
 remote: Total 8115 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (8115/8115), 2.07 MiB | 28.00 KiB/s, done.
 Resolving deltas: 100% (4762/4762), done.
 Checking connectivity... done.
 git clone 'https://github.com/phpengine/ptconfigure-phpunit-php-timer'  /tmp/phpunit/php-timerCloning into '/tmp/phpunit/php-timer'...
 remote: Counting objects: 253, done.
 remote: Total 253 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (253/253), 31.55 KiB | 12.00 KiB/s, done.
 Resolving deltas: 100% (126/126), done.
 Checking connectivity... done.
 git clone 'https://github.com/sebastianbergmann/php-text-template.git'  /tmp/phpunit/php-text-templateCloning into '/tmp/phpunit/php-text-template'...
 remote: Counting objects: 209, done.
 remote: Total 209 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (209/209), 33.69 KiB | 16.00 KiB/s, done.
 Resolving deltas: 100% (92/92), done.
 Checking connectivity... done.
 Program Data folder populated
 Program Executor Deleted if existed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 PHPUnit35: Success
 ------------------------------
 Installer Finished
 ******************************

Vorteile
------------

* Dieses Modul ermöglicht den Anwender bei der Installation von PHP-Einheit aus der GC-Repo-Version.
* Der Benutzer kann seinen eigenen Weg für die Programmdatenverzeichnis und Vollstrecker wählen
* Die Parameter Deklaration der Hilfe verwendet und Anlagen muss nicht beachtet werden, die aufgenommen wird, während Vorteil im Vergleich zu 
  anderen.
* Es ist gut-to-do in beiden Cent OS und als auch in Ubuntu.

