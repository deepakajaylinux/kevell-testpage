=============
Run Command
=============

Zusammenfassung
-----------------------

Die Fahrbefehl Module ermöglicht den Benutzern, einen Betriebssystembefehl auszuführen. Dies ist vor allem in einem Autopilot verwendet werden. Mit diesem Lauf Befehl kann der Anwender den Befehl angeben, Name des Benutzers und auch die entweder im Hintergrund oder Front-End-Funktionalität. Lassen Sie uns die Nutzung der Fahrbefehl.

Hilfe Befehl
----------------

Der Befehl Hilfe beschreibt die Verwendung von Fahrbefehl, seiner Funktionalität, seiner alternative Parameter, die für die Ausführung eines Befehls verwendete Befehle, und auch über die Syntax für den Befehl, den Namen des Benutzers und auch für die entweder im Hintergrund oder Frontauftritt -ende. Die zur Feststellung der Befehl help Syntax ist unten dargestellt.

.. code-block:: bash

		ptconfigure RunCommand help

Der folgende Screenshot zeigt bildhaft über die Arbeit der Befehl help.

.. code-block:: bash

 kevell@corp:/# ptconfigure RunCommand help
 ******************************


  This allows you to execute an Operating System command. This would primarily be used in an Autopilot.

  RunCommand, runcommand, run-command

        - execute
        Execute a Command
        example: ptconfigure run-command --yes --command="ls -lah /tmp" --run-as-user="ubuntu" --background

 ------------------------------
 End Help
 ******************************

Wie Befehl Ausführen verwenden
------------------------------------

Die Syntax für die Angabe der Fahrbefehl in unten gezeigt verwendet.

.. code-block:: bash

		ptconfigure run-command --yes --command="ls -lah /tmp" --run-as-user="ubuntu" --background


.. cssclass:: table-bordered

 +-------------------------+------------------------------------------------+-------------------------------------------------+
 | Parameter               | Funktion                                       | Verwendung                                      |
 +=========================+================================================+=================================================+
 |command=”ls -lah /tmp”   | Es ermöglicht dem Benutzer, den Befehl und     | Durch die Nutzung dieser, kann der Benutzer     |
 |                         | dessen Zweck angeben.                          | seinen eigenen Befehl nach ihren Anforderungen  |
 |                         |                                                | angeben.                                        |
 +-------------------------+------------------------------------------------+-------------------------------------------------+
 |run-as-user=”ubuntu”     | Durch die Nutzung dieser, kann der Benutzer    | Durch die Nutzung dieser, kann der Benutzer     |
 |                         | den Namen des Benutzers angeben.               | die erforderliche Benutzeranmeldung nach ihren  |
 |                         |                                                | festzulegen.                                    |
 +-------------------------+------------------------------------------------+-------------------------------------------------+
 |” –background            | Es erlaubt dem Benutzer, festzulegen, wo die   | Durch die Nutzung dieser, kann der Benutzer     |
 |                         | bestimmten Befehl entweder im Hintergrund oder | der Plattform ihrer Nutzung nach ihren          |
 |                         | in der Front-End-laufen.                       | Anforderungen angeben.|                         |
 +-------------------------+------------------------------------------------+-------------------------------------------------+


Vorteile
------------

* Die Hilfe Befehl deklarieren verwendeten Parameter werden Installation nicht beachtet, welche ein zusätzlicher Vorteil ist, während im 
  Vergleich zu anderen.
* Es ist gut-to-do in beiden Cent OS und als auch in Ubuntu.
* Die Benutzer können den Befehl geben, Name des Benutzers und auch die entweder im Hintergrund oder Front-End-Funktionalität.
* Der Befehl Hilfe führt die Anwender in, wie man den Lauf der Ausführung des Befehls ein auch seinen Zweck.





