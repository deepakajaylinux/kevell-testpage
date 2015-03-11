============
DBConfigure
============


Zusammenfassung
-----------------

Diese Module Moniker Datenbankfunktion. Die Konfiguration kann aus dieser Datenbank abgeleitet werden können in der gleichen Baugruppe als von DbContext abgeleitet zu Entity Framework-Konfiguration für eine Anwendung definieren Datenbank gespeichert. Die Konfiguration erfolgt durch den Aufruf geschützten Methoden und Einrichtung geschützter Eigenschaften dieser Datenbank im Konstruktor der abgeleiteten Typ Benutzers festgelegt. Die Art zu verwenden, auch in der Konfigurationsdatei der Anwendung gespeichert werden. Dies ist ausreichend, mit Ubuntu und CentOS.


Hilfe Befehl
-----------------------

Der Befehl help führt den Benutzer zu Datenbank in ptdeploy behandeln. Dieser Befehl help führt den Benutzer, um eine conf erstellen. Dieser Reset auch die aktuelle Datenbank. Datenbanken werden verwendet, um interne Abläufe von Organisationen zu unterstützen und Online-Interaktionen mit Kunden und Lieferanten zu untermauern. Der Befehl help für dbconfigure ist nachfolgend dargestellt.

.. code-block:: bash
	
	ptdeploy  DBConfigure help

Nach Eingang der obige Befehl, beginnt es funktioniert, um Datenbank zu handhaben. Es Katechese die Funktionen in den Screenshots.
  Der folgende Screenshot zeigt etwa DBConfigure.

.. code-block:: bash

 kevell@corp:/# ptdeploy DBConfigure help
 ******************************


 Dieser Befehl ist Teil der Standard-Module und Griffe Databasing Funktionen.
  DBConfigure, db-configure, dbconfigure, db-conf

      - configure, conf
      set up db user & pw for a project, use admins to create new resources as needed.
      example: ptdeploy db-conf conf drupal
      example: ptdeploy db-conf conf --yes --platform=joomla30 --mysql-host=127.0.0.1 --mysql-admin-user="" --mysql-user="impi_dv_user" --mysql-pass="impi_dv_pass" --mysql-db="impi_dv_db"

      - reset
      reset current db to generic values so ptdeploy can write them. may need to be run before db conf.
      example: ptdeploy db-conf reset drupal
      example: ptdeploy db-conf reset --yes --platform=joomla30


Alternative Parameter
-----------------------------------

Es gibt viele Alternativen in DBConfigure. Jede Alternative zeigt eine weitere Vorteile zu diesen Modulen. Sie sind,

DBConfigure, db-configure, dbconfigure, db-conf.

Configure, conf
-----------------------

This process set up database user  and passward for a project. Also use admin to create new resources if they need . The following screen shot shows its function.

.. code-block:: bash

      - configure, conf
      set up db user & pw for a project, use admins to create new resources as needed.
      example: ptdeploy db-conf conf drupal
      example: ptdeploy db-conf conf --yes --platform=joomla30 --mysql-host=127.0.0.1 --mysql-admin-user="" --mysql-user="impi_dv_user" --m	     ysql-pass="impi_dv_pass" --mysql-db="impi_dv_db"


Mit dem folgenden Befehl zur Konfiguration.

.. code-block:: bash

	ptdeploy  db-conf Conf

Nach dem Schlüssel in der oben genannten Befehl kann das folgende Verfahren funktioniert werden. Es hat sich in den Screenshots gezeigt.

Nach Eingang als '' Y ", fragt Sie MySQL-Benutzer admin, Mysql Host, Anwendung Db Benutzer und Anwendung db-Passwort, Db Namen. Der Benutzer gibt die Eingabe für diese diesen Vorgang zu starten Funktionen

rücksetzen
------------

Dieses Verfahren, das zur aktuellen Datenbank zu generischen Werte zurückzusetzen. In solchen Fällen kann ptdeploy vor Laufdatenbankkonfiguration zu schreiben. Der Name der Datenbank eingegeben in derselben Zeile selbst sein.

Der folgende Befehl verwendet werden, um zurückzusetzen.

.. code-block:: bash

	ptdeploy  db-conf reset


Der folgende Screenshot zeigt die Funktion dieses Prozesses.

.. code-block:: bash

      - reset
      reset current db to generic values so ptdeploy can write them. may need to be run before db conf.
      example: ptdeploy db-conf reset drupal
      example: ptdeploy db-conf reset --yes --platform=joomla30



Option
---------------

.. cssclass:: table-bordered


 +--------------------------------------------+----------+------------------------------------------------+
 | Parameters                                 | Option   | Kommentare                                     |
 +============================================+==========+================================================+
 |Do you want to configure a database?(Y/N)   | Yes      | Konfiguriert die Datenbank undder ptdeploy.    |
 +--------------------------------------------+----------+------------------------------------------------+
 |Do you want to configure a database?(Y/N)   | No       | Verlassen Sie das Konfigurationsfenster|       |
 +--------------------------------------------+----------+------------------------------------------------+



Vorteile
--------------

* Der Advantage Database config ist ein hochleistungsfähiges, wartungsarme, Remote-Datenbank-Konfiguration, die es dem Benutzer ermöglicht die 
  einfache Erstellung und implementieren Client / Server-Anwendungen und Web-basierte Anwendungen.
* Es ist benutzerfreundlich mit Ubuntu und CentOS.
* Nicht Groß- und Kleinschreibung ist ein großes Verdienst für dieses Modul
* Es unterstützt die Standardschnittstellen wie PHP
* Es ist leicht, mit Datenbank-Funktionen verarbeiten
