============
User
============

Zusammenfassung
-------------------------

Ein Benutzer ist jeder, der einen Computer verwendet. Computer hat einen Namen für jedes Konto schafft, und es ist dieser Name, mit dem eine Person Zugriff auf den Computer zu benutzen. Einige Systemdienste laufen auch mit eingeschränkten oder privilegierte Benutzerkonten.

Die Verwaltung von Benutzern zum Zweck der Sicherheit, indem der Zugriff auf bestimmte Arten erfolgen. Der Superuser (root), hat Zugriff auf das Betriebssystem und seine Konfiguration; Es ist nur für den Verwaltungs Gebrauch bestimmt. Benutzer ohne Privilegien haben die su und sudo Programme für gesteuerte Zugriffsrechten verwenden.

Ein wesentlicher Bestandteil der Systemadministration ist die Konfiguration und Verwaltung von Benutzern und Gruppen. Ein Teil dieser Aufgabe besteht darin, die Überwachung der Protokoll in Fähigkeiten aller Systemeinheiten.

Wir werden diese Konzepte auf einem Ubuntu 12.04 VPS erkunden, aber Sie können zusammen auf einer up-to-date-Linux-Distribution zu folgen.
ptconfigure user help

Der Screenshot für den obigen Befehl aufgelistet unten,

.. code-block:: bash 

 kevell@corp:/# ptconfigure user help
 ******************************

 This command allows you to modify create or modify users

 User, user

       - create
       Create a new system user, overwriting if it exists
       example: ptconfigure user create --username="somename"

       - remove
       Remove a system user
       example: ptconfigure user remove --username="somename"

       - set-password
       Set the password of a system user
       example: ptconfigure user set-password --username="somename" --new-password="somepassword"

       - exists
       Check the existence of a user
       example: ptconfigure user exists --username="somename"

       - show-groups
       Show groups to which a user belongs
       example: ptconfigure user show-groups --username="somename"

       - add-to-group
       Add user to a group
       example: ptconfigure user add-to-group --username="somename" --groupname="somegroupname"

       - remove-from-group
       Remove user from a group
       example: ptconfigure user remove-from-group --username="somename" --groupname="somegroupname"

 ------------------------------
 End Help
 ******************************

Create
-----------

Wenn der Benutzer muss ein neues System-Benutzerkonto erstellen, wird der unten angegebenen Befehl den Prozess und führen.

.. code-block:: bash

	ptconfigure user create --username="somename"

.. code-block:: bash

 kevell@corp:/# ptconfigure user create
 
 Enter Username:
 kevell
 ******************************


 User Modifications:
 --------------------------------------------

 User: 1

 ------------------------------
 User Mods Finished
 ******************************

Remove
-------------

Wenn der Benutzer muss ein Systembenutzerkonto zu entfernen, wird der unten angegebenen Befehl den Prozess auszuführen.

.. code-block:: bash

	ptconfigure user remove --username="somename"

.. code-block:: bash

 kevell@corp:/# ptconfigure user remove

 Enter Username:
 kevell
 ******************************


 User Modifications:
 --------------------------------------------

 User: 1

 ------------------------------
 User Mods Finished
 ******************************


Set-Password
---------------------

Wenn der Benutzer das Kennwort eines Systembenutzers eingestellt benötigt, wird der unten angegebenen Befehl den Prozess auszuführen.

.. code-block:: bash

	ptconfigure user set-password --username="somename" --new-password="somepassword"

.. code-block:: bash

 kevell@corp:/# ptconfigure user set-password

 Enter Username:
 kevell
 Enter New Password:
 kevell
 ******************************


 User Modifications:
 --------------------------------------------

 User: 

 ------------------------------
 User Mods Finished
 ******************************

Exists
----------

Wenn der Benutzer braucht, um das Vorhandensein eines Benutzers zu überprüfen, werden die unten angegebenen Befehl den Prozess auszuführen.

.. code-block:: bash

	ptconfigure user exists --username="somename"

.. code-block:: bash

 kevell@corp:/# ptconfigure user exists

 Enter Username:
 kevell
 ****************************** 


 User Modifications:
 --------------------------------------------

 User: Success = User Exists
 User Name: 

 ------------------------------
 User Mods Finished
 ******************************

.. code-block:: bash

 kevell@corp:/# ptconfigure user exists

 Enter Username:
 karuna
 ******************************


 User Modifications:
 --------------------------------------------

 User: Failure - User Does Not Exist
 User Name: 

 ------------------------------
 User Mods Finished
 ******************************

Show-Groups
----------------------

Wenn der Benutzer benötigt, um Gruppen, denen ein Benutzer angehört zu zeigen, wird der unten angegebenen Befehl den Prozess auszuführen.

.. code-block:: bash

	ptconfigure user show-groups --username="somename"

.. code-block:: bash

 kevell@corp:/# ptconfigure user show-groups

 Enter Username:
 kevell
 ******************************


 User Modifications:
 --------------------------------------------

 User: kevell


 ------------------------------
 User Mods Finished
 ******************************

Add-to-Group
---------------------

Wenn der Benutzer benötigt, um Benutzer zu einer Gruppe hinzuzufügen, wird der unten angegebenen Befehl den Prozess auszuführen.

.. code-block:: bash

	ptconfigure user add-to-group --username="somename" --groupname="somegroupname"

.. code-block:: bash


 kevell@corp:/# ptconfigure user add-to-group --username="kevell" --groupname="kumar"

 Enter New Password:
 kevell
 ******************************


 User Modifications:
 --------------------------------------------

 User: 1

 ------------------------------
 User Mods Finished
 ******************************


Remove from group
-------------------------------

Wenn der Benutzer benötigt, um Benutzer aus einer Gruppe zu entfernen, wird der unten angegebenen Befehl den Prozess auszuführen.

.. code-block:: bash

	ptconfigure user remove-from-group --username="somename" --groupname="somegroupname"

.. code-block:: bash

 kevell@corp:/# ptconfigure user remove-from-group --username="kevell" --groupname="kumar"

 Enter New Password:
 kevell

 /usr/sbin/deluser: You may not remove the user from their primary group.
 [Pharaoh Logging] [User] Removing User kevell from the Group kevell did not execute correctly
 ******************************


 User Modifications:
 --------------------------------------------

 User: 

 ------------------------------
 User Mods Finished
 ******************************



Alternative Parameter
----------------------------------

Es gibt zwei alternative Parameter, die in der Befehlszeile verwendet werden kann.

User, user

Example: ptconfigure User help /ptconfigure user help

Vorteile
---------------

Die Benutzerauthentifizierung auf Linux ist eine relativ flexible Bereich der Systemverwaltung. Es gibt viele Möglichkeiten zum Erreichen des gleichen Ziels mit einfachen Werkzeugen.User authentication on Linux is a relatively flexible area of system management. There are many ways of accomplishing the same objective with very simple tools.


