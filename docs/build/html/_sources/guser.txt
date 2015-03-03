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

schaffen
-----------

Wenn der Benutzer muss ein neues System-Benutzerkonto erstellen, wird der unten angegebenen Befehl den Prozess und führen.
ptconfigure user create --username="somename"

entfernen
-------------

Wenn der Benutzer muss ein Systembenutzerkonto zu entfernen, wird der unten angegebenen Befehl den Prozess auszuführen.

ptconfigure user remove --username="somename"

Set-Passwort
---------------------

Wenn der Benutzer das Kennwort eines Systembenutzers eingestellt benötigt, wird der unten angegebenen Befehl den Prozess auszuführen.

ptconfigure user set-password --username="somename" --new-password="somepassword"

vorhanden
----------

Wenn der Benutzer braucht, um das Vorhandensein eines Benutzers zu überprüfen, werden die unten angegebenen Befehl den Prozess auszuführen.

ptconfigure user exists --username="somename"

Show-Gruppen
----------------------

Wenn der Benutzer benötigt, um Gruppen, denen ein Benutzer angehört zu zeigen, wird der unten angegebenen Befehl den Prozess auszuführen.

ptconfigure user show-groups --username="somename"

Add-to-Gruppe
---------------------

Wenn der Benutzer benötigt, um Benutzer zu einer Gruppe hinzuzufügen, wird der unten angegebenen Befehl den Prozess auszuführen.

ptconfigure user add-to-group --username="somename" --groupname="somegroupname"

Entfernen-von-Gruppe
-------------------------------

Wenn der Benutzer benötigt, um Benutzer aus einer Gruppe zu entfernen, wird der unten angegebenen Befehl den Prozess auszuführen.

ptconfigure user remove-from-group --username="somename" --groupname="somegroupname"

Alternative Parameter
----------------------------------

Es gibt zwei alternative Parameter, die in der Befehlszeile verwendet werden kann.

User, user

Example: ptconfigure User help /ptconfigure user help

Vorteile
---------------

Die Benutzerauthentifizierung auf Linux ist eine relativ flexible Bereich der Systemverwaltung. Es gibt viele Möglichkeiten zum Erreichen des gleichen Ziels mit einfachen Werkzeugen.User authentication on Linux is a relatively flexible area of system management. There are many ways of accomplishing the same objective with very simple tools.


