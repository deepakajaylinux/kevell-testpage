============
VNCPasswd
============

Zusammenfassung
--------------------------

Die vncpasswd Dienstprogramm zu verwenden, um zu erstellen, und ändern Sie die Passwörter für den VNC-Server-Authentifizierung. Sie verwendet solche Passwörter beim Start mit dem lokalen Desktop-Manager, wenn aus dem Skript vncserver gestartet. vncpasswd erlaubt, entweder eine oder zwei Passwörter eingeben. Die vncpasswd Dienstprogramm fragt interaktiv, ob er die zweite Passwort festlegen. Dies ist am bequemsten mit ubunt und CentOS.

Hilfe Befehl
----------------------

Hilfe Befehl umfasst ein umfangreiches, konsolenbasierten Hilfesystem, erinnert man-Seiten in Ubuntu. Die Hilfethemen enthalten auch Hilfe für die Installation des PASSWORT zum Remote- und lokalen Bereich. Einfach, um die Befehle ohne Argumente zu schreiben.

.. code-block:: bash

                ptconfigure  VNC-passwd help

Der folgende Screenshot kann sie sichtbar zu machen.

.. code-block:: bash

 kevell@corp:/# ptconfigure VNCPasswd help

 ******************************


  This command allows you to install VNCPasswd, the popular Remote/Local Desktop Manager Solution.

  VNCPasswd, vncpasswd, vnc-passwd

        - install
        Installs VNCPasswd through a package manager
        example: ptconfigure vnc install

 ------------------------------
 End Help
 ******************************

Installation
-----------------

Installation kann der Benutzer vncpassward installieren. Es ist sehr beliebt im Remote- oder lokalen Desktop. Es installiert die vnc passwd durch Paket Manager.The erste Passwort ist auch das erste, das zweite Passwort für schreibgeschützten authentication.It verwendet wird, ist bequem mit Ubuntu und CentOS werden.

.. code-block:: bash

                ptconfigure  VNC-passwd install

Nach dem Schlüssel im Befehl kann das System den Benutzer zur Eingabe fragen. Wenn die Benutzereingabe als Y kann es die VNCpassward anderes installieren kann zu verlassen. folgende Screenshot kann sie sichtbar zu machen.

.. code-block:: bash

 kevell@corp:/# ptconfigure VNC-passwd install

 Install VNCPasswd? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *          ! VNCPasswd !        *
 *******************************
 E: Could not get lock /var/cache/apt/archives/lock - open (11: Resource temporarily unavailable)
 E: Unable to lock directory /var/cache/apt/archives/
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following packages were automatically installed and are no longer required:
  gyp libc-ares-dev libc-ares2 libjs-node-uuid libv8-3.14-dev
  linux-headers-3.13.0-32 linux-headers-3.13.0-32-generic
  linux-image-3.13.0-32-generic linux-image-extra-3.13.0-32-generic
  node-abbrev node-ansi node-archy node-async node-block-stream
  node-combined-stream node-cookie-jar node-delayed-stream node-forever-agent
  node-form-data node-fstream node-fstream-ignore node-github-url-from-git
  node-glob node-graceful-fs node-gyp node-inherits node-ini
  node-json-stringify-safe node-lockfile node-lru-cache node-mime
  node-minimatch node-mkdirp node-mute-stream node-node-uuid node-nopt
  node-normalize-package-data node-npmlog node-once node-osenv node-qs
  node-read node-read-package-json node-request node-retry node-rimraf
  node-semver node-sha node-sigmund node-slide node-tar node-tunnel-agent
  node-which nodejs nodejs-dev ttf-dejavu-core
 Use 'apt-get autoremove' to remove them.
 The following NEW packages will be installed:
  expect
 0 upgraded, 1 newly installed, 0 to remove and 79 not upgraded.
 9 not fully installed or removed.
 [Pharaoh Logging] Adding Package expect from the Packager Apt did not execute correctly
 Enter VNC User:

 Enter VNC Pass:

 Creating /tmp/ptconfigure-temp-script-40114506906.sh
 chmod 755 /tmp/ptconfigure-temp-script-40114506906.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-40114506906.sh Permissions
 Executing /tmp/ptconfigure-temp-script-40114506906.sh
 sudo: unknown user: /usr/bin/expect
 sudo: unable to initialize policy plugin
 Temp File /tmp/ptconfigure-temp-script-40114506906.sh Removed
 [Pharaoh Logging] Removing Package expect
 E: Could not get lock /var/cache/apt/archives/lock - open (11: Resource temporarily unavailable)
 E: Unable to lock directory /var/cache/apt/archives/
 Reading package lists...
 Building dependency tree...
 Reading state information...
 Package 'expect' is not installed, so not removed
 The following packages were automatically installed and are no longer required:
  gyp libc-ares-dev libc-ares2 libjs-node-uuid libv8-3.14-dev
  linux-headers-3.13.0-32 linux-headers-3.13.0-32-generic
  linux-image-3.13.0-32-generic linux-image-extra-3.13.0-32-generic
  node-abbrev node-ansi node-archy node-async node-block-stream
  node-combined-stream node-cookie-jar node-delayed-stream node-forever-agent
  node-form-data node-fstream node-fstream-ignore node-github-url-from-git
  node-glob node-graceful-fs node-gyp node-inherits node-ini
  node-json-stringify-safe node-lockfile node-lru-cache node-mime
  node-minimatch node-mkdirp node-mute-stream node-node-uuid node-nopt
  node-normalize-package-data node-npmlog node-once node-osenv node-qs
  node-read node-read-package-json node-request node-retry node-rimraf
  node-semver node-sha node-sigmund node-slide node-tar node-tunnel-agent
  node-which nodejs nodejs-dev ttf-dejavu-core
 Use 'apt-get autoremove' to remove them.
 0 upgraded, 0 newly installed, 0 to remove and 79 not upgraded.
 9 not fully installed or removed.
 [Pharaoh Logging] Package expect from the Packager Apt is not installed, so not removed.
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 VNCPasswd: Success
 ------------------------------
 Installer Finished
 ******************************

Options
---------------

.. cssclass:: table-bordered

 +-------------------------+------------------------------------------------------+---------------+----------------------------------------+
 | Parameters              | Alternate Parameters                                 | Option        | Kommentare                             |
 +=========================+======================================================+===============+========================================+
 |Install VNCpasswd?(Y/N)  | Anstelle der Verwendung von vncpasswd wir verwenden  | Y             | Es wird installiert VNCPassward        |
 |                         | können, VNCPasswd,vncpasswd,vnc-passward             |               | unter ptconfigure                      |
 +-------------------------+------------------------------------------------------+---------------+----------------------------------------+
 |Install VNCpasswd?(Y/N)  | Anstelle der Verwendung von vncpasswd wir verwenden  |               | Das System Ausfahrt die Installation   |
 |                         | können, VNCPasswd,vncpasswd,vnc-passward|            |               |                                        |
 +-------------------------+------------------------------------------------------+---------------+----------------------------------------+

Vorteile
-----------------

* Multi-Language-Support
* VNC Authentisierung
* Optimierte Leistung
* Dateiübertragung möglich
* Leistungsstarke Bereitstellungsstrategien

