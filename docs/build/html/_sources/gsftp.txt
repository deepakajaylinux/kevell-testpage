=======
SFTP
=======

Zusammenfassung
-------------------------

           Dieses Modul unterstützen die Übertragung von Dateien von einem System auf ein anderes. Es kann Hoch- und Herunterladen der Dateien auf das System. Automation möglich. Setzen Sie und erhalten Sie Optionen in diesem Modul zur Verfügung. Es gibt die Konfiguration Ihrer Umgebung. Es ist benutzerfreundlich mit Ubuntu und Cent-OS.

Hilfe Befehl
---------------

Hilfe Befehl verwendet werden, um Informationen zu einem bestimmten Befehl zu finden. Weitere Informationen zu den Funktionsänderungen von SFTP können wir diese Hilfe Befehl verwenden.

.. code-block:: bash

 		ptconfigure sftp help

Der folgende Screenshot wird dich führen.

.. code-block:: bash


 kevell@corp:/# ptconfigure sftp help
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

Installation
-------------

Als Unternehmen und als Individuen, SFTP wurde zur Erfüllung technologischen Herausforderungen der einzelnen Partner, die Erfüllung ihrer technischen Anforderungen und Erfüllung ihrer Unternehmensziele gewidmet. Es ist offensichtlich, dass die Verfahren zur SFTP-Modul unter ptconfigure installieren, indem einfach mit dem Befehl unten angegeben,

.. code-block:: bash

		ptconfigure SFTP put


After giving the command then the system will raise the question as,

Install SFTP server group? Y/N

If the user input as Y then

SSh timeout section?

The user has to enter the value

Please enter remote ssh port

Default value is 22. The user can enter any value

Enter server host IP? 

The user has to enter username, password, and key path.

Add another server?

If the user input as Y he has to enter new server name

Then everything will be connected.

If the user input as N previous server name can be accessed.


The following screenshot will guide you.

.. code-block:: bash

 kevell@corp:/# ptconfigure sftp put

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



Options
----------

.. cssclass:: table-bordered


 +--------------------+------------------------+---------------------------------------------------------------------+
 | Parameters         | Alternative Parameter  | Kommentare                                                          |
 +====================+========================+=====================================================================+
 |put                 | SFTP, sftp             | Quelle zu -Die Zieldatei übertragen werden können                   |
 +--------------------+------------------------+---------------------------------------------------------------------+
 |get                 | SFTP, sftp             | Pfad zur Datei -Die Quelle kann von Remote-System heruntergeladen|  |
 +--------------------+------------------------+---------------------------------------------------------------------+



Vorteile
-------------

* Multi-Server von Einöde.
* Die angegebene Datei ist nicht verfügbar Fehlermeldung kommen.
* Erreichbarkeit ist schwierig ohne Genehmigung.
* Automatisch bei bereits überschreiben bei Datei vorhanden.
* Nicht Groß- und Kleinschreibung.
* Geheimhaltung und Sicherheit möglich ist.
