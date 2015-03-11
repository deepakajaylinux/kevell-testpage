==============
DBInstall
==============

Zusammenfassung
-----------------------

Dbinstall Modul hilft im Umgang mit Datenbank-Installation funktioniert. Dieser Befehl verwendet werden, um eine neue Datenbank zu installieren. Die Installation erfordert sudo-Zugriff, oder als root ausgeführt werden hat. Dies beinhaltet die Ausführung des Befehls rpm oder die miminstall Befehl des tar-Paket, und auch bei der Verwendung der dbinstall Befehl, der eine erste Datenbank erstellt.

Beim Erstellen einer anfänglichen Datenbank, die Software können Sie eine Mimer SQL-Datenbank mit Hilfe des Befehls dbinstall bauen installiert haben.

Wir haben gerade installiert eine neue Datenbank auf einem Linux (CentOS) Server und wenn ich versuche, auf die Datenbank (auf dem Server) verbinden Sie den Namen der Datenbank in der Verbindungszeichenfolge erfordert. Wie bereits erwähnt, die dbinstall Befehl sudo-Zugriff benötigt oder muss von root ausgeführt werden. Wenn nicht von einer privilegierten Shell sudo Passwort gestartet werden gefragt.

Während der Sitzung dbinstall, Datenbankname, Datenbankposition, und das Kennwort für den Datenbankadministrator (dh SYSADM) festgelegt werden. Es gibt auch Optionen für die Installation beispielsweise Umgebungen usw. Wenn die Sitzung abgeschlossen ist, ist eine voll funktionsfähige Datenbank verfügbar - für Client / Server-Zugriff über TCP und automatischer Start beim Neustart aktiviert.

Hilfe Befehl
----------------------

Diese Funktion dient, um die Verwendung von DBinstall Modul bestimmen. Der Benutzer wird kommen, um über die verschiedenen Möglichkeiten / Format um dieses Modul ausführen kennen. Dieser Befehl leitet den Anwender, um den Zweck dieses Befehls kennen. Da unten sind die Befehls- und die Screenshot der gleiche.

.. code-block:: bash
	
	ptdeploy DBInstall help
       
The pictorial representation of the above command is shown below,

.. code-block:: bash

 kevell@corp:/# ptdeploy DBInstall help
 ******************************


  Dieser Befehl ist Teil der Standard-Module und Griffe Installation der Datenbank-Funktionen.
  DBInstall, db-install, dbinstall

          - install
          install the database for a project. run DBConfigure first to set up users unless you already have them.
          example: ptdeploy db-install install

          - save
          save the database for a project. run DBConfigure first to set up users unless you already have them.
          example: ptdeploy db-install save

          - drop
          drop the database for a project.
          example: ptdeploy db-install drop

      
 --------------
  Wordpress Module:

  The Wordpress module extends DBInstall by adding wordpress-install

  Wordpress module adds the actions wordpress-install and wp-install to DBInstall, requiresd to allow the Post DB
  Install hooks for Wordpress, the DB restore won't work correctly without at least the url.

  ptdeploy dbinstall wordpress-install --yes --guess --hook-url=www.site.env
 ------------------------------
 End Help
 ******************************







Installation
----------------

Wenn der Benutzer zu installieren muss, kann der Benutzer die folgenden Befehle für DBIstall ausgeben. Das System wird den Prozess der Installation durchzuführen.
.. code-block:: bash
	
	 ptdeploy dbinstall install

Das System fordern Sie die MySQL-Host, Drücken Sie die Eingabetaste, um den Standard-Host zu verwenden.

.. code-block:: bash

 What's the Mysql Host? Enter for 127.0.0.1


Dann wird das System fordern Mysql Admin-Benutzer, wird die Benutzernamen "root" und die der MySQL-Admin-Kennwort ist.

.. code-block:: bash

 What's the MySQL Admin User?
 root
 What's the MySQL Admin Password?
 123456

 
Dann wird das System fragen, für die Anwendung DB Benutzer, können Sie mit den vorhandenen Benutzern weiter oder erstellen Sie einen neuen Benutzer. Sobald Sie mit der Option "0" für neue Benutzer zu liefern das System fragen Sie nach dem neuen Benutzernamen, Passwort und Anwendung DB Anwendung DB Namen.

.. code-block:: bash



Sobald die oben genannten Angaben, das System nach Bestätigung. Nach der Bestätigung, führen Sie das System den Vorgang.

.. code-block:: bash



Speichern
----------------

Wenn der Benutzer auf die Datenbank für ein Projekt zu speichern muss, wird der unten angegebenen Befehl den Prozess auszuführen.

.. code-block:: bash
	
	ptdeploy dbinstall save	

Vor der Ausführung ist das System fragen Sie nach der Bestätigung, um fortzufahren, wenn Sie fortfahren 'J' eingeben möchten, wenn keine geben 'N'.

.. code-block:: bash

Das System fordern Sie die MySQL-Host, Drücken Sie die Eingabetaste, um den Standard-Host zu verwenden.

.. code-block:: bash

 What's the Mysql Host? Enter for 127.0.0.1


Then the system ask for Mysql Admin user, the user name will be “root” and the the Mysql Admin password.

.. code-block:: bash

 What's the MySQL Admin User?
 root
 What's the MySQL Admin Password?
 123456

 
Then the system ask for the application DB user. 

.. code-block:: bash

Fallen Lassen
----------------

Wenn der Benutzer auf die Datenbank für ein Projekt fallen muss, wird die unten gegebenen Befehl das Verfahren auszuführen.

.. code-block:: bash
	
	ptdeploy dbinstall drop      

Vor der Ausführung ist das System fragen Sie nach der Bestätigung, um fortzufahren, wenn Sie fortfahren 'J' eingeben möchten, wenn keine geben 'N'.

.. code-block:: bash

Das System fordern Sie die MySQL-Host, Drücken Sie die Eingabetaste, um den Standard-Host zu verwenden.

.. code-block:: bash

 What's the Mysql Host? Enter for 127.0.0.1


Dann wird das System fordern Mysql Admin-Benutzer, wird die Benutzernamen "root" und die der MySQL-Admin-Kennwort ist.

.. code-block:: bash

 What's the MySQL Admin User?
 root
 What's the MySQL Admin Password?
 123456

 
Dann wird das System fragen, für die Anwendung DB Benutzer.

.. code-block:: bash

Alternative Parameter
------------------------------

Entweder der drei alternativen Parameter kann in Befehls verwendet werdendbinstall, DBInstall and db-install

eg: ptdeploy DBInstall help/  ptdeploy db-install help                 

Vorteile
--------------

* Es wird zu überprüfen und überprüfen Sie die Abhängigkeiten für das Paket es installieren
* Dieser läuft dbconfigure zuerst die Einrichtung von Benutzern, wenn das System bereits haben
* Dbinstall erstellt alle Systemdatenbanken in der angegebenen Datenbankserver Home-Verzeichnis
