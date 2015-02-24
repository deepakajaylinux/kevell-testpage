============
Pear
============


Zusammenfassung
----------------------

PEAR ist die Abkürzung für "PHP-Erweiterung und Application Repository" und ist genau wie die Frucht ausgeprägt. Der Zweck ist die Bereitstellung von PEAR:

* Eine strukturierte Sammlung von Open-Source-Code für PHP-Benutzer
* Ein System zur Code-Distribution und Paketverwaltungs
* Ein Standard-Stil für Code in PHP geschrieben, hier angegebenen
* Die PHP-Erweiterung Community Library (PECL)


PEAR-Mission ist es, wiederverwendbare Komponenten, führen Innovationen in PHP zur Verfügung stellen Best Practices für die PHP-Entwicklung und zu erziehen Entwickler.

Der Code in PEAR in "Pakete" aufgeteilt. Jedes Paket ist ein eigenes Projekt mit einem eigenen Entwicklungsteam, Versionsnummer, Release-Zyklus, Dokumentation und einem definierten Verhältnis zu anderen Paketen (einschließlich Abhängigkeiten). Pakete werden gzipped tar-Dateien mit einer Beschreibungsdatei im Inneren verteilt und auf dem lokalen System mit dem PEAR Installer installiert.

Hilfe Befehl
----------------------

Dieser Befehl hilft, die Verwendung von PEAR-Modul zu bestimmen. Der Benutzer wird kommen, um über die andere Art und Weise / Format um dieses Modul ausführen kennen. Dieser Befehl leitet den Anwender, um den Zweck dieses Befehls kennen. Da unten sind die Kommando- und der Screenshot der gleiche.

.. code-block:: bash
        
	        ptconfigure pear help

The pictorial representation of the above command is listed below,

.. code-block:: bash


 kevell@corp:/# ptconfigure pear help
 ******************************


  This command allows you to modify create or modify pears

  Pear, pear

        - create
        Create a new system pear, overwriting if it exists
        example: ptconfigure pear create --pearname="somename"

        - remove
        Remove a system pear
        example: ptconfigure pear remove --pearname="somename"

        - set-password
        Set the password of a system pear
        example: ptconfigure pear set-password --pearname="somename" --new-password="somepassword"

        - exists
        Check the existence of a pear
        example: ptconfigure pear exists --pearname="somename"

        - show-groups
        Show groups to which a pear belongs
        example: ptconfigure pear show-groups --pearname="somename"

        - add-to-group
        Add pear to a group
        example: ptconfigure pear add-to-group --pearname="somename" --groupname="somegroupname"

        - remove-from-group
        Remove pear from a group
        example: ptconfigure pear remove-from-group --pearname="somename" --groupname="somegroupname"

 ------------------------------
 End Help
 ******************************

schaffen
------------


Wenn der Benutzer ein neues System zu schaffen Birne müssen, bzw. die bestehende überschrieben wird die unten gegebenen Befehl das Verfahren auszuführen.

.. code-block:: bash
	
	ptconfigure pear create - -pearname=”somename”

entfernen
------------

Wenn der Benutzer braucht, um ein System Birne zu entfernen, wird der unten angegebenen Befehl den Prozess auszuführen.

.. code-block:: bash

	ptconfigure pear remove - -pearname=”somename”


Passwort wählen
---------------------

Wenn der Benutzer das Kennwort eines System Birne setzen muss, wird der unten angegebenen Befehl den Prozess auszuführen.

.. code-block:: bash
	
	ptconfigure pear setpassword - -pearname=”somename”- - new-password=”somepassword”


vorhanden
---------------------

Wenn der Benutzer braucht, um die Existenz von Birne wissen, wird die unten gegebenen Befehl das Verfahren auszuführen.

.. code-block:: bash
	
	ptconfigure pear exists - -pearname=”somename”


Show-Gruppen
---------------------

Wenn der Benutzer braucht, um die Gruppe, zu der eine Birne gehört kennen, wird der unten angegebenen Befehl den Prozess auszuführen.

.. code-block:: bash
	
	ptconfigure pear show-groups - -pearname=”somename”


Zur Gruppe hinzufügen
---------------------

Wenn der Benutzer Birne zu einer bestimmten Gruppe zuordnen muss, wird der unten angegebenen Befehl den Prozess auszuführen.

.. code-block:: bash
	
 	ptconfigure pear add-to-group - -pearname=”somename” - - groupname=”somegroupname”

Aus Gruppe entfern
----------------------------

Wenn der Benutzer muss Birne aus einer Gruppe entfernen, wird der unten angegebenen Befehl den Prozess auszuführen.

.. code-block:: bash
	
	ptconfigure pear remove-from-group - -pearname=”name” - -groupname=”groupname”

Alternative Parameter
--------------------------------

Es gibt zwei alternative Parameter, die in der Befehlszeile verwendet werden kann.

Pear, pear

.. code-block:: bash

 Eg: ptconfigure pear create - -pearname=”somename”/ ptconfigure Pear create - -pearname=”somename”

Vorteile
--------------
 
Pear.php.net bietet sowohl eine menschenfreundliche (HTML) und maschinenfreundlich (derzeit REST) Schnittstelle zu den von pear.php.net Pakete. Die gesamte Kommunikation findet über das HTTP-Protokoll. Weitere Funktionen der pear.php.net Website bietet, sind:


* Benutzerkontenverwaltung (unabhängig von der SVN-Server)
* Paketverwaltung
* Release-Management
* Well-to-do in Ubuntu und Cent OS
* Nicht Groß- und Kleinschreibung

