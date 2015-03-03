===============
SshKeyInstall
===============

Zusammenfassung
------------------------

SSH-Schlüssel installieren verwendet werden, um SSH-Schlüssel für einen neuen Benutzer zu installieren. Eine Authentifizierung ist sicherer als Passwort-Authentifizierung. Dies ist besonders wichtig, wenn das System im Internet sichtbar ist. Bei Authentifizierung über öffentliche Schlüssel hat der Authentisierungsinstanz einen öffentlichen Schlüssel und einen privaten Schlüssel. Jede Taste ist eine große Zahl mit speziellen mathematischen Eigenschaften. Es eignet sich mit Ubuntu und CentOS.

Hilfe Befehl
-------------------------

Die Befehlshilfe führt die Benutzer über den Zweck und als auch über die Möglichkeiten, die in der SSHKEY enthalten sind, installieren Modul. Es listet einige der alternativen Parameter Sshkeyinstall Modul. Es beschreibt auch die Syntax für die Installation des Sshkeyinstall Moduls. Der Befehl help für Sshkeyinstall Modul wird wie unten dargestellt.

.. code-block:: bash
 
		ptconfigure Sshkeyinstall help

Die Syntax für die Deklaration den Befehl help wird nicht zwischen Groß- und Klein was ein zusätzlicher Vorteil ist. Der folgende Screenshot den Benutzer über den Befehl help unter Sshkeyinstall visualisieren.

.. code-block:: bash

 kevell@corp:/# ptconfigure SshKeyInstall help

 ******************************


  This command allows you to install an SSH Public key for a user

  SshKeyInstall, sshkeyinstall, ssh-key-install

        - public-key
        Add an SSH Public Key to an account
        example: ptconfigure ssh-key-install public-key
        example: ptconfigure ssh-key-install public-key --yes --public-key-data="zzzzz"
        example: ptconfigure ssh-key-install public-key --yes --public-key-file="id_rsa.pub" --user-name=dave

 ------------------------------
 End Help
 ******************************

Installation
------------------

Die Installation umfasst die Installation von Sshkeyinstall erforderlich, um die Installation in einer aktualisierten Version zu machen. Es ist eine offensichtliche Prozess Sshkeyinstall Modul unter ptconfigure Sshkeyinstall installieren, indem einfach mit dem Befehl unten angegeben,

.. code-block:: bash

 		ptconfigure  Sshkeyinstall  public-key

Nach beleben den Befehl geben Sie den Wert katechisieren.

Wenn die Benutzereingaben wie ja es wird automatisch Sshkeyinstall mit der Überprüfung aus dem System zu installieren. Wenn nicht beenden Sie die Installation. Der folgende Screenshot demonstSshkeyinstallte Sshkeyinstall es.

Options
--------------

.. cssclass:: table-bordered

 +----------------------------+--------------------------------------------+-------------+--------------------------------------------+
 | Parameters                 | Alternate Parameters                       | Optionen    | Kommentare                                 |
 +============================+============================================+=============+============================================+
 |Install Sshkeyinstall?(Y/N) | Anstelle der Verwendung SshKeyInstall wir  | Y           | Es wird installiert Sshkeyinstall unter    |
 |                            | verwenden können, Sshkeyinstall,           |             | ptconfigure in Pharaoh tools               |
 |                            | ssh-key-install                            |             |                                            |
 +----------------------------+--------------------------------------------+-------------+--------------------------------------------+
 |Install Sshkeyinstall?(Y/N) | Anstelle der Verwendung SshKeyInstall wir  | N           | Das System Ausfahrt die Installation       |
 |                            | verwenden können, Sshkeyinstall,           |             |                                            |
 |                            | ssh-key-install|                           |             |                                            |
 +----------------------------+--------------------------------------------+-------------+--------------------------------------------+

Vorteile
----------------

* Sshkeyinstall ist gut-to-do in Ubuntu und CentOS
* Sshkeyinstall kann nicht Kleinschreibung Überfall
* Sshkeyinstall ist flexibel
* Sshkeyinstall verwendet installieren sshkey

