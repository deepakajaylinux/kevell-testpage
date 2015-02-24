===============
Mysqlserver
===============

Zusammenfassung
----------------------

Dieses Modul fungiert als Vermittler, um MySQL-Server mit der aktualisierten Version über apt-get install. Wenn der MySQL-Server in Ihrer Maschine bereits vorhanden ist, wird es überprüft die Verfügbarkeit der neu aktualisierte Modul.

Der Befehl help
--------------------

Der Befehl help führt den Anwender in Bezug auf die Methodik in der Nutzung sowie über die Maßnahmen, die im Rahmen dieser Module durchgeführt werden können. Es beschreibt auch die alternative Namen für die mysql-server. Der Befehl für die Verwendung von Hilfe-Option ist unten angegeben

.. code-block:: bash

	ptconfigure  mysql-server help

Dieser Befehl erlaubt den Benutzern, sich seiner Aufgabe und auch über den Befehl für die Installation der MySQL-Server verwendet wird.

Der Screenshot unten angegeben eine bildliche Darstellung über den Befehl Hilfe.

.. code-block:: bash


 kevell@corp:/# ptconfigure  MysqlServer help
 ******************************


  This command allows you to install the MySQL Server. Currently only
  Mysql Workbench, the Database management GUI provided by Oracle for
  Mysql.

  MysqlServer, mysql-server, mysqlserver

        - install
        Install some Mysql Server Tools through apt-get.
        example: ptconfigure  mysql-server install

  Notes, during mysql install a root password will be set. First, it'll look
  for the parameter --mysql-root-pass, if this is not set, it'll look in the
  ptconfigure  config for a mysql-default-root-pass setting, and failing both of
  those it will just set the password for root to ptconfigure .

 ------------------------------
 End Help
 ******************************

Installation
--------------

Der Befehl für die Installation der MySQL-Server verwendet, wird unten gegeben.

.. code-block:: bash

	ptconfigure  mysql-server install

Während der Installation wird der folgende Prozess
---------------------------------------------------------

* Dieses Modul hilft, einige Werkzeuge für MySQL-Server via installieren apt-get.
* Zunächst wird ein Root-Passwort gesetzt.
* Bei der Installation, wird es für einen Parameter --mysql-root Pass suchen.
* Wenn die --mysql-root Pass nicht verfügbar ist, wird sie die Kleopatra Config für die Einstellungen der mysql-default-root Pass suchen.
* Bei den beiden oben genannten Schritte wird versagt, wird es, indem Sie root-Passwort zu Kleopatra gehen.

Zusätzliche Optionen
------------------------

Lassen Sie uns über, die zusätzliche Optionen bei der Installation der MySQL-Server beteiligt sehen.

.. cssclass:: table-bordered

 +--------------------------+-------------------------------------------------+------------+------------------------------------------+
 | Parameters               | Verzeichnis (Standard)                          | Optionen   | Kommentare                               |
 +==========================+=================================================+============+==========================================+
 |Install MySQL Server?     | An der Stelle MySQL Server diese alternative    | Y(Yes)     | Wenn der Benutzer wünschen, den          |
 |(Y/N)                     | Namen können verwendet werden: MysqlServer,     |            | Installationsprozess können sie Eingang  |
 |                          | mysql-server, mysqlserver.                      |            | als Y. gehen                             |
 +--------------------------+-------------------------------------------------+------------+------------------------------------------+
 |Install MySQL Server?     | An der Stelle MySQL Server diese alternative    | N(No)      | Wenn der Benutzer wünschen, den          |
 |(Y/N)                     | Namen können verwendet werden: MysqlServer,     |            | Installationsprozess können sie Eingang  |
 |                          | mysql-server, mysqlserver.                      |            | als N beenden|                           |
 +--------------------------+-------------------------------------------------+------------+------------------------------------------+


Der folgende Screenshot gibt Ihnen eine grafische Darstellung über den Installationsprozess.


Wenn der MySQL-Server gibt es in Ihrem Computer bereits, dann wird es eine Meldung an den Benutzer zu werfen, wie es bereits installiert ist. Der folgende Screenshot stellt den Prozess der Sicherstellung:



Vorteile
----------

* Bei der Installation der MySQL-Server, installiert es mit der aktualisierten Version.
* Es sorgt dafür, vor der Installation, und überprüfen Sie die Verfügbarkeit von Modulen.
* Im Falle von neuen Modulen in der aktualisierten Version enthalten ist, wird das fehlende Modul einzeln installiert werden.
* Es prüft die Verfügbarkeit der Bibliotheksfunktionen in der MySQL-Server.
