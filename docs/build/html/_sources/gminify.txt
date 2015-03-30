=========
Minify
=========

Zusammenfassung
-----------------------

Minify ist die Entfernung von unnötigen Zeichen aus dem Quellcode. Mini, wenn als Präfix verwendet wird, bedeutet, klein. Das Ziel ist minify Quellcode "kleineren" zu machen und die Leistung zu verbessern.

Der Begriff wird oft mit minify interpretiert Skriptsprachen wie PHP, die bereitgestellt werden und über das Internet übertragen verbunden. Code, der durch den Austausch läuft von Räumen durch ein Leerzeichen, zB minimierte wurde, ist leichter und benötigt weniger Zeit für ein Browser zu laden. Beliebte minify Werkzeuge für Web-Entwicklung sind Kompressor und ubuntu Compiler. Minifizieren passt mit Ubuntu und Cent-OS arbeiten.

Hilfe Befehl
-----------------------

Minifizieren macht Paketentwicklung ein Kinderspiel: Konzeptionell ist minify ähnlich Kompression. Anders als Code, der komprimiert worden ist, aber Code, minimierte Gruppe kann weiterhin mit, ohne den zusätzlichen Schritt der Dekompression erforderlich eingearbeitet werden. Verkleinerte Quellencode kann auch als eine Art von Verschleierung verwendet werden, wenn der Begriff Verschleierung kann als eine Form der falschen Kryptographie unterscheiden, während ein verkleinertes Code Beispiel kann mit einem Pretty-Printer umgekehrt werden kann.

Der folgende Befehl help führt den Benutzer zu minify behandeln.

.. code-block:: bash

                ptconfigure  minify help

Dieser Screenshot zeigt den Befehl help Nutzung

.. code-block:: bash

 kevell@corp:/# ptconfigure minify help

 ******************************


  This command allows you to update Minify.

  Minify, minify

        - install
        Installs the latest version of minify
        example: ptconfigure minify install

 ------------------------------
 End Help
 ******************************


Installation
------------------

Es arbeitet mit den bestehenden Konventionen für Code-Struktur, indem effiziente Werkzeuge, um den Kreislauf der Codierung Entwicklung zu unterstützen. Mit minify, die Entwicklung einer Codierung wird so einfach, dass es der Benutzer Standard-Layout, wenn der Benutzer schreibt eine erhebliche Menge an Code. Dieser Befehl zum Installieren minify ist wie folgt,

.. code-block:: bash

                ptconfigure  minify install

Die folgende Abbildung erklärt es.


.. code-block:: bash


 kevell@corp:/# ptconfigure minify install 
 Install Minify? (Y/N) 
 y 
 ******************************* 
 *        Pharaoh Tools        * 
 *         Minify!        * 
 ******************************* 
 Reading package lists... 
 Building dependency tree... 
 Reading state information... 
 The following packages were automatically installed and are no longer required: 
  libmemcached10 pear-channels php5-xdebug 
 Use 'apt-get autoremove' to remove them. 
 The following extra packages will be installed: 
  java-wrappers libjargs-java 
 Suggested packages: 
  libjargs-java-doc 
 The following NEW packages will be installed: 
  java-wrappers libjargs-java yui-compressor 
 0 upgraded, 3 newly installed, 0 to remove and 34 not upgraded. 
 Need to get 587 kB of archives. 
 After this operation, 776 kB of additional disk space will be used. 
 Get:1 http://archive.ubuntu.com/ubuntu/ trusty/main java-wrappers all 0.1.27 [9,908 B] 
 Get:2 http://archive.ubuntu.com/ubuntu/ trusty/main libjargs-java all 1.0.0-4 [14.3 kB] 
 Get:3 http://archive.ubuntu.com/ubuntu/ trusty/main yui-compressor all 2.4.7-1 [563 kB] 
 Fetched 587 kB in 41s (14.2 kB/s) 
 Selecting previously unselected package java-wrappers. 
 (Reading database ... 362717 files and directories currently installed.) 
 Preparing to unpack .../java-wrappers_0.1.27_all.deb ... 
 Unpacking java-wrappers (0.1.27) ... 
 Selecting previously unselected package libjargs-java. 
 Preparing to unpack .../libjargs-java_1.0.0-4_all.deb ... 
 Unpacking libjargs-java (1.0.0-4) ... 
 Selecting previously unselected package yui-compressor. 
 Preparing to unpack .../yui-compressor_2.4.7-1_all.deb ... 
 Unpacking yui-compressor (2.4.7-1) ... 
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ... 
 Setting up java-wrappers (0.1.27) ... 
 Setting up libjargs-java (1.0.0-4) ... 
 Setting up yui-compressor (2.4.7-1) ... 
 [Pharaoh Logging] Adding Package yui-compressor from the Packager Apt executed correctly 
 ... All done! 
 ******************************* 
 Thanks for installing , visit www.pharaohtools.com for more 
 ****************************** 


 Single App Installer: 
 -------------------------------------------- 
 Minify: Success 
 ------------------------------ 
 Installer Finished 
 ****************************** 

Option
----------

Minify Quellcode ist besonders nützlich für interpretierte Sprachen bereitgestellt und über das Internet übertragen werden, weil sie die Menge an Daten, die übertragen werden muss, reduziert.

.. cssclass:: table-bordered


 +---------------------------+-----------------------------------------+------------+-------------------------------------------+
 | Parameter                 |  Alternative Parameter                  | Optionen   | Kommentare                                |
 +===========================+=========================================+============+===========================================+
 |Install minify?(Y/N)       | Anstelle der Verwendung minify wir      | Y          | Es installiert minify unter ptconfigure   |
 |                           | verwenden können, Minify                |            |                                           |
 +---------------------------+-----------------------------------------+------------+-------------------------------------------+
 |Install minify?(Y/N)       | Anstelle der Verwendung minify wir      | N          | Das System Ausfahrt die Installation      |
 |                           | verwenden können, Minify|               |            |                                           |
 +---------------------------+-----------------------------------------+------------+-------------------------------------------+


Vorteile
------------

* Minifizieren kommuniziert über PHP-Programmierung.
* Minifizieren Komfort mit Ubuntu und Cent-OS.
* Minifizieren unterstützt Nicht Groß- und Kleinschreibung.
* Minifizieren zieht unnötigen Zeichen aus dem Quellcode.

