================
MysqlAdmins
================

Zusammenfassung
-------------------------

Dieses Modul hilft bei der Installation und als auch die Verwaltung der Admin-Benutzer für MySQL ohne Root-Benutzer. Durch die Nutzung dieser, können die Benutzer ihre administrativen Funktionen zu verwalten.

Hilfe Befehl
---------------

Die Hilfe-Befehl führt den Anwender in Bezug auf den Befehl für die Installation der MySQL-Administratoren verwendet werden, und auch seine Vorteile. Der Befehl für die Hilfe-Option im Rahmen dieser MySQL Administratoren verwendet wird unten gezeigt.

.. code-block:: bash

	ptconfigure  MysqlAdmins help

Der Screenshot wie unten angegeben können die Benutzer im Umgang mit dem Befehl help für MySQL Administratoren führen.

.. code-block:: bash


 kevell@corp:/# ptconfigure  MysqlAdmins help
 ******************************


  This command allows you to install admin users for MySQL so that MySQL can
  be managed without using the Root User.

  MysqlAdmins, mysql-admins, mysqladmins

        - install
        Installs Mysql Admin Users.
        example: ptconfigure  mysql-admins install

 ------------------------------
 End Help
 ******************************

Installation
-------------

Installation von MySQL Administratoren auf Ihren Rechner erleichtert die Benutzer festlegen, und ihre Verwaltungsaktionen verwalten. Der Befehl für die Installation von MySQL-Administratoren verwendet wird unten markiert.

.. code-block:: bash

	ptconfigure  MysqlAdmins install

Darüber hinaus sind die folgenden in tabellarischer Form dargestellt Operationen.

.. cssclass:: table-bordered

 +--------------------------+--------------------------------------------------+------------+-----------------------------------------+
 | Parameter                | Alternative Parameter                            | Optionen   | Kommentare                              | 
 +==========================+==================================================+============+=========================================+
 |Install Admin User for    | An der Stelle MysqlAdmins Diese alternative      | Y(Yes)     | Wenn der Benutzer wünschen, den         |
 |MySQL? (Y/N)              | Namen verwendet werden können: mysql-admins,     |            | Installationsprozess können sie Eingang |
 |                          | mysqladmins.                                     |            | als Y. gehen                            |
 +--------------------------+--------------------------------------------------+------------+-----------------------------------------+
 |Install MySQL Server?     | mysql-admins,mysqladmins.                        | N(No)      | Wenn der Benutzer den                   |
 |(Y/N)                     |                                                  |            | Installationsprozess Wunsch können sie  |
 |                          |                                                  |            | Eingang als N zu beenden|               |
 +--------------------------+--------------------------------------------------+------------+-----------------------------------------+

Wenn der Benutzer den Installationsprozess zu gehen, können sie ihre Verwaltungsfunktionen , indem Sie die folgenden Bedingungen zu gestalten.

* MySQL-Benutzer root
* MySQL Root-Pass
* MySQL New Admin Benutzer
* MySQL New Admin Pass

Wenn der Benutzer wünschen, Installation von MySQL-Administratoren in einem Remote-System können sie festlegen, zu verarbeiten:

* MySQL-Host.

Die folgende Abbildung gibt Ihnen eine bildliche Darstellung über den Prozess der Installation, wie oben beschrieben.

.. code-block:: bash


 kevell@corp:/# ptconfigure mysql-admins install 
 Install Admin User for MySQL? (Y/N) 
 y 
 ******************************* 
 *        Pharaoh Tools        * 
 *         MySQL Admins!        * 
 ******************************* 
 Enter MySQL Root User: 
 root 
 Enter MySQL Root Pass: 
 root123 
 Enter MySQL New Admin User: 
 kevells 
 Enter MySQL New Admin Pass: 
 kevells
 Enter MySQL Host: Enter nothing for 127.0.0.1 
 127.0.0.1   
 Creating /tmp/ptconfigure-temp-script-4745646149.sh 
 chmod 755 /tmp/ptconfigure-temp-script-4745646149.sh 2>/dev/null 
 Changing /tmp/ptconfigure-temp-script-4745646149.sh Permissions 
 Executing /tmp/ptconfigure-temp-script-4745646149.sh 
 Warning: Using a password on the command line interface can be insecure. 
 Temp File /tmp/ptconfigure-temp-script-4745646149.sh Removed 
 ... All done! 
 ******************************* 
 Thanks for installing , visit www.pharaohtools.com for more 
 ****************************** 


 Single App Installer: 
 -------------------------------------------- 
 MysqlAdmins: Success 
 ------------------------------ 
 Installer Finished 
 ******************************  




Vorteile
----------

* Bei MySQL Admins ist bereits in der Benutzer installiert, wird eine Nachricht wird erscheinen, um die Benutzer zu informieren, wie sie bereits  installiert ist.
* Durch die Verwendung dieses Moduls die Administratoren können ihre Verwaltungsmaßnahmen gemäß den Anforderungen zu verwalten.
* Sie können den Installationsvorgang auch in einem entfernten System auszuführen.
* Ohne die Root-Benutzern können die Benutzer die MySQL-Administratoren installieren.
