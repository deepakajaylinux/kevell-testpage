======
SFTP
======



Zusammenfassung
----------------------

Dieses Modul unterstützen die Übertragung von Dateien von einem System auf ein anderes. Es kann Hoch- und Herunterladen der Dateien auf das System. Automation möglich. Setzen Sie und erhalten Sie Optionen in diesem Modul zur Verfügung. Es gibt die Konfiguration Ihrer Umgebung. Es ist benutzerfreundlich mit Ubuntu und Cent-OS.

Hilfe Befehl
-----------------------

Hilfe Befehl verwendet werden, um Informationen zu einem bestimmten Befehl zu finden. Weitere Informationen zu den Funktionsänderungen von SFTP können wir diese Hilfe Befehl verwenden.

.. code-block:: bash
   
        ptdeploy SFTP help


Der folgende Screenshot führt Sie.

.. code-block:: bash

 kevell@corp:/# ptdeploy sftp help
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
-----------------

Als Unternehmen und als Individuen, SFTP wurde zur Erfüllung technologischen Herausforderungen der einzelnen Partner, die Erfüllung ihrer technischen Anforderungen und Erfüllung ihrer Unternehmensziele gewidmet. Es ist offensichtlich, dass die Verfahren zur SFTP-Modul unter ptdeploy installieren, indem einfach mit dem Befehl unten angegeben,

.. code-block:: bash
  
	ptdeploy SFTP  install 

Nachdem er den Befehl wird das System die Frage aufwerfen,

Installieren Sie SFTP-Server-Gruppe? Y / N

Wenn die Benutzereingabe als Y dann

SSh Timeout Abschnitt?

Der Benutzer muss den Wert einzugeben

Bitte geben Sie Remote SSH-Port

Der Standardwert ist 22. Der Benutzer kann einen beliebigen Wert eingeben

Geben Sie Server-Host-IP?

Der Benutzer muss mit Benutzername, Passwort und Schlüsselpfad eingeben.

Fügen Sie einen anderen Server?

Wenn der Benutzereingaben wie Y hat er auf neue Servernamen eingeben

Dann wird alles angeschlossen werden.

Wenn der Benutzereingaben wie N vorherigen Server-Namen zugegriffen werden kann.


.. code-block:: bash


 kevell@corp:/# ptdeploy sftp put 

 SFTP on Server group? (Y/N) 
 y 
 Please Enter SSH Timeout in seconds 
 20 
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
 192.168.1.14 
 Please Enter SSH User 
 karthik 
 Please Enter Server Password or Key Path 
 123456 
 Add Another Server? (Y/N) 
 n 
 [Pharaoh Logging] Attempting to load SFTP connections... 
 [Pharaoh Logging] Connection to Server 192.168.1.14 successful. 
 Enter local source file path 
 /home/karunakaran/Desktop/server.odt 
 Enter remote target file path 
 /home/karthik/Desktop/server.odt 
 [Pharaoh Logging] Opening SFTP Connections... 
 [Pharaoh Logging] [192.168.1.14] Executing SFTP Put... 
 [Pharaoh Logging] 1 
 [Pharaoh Logging] [192.168.1.14] SFTP Put Completed... 
 [Pharaoh Logging] All SFTP Puts Completed 
 ****************************** 

 SFTP Put: Success 

 ------------------------------ 
 Installer Finished 
 ****************************** 

.. code-block:: bash


 kevell@corp:/# ptdeploy sftp put --yes --environment-name=karthik --source="/tmp/kk.txt" --target="/tmp/kk.txt" 

 Please Enter SSH Timeout in seconds 
 20 
 Please Enter remote SSH Port 
 22 
 [Pharaoh Logging] Attempting to load SFTP connections... 
 [Pharaoh Logging] Connection to Server 192.168.1.14 successful. 
 [Pharaoh Logging] Opening SFTP Connections... 
 [Pharaoh Logging] [192.168.1.14] Executing SFTP Put... 
 [Pharaoh Logging] 1 
 [Pharaoh Logging] [192.168.1.14] SFTP Put Completed... 
 [Pharaoh Logging] All SFTP Puts Completed 
 ****************************** 
 
 SFTP Put: Success 
 
 ------------------------------ 
 Installer Finished 
 ****************************** 

