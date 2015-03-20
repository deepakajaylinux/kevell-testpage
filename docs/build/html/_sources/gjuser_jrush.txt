==============
JUser
==============

Zusammenfassung
---------------------

Ein Benutzer ist eine Person, die ein Computer oder Netzwerk-Dienst verwendet. Benutzer verwenden in der Regel ein System oder ein Software-Produkt ohne das Fachwissen benötigt, um es vollständig zu verstehen.


Ein Benutzer hat ein Benutzerkonto häufig und wird auf das System durch einen Benutzernamen (oder Benutzernamen) identifiziert. Andere Begriffe für Benutzernamen enthalten Login-Namen, Benutzernamen.


Das Konto eines Benutzers ermöglicht einem Benutzer, um ein System zu authentifizieren und Autorisierung Zugriff auf Ressourcen durch oder an das System angeschlossenen gewährt werden; Authentifizierung bedeutet jedoch keine Genehmigung. Um sich ein Konto anzumelden, wird ein Benutzer in der Regel benötigt, um sich mit einem Kennwort oder andere Anmeldeinformationen für die Zwecke der Rechnungslegung, Sicherheit, Protokollierung und Ressourcenmanagement zu authentifizieren.


Hilfe Befehl
----------------------

Dieser Befehl hilft, die Verwendung von Juser Modul bestimmen. Der Benutzer wird kommen, über die verschiedenen Möglichkeiten/Format wissen, dieses Modul ausgeführt. Dieser Befehl führt den Endbenutzer, um diesen Befehl zu erfahren. Im folgenden sind mit dem Befehl und der Screenshot von der gleichen.



.. code-block:: bash
        
	jrush juser help

.. code-block:: bash

 kevell@corp:/# jrush juser help
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

  This command allows you to update JUser.

  JUser, juser

        - delete
        Deletes a user
        example: jrush juser delete

        - info
        Display the details of a user
        example: jrush juser info

        - change the password of a user
        Change a users password
        example: jrush juser password

 ------------------------------
 End Help
 ****************************************




Delete
----------------

Wenn der Benutzer zum Löschen eines Benutzers in der Maschine muss, die unten mit dem Befehl wird ausgeführt, den Prozess der Installation.


.. code-block:: bash
        
	jrush juser delete ..config file=”bootstrap file path”

Die bildliche Darstellung der oben genannte Befehl ist im folgenden aufgeführt,


.. code-block:: bash

 kevell@corp:/# jrush juser delete --config-file="/var/www/html/joomla/configuration.php"
 Enter a JUser ID. To enter email/username use --user-email or --username parameters
 2
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

 JUser Delete:
 -------------------------

 The following user has been deleted:

 User ID: 0
 Name: 
 User Name: 
 Email: 
 ------------------------------
 JUser Delete Finished
 ****************************************


Info
----------------

Wenn der Benutzer zum Anzeigen von Details eines Benutzers in Maschine muss, die unten mit dem Befehl wird ausgeführt, den Prozess der Installation.


.. code-block:: bash
        
	jrush juser info ..config file=”bootstrap file path”

Die bildliche Darstellung der oben genannte Befehl ist im folgenden aufgeführt,


.. code-block:: bash


 kevell@corp:/# jrush juser info --config-file="/var/www/html/joomla/configuration.php"
 Enter a JUser ID. To enter email/username use --user-email or --username parameters
 1
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

 JUser Info:
 -------------------------
 
 User ID: 
 Name: 
 User Name: 
 Email: 

 ------------------------------
 JUser Info Finished
 ****************************************

Password
----------------

Wenn der Benutzer zum Ändern des Kennworts eines Benutzers in der Maschine muss, die unten mit dem Befehl wird ausgeführt, den Prozess der Installation.


.. code-block:: bash
        
	jrush juser password ..config file=”bootstrap file path”


Alternative Parameter
-----------------------------

Eines der zwei alternative Parameter einsetzbar in Befehl - juser and JUser

eg: jrush juser info ..config file=”bootstrap file path” / jrush JUser info ..config file=”bootstrap file path”                            

.. code-block:: bash

 kevell@corp:/# jrush juser password --config-file="/var/www/html/joomla/configuration.php"
 Enter a JUser ID. To enter email/username use --user-email or --username parameters
 5
 Enter a new Password. To enter as parameter use --password 
 12345
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

 JUser Password:
 -------------------------

 User ID: 0
 Name: 
 User Name: 
 Email: 
 User Password: NOT SET

 ------------------------------
 JUser Password Finished
 ****************************************


Vorteile 
--------------

* Einfach zum Abrufen der Informationen über einen Benutzer mithilfe eines einzelnen Befehls 
* Easy zum Ändern des Kennworts eines Benutzers vom Back-End mit einzelnen Befehl 
* Easy, Benutzerkonten zu behandeln

