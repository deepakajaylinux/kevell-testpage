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


.. code-block:: bash

 kevell@corp:/# ptconfigure sftp put

 SFTP on Server group? (Y/N) 
 y
 Please Enter SSH Timeout in seconds
 100
 Please Enter remote SSH Port
 22
 ***********************************
 *   Due to a software limitation, *
 *    The user that you use here   *
 *  will have their command prompt *
 *    changed to PHARAOHPROMPT     *
 *  ... I'm working on that one... *
 *  Exit program to stop (CTRL+C)  *
 ***********************************
 Enter Server Info:
 Please Enter SSH Server Target Host Name/IP
 192.168.1.4
 Please Enter SSH User
 murali
 Please Enter Server Password or Key Path
 123456
 Add Another Server? (Y/N) 
 n
 [Pharaoh Logging] Attempting to load SFTP connections...
 [Pharaoh Logging] Connection to Server 192.168.1.4 failed.
 Enter local source file path
 /home/kevells/Desktop/graphs
 Enter remote target file path
 /home/murali/Desktop/graphs
 [Pharaoh Logging] Opening SFTP Connections...
 [192.168.1.4]Connection failure. Will not execute commands on this box..
 [Pharaoh Logging] All SFTP Puts Completed
 ******************************



 SFTP Put: Success

 ------------------------------
 Installer Finished
 ******************************

.. code-block:: bash



 kevell@corp:/# ptconfigure sftp get

 SFTP on Server group? (Y/N) 
 y
 Please Enter SSH Timeout in seconds
 100
 Please Enter remote SSH Port
 22
 ***********************************
 *   Due to a software limitation, *
 *    The user that you use here   *
 *  will have their command prompt *
 *    changed to PHARAOHPROMPT     *
 *  ... I'm working on that one... *
 *  Exit program to stop (CTRL+C)  *
 ***********************************
 Enter Server Info:
 Please Enter SSH Server Target Host Name/IP
 192.168.1.4
 Please Enter SSH User
 murali
 Please Enter Server Password or Key Path
 123456
 Add Another Server? (Y/N) 
 n
 [Pharaoh Logging] Attempting to load SFTP connections...
 [Pharaoh Logging] Connection to Server 192.168.1.4 failed.
 Enter remote source file path
 /home/murali/Desktop/graphs
 Enter local target file path
 /hoem/kevells/Desktop/graphs1
 [Pharaoh Logging] Opening SFTP Connections...
 [Pharaoh Logging] [192.168.1.4] Executing SFTP Get...
 [Pharaoh Logging] No SFTP Object
 [Pharaoh Logging] 
 [Pharaoh Logging] [192.168.1.4] SFTP Get Completed...
 [Pharaoh Logging] All SFTP Gets Completed
 ******************************


 Shell Result: Success
 SFTP Get

 ------------------------------
 Installer Finished
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
