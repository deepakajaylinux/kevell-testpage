==========
Memcached
==========

Zusammenfassung
-----------------

Der Hauptaspekt dieses Moduls ist für die Installation und Aktualisierung der memcache mit der neuesten Version.
Memcached ist ein Mehrzweck-Distributed-Memory-Caching-System. Es wird häufig verwendet, um durch die Zwischenspeicherung von Daten und Objekten im Arbeitsspeicher, um die Anzahl, wie oft eine externe Datenquelle (wie zB einer Datenbank oder API) hinausgehen, darf gelesen werden beschleunigen dynamische Datenbank-gestützte Websites.


Lassen Sie uns über den Prozess der Installation und Verwendung dieses Moduls im kommenden Themen sehe

Hilfe Befehl
---------------------

Der Befehl help führt den Anwender über den Zweck und als auch über die Möglichkeiten, die in der Memcached-Modul enthalten sind. Es listet einige der alternativen Parameter der Memcached-Modul. Es beschreibt auch die Syntax für die Installation des Memcached Moduls. Der Befehl help für Memcached-Modul ist wie unten dargestellt.

.. code-block:: bash

		ptconfigure  Memcached help

Die Syntax für die Deklaration den Befehl help ist nicht case sensitive was ein zusätzlicher Vorteil ist. Der folgende Screenshot visualisieren Sie den Befehl help unter Memcached.

.. code-block:: bash

 kevell@corp:/# ptconfigure Memcached help

 ******************************


  This command allows you to update Memcached.

  Memcached, memcached

        - install
        Installs the latest version of memcache
        example: ptconfigure  memcached install

 ------------------------------
 End Help
 ******************************

Die Syntax für die Deklaration den Befehl help ist nicht case sensitive was ein zusätzlicher Vorteil ist. Der folgende Screenshot visualisieren Sie den Befehl help unter Memcached.
Nach der Eingabe des Befehls oben, passiert folgendes Verfahren im Tabellenformat angezeigt.

.. cssclass:: table-bordered


 +-------------------------+-------------------------------------------+-------------+------------------------------------------+
 | Parameter               |  Alternative Parameter                    | Optionen    | Kommentare                               |
 +=========================+===========================================+=============+==========================================+
 |Install Memcached? (Y/N) | Statt of memcached wir verwenden können,  | Y(Yes)      | Wenn der Benutzer wünschen, den          |
 |                         | Memcached also.                           |             | Installationsprozess können sie          |
 |                         |                                           |             | Eingang als Y gehen                      |
 +-------------------------+-------------------------------------------+-------------+------------------------------------------+
 |Install Memcached? (Y/N) | Statt of memcached wir verwenden können,  | N(No)       | Wenn der Benutzer wünschen, den          |
 |                         | Memcached also.                           |             | Installationsprozess können sie          |
 |                         |                                           |             | Eingang als N. beenden|                  |
 +-------------------------+-------------------------------------------+-------------+------------------------------------------+

Der folgende Screenshot kann Ihnen eine bildliche Darstellung in Bezug auf den Prozess der Installation.

