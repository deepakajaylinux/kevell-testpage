=========
PhpSSH
=========

Zusammenfassung
-----------------------

 PhpSSH ist jetzt noch einfacher geworden, um es zum Laufen zu bringen. Macht es viel einfacher, um die automatische Aktualisierung ptconfigure über PhpSSH. Unter Remote-Shell,

für die Durchführung verschiedener Aufgaben ist eine Norm, wenn der Benutzer mehrere Maschinen Server in einer Infrastruktur.

Hilfe Befehl
--------------

In diesem Befehl help, wird der Benutzer diskutieren ein solches Tool, das entwickelt wurde, um die Mängel in den vergangenen Remote-Shell-Programmen zu vermeiden. ptconfigure Thema von Interesse für diesen Befehl ist kein anderer als der sichere Verkauf, besser bekannt als phpSSH bekannt. Der Befehl, um Hilfe wie folgt

.. code-block:: bash

                ptconfigure PHPSSH help

Die Syntax für die Deklaration den Befehl help ist nicht case sensitive was ein zusätzlicher Vorteil ist. Der folgende Screenshot visualisieren Sie den Befehl help unter PHP SSH.

.. code-block:: bash

 kevell@corp:/# ptconfigure PHPSSH help
 ******************************


  This command allows you to install the PHP SSH default Module

  PHPSSH, php-ssh, phpssh

        - install
        Installs the PECL PHP SSH Extension.
        example: ptconfigure phpssh install

 ------------------------------
 End Help
 ******************************
Installation
---------------------

Dies ist ein bekannter Prozess Phpssh Modul unter ptconfigure installieren, indem einfach mit dem Befehl unten angegeben,

.. code-block:: bash
         
                ptconfigure phpssh install

Nach der Eingabe des Befehls oben, sind die folgenden Schritte im Prozess der Installation beteiligt, wie in der Tabelle beschrieben,

.. cssclass:: table-bordered

 +------------------------+--------------------------------------+-----------+----------------------------------------------------------+
 | Parameters             | Alternative Parameter                | Optionen  | Kommentare                                               |
 +========================+======================================+===========+==========================================================+
 |Install PHP SSH? (Y/N)  | anstelle von using PHP SSH Wir       | Y(Yes)    | Wenn der Benutzer wünschen, den                          |
 |                        | verwenden PHPSSH, phpssh,php-ssh     |           | Installationsprozess können sie Eingang als Y. gehen     |
 +------------------------+--------------------------------------+-----------+----------------------------------------------------------+
 |Install PHP SSH? (Y/N)  | anstelle von using PHP SSH Wir       | N(No)     | Wenn der Benutzer wünschen, den                          |
 |                        | verwenden PHPSSH, phpssh,php-ssh     |           | Installationsprozess können sie Eingang als N. beenden|  |
 +------------------------+--------------------------------------+-----------+----------------------------------------------------------+

Wenn der Benutzer geht der Installation, während des Prozesses der Anlage wird in den folgenden Listen beschrieben:


* Baut die Abhängigkeitsstruktur.
* Liest den Status Informationen.
* Liste outs die zusätzlichen Pakete, installieren.
* Liste outs die neuen Pakete installieren.
* Details über die Anzahl der Dateien aktualisiert, neu installiert, entfernt und nicht aktualisiert.



Der folgende Screenshot zeigt bildhaft die oben beschriebene Prozess der Installation.

.. code-block:: bash


 kevell@corp:/# ptconfigure phpssh install
 Install PHP SSH? (Y/N)
 Y
 *******************************
 *        Pharaoh Tools        *
 *         PHP SSH!        *
 *******************************
 
 Creating config file /etc/php5/mods-available/ssh2.ini with new version
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  libssh2-1
 The following NEW packages will be installed:
  libssh2-1 libssh2-php
 0 upgraded, 2 newly installed, 0 to remove and 301 not upgraded.
 Need to get 91.0 kB of archives.
 After this operation, 389 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libssh2-1 amd64 1.4.3-2 [66.3 kB]
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libssh2-php amd64 0.12-1build1 [24.7 kB]
 Fetched 91.0 kB in 4s (19.8 kB/s)
 Selecting previously unselected package libssh2-1:amd64.
 (Reading database ... 183000 files and directories currently installed.)
 Preparing to unpack .../libssh2-1_1.4.3-2_amd64.deb ...
 Unpacking libssh2-1:amd64 (1.4.3-2) ...
 Selecting previously unselected package libssh2-php.
 Preparing to unpack .../libssh2-php_0.12-1build1_amd64.deb ...
 Unpacking libssh2-php (0.12-1build1) ...
 Setting up libssh2-1:amd64 (1.4.3-2) ...
 Setting up libssh2-php (0.12-1build1) ...
 Processing triggers for libc-bin (2.19-0ubuntu6) ...
 [Pharaoh Logging] Adding Package libssh2-php from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 PHPSSH: Success
 ------------------------------
 Installer Finished
 ******************************

Vorteile
-----------------

* Die erste und wichtigste ist die Privatsphäre der Kommunikation. Das bedeutet, die Verbindung, die eine Remote-Shell-Login bietet, muss es 
  sein verschlüsselt, um das Abhören zu verhindern.
* Es muss ein Mechanismus, um zu prüfen, ob die von einer der Parteien zu senden Daten nicht verändert oder manipuliert werden. Kurz gesagt, ist  Integritätsprüfung notwendig.
* Identität sowohl der Server und Client müssen aufeinander gestellt werden, um eine ordnungsgemäße Authentifizierung einzurichten.
* Verschlüsselungs und Authentifizierungsmechanismen durch PhpSSH vorgesehen erhöht die Sicherheit in einem größeren Ausmaß.

