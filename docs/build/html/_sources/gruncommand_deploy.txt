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

 kevell@corp:/# ptdeploy runcommand help 

 ****************************** 

  This allows you to execute an Operating System command. This would primarily be used in an Autopilot. 

  RunCommand, runcommand, run-command 

        - execute 
        Execute a Command 
        example: ptdeploy run-command install --yes --command="ls -lah /tmp" --run-as-user="ubuntu" --background 

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



.. code-block:: bash

 kevell@corp:/# ptdeploy run-command install --yes --command="ls -lah /tmp" --run-as-user="ubuntu" --background 

 ******************************* 
 *   Golden Contact Computing  * 
 *         Run Command        * 
 ******************************* 
 Use NoHup?: (Y/N) 
 y 
 cd /home/karunakaran 
 su  ubuntu 
 nohup ls -lah /tmp & 
 exit 
 Creating /tmp/ptconfigure-temp-script-56005480696.sh 
 chmod 755 /tmp/ptconfigure-temp-script-56005480696.sh 2>/dev/null 
 Changing /tmp/ptconfigure-temp-script-56005480696.sh Permissions 
 Executing /tmp/ptconfigure-temp-script-56005480696.sh 
 No passwd entry for user 'ubuntu' 
 nohup: redirecting stderr to stdout 
 total 92K 
 drwxrwxrwt 10 root        root        4.0K Mar 20 17:06 . 
 drwxr-xr-x 29 root        root        4.0K Mar 20 16:18 .. 
 -rw-------  1 karunakaran karunakaran 4.1K Mar 20 11:27 .bamficonKEKGVX 
 -rw-------  1 karunakaran karunakaran 4.1K Mar 20 11:27 .bamficonMKENVX 
 -rw-------  1 karunakaran karunakaran 4.1K Mar 20 10:07 .bamficonN2NXVX 
 -rw-------  1 karunakaran karunakaran 4.1K Mar 20 11:27 .bamficonSM8KVX 
 -rwxr-xr-x  1 root        root          58 Mar 20 17:06 ptconfigure-temp-script-56005480696.sh 
 -rw-------  1 karunakaran karunakaran    0 Mar 20 09:50 config-err-UrGst6 
 -rw-------  1 root        root        1000 Mar 20 09:49 .configtest.KiQIacNN 
 -rw-r--r--  1 root        root          33 Mar 20 09:50 cxtracker.start.log 
 drwxr-xr-x  2 root        root        4.0K Mar 20 09:50 hsperfdata_root 
 drwxrwxrwt  2 root        root        4.0K Mar 20 09:50 .ICE-unix 
 -rw-r--r--  1 root        root           3 Mar 20 15:40 kk.txt 
 drwx------  2 karunakaran karunakaran 4.0K Mar 20 16:58 luh3hawd.tmp 
 srwxrwxrwx  1 mongodb     nogroup        0 Mar 20 09:49 mongodb-27017.sock 
 drwx------  2 karunakaran karunakaran 4.0K Mar 20 10:07 .org.chromium.Chromium.VRBmwX 
 srwxrwxr-x  1 karunakaran karunakaran    0 Mar 20 10:06 OSL_PIPE_1000_SingleOfficeIPC_8a32f718ac801a6e525d3030e0878e45 
 -rw-r--r--  1 root        root           0 Mar 20 15:42 papyrusfile 
 drwx------  2 karunakaran karunakaran 4.0K Mar 20 14:33 plugtmp 
 drwxr-xr-x  2 root        root        4.0K Mar 20 14:42 ServerBlocktemp 
 -rw-rw-r--  1 karunakaran karunakaran    0 Mar 20 09:50 unity_support_test.0 
 drwxr-xr-x  2 root        root        4.0K Mar 20 13:02 vhosttemp 
 -r--r--r--  1 root        root          11 Mar 20 09:49 .X0-lock 
 drwxrwxrwt  2 root        root        4.0K Mar 20 09:49 .X11-unix 
 Temp File /tmp/ptconfigure-temp-script-56005480696.sh Removed 
 ... All done! 
 ******************************* 
 Thanks for installing , visit www.gcsoftshop.co.uk for more 
 ****************************** 

 Single App Installer: 
 -------------------------------------------- 

 RunCommand: Success 

 ------------------------------ 
 Installer Finished 
 ****************************** 




Vorteile
------------

* Die Hilfe Befehl deklarieren verwendeten Parameter werden Installation nicht beachtet, welche ein zusätzlicher Vorteil ist, während im 
  Vergleich zu anderen.
* Es ist gut-to-do in beiden Cent OS und als auch in Ubuntu.
* Die Benutzer können den Befehl geben, Name des Benutzers und auch die entweder im Hintergrund oder Front-End-Funktionalität.
* Der Befehl Hilfe führt die Anwender in, wie man den Lauf der Ausführung des Befehls ein auch seinen Zweck.
