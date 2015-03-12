=============
Run Command
=============

Zusammenfassung
----------------

Die Fahrbefehl Module ermöglicht den Benutzern, einen Betriebssystembefehl auszuführen. Dies ist vor allem in einem Autopilot verwendet werden. Mit diesem Lauf Befehl kann der Anwender den Befehl angeben, Name des Benutzers und auch die entweder im Hintergrund oder Front-End-Funktionalität. Lassen Sie uns die Nutzung der Fahrbefehl.

Hilfe Befehl
---------------------

Der Befehl Hilfe beschreibt die Verwendung von Fahrbefehl, seiner Funktionalität, seiner alternative Parameter, die für die Ausführung eines Befehls verwendete Befehle, und auch über die Syntax für den Befehl, den Namen des Benutzers und auch für die entweder im Hintergrund oder Frontauftritt -ende. Die zur Feststellung der Befehl help Syntax ist unten dargestellt.

.. code-block:: bash

	ptdeploy RunCommand help

Der folgende Screenshot zeigt bildhaft über die Arbeit der Befehl help.

.. code-block:: bash

 kevell@corp:/# ptdeploy RunCommand help
 ******************************


  Damit können Sie ein Betriebssystem Befehl auszuführen. Dies würde vor allem in einem Autopilot verwendet werden.
  RunCommand, runcommand, run-command

        - execute
        Execute a Command
        example: ptconfigure run-command --yes --command="ls -lah /tmp" --run-as-user="ubuntu" --background

 ------------------------------
 End Help
 ******************************


Wie Befehl Ausführen verwenden
-----------------------------------


Die Syntax für die Angabe der Fahrbefehl in unten gezeigt verwendet.

.. code-block:: bash

	ptconfigure run-command --yes --command="ls -lah /tmp" --run-as-user="ubuntu" --background


.. cssclass:: table-bordered

 +-------------------------+----------------------------+------------------------------------+--------------------------------------+
 | Parameter               | Alternative parameters     | Function                           | Usage                                |
 +=========================+============================+====================================+======================================+
 |command=”ls -lah /tmp”   | RunCommand, runcommand,    | Es ermöglicht dem Benutzer, den    | Durch die Nutzung dieser, kann der   |
 |                         | run-command                | Befehl und dessen Zweck angeben.   | Benutzer seinen eigenen Befehl nach  |
 |                         |                            |                                    | ihren Anforderungen angeben.         |
 +-------------------------+----------------------------+------------------------------------+--------------------------------------+
 |run-as-user=”ubuntu”     | RunCommand, runcommand,    | Durch die Nutzung dieser, kann der | Durch die Nutzung dieser, kann der   |
 |                         | run-command                | Benutzer den Namen des Benutzers   | Benutzer die erforderliche           |
 |                         |                            | angeben.                           | Benutzeranmeldung nach ihren         |
 |                         |                            |                                    | Anforderungen festzulegen.           |
 +-------------------------+----------------------------+------------------------------------+--------------------------------------+
 |” –background            | RunCommand, runcommand,    | Es erlaubt dem Benutzer,           | Durch die Nutzung dieser, kann       |
 |                         | run-command                | festzulegen, wo die bestimmten     | der Benutzer der Plattform ihrer     |
 |                         |                            | Befehl entweder im Hintergrund     | Nutzung nach ihren Anforderungen     |
 |                         |                            | oder in der Front-End-laufen.      | angeben..|                           |
 +-------------------------+----------------------------+------------------------------------+--------------------------------------+
Die Syntax und die Tabelle wie oben beschrieben, kann hilft dem Benutzer, wie Sie den Startbefehl zu verwenden.

Vorteile
------------

* Die Hilfe Befehl deklarieren verwendeten Parameter werden Installation nicht beachtet, welche ein zusätzlicher Vorteil ist, während im 
  Vergleich zu anderen.
* Es ist gut-to-do in beiden Cent OS und als auch in Ubuntu.
* Die Benutzer können den Befehl geben, Name des Benutzers und auch die entweder im Hintergrund oder Front-End-Funktionalität.
* Der Befehl Hilfe führt die Anwender in, wie man den Lauf der Ausführung des Befehls ein auch seinen Zweck.