.. code-block:: bash

 kevell@corp:/# ptconfigure memcached install 
 Install Memcached? (Y/N) 
 y 
 ******************************* 
 *        Pharaoh Tools        * 
 *         Memcached!        * 
 ******************************* 
 Creating /tmp/ptconfigure-temp-script-43944931598.sh 
 chmod 755 /tmp/ptconfigure-temp-script-43944931598.sh 2>/dev/null 
 Changing /tmp/ptconfigure-temp-script-43944931598.sh Permissions 
 Executing /tmp/ptconfigure-temp-script-43944931598.sh 
 Ign http://dl.google.com stable InRelease 
 Hit http://dl.google.com stable Release.gpg 
 Hit http://dl.google.com stable Release 
 Hit http://dl.google.com stable/main amd64 Packages 
 Ign http://security.ubuntu.com trusty-security InRelease 
 Hit http://dl.google.com stable/main i386 Packages 
 Ign http://us.archive.ubuntu.com precise InRelease 
 Ign http://archive.canonical.com precise InRelease 
 Ign http://archive.ubuntu.com trusty InRelease 
 Hit http://downloads.hipchat.com stable InRelease 
 Ign http://packages.elasticsearch.org stable InRelease 
 Get:1 http://security.ubuntu.com trusty-security Release.gpg [933 B] 
 Ign http://us.archive.ubuntu.com precise-security InRelease 
 Ign http://archive.ubuntu.com trusty-updates InRelease 
 Ign http://packages.elasticsearch.org stable InRelease 
 Ign http://pkg.jenkins-ci.org binary/ InRelease 
 Hit http://archive.canonical.com precise Release.gpg 
 Get:2 http://security.ubuntu.com trusty-security Release [63.5 kB] 
 Hit http://downloads.hipchat.com stable/main amd64 Packages 
 Ign http://us.archive.ubuntu.com precise-updates InRelease 
 Ign http://archive.ubuntu.com trusty-proposed InRelease 
 Ign http://packages.elasticsearch.org stable InRelease 
 Ign http://dl.google.com stable/main Translation-en_IN 
 Hit http://archive.canonical.com precise Release 
 Ign http://dl.google.com stable/main Translation-en 
 Hit http://downloads.hipchat.com stable/main i386 Packages 
 Ign http://us.archive.ubuntu.com precise-backports InRelease 
 Hit http://mirror.stshosting.co.uk precise InRelease 
 Hit http://packages.elasticsearch.org stable Release.gpg 
 Hit http://archive.canonical.com precise/partner Sources 
 Hit http://packages.elasticsearch.org stable Release.gpg 
 Get:3 http://security.ubuntu.com trusty-security/universe amd64 Packages [89.7 kB] 
 Ign http://archive.ubuntu.com trusty-backports InRelease 
 Hit http://archive.canonical.com precise/partner amd64 Packages 
 Hit http://packages.elasticsearch.org stable Release.gpg 
 Ign http://downloads-distro.mongodb.org dist InRelease 
 Hit http://archive.ubuntu.com trusty Release.gpg 
 Hit http://us.archive.ubuntu.com precise Release.gpg 
 Hit http://packages.elasticsearch.org stable Release 
 Get:4 http://us.archive.ubuntu.com precise-security Release.gpg [198 B] 
 Get:5 http://archive.ubuntu.com trusty-updates Release.gpg [933 B] 
 Hit http://packages.elasticsearch.org stable Release 
 Get:6 http://us.archive.ubuntu.com precise-updates Release.gpg [198 B] 
 Get:7 http://archive.ubuntu.com trusty-proposed Release.gpg [933 B] 
 Hit http://archive.canonical.com precise/partner i386 Packages 
 Hit http://us.archive.ubuntu.com precise-backports Release.gpg 
 Hit http://archive.ubuntu.com trusty-backports Release.gpg 
 Get:8 http://oss.oracle.com unstable InRelease 
 Ign http://oss.oracle.com unstable InRelease 
 Hit http://us.archive.ubuntu.com precise Release 
 Hit http://packages.elasticsearch.org stable Release 
 Hit http://archive.ubuntu.com trusty Release 
 Get:9 http://us.archive.ubuntu.com precise-security Release [54.3 kB] 
 Hit http://packages.elasticsearch.org stable/main amd64 Packages 
 Get:10 http://archive.ubuntu.com trusty-updates Release [63.5 kB] 
 Hit http://packages.elasticsearch.org stable/main i386 Packages 
 Get:11 http://security.ubuntu.com trusty-security/restricted amd64 Packages [8,875 B] 
 Ign http://downloads.hipchat.com stable/main Translation-en_IN 
 Get:12 http://security.ubuntu.com trusty-security/multiverse amd64 Packages [3,459 B] 
 Ign http://archive.canonical.com precise/partner Translation-en 
 Get:13 http://security.ubuntu.com trusty-security/main amd64 Packages [251 kB] 
 Hit http://oss.oracle.com unstable Release 
 Ign http://oss.oracle.com unstable Release 
 Ign http://extras.ubuntu.com precise InRelease 
 Get:14 http://archive.ubuntu.com trusty-proposed Release [211 kB] 
 Hit http://extras.ubuntu.com precise Release.gpg 
 Get:15 http://oss.oracle.com unstable/main amd64 Packages 
 Ign http://downloads.hipchat.com stable/main Translation-en 
 Hit http://extras.ubuntu.com precise Release 
 Get:16 http://us.archive.ubuntu.com precise-updates Release [196 kB] 
 Hit http://extras.ubuntu.com precise/main Sources 
 Ign http://oss.oracle.com unstable/main i386 Packages/DiffIndex 
 Hit http://extras.ubuntu.com precise/main amd64 Packages 
 Ign http://oss.oracle.com unstable/non-free i386 Packages/DiffIndex 
 Hit http://packages.elasticsearch.org stable/main amd64 Packages 
 Hit http://extras.ubuntu.com precise/main i386 Packages 
 Hit http://packages.elasticsearch.org stable/main i386 Packages 
 Get:17 http://security.ubuntu.com trusty-security/universe i386 Packages [89.6 kB] 
 Hit http://packages.elasticsearch.org stable/main amd64 Packages 
 Hit http://us.archive.ubuntu.com precise-backports Release 
 Hit http://packages.elasticsearch.org stable/main i386 Packages 
 Hit http://us.archive.ubuntu.com precise/main Sources 
 Hit http://oss.oracle.com unstable/main i386 Packages 
 Hit http://us.archive.ubuntu.com precise/restricted Sources 
 Get:18 http://security.ubuntu.com trusty-security/restricted i386 Packages [8,846 B] 
 Hit http://oss.oracle.com unstable/non-free i386 Packages 
 Hit http://us.archive.ubuntu.com precise/universe Sources 
 Get:19 http://security.ubuntu.com trusty-security/multiverse i386 Packages [3,628 B] 
 Get:20 http://oss.oracle.com unstable/main Translation-en_IN 
 Hit http://us.archive.ubuntu.com precise/multiverse Sources 
 Get:21 http://security.ubuntu.com trusty-security/main i386 Packages [241 kB] 
 Ign http://extras.ubuntu.com precise/main Translation-en_IN 
 Hit http://us.archive.ubuntu.com precise/main amd64 Packages 
 Hit http://us.archive.ubuntu.com precise/restricted amd64 Packages 
 Ign http://extras.ubuntu.com precise/main Translation-en 
 Hit http://archive.ubuntu.com trusty-backports Release 
 Hit http://us.archive.ubuntu.com precise/universe amd64 Packages 
 Hit http://archive.ubuntu.com trusty/main Sources 
 Hit http://archive.ubuntu.com trusty/universe Sources 
 Hit http://us.archive.ubuntu.com precise/multiverse amd64 Packages 
 Hit http://archive.ubuntu.com trusty/restricted Sources 
 Hit http://us.archive.ubuntu.com precise/main i386 Packages 
 Hit http://archive.ubuntu.com trusty/multiverse Sources 
 Hit http://us.archive.ubuntu.com precise/restricted i386 Packages 
 Hit http://repo.mysql.com trusty InRelease 
 Hit http://archive.ubuntu.com trusty/main amd64 Packages 
 Hit http://archive.ubuntu.com trusty/universe amd64 Packages 
 Hit http://us.archive.ubuntu.com precise/universe i386 Packages 
 Hit http://archive.ubuntu.com trusty/restricted amd64 Packages 
 Ign http://apt.newrelic.com newrelic InRelease 
 Hit http://us.archive.ubuntu.com precise/multiverse i386 Packages 
 Hit http://archive.ubuntu.com trusty/multiverse amd64 Packages 
 Hit http://security.ubuntu.com trusty-security/main Translation-en 
 Hit http://archive.ubuntu.com trusty/main i386 Packages 
 Hit http://security.ubuntu.com trusty-security/multiverse Translation-en 
 Hit http://us.archive.ubuntu.com precise/main Translation-en 
 Hit http://archive.ubuntu.com trusty/universe i386 Packages 
 Ign http://ppa.launchpad.net trusty InRelease 
 Hit http://security.ubuntu.com trusty-security/restricted Translation-en 
 Ign http://ppa.launchpad.net trusty InRelease 
 Hit http://archive.ubuntu.com trusty/restricted i386 Packages 
 Hit http://security.ubuntu.com trusty-security/universe Translation-en 
 Hit http://us.archive.ubuntu.com precise/multiverse Translation-en 
 Hit http://archive.ubuntu.com trusty/multiverse i386 Packages 
 Hit http://us.archive.ubuntu.com precise/restricted Translation-en 
 Get:22 http://www.apache.org 21x InRelease [3,167 B] 
 Hit http://us.archive.ubuntu.com precise/universe Translation-en 
 Hit http://archive.ubuntu.com trusty/main Translation-en 
 Get:23 http://us.archive.ubuntu.com precise-security/main Sources [125 kB] 
 Hit http://archive.ubuntu.com trusty/multiverse Translation-en 
 Ign http://packages.elasticsearch.org stable/main Translation-en_IN 
 Hit http://archive.ubuntu.com trusty/restricted Translation-en 
 Hit http://pkg.jenkins-ci.org binary/ Release.gpg 
 Ign http://packages.elasticsearch.org stable/main Translation-en 
 Err http://oss.oracle.com unstable/main amd64 Packages 
   HttpError404 
 Hit http://mirror.stshosting.co.uk precise/main amd64 Packages 
 Ign http://packages.elasticsearch.org stable/main Translation-en_IN 
 Err http://oss.oracle.com unstable/non-free amd64 Packages 
   HttpError404 
 Hit http://archive.ubuntu.com trusty/universe Translation-en 
 Hit http://mirror.stshosting.co.uk precise/main i386 Packages 
 Ign http://packages.elasticsearch.org stable/main Translation-en 
 Ign http://oss.oracle.com unstable/main Translation-en_IN 
 Get:24 http://archive.ubuntu.com trusty-updates/universe amd64 Packages [260 kB] 
 Ign http://packages.elasticsearch.org stable/main Translation-en_IN 
 Ign http://oss.oracle.com unstable/main Translation-en 
 Ign http://packages.elasticsearch.org stable/main Translation-en 
 Ign http://oss.oracle.com unstable/non-free Translation-en_IN 
 Ign http://oss.oracle.com unstable/non-free Translation-en 
 Hit http://downloads-distro.mongodb.org dist Release.gpg 
 Get:25 http://us.archive.ubuntu.com precise-security/restricted Sources [3,759 B] 
 Get:26 http://us.archive.ubuntu.com precise-security/universe Sources [34.2 kB] 
 Get:27 http://us.archive.ubuntu.com precise-security/multiverse Sources [1,815 B] 
 Get:28 http://us.archive.ubuntu.com precise-security/main amd64 Packages [492 kB] 
 Hit http://repo.mysql.com trusty/mysql-5.6 Sources 
 Hit http://repo.mysql.com trusty/mysql-5.6 amd64 Packages 
 Hit http://repo.mysql.com trusty/mysql-5.6 i386 Packages 
 Hit http://apt.newrelic.com newrelic Release.gpg 
 Hit http://ppa.launchpad.net trusty Release.gpg 
 Hit http://ppa.launchpad.net trusty Release.gpg 
 Get:29 http://archive.ubuntu.com trusty-updates/restricted amd64 Packages [9,238 B] 
 Get:30 http://archive.ubuntu.com trusty-updates/multiverse amd64 Packages [11.8 kB] 
 Get:31 http://www.apache.org 21x/main amd64 Packages [698 B] 
 Get:32 http://archive.ubuntu.com trusty-updates/main amd64 Packages [488 kB] 
 Get:33 http://www.apache.org 21x/main i386 Packages [698 B] 
 Hit http://pkg.jenkins-ci.org binary/ Release 
 Hit http://downloads-distro.mongodb.org dist Release 
 Get:34 http://us.archive.ubuntu.com precise-security/restricted amd64 Packages [8,943 B] 
 Get:35 http://us.archive.ubuntu.com precise-security/universe amd64 Packages [108 kB] 
 Get:36 http://us.archive.ubuntu.com precise-security/multiverse amd64 Packages [2,463 B] 
 Get:37 http://us.archive.ubuntu.com precise-security/main i386 Packages [531 kB] 
 Hit http://apt.newrelic.com newrelic Release 
 Hit http://ppa.launchpad.net trusty Release 
 Hit http://ppa.launchpad.net trusty Release 
 Get:38 http://archive.ubuntu.com trusty-updates/universe i386 Packages [262 kB] 
 Hit http://pkg.jenkins-ci.org binary/ Packages 
 Get:39 http://archive.ubuntu.com trusty-updates/restricted i386 Packages [9,256 B] 
 Get:40 http://archive.ubuntu.com trusty-updates/multiverse i386 Packages [11.9 kB] 
 Get:41 http://archive.ubuntu.com trusty-updates/main i386 Packages [477 kB] 
 Hit http://downloads-distro.mongodb.org dist/10gen amd64 Packages 
 Hit http://downloads-distro.mongodb.org dist/10gen i386 Packages 
 Hit http://archive.ubuntu.com trusty-updates/main Translation-en 
 Hit http://archive.ubuntu.com trusty-updates/multiverse Translation-en 
 Hit http://archive.ubuntu.com trusty-updates/restricted Translation-en 
 Hit http://archive.ubuntu.com trusty-updates/universe Translation-en 
 Get:42 http://archive.ubuntu.com trusty-proposed/universe amd64 Packages [28.6 kB] 
 Hit http://apt.newrelic.com newrelic/non-free amd64 Packages 
 Hit http://apt.newrelic.com newrelic/non-free i386 Packages 
 Get:43 http://archive.ubuntu.com trusty-proposed/restricted amd64 Packages [28 B] 
 Get:44 http://archive.ubuntu.com trusty-proposed/multiverse amd64 Packages [1,134 B] 
 Get:45 http://archive.ubuntu.com trusty-proposed/main amd64 Packages [159 kB] 
 Hit http://ppa.launchpad.net trusty/main amd64 Packages 
 Hit http://ppa.launchpad.net trusty/main i386 Packages 
 Hit http://ppa.launchpad.net trusty/main Translation-en 
 Hit http://ppa.launchpad.net trusty/main amd64 Packages 
 Hit http://ppa.launchpad.net trusty/main i386 Packages 
 Hit http://ppa.launchpad.net trusty/main Translation-en 
 Get:46 http://archive.ubuntu.com trusty-proposed/universe i386 Packages [28.6 kB] 
 Get:47 http://us.archive.ubuntu.com precise-security/restricted i386 Packages [8,939 B] 
 Get:48 http://archive.ubuntu.com trusty-proposed/restricted i386 Packages [28 B] 
 Get:49 http://us.archive.ubuntu.com precise-security/universe i386 Packages [116 kB] 
 Get:50 http://archive.ubuntu.com trusty-proposed/multiverse i386 Packages [1,133 B] 
 Get:51 http://archive.ubuntu.com trusty-proposed/main i386 Packages [155 kB] 
 Get:52 http://us.archive.ubuntu.com precise-security/multiverse i386 Packages [2,652 B] 
 Hit http://us.archive.ubuntu.com precise-security/main Translation-en 
 Hit http://us.archive.ubuntu.com precise-security/multiverse Translation-en 
 Hit http://us.archive.ubuntu.com precise-security/restricted Translation-en 
 Hit http://us.archive.ubuntu.com precise-security/universe Translation-en 
 Get:53 http://us.archive.ubuntu.com precise-updates/main Sources [487 kB] 
 Hit http://archive.ubuntu.com trusty-proposed/main Translation-en 
 Hit http://archive.ubuntu.com trusty-proposed/multiverse Translation-en 
 Hit http://archive.ubuntu.com trusty-proposed/restricted Translation-en 
 Hit http://archive.ubuntu.com trusty-proposed/universe Translation-en 
 Hit http://archive.ubuntu.com trusty-backports/universe amd64 Packages 
 Hit http://archive.ubuntu.com trusty-backports/restricted amd64 Packages 
 Hit http://archive.ubuntu.com trusty-backports/multiverse amd64 Packages 
 Hit http://archive.ubuntu.com trusty-backports/main amd64 Packages 
 Hit http://archive.ubuntu.com trusty-backports/universe i386 Packages 
 Hit http://archive.ubuntu.com trusty-backports/restricted i386 Packages 
 Hit http://archive.ubuntu.com trusty-backports/multiverse i386 Packages 
 Hit http://archive.ubuntu.com trusty-backports/main i386 Packages 
 Hit http://archive.ubuntu.com trusty-backports/main Translation-en 
 Ign http://mirror.stshosting.co.uk precise/main Translation-en_IN 
 Hit http://archive.ubuntu.com trusty-backports/multiverse Translation-en 
 Hit http://archive.ubuntu.com trusty-backports/restricted Translation-en 
 Hit http://archive.ubuntu.com trusty-backports/universe Translation-en 
 Ign http://mirror.stshosting.co.uk precise/main Translation-en 
 Get:54 http://us.archive.ubuntu.com precise-updates/restricted Sources [7,981 B] 
 Get:55 http://us.archive.ubuntu.com precise-updates/universe Sources [112 kB] 
 Ign http://repo.mysql.com trusty/mysql-5.6 Translation-en_IN 
 Get:56 http://us.archive.ubuntu.com precise-updates/multiverse Sources [9,417 B] 
 Ign http://archive.ubuntu.com trusty/main Translation-en_IN 
 Get:57 http://us.archive.ubuntu.com precise-updates/main amd64 Packages [884 kB] 
 Ign http://archive.ubuntu.com trusty/multiverse Translation-en_IN 
 Ign http://archive.ubuntu.com trusty/restricted Translation-en_IN 
 Ign http://archive.ubuntu.com trusty/universe Translation-en_IN 
 Ign http://repo.mysql.com trusty/mysql-5.6 Translation-en 
 Ign http://www.apache.org 21x/main Translation-en_IN 
 Ign http://www.apache.org 21x/main Translation-en 
 Ign http://pkg.jenkins-ci.org binary/ Translation-en_IN 
 Ign http://pkg.jenkins-ci.org binary/ Translation-en 
 Ign http://downloads-distro.mongodb.org dist/10gen Translation-en_IN 
 Ign http://downloads-distro.mongodb.org dist/10gen Translation-en 
 Ign http://apt.newrelic.com newrelic/non-free Translation-en_IN 
 Ign http://apt.newrelic.com newrelic/non-free Translation-en 
 Get:58 http://us.archive.ubuntu.com precise-updates/restricted amd64 Packages [13.6 kB] 
 Get:59 http://us.archive.ubuntu.com precise-updates/universe amd64 Packages [255 kB] 
 Get:60 http://us.archive.ubuntu.com precise-updates/multiverse amd64 Packages [16.4 kB] 
 Get:61 http://us.archive.ubuntu.com precise-updates/main i386 Packages [922 kB] 
 Get:62 http://us.archive.ubuntu.com precise-updates/restricted i386 Packages [13.6 kB] 
 Get:63 http://us.archive.ubuntu.com precise-updates/universe i386 Packages [264 kB] 
 Get:64 http://us.archive.ubuntu.com precise-updates/multiverse i386 Packages [16.6 kB] 
 Hit http://us.archive.ubuntu.com precise-updates/main Translation-en 
 Hit http://us.archive.ubuntu.com precise-updates/multiverse Translation-en 
 Hit http://us.archive.ubuntu.com precise-updates/restricted Translation-en 
 Hit http://us.archive.ubuntu.com precise-updates/universe Translation-en 
 Hit http://us.archive.ubuntu.com precise-backports/main Sources 
 Hit http://us.archive.ubuntu.com precise-backports/restricted Sources 
 Hit http://us.archive.ubuntu.com precise-backports/universe Sources 
 Hit http://us.archive.ubuntu.com precise-backports/multiverse Sources 
 Hit http://us.archive.ubuntu.com precise-backports/main amd64 Packages 
 Hit http://us.archive.ubuntu.com precise-backports/restricted amd64 Packages 
 Hit http://us.archive.ubuntu.com precise-backports/universe amd64 Packages 
 Hit http://us.archive.ubuntu.com precise-backports/multiverse amd64 Packages 
 Hit http://us.archive.ubuntu.com precise-backports/main i386 Packages 
 Hit http://us.archive.ubuntu.com precise-backports/restricted i386 Packages 
 Hit http://us.archive.ubuntu.com precise-backports/universe i386 Packages 
 Hit http://us.archive.ubuntu.com precise-backports/multiverse i386 Packages 
 Hit http://us.archive.ubuntu.com precise-backports/main Translation-en 
 Hit http://us.archive.ubuntu.com precise-backports/multiverse Translation-en 
 Hit http://us.archive.ubuntu.com precise-backports/restricted Translation-en 
 Hit http://us.archive.ubuntu.com precise-backports/universe Translation-en 
 Ign http://us.archive.ubuntu.com precise/main Translation-en_IN 
 Ign http://us.archive.ubuntu.com precise/multiverse Translation-en_IN 
 Ign http://us.archive.ubuntu.com precise/restricted Translation-en_IN 
 Ign http://us.archive.ubuntu.com precise/universe Translation-en_IN 
 Fetched 7,633 kB in 2min 57s (43.1 kB/s) 
 Temp File /tmp/ptconfigure-temp-script-43944931598.sh Removed 
 Reading package lists... 
 Building dependency tree... 
 Reading state information... 
 Some packages could not be installed. This may mean that you have 
 requested an impossible situation or if you are using the unstable 
 distribution that some required packages have not yet been created 
 or been moved out of Incoming. 
 The following information may help to resolve the situation:  

 The following packages have unmet dependencies: 
 mysql-server-5.5 : Depends: mysql-client-5.5 (>= 5.5.41-0ubuntu0.14.04.1) 
 [Pharaoh Logging] Adding Package mysql-server-5.5 from the Packager Apt did not execute correctly 
 [Pharaoh Logging] Package mysql-server from the Packager Apt is already installed, so not installing 
 [Pharaoh Logging] Package php5-mysql from the Packager Apt is already installed, so not installing 
 [Pharaoh Logging] Package php5 from the Packager Apt is already installed, so not installing 
 Reading package lists... 
 Building dependency tree... 
 Reading state information... 
 The following packages were automatically installed and are no longer required: 
   java-wrappers libjargs-java pear-channels php5-xdebug 
 Use 'apt-get autoremove' to remove them. 
 The following extra packages will be installed: 
   php-pear 
 Suggested packages: 
  php5-dev 
 The following NEW packages will be installed: 
  php-pear php5-memcached 
 0 upgraded, 2 newly installed, 0 to remove and 34 not upgraded. 
 Need to get 0 B/307 kB of archives. 
 After this operation, 2,475 kB of additional disk space will be used. 
 Selecting previously unselected package php-pear. 
 (Reading database ... 362745 files and directories currently installed.) 
 Preparing to unpack .../php-pear_5.5.9+dfsg-1ubuntu4.7_all.deb ... 
 Unpacking php-pear (5.5.9+dfsg-1ubuntu4.7) ... 
 Selecting previously unselected package php5-memcached. 
 Preparing to unpack .../php5-memcached_2.1.0-6build1_amd64.deb ... 
 Unpacking php5-memcached (2.1.0-6build1) ... 
 Processing triggers for doc-base (0.10.5) ... 
 Processing 1 added doc-base file... 
 Setting up php-pear (5.5.9+dfsg-1ubuntu4.7) ... 
 Setting up php5-memcached (2.1.0-6build1) ... 
 [Pharaoh Logging] Adding Package php5-memcached from the Packager Apt executed correctly 
 Reading package lists... 
 Building dependency tree... 
 Reading state information... 
 The following packages were automatically installed and are no longer required: 
  java-wrappers libjargs-java pear-channels php5-xdebug 
 Use 'apt-get autoremove' to remove them. 
 Suggested packages: 
  libcache-memcached-perl libmemcached 
 The following NEW packages will be installed: 
  memcached 
 0 upgraded, 1 newly installed, 0 to remove and 34 not upgraded. 
 Need to get 66.7 kB of archives. 
 After this operation, 229 kB of additional disk space will be used. 
 Get:1 http://archive.ubuntu.com/ubuntu/ trusty/main memcached amd64 1.4.14-0ubuntu9 [66.7 kB] 
 Fetched 66.7 kB in 2s (24.0 kB/s) 
 Selecting previously unselected package memcached. 
 (Reading database ... 362947 files and directories currently installed.) 
 Preparing to unpack .../memcached_1.4.14-0ubuntu9_amd64.deb ... 
 Unpacking memcached (1.4.14-0ubuntu9) ... 
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ... 
 Processing triggers for ureadahead (0.100.0-16) ... 
 Setting up memcached (1.4.14-0ubuntu9) ... 
 Starting memcached: memcached. 
 Processing triggers for ureadahead (0.100.0-16) ... 
 [Pharaoh Logging] Adding Package memcached from the Packager Apt executed correctly 
 ... All done! 
 ******************************* 
 Thanks for installing , visit www.pharaohtools.com for more 
 ****************************** 


 Single App Installer: 
 -------------------------------------------- 
 Memcached: Success 
 ------------------------------ 
 Installer Finished 
 ******************************  



