==========
AutoSSH
==========


Übersicht
-----------

Dieses Modul ermöglicht die Benutzern, AutoSSH ein Phlagrant Feld. Autossh ist ein kleines Frontend für SSH, die die Verbindung zu überwachen, und starten Sie den Tunnel, wenn es fällt oder nicht mehr reagiert.

Autossh verwendet ssh um eine Schleife von ssh Versand (eine vom lokalen zum entfernten, aus der Ferne zu lokalen) zu erstellen, und dann sendet Daten, die sie erwartet, um wieder testen. 

Lassen Sie uns sehen Sie die Funktionen der automatischen ssh in anstehenden Themen.


Help-Befehl
-------------------

Der Help-Befehl führt die Benutzer über den Zweck und auch als zu den Optionen, die im Auto SSH-Modul enthalten sind. Es listet alternative Ausgabeparameter des Auto-SSH-Moduls. Es beschreibt auch die Syntax für die Verwendung der Cli, Sftp_put, Sftp_get Befehle. Der Help-Befehl für Auto-SSH-Modul wird gezeigt wie unten beschrieben.


.. code-block:: bash

		phlagrant AutoSSH help


Die Syntax zum Deklarieren des Help-Befehls ist nicht Groß-/Kleinschreibung einen zusätzlichen Vorteil. Der folgende Screenshot visualisieren Sie über den Befehl Help unter Auto SSH.


.. code-block:: bash


 kevells@corp:/# phlagrant AutoSSH help

 ******************************
 Pharaoh Tools - Phlagrant
 ******************************


  This command allows you to autoSSH a phlagrant box

  AutoSSH, auto-ssh, autossh, ssh, SSH

        - cli
        Open an SSH Cli to your Phlagrant Box
        example: phlagrant auto-ssh cli --yes --guess

        - sftp-put
        SFTP Put a file on to your Phlagrant Box
        example: phlagrant auto-ssh sftp-put --yes --guess --source=/path/to/source --target=/path/to/target

        - sftp-get
        SFTP Get a file from your Phlagrant Box
        example: phlagrant auto-ssh sftp-get --yes --guess --source=/path/to/source --target=/path/to/target

 ------------------------------
 End Help
 ******************************


Funktionen der AutoSSH
----------------------

Wie in den oben genannten Befehl Help dargestellt, enthält die wichtigsten Funktionen von diesem Auto ssh-Modul

* cli
* sftp_put
* sftp_get


CLI
------

Nach Aktivierung oder Aufbau eines automatisch ssh in der Benutzer-Umgebung, kann die Cli erstellt werden, die verwendet wird, um einen SSH-Cli an die Benutzer-Phlagrant-Box zu öffnen, mithilfe des folgenden Befehls:

.. code-block:: bash

		phlagrant auto-ssh cli --yes --guess


Cli wird verwendet, für die Auflistung der verfügbaren Clients in bestimmten Umgebungen, wo wird das automatisch ssh generiert.


Sftp_put
-----------

Diese Funktion dient für platzieren oder verschieben die erforderlichen Dateien oder Daten von der Quelle zum Ziel einer bestimmten Umgebung, wo die Auto ssh generiert wird. Dies kann mithilfe des Befehls, die unten gegeben:

.. code-block:: bash

		phlagrant auto-ssh sftp-put --yes --guess --source="path/to/source --target=/path/to/target

Der obigen Befehl wird eine Datei auf das Feld Benutzer Phlagrant setzen. Der folgende Screenshot zeigt visuell den Prozess.


Sftp_get
-----------

Diese Funktion dient zum Abrufen oder Abrufen der erforderlichen Dateien oder Daten von der Quelle zum Ziel einer bestimmten Umgebung, wo die Auto ssh generiert wird. Dies kann mithilfe des Befehls, die unten gegeben:

.. code-block:: bash

		phlagrant auto-ssh sftp-get --yes --guess --source="path/to/source --target=/path/to/target

Der Befehl, die oben gezeigt wird Ruft oder erhält eine Datei aus dem Benutzer-Phlagrant-Feld. Der folgende Screenshot zeigt visuell den Prozess.


Alternative Parameter
-----------------------------

* AutoSSH
* auto-ssh
* autossh
* ssh
* SSH

In der oben genannten Liste können alternative Parameter in Deklaration verwendet werden.


Vorteile
-----------

* Die Parameter in der Hilfe verwendet und Installation und un Installationsvorgänge Groß-/Kleinschreibung keinen zusätzlichen Vorteil, 
  während im Vergleich zu anderen ist.
* Es ist wohlhabend, in beiden Ubuntu sowie als Cent OS.
* Die Cli-Funktionsliste outet die verfügbaren Clients in einer bestimmten Umgebung mit Auto SSH.
* Sftp_put, Sftp_get können und rufen Sie die Dateien bzw. zwischen Quelle und Ziel einer bestimmten Umgebung mithilfe von automatischen SSH.
* Die Syntax zum Deklarieren der Cli gelegt, Get deutlich in dem Help-Befehl dargestellt.

