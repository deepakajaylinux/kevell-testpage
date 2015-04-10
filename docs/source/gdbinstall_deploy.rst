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

.. code-block:: bash


 kevell@corp:/# ptdeploy DBInstall install
 Do you want to install a database? (Y/N) 
 y
 What's the Mysql Host? Enter for 127.0.0.1 

 What's the MySQL Admin User? 

 You must enter a value. Please try again.
 What's the MySQL Admin User?

 You must enter a value. Please try again.
 What's the MySQL Admin User?
 root
 What's the MySQL Admin Password?
 root
 What's the application DB User?
 (0) **CREATE NEW USER** 
 (1) phpci 
 (2) debian-sys-maint 
 (3) phpci 
 (4) phpmyadmin 
 1
 What's the application DB Password?
 phpci_pass
 What's the application DB Name?
 Current Db's are:
 hps
 phpci
 phpmyadmin

 phpci
 Database script executed
 **************************************
 Seems Fine...Database Actions Finished
 **************************************



Save
----------------

Wenn der Benutzer auf die Datenbank für ein Projekt zu speichern muss, wird der unten angegebenen Befehl den Prozess auszuführen.

.. code-block:: bash
	
	ptdeploy dbinstall save	

.. code-block:: bash

 kevell@corp:/# ptdeploy DBInstall save
 Do you want to save a database? (Y/N) 
 y
 What's the Mysql Host? Enter for 127.0.0.1

 What's the MySQL Admin User?
 root
 What's the MySQL Admin Password?
 root
 What's the application DB Name?
 Current Db's are:
 asdf
 hps
 phpci 

 asdf
 Cannot connect with these details. Sure you want to continue? (Y/N) 
 y
 Exporting DB to /opt/db/database.sql 
 Database Dumping...
 **************************************
 Seems Fine...Database Actions Finished
 ************************************** 




Drop
----------------

Wenn der Benutzer auf die Datenbank für ein Projekt fallen muss, wird die unten gegebenen Befehl das Verfahren auszuführen.

.. code-block:: bash
	
	ptdeploy dbinstall drop      

.. code-block:: bash


 kevell@corp:/# ptdeploy db-install drop 

 Do you want to perform drop actions (user/db)? (Y/N) 
 y
 Do you want to drop a database? (Y/N) 
 y
 What's the Mysql Host? Enter for 127.0.0.1 

 What's the MySQL Admin User?
 root
 What's the MySQL Admin Password?
 root123
 What's the application DB Name?
 (0) karuna 
 (1) test1 
 (2) test2 
 2
 Database test2 dropped
 **************************************
 Seems Fine...Database Actions Finished
 **************************************




Alternative Parameter
------------------------------

Entweder der drei alternativen Parameter kann in Befehls verwendet werdendbinstall, DBInstall and db-install

eg: ptdeploy DBInstall help/  ptdeploy db-install help                 

Vorteile
--------------

* Es wird zu überprüfen und überprüfen Sie die Abhängigkeiten für das Paket es installieren
* Dieser läuft dbconfigure zuerst die Einrichtung von Benutzern, wenn das System bereits haben
* Dbinstall erstellt alle Systemdatenbanken in der angegebenen Datenbankserver Home-Verzeichnis