Funktionen des Memcached
-------------------------------

Während der Verwendung des Memcached kann der Prozess zu lesen und umzusetzen, die folgenden Funktionen, die im memcached enthalten sind,

* Memcache :: hinzufügen - Setzen Sie einen Artikel auf den Server
* Memcache :: addServer - zum Verbindungspool hinzufügen Memcached Server
* Memcache :: close - Close Memcached-Server-Verbindung
* Memcache :: connect - Offene Memcached-Server-Verbindung
* Memcache :: Dekrement - Wert Decrement Elements
* Memcache :: löschen - Los Löschen vom Server
* Memcache :: flush - alle vorhandenen Einträge auf dem Server
* Memcache :: get - abrufen Artikel vom Server
* Memcache :: getExtendedStats - Holen Sie Statistiken für alle Server im Pool
* Memcache :: GetServerStatus - Gibt den Serverstatus
* Memcache :: getStats - Get Statistiken des Servers
* Memcache :: getVersion - Return Version des Servers
* Memcache :: Schritt - Wert Schrittweite Elements
* Memcache :: pconnect - Offene Memcached Server persistente Verbindung
* Memcache :: ersetzen - Wert der bestehenden Artikel ersetzen
* Memcache :: set - Speichern Sie Daten auf dem Server
* Memcache :: setCompressThreshold - Aktivieren Sie die automatische Komprimierung von großen Werten
* Memcache :: setServerParams - Änderungen Server Parameter und Status zur Laufzeit

Vorteile
------------

* Die in Hilfe und Installation verwendet muss nicht beachtet werden, welche ein zusätzlicher Vorteil ist, während im Vergleich zu anderen 
  Parametern.
* Es ist gut-to-do sowohl Ubuntu und sowie Cent OS.
* Dies wird Modul installiert die Memcached in aktualisierte Version.
* Wenn das Modul bereits in der Benutzermaschine vorhandene es wird eine Meldung angezeigt werden, da sie bereits vorhanden sind.

