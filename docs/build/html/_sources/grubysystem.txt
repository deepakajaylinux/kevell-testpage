==================
RubySystem
==================

Zusammenfassung
------------------------

Ruby-System ist ein dynamisches, reflektierend, High-Level-Skriptsprache. Ruby-System ist nicht nur für die Entwicklung von Webanwendungen Arbeit mit der Ruby-RVM. Es kann auch als ein mächtiger als Skriptsprache und eine sehr gute Alternative zu den üblichen Shell-Skripten verwendet werden, üblicherweise für die Scripting-Anforderungen in Systeme adminstration.Set von eingebauten Modulen und einigen externen Bibliotheken zu erreichen, kann Ruby-System vornehmen Systeme Verabreichung mehr efficient.Ruby System ist ein sehr nützliches und mächtiges Werkzeug, das ist ein Muss in eines jeden Systemadministrator toolbox.It haben ist bequem mit Ubuntu und Cent OS.

Hilfe Befehl
--------------------

Dieser Befehl kann über die Ziele und Befehle unter Ruby-System-Modul funktionieren. Es erklärt auch den Befehl zum Ruby-System zu installieren. Vor der Installation kann der Benutzer lesen diese Hilfe Befehl erklärt seine Funktion.

.. code-block:: bash
        
		ptconfigure RubySystem help


Das folgende Bild hilft Ihnen auch dieses Modul genau verstehen.

.. code-block:: bash

 kevell@corp:/# ptconfigure RubySystem help
 ******************************


  This command allows you to install Ruby RVM, the system wide version.

  RubySystem, rubysystem, ruby-system, rubysys

        - install
        Installs Ruby a System Wide version of Ruby for you
        example: ptconfigure ruby-rvm install

  Ruby is installed the recommended per-user way. To use ruby after the install
  first run "source ~/.rvm/scripts/rvm" to get access to the Ruby install for
  your user, then "rvm install 1.9.3" (to install, specify version as needed)
  then "rvm use 1.9.3" (to select your default version for the session)

 ------------------------------
 End Help
 ******************************


Installation
-------------------

Es ist eine eklatante Prozess Ruby Systemmodul unter ptconfigure installieren, indem einfach mit dem Befehl unten angegeben,

.. code-block:: bash
        
        ptconfigure rubysystem install

After key in the command, it can asks

Install Ruby, system wide?(Y/N)

Falls die Benutzereingaben, wie Y, kann Rubysystem aus dem Paket zu installieren. Else, kann sie den Bildschirm zu verlassen. Die folgenden Screenshots können erklären,es.

.. code-block:: bash


 kevell@corp:/# ptconfigure RubySystem install
 
 Install Ruby, System Wide? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         Ruby System!        *
 *******************************

 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following packages were automatically installed and are no longer required:
  linux-headers-3.13.0-32 linux-headers-3.13.0-32-generic
  linux-image-3.13.0-32-generic linux-image-extra-3.13.0-32-generic
 Use 'apt-get autoremove' to remove them.
 Suggested packages:
  ruby1.9.1-examples ri1.9.1 graphviz ruby1.9.1-dev
 The following NEW packages will be installed:
  ruby1.9.1
 0 upgraded, 1 newly installed, 0 to remove and 12 not upgraded.
 1 not fully installed or removed.
 Need to get 37.5 kB of archives.
 After this operation, 240 kB of additional disk space will be used.
 Get:1 http://us.archive.ubuntu.com/ubuntu/ precise/main ruby1.9.1 amd64 1.9.3.0-1ubuntu1 [37.5 kB]
 Fetched 37.5 kB in 7s (5232 B/s)
 Selecting previously unselected package ruby1.9.1.
 (Reading database ... 282890 files and directories currently installed.)
 Preparing to unpack .../ruby1.9.1_1.9.3.0-1ubuntu1_amd64.deb ...
 Unpacking ruby1.9.1 (1.9.3.0-1ubuntu1) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Setting up zend-server-php-5.3 (6.1.0+b1177) ...
 Module php5 already enabled
 Module rewrite already enabled
 Site zendserver_gui already enabled
 X-Powered-By: PHP/5.3.26 ZendServer/6.1.0
 Content-type: text/html

 Setting up ruby1.9.1 (1.9.3.0-1ubuntu1) ...
 update-alternatives: using /usr/bin/gem1.9.1 to provide /usr/bin/gem (gem) in auto mode
 [Pharaoh Logging] Adding Package ruby1.9.1 from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 RubySystem: Success
 ------------------------------
 Installer Finished
 ******************************

Options
--------------


.. cssclass:: table-bordered

 +-------------------------+--------------------------------------------+-------------+-----------------------------------------+
 | Parameters              | Alternative Parameters                     | Optionen    | Kommentare                              |
 +=========================+============================================+=============+=========================================+
 |ptconfigure Rubysystem   | Anstelle der Verwendung RubySystem,        | Y           | System startet Installation             |
 |Install                  | rubysystem, ruby-system, rubysys.          |             |                                         |
 +-------------------------+--------------------------------------------+-------------+-----------------------------------------+
 |ptconfigure Rubysystem   | Anstelle der Verwendung RubySystem,        | N           | Das System stoppt den                   |
 |Install                  | rubysystem, ruby-system, rubysys.          |             | Installationsprozess|                   |
 +-------------------------+--------------------------------------------+-------------+-----------------------------------------+


Vorteile
----------------

* Ruby-System ist ein dynamisches, reflektierend, High-Level-Skriptsprache für die schnelle und einfache objektorientierte Programmierung.
* In Ruby-System, ist ein bequemer und angenehmer Werkzeug. Einschließlich der Werkzeuge, die im Bereitstellungsprozess verwendet werden.
* Die Ruby-System bereits ein erfahrener Profi mit extremen Wissen sowohl in Web-Entwicklung und allgemeine Softwareentwicklung
  Fähigkeiten.
* Der Hauptvorteil der Programmiersprache Ruby und Ruby-System gilt als die Geschwindigkeit der Entwicklung.


