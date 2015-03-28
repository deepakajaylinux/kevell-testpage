===============
Appsettings
===============

Zusammenfassung
-----------------

AppSetting dass erlaubt uns, konfigurierbare und anwendungsweite Einstellungen , die eine Anwendung benötigt , um die Aufgaben richtig ausführen zu halten. Dies hilft bei der einfachen Wartung und Bereitstellung der Anwendung . Durch die Verwendung von Appsetting können wir benutzerdefinierte Werte zu definieren.

Hilfe Befehl
------------------

Diese Funktion dient , um die Verwendung von appsettings bestimmen. Es listet einige der alternativen Parameter und Syntax für die Funktionsfähigkeit appsettings Modul . Der Befehl help für appsettings wird wie unten dargestellt.


.. code-block:: bash

	ptdeploy appsettings help

Die bildliche Darstellung der Hilfebefehl ist unten angegeben ,


.. code-block:: bash


 kevell@corp:/# ptdeploy appsettings help

 ******************************


  This command is part of Default Modules and provides you  with a method by which you can configure Application Settings.
  You can configure default application settings, ie: mysql admin user, host, pass

  AppSettings, appsettings
	
        - set
        Set a configuration value
        example: ptdeploy appsettings set

        - get
        Get the value of a setting you have configured
        example: ptdeploy appsettings get

        - delete
        Delete a setting you have configured
        example: ptdeploy appsettings delete

        - list
        Display a list of all default available settings
        example: ptdeploy appsettings list

 ------------------------------
 End Help
 ******************************


Set
---------

Der Befehl set hilft, einen Konfigurationswert eingestellt . Die folgende Aufruf den Prozess auszuführen .

.. code-block:: bash

	ptdeploy appsettings set

Die bildliche Darstellung der obigen Befehl aufgelistet unten ,


.. code-block:: bash

 kevell@corp:/# ptdeploy appsettings set

 Do you want to Configure Application Settings? (Y/N) 
 y
 What's the App Config Variable?

 (0) **ENTER PLAIN TEXT** 
 (1) mysql-admin-user 
 (2) mysql-admin-host 
 (3) mysql-admin-pass 
 (4) linux-user 
 (5) linux-user-dir 
 (6) program-dir 
 (7) temp-base-dir 
 (8) distro 
 (9) op-sys 
 (10) linux-type 
 5
 What Value do you want to give this variable?
 /tmp/
 ******************************

 Seems Fine...
 In Application Config
 ******************************


Get
--------

Die Get -Befehl hilft, den Wert einer Einstellung Sie bereits konfiguriert haben zu bekommen. Die folgende Aufruf den Prozess auszuführen .


.. code-block:: bash

	ptdeploy appsettings get


Die bildliche Darstellung der obigen Befehl aufgelistet unten ,

.. code-block:: bash

 kevell@corp:/# ptdeploy appsettings get

 Do you want to Configure Application Settings? (Y/N) 
 y
 What's the App Config Variable?

 (0) **ENTER PLAIN TEXT** 
 (1) mysql-admin-user 
 (2) mysql-admin-host 
 (3) mysql-admin-pass 
 (4) linux-user 
 (5) linux-user-dir 
 (6) program-dir 
 (7) temp-base-dir 
 (8) distro 
 (9) op-sys 
 (10) linux-type 
 4
 ******************************


 Variable Name: linux-user
 Variable Value: karuna
 
 In Application Config
 ******************************


Delete
--------

Der Löschbefehl hilft , um eine Einstellung von Ihnen konfigurierten löschen. Die folgende Aufruf den Prozess auszuführen.

.. code-block:: bash

	ptdeploy appsettings delete

Die bildliche Darstellung der obigen Befehl aufgelistet unten ,

.. code-block:: bash


 kevell@corp:/# ptdeploy appsettings delete

 Do you want to Configure Application Settings? (Y/N) 
 y
 What's the App Config Variable?

 (0) **ENTER PLAIN TEXT** 
 (1) mysql-admin-user 
 (2) mysql-admin-host 
 (3) mysql-admin-pass 
 (4) linux-user 
 (5) linux-user-dir 
 (6) program-dir 
 (7) temp-base-dir 
 (8) distro 
 (9) op-sys 
 (10) linux-type 
 5
 ******************************


 Seems Fine...
 In Application Config
 ******************************



List
-------

The list command helps to display a list of all default available settings. The below commad will execute the process.


.. code-block:: bash

	ptdeploy appsettings list

Die Befehlsliste hilft, eine Liste aller verfügbaren Standardeinstellungen anzuzeigen. Die folgende commad wird den Prozess auszuführen.


.. code-block:: bash

 kevell@corp:/# ptdeploy appsettings list

 Do you want to Configure Application Settings? (Y/N) 
 y
 ******************************


   Variable Type is: allSet 
   linux-user is: karuna 
   mysql-admin-user is: mani 
   Variable Type is: allTotal 
   mysql-admin-user 
   mysql-admin-host 
   mysql-admin-pass 
   linux-user 
   linux-user-dir 
   program-dir 
   temp-base-dir 
   distro 
   op-sys 
   linux-type 

 In Application Config
 ******************************



Alternative Parameter
--------------------------

Es gibt zwei alternative Parameter, die in der Befehlszeile verwendet werden kann.

AppSettings, appsettings


Vorteile
-----------

* Stark typisierten Zugriff
* Nicht Groß- und Kleinschreibung
