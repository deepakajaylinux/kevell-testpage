=======
SFTP
=======


Zusammenfassung
-----------------------

Dieses Modul unterstützen die Übertragung von Dateien von einem System auf ein anderes. Es kann Hoch- und Herunterladen der Dateien auf das System. Automation möglich. Setzen Sie und erhalten Sie Optionen in diesem Modul zur Verfügung. Er verwaltet auch virtuelle Box. Es ist benutzerfreundlich mit Ubuntu und Cent-OS.

Hilfe Befehl
-------------------------

Hilfe Befehl verwendet werden, um Informationen zu einem bestimmten Befehl zu finden. Weitere Informationen zu den Funktionsänderungen von Secure File Transfer Protocol (SFTP) unter ptvirtualize der Benutzer kann diese Hilfe Befehl verwenden.

.. code-block:: bash

	ptvirtualize  sftp help


Der folgende Screenshot führt Sie.

.. code-block:: bash

 kevell@corp:/# ptvirtualize sftp help

 ******************************
 Pharaoh Tools - ptvirtualize
 ******************************


  This command handles SFTP Transfer Functions.

  SFTP, sftp

        - put
        Will ask you for details for servers, then copy a file or directory from local to remote
        example: ptconfigure sftp put
        example: ptconfigure sftp put --yes --environment-name=staging --source="/tmp/file" --target="/home/user/file"
        example: ptconfigure sftp put --yes --source="/tmp/file" --target="/home/user/file" # will ask for server details

        - get
        Will ask you for details for servers, then copy a file or directory from remote to local
        example: ptconfigure sftp get
        example: ptconfigure sftp get --yes --environment-name=staging --source="/tmp/file" --target="/home/user/file"
        example: ptconfigure sftp get --yes --source="/tmp/file" --target="/home/user/file" # will ask for server details

 ------------------------------
 End Help
 ******************************


Alternative Parameter
---------------------------------

Es gibt zwei alternative Parameter verfügbar. Sie sind SFTP und SFTP. Anstelle der Verwendung von sftp, kann der Benutzer SFTP verwenden.


setzen
------

Die Dateiübertragung kann von der lokalen bis Remote-Server durchgeführt werden. Diese Put-Option stellt der Benutzerin datails für Server. Mit dem folgenden Befehl für Put-Option verwendet.

.. code-block:: bash

	ptvirtualize  sftp put – yes –source=”/tmp/file” – target=”/home/user/file”

The following screen shot denotes the usage of this command.


.. code-block:: bash

 kevell@corp:ptconfigure sftp put
 
 SFTP on Server group? (Y/N) 
 Y
 Please Enter SSH Timeout in seconds
 90
 Please Enter remote SSH Port
 22
 Use Environments Configured in Project? (Y/N) 
 N
 [Pharaoh Logging] Attempting to load SFTP connections...
 Enter local source file path
 /root/vv
 Enter remote target file path
 /root/gg/vv
 [Pharaoh Logging] Opening SFTP Connections...
 [Pharaoh Logging] All SFTP Puts Completed
 ******************************


SFTP on server group? Y/N

If the user input as Y then

SSh timeout section?

The user has to enter the value

Please enter remote ssh port

Default value is 22. The user can enter any value

Enter environments configured in project? (Y/N)

The user has to enter y then it starts loading.

Enter local source file path?

The user  has to enter the file path

Then everything will be connected.

If the user input as N, it can be terminated.



erhalten
----------

Die Dateiübertragung kann zwischen Fernbedienung und lokalen Server durchgeführt werden. Es fordert den Benutzer auf Server-Gruppe ein. Mit dem folgenden Befehl für get-Option verwendet.

.. code-block:: bash

	ptvirtualize  sftp get – yes –source=”/tmp/file” – target=”/home/user/file”

The following screen shot explains it.


.. code-block:: bash

 kevell@corp:/# ptconfigure sftp get
 SFTP on Server group? (Y/N) 
 Y
 Please Enter SSH Timeout in seconds

 Please Enter remote SSH Port

 Use Environments Configured in Project? (Y/N) 

 [Pharaoh Logging] Attempting to load SFTP connections...
 Enter remote source file path

 Enter local target file path

 [Pharaoh Logging] Opening SFTP Connections...
 [Pharaoh Logging] All SFTP Gets Completed
 ******************************


 Shell Result: Success
 SFTP Get

 ------------------------------
 Installer Finished
 ******************************


SFTP auf Server-Gruppe? Y / N

Wenn die Benutzereingabe als Y dann

SSh Timeout Abschnitt?

Der Benutzer muss den Wert einzugeben

Bitte geben Sie Remote SSH-Port

Der Standardwert ist 22. Der Benutzer kann einen beliebigen Wert eingeben

Geben Sie in Umgebungen Projekt konfiguriert? (Y / N)

Der Benutzer muss y geben Sie es beginnt Belastung.

Geben Sie lokale Zieldateipfad?

Der Benutzer muss die lokale Zieldateipfad eingeben

Dann wird alles angeschlossen werden.

Wenn die Benutzereingabe, wie N, kann sie beendet werden. Die folgenden Screenshots zeigen die Funktion.
.. code-block:: bash

 kevell@corp:/# ptconfigure sftp get
 SFTP on Server group? (Y/N) 
 N
 ******************************


 Shell Result: Failure
 SFTP Get

 ------------------------------
 Installer Finished
 ******************************



Options
-------------

.. cssclass:: table-bordered


 +--------------+----------------------------+---------------------+-----------------------------------------------------+
 | Parameters   | Alternative Parameters     | Syntax              | Kommentare                                          |
 +==============+============================+=====================+=====================================================+
 |put           | SFTP, sftp                 | Source to target    | Die Zieldatei übertragen werden können              |
 +--------------+----------------------------+---------------------+-----------------------------------------------------+
 |get           | SFTP, sftp                 | Path to source      | Die Quelle kann von Remote-System heruntergeladen|  |
 +--------------+----------------------------+---------------------+-----------------------------------------------------+

Vorteile
-------------

* Multi-Server von Einöde.
* Die angegebene Datei ist nicht verfügbar Fehlermeldung kommen.
* Erreichbarkeit ist schwierig ohne Genehmigung.
* Automatisch bei bereits überschreiben bei Datei vorhanden.
* Nicht Groß- und Kleinschreibung.
* Geheimhaltung und Sicherheit möglich ist.

