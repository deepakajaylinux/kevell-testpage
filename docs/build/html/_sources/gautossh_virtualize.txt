==========
AutoSSH
==========


Zusammenfassung
----------------

Mit diesem Modul können die Benutzer einen ptvirtualize Box autossh. Autossh ist ein kleines Frontend für SSH, die die Verbindung zu überwachen können, und starten Sie den Tunnel wenn es fällt oder nicht mehr reagiert.

autossh verwendet ssh, um eine Schleife von ssh-Weiterleitungen (eine von lokaler auf externe, eine von Remote auf Lokal) konstruieren und sendet Testdaten, die sie erwartet, um zurück zu gelangen.

Lassen Sie uns die Funktionen des Auto ssh in kommenden Themen sehen.


Hilfe Befehl
-------------------

Der Befehl help führt den Anwender über den Zweck und als auch über die Möglichkeiten, die in der Auto-SSH-Modul enthalten sind. Es listet einige der alternativen Parameter Auto SSH-Modul. Es beschreibt auch die Syntax für die Verwendung der CLI sftp_put, sftp_get Befehle. Der Befehl help für Auto SSH-Modul wird wie unten dargestellt.

.. code-block:: bash

	ptvirtualize AutoSSH help

Die Syntax für die Deklaration den Befehl help ist nicht case sensitive was ein zusätzlicher Vorteil ist. Der folgende Screenshot visualisieren Sie den Befehl help unter Auto SSH.

.. code-block:: bash


 kevell@corp:/# ptvirtualize AutoSSH help

 ******************************
 Pharaoh Tools - Virtualize
 ******************************


  This command allows you to autoSSH a ptvirtualize box

  AutoSSH, auto-ssh, autossh, ssh, SSH

        - cli
        Open an SSH Cli to your ptvirtualize Box
        example: ptvirtualize auto-ssh cli --yes --guess

        - sftp-put
        SFTP Put a file on to your ptvirtualize Box
        example: ptvirtualize auto-ssh sftp-put --yes --guess --source=/path/to/source --target=/path/to/target

        - sftp-get
        SFTP Get a file from your ptvirtualize Box
        example: ptvirtualize auto-ssh sftp-get --yes --guess --source=/path/to/source --target=/path/to/target

 ------------------------------
 End Help
 ******************************


Funktionen autossh
----------------------

Wie im obigen Befehl help dargestellt, die wichtigsten Funktionen dieses Auto ssh Modul
* cli
* sftp_put
* sftp_get

cli
------

Nach der Aktivierung oder den Aufbau eines Auto ssh in der Benutzer-Umgebung kann der cli geschaffen, die verwendet wird, um einen SSH-Cli indem Sie den folgenden Befehl aus, um die Benutzer ptvirtualize Feld geöffnet werden:

.. code-block:: bash

	ptvirtualize auto-ssh cli --yes --guess


Die CLI wird für den verfügbaren Clients in einer bestimmten Umgebungen, in denen die Auto ssh erzeugt eingesetzt.


Sftp_put
-----------

Diese Funktion wird zum Anordnen und Verschieben der erforderlichen Dateien oder Daten von der Quelle bis zum Ziel eines besonderen Umgebung, in der die Auto SSH erzeugt eingesetzt. Dies kann mit dem Befehl unten angegeben durchgeführt werden:

.. code-block:: bash

	ptvirtualize auto-ssh sftp-put --yes --guess --source="path/to/source --target=/path/to/target

Dieser Befehl veran wird eine Datei auf, um der Benutzer ptvirtualize Box. Der folgende Screenshot zeigt visuell den Vorgang.


Sftp_get
-----------

Diese Funktion ist für das Erhalten oder holen die erforderlichen Dateien oder Daten von der Quelle zum Ziel einer bestimmten Umgebung, in der Auto ssh erzeugt eingesetzt. Dies kann mit dem Befehl unten angegeben durchgeführt werden:


.. code-block:: bash

	ptvirtualize auto-ssh sftp-get --yes --guess --source="path/to/source --target=/path/to/target

Der obige Befehl wird angezeigt bekommt oder erhält eine Datei aus der Anwender-Box ptvirtualize. Der folgende Screenshot zeigt visuell den Vorgang.


Alternative Parameter
-----------------------------

* AutoSSH
* auto-ssh
* autossh
* ssh
* SSH

Bei der oben genannten Liste eine der alternativen Parameter können in Erklärung verwendet werden.


Vorteile
-----------

* Die in Hilfe und Installation und un-Installation Operationen verwendet sind nicht case sensitive Parameter, die ein zusätzlicher Vorteil ist,  während im Vergleich zu anderen.
* Es ist gut-to-do sowohl Ubuntu und sowie Cent OS.
* Die CLI-Funktionen Liste outs die verfügbaren Clients in einer bestimmten Umgebung mit Hilfe von Auto SSH.
* Sftp_put, Sftp_get platzieren können und holen Sie die Dateien jeweils zwischen Quelle und Ziel einer bestimmten Umgebung mit Auto SSH.
* Die Syntax für die Deklaration der cli, setzen, lassen sich deutlich in der Eingabehilfe dargestellt.