.. code-block:: bash


 kevell@corp:/# ptdeploy sftp put --yes --source="/home/karunakaran/Desktop/readme.txt" --target="/home/karthik/Desktop/readme.txt" 

 Please Enter SSH Timeout in seconds 
 20 
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
 192.168.1.14 
 Please Enter SSH User 
 karthik 
 Please Enter Server Password or Key Path 
 123456 
 Add Another Server? (Y/N) 
 n 
 [Pharaoh Logging] Attempting to load SFTP connections... 
 [Pharaoh Logging] Connection to Server 192.168.1.14 successful. 
 [Pharaoh Logging] Opening SFTP Connections... 
 [Pharaoh Logging] [192.168.1.14] Executing SFTP Put... 
 [Pharaoh Logging] 1 
 [Pharaoh Logging] [192.168.1.14] SFTP Put Completed... 
 [Pharaoh Logging] All SFTP Puts Completed 
 ****************************** 
 
 SFTP Put: Success 
 
 ------------------------------ 
 Installer Finished 
 ****************************** 

.. code-block:: bash

 kevell@corp:/# ptdeploy sftp get 

 SFTP on Server group? (Y/N) 
 y 
 Please Enter SSH Timeout in seconds 
 200 
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
 192.168.1.14 
 Please Enter SSH User 
 karthik 
 Please Enter Server Password or Key Path 
 123456 
 Add Another Server? (Y/N) 
 n 
 [Pharaoh Logging] Attempting to load SFTP connections... 
 [Pharaoh Logging] Connection to Server 192.168.1.14 successful. 
 Enter remote source file path 
 /tmp/testing 
 Enter local target file path 
 /opt/testr 
 [Pharaoh Logging] Opening SFTP Connections... 
 [Pharaoh Logging] [192.168.1.14] Executing SFTP Get... 
 [Pharaoh Logging] 1 
 [Pharaoh Logging] [192.168.1.14] SFTP Get Completed... 
 [Pharaoh Logging] All SFTP Gets Completed 
 ****************************** 
 
 Shell Result: Success 
 SFTP Get 
 
 ------------------------------ 
 Installer Finished 
 ****************************** 
 

.. code-block:: bash


 kevell@corp:/# ptdeploy sftp get --yes --environment-name=karthik --source="/tmp/testing" --target="/opt/testr" 

 Please Enter SSH Timeout in seconds 
 200 
 Please Enter remote SSH Port 
 22 
 [Pharaoh Logging] Attempting to load SFTP connections... 
 [Pharaoh Logging] Connection to Server 192.168.1.14 successful. 
 [Pharaoh Logging] Opening SFTP Connections... 
 [Pharaoh Logging] [192.168.1.14] Executing SFTP Get... 
 [Pharaoh Logging] 1 
 [Pharaoh Logging] [192.168.1.14] SFTP Get Completed... 
 [Pharaoh Logging] All SFTP Gets Completed 
 ****************************** 
 
 Shell Result: Success 
 SFTP Get 
 
 ------------------------------ 
 Installer Finished 
 ****************************** 

.. code-block:: bash

 kevell@corp:/# ptdeploy sftp get --yes --source="/tmp/testing" --target="/opt/testr" 

 Please Enter SSH Timeout in seconds 
 200 
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
 192.168.1.14 
 Please Enter SSH User 
 karthik 
 Please Enter Server Password or Key Path 
 123456 
 Add Another Server? (Y/N) 
 n 
 [Pharaoh Logging] Attempting to load SFTP connections... 
 [Pharaoh Logging] Connection to Server 192.168.1.14 successful. 
 [Pharaoh Logging] Opening SFTP Connections... 
 [Pharaoh Logging] [192.168.1.14] Executing SFTP Get... 
 [Pharaoh Logging] 1 
 [Pharaoh Logging] [192.168.1.14] SFTP Get Completed... 
 [Pharaoh Logging] All SFTP Gets Completed 
 ****************************** 
 
 Shell Result: Success 
 SFTP Get 
 
 ------------------------------ 
 Installer Finished 
 ****************************** 




.. cssclass:: table-bordered

 +-------------------+-----------------------------+---------------------------+------------------------------------------+
 | Parameter         | Alternative Parameter       | Syntax                    | Kommentare                               |
 +===================+=============================+===========================+==========================================+
 |put                | SFTP, sftp                  | Source to target          | Die Datei übertragen können              |
 +-------------------+-----------------------------+---------------------------+------------------------------------------+
 |get                | SFTP, sftp                  | Path to source            | Die Datei kann von der Remote-System     |
 |                   |                             |                           | heruntergeladen|                         |
 +-------------------+-----------------------------+---------------------------+------------------------------------------+



Vorteile
----------


* Multi-Server von Einöde.
* Die angegebene Datei ist nicht verfügbar Fehlermeldung kommen.
* Erreichbarkeit ist schwierig ohne Genehmigung.
* Automatisch bei bereits überschreiben bei Datei vorhanden.
* Nicht Groß- und Kleinschreibung.
* Geheimhaltung und Sicherheit möglich ist.


  Lösen Kunden die anspruchsvollsten Technologieprobleme und ermöglicht ihren Erfolg ist die SFTP-Mission und Leidenschaft.
