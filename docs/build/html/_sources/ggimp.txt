=======
GIMP
=======


Zusammenfassung
-----------------------

Dieses Modul ermöglicht es Anwendern, GIMP, die ein beliebtes Bild-Editor zu installieren.

GIMP ein Akronym für GNU Image Manipulation Program) ist für die Bildretusche und Bearbeiten, Freiform-Zeichnung verwendet, Skalieren, Beschneiden, Fotomontagen, die Konvertierung zwischen verschiedenen Bildformaten und mehr spezialisierte Aufgaben.

GIMP ist frei (und nach) jeder verteilt, und jeder kann in ihrem Inhalt und ihrer Quellcode schauen und können Funktionen hinzufügen oder Probleme beheben. Es wird unter LGPLv3 und GPLv3 + Lizenzen freigegeben. GIMP begann 1995 als Schulprojekt von zwei Studenten; Jetzt GIMP ist eine vollwertige Anwendung, auf allen Distributionen von GNU / Linux und die jüngsten Versionen von Microsoft Windows und Mac OS X.

Lassen Sie uns sehen, wie dieses Modul erleichtert die Installation von GIMP aus den anstehenden Themen.


Hilfe Befehl
-------------------

Der Befehl help ist eine kurze Bedienungsanleitung, die die Benutzer über den Zweck dieses Moduls Die Listen outs sein alternatives Parameter, die in den Erklärungen für die Installation von GIMP durch verwendet werden kann, zusammen mit der Syntax Apt-get stellt. Die Syntax für die Hilfe-Option im Rahmen dieses Moduls ist unten dargestellt,

.. code-block:: bash

	ptconfigure GIMP help


Die Syntax für die Deklaration den Befehl help ist nicht case sensitive was ein zusätzlicher Vorteil ist. Der folgende Screenshot visualisieren Sie den Befehl help unter GIMP.

.. code-block:: bash

 kevell@corp:/# ptconfigure GIMP help 
 ******************************** 

  This command allows you to install GIMP, the popular Image Editor 
  GIMP, gimp 

        - install 
        Installs GIMP through apt-get 
        example: ptconfigure gimp install 

 ------------------------------ 
 End Help 
 ****************************** 

Installation
--------------

Der Befehl für die Installation von GIMP durch verwendet apt-get mit diesem Modul ist einfach nur mit Hilfe von unter dem Befehl,

.. code-block:: bash

	ptconfigure GIMP install

Nach der Eingabe des Befehls vor, werden die folgenden Schritte, wie in der Tabelle dargestellt, durchgeführt,

.. cssclass:: table-bordered

 +---------------------+--------------------------------------+--------------+---------------------------------------------------------+
 | Parameters          | Alternative Parameters               | Options      | Kommentar                                               |
 +=====================+======================================+==============+=========================================================+
 |GIMP Install? (Y/N)  | anstelle von GIMP wir verwenden      | Y(Yes)       | Wenn der Benutzer auf Wunsch Installation               |
 |                     | können, gimp also.                   |              | fortzusetzen, können sie Eingang als Y.                 |
 +---------------------+--------------------------------------+--------------+---------------------------------------------------------+
 |GIMP Install? (Y/N)  | anstelle von GIMP wir verwenden      | N(No)        | Wenn der Benutzer wünschen, um die Installation         |
 |                     | können, gimp also.                   |              | zu beenden, können sie Eingang als N.|                  |
 +---------------------+--------------------------------------+--------------+---------------------------------------------------------+

Der folgende Screenshot zeigt visuell über den Prozess der Installation.


.. code-block:: bash


 kevell@corp:/# ptconfigure gimp install 
 Install GIMP? (Y/N) 
 y 
 ******************************* 
 *        Pharaoh Tools        * 
 *          ! GIMP !        * 
 ******************************* 
 Creating /tmp/ptconfigure-temp-script-67656420389.sh 
 chmod 755 /tmp/ptconfigure-temp-script-67656420389.sh 2>/dev/null 
 Changing /tmp/ptconfigure-temp-script-67656420389.sh Permissions 
 Executing /tmp/ptconfigure-temp-script-67656420389.sh 
 Reading package lists... 
 Building dependency tree... 
 Reading state information... 
 The following package was automatically installed and is no longer required: 
  libjemalloc1 
 Use 'apt-get autoremove' to remove it. 
 The following extra packages will be installed: 
  gimp-data libamd2.3.1 libbabl-0.1-0 libblas3 libcamd2.3.1 libccolamd2.8.0 
  libcholmod2.1.2 libgegl-0.2-0 libgfortran3 libgimp2.0 libilmbase6 
  libjavascriptcoregtk-1.0-0 liblapack3 libmng2 libopenexr6 libumfpack5.6.2 
  libwebkitgtk-1.0-0 libwebkitgtk-1.0-common 
 Suggested packages: 
  gimp-help-en gimp-help gimp-data-extras 
 The following NEW packages will be installed: 
  gimp gimp-data libamd2.3.1 libbabl-0.1-0 libblas3 libcamd2.3.1 
  libccolamd2.8.0 libcholmod2.1.2 libgegl-0.2-0 libgfortran3 libgimp2.0 
  libilmbase6 libjavascriptcoregtk-1.0-0 liblapack3 libmng2 libopenexr6 
  libumfpack5.6.2 libwebkitgtk-1.0-0 libwebkitgtk-1.0-common 
 0 upgraded, 19 newly installed, 0 to remove and 6 not upgraded. 
 Need to get 14.2 MB/19.7 MB of archives. 
 After this operation, 87.2 MB of additional disk space will be used. 
 Get:1 http://archive.ubuntu.com/ubuntu/ trusty-proposed/main libwebkitgtk-1.0-0 amd64 2.4.8-1ubuntu1/ubuntu14.04.1 [7,224 kB] 
 Get:2 http://archive.ubuntu.com/ubuntu/ trusty-proposed/main libwebkitgtk-1.0-0 amd64 2.4.8-1ubuntu1/ubuntu14.04.1 [7,224 kB] 
 Get:3 http://archive.ubuntu.com/ubuntu/ trusty/main libgimp2.0 amd64 2.8.10-0ubuntu1 [484 kB] 
 Get:4 http://archive.ubuntu.com/ubuntu/ trusty/main gimp-data all 2.8.10-0ubuntu1 [3,068 kB] 
 Get:5 http://archive.ubuntu.com/ubuntu/ trusty/main gimp amd64 2.8.10-0ubuntu1 [3,411 kB] 
 Fetched 9,355 kB in 18min 31s (8,412 B/s) 
 Selecting previously unselected package libamd2.3.1:amd64. 
 (Reading database ... 381874 files and directories currently installed.) 
 Preparing to unpack .../libamd2.3.1_1%3a4.2.1-3ubuntu1_amd64.deb ... 
 Unpacking libamd2.3.1:amd64 (1:4.2.1-3ubuntu1) ... 
 Selecting previously unselected package libbabl-0.1-0:amd64. 
 Preparing to unpack .../libbabl-0.1-0_0.1.10-1ubuntu2_amd64.deb ... 
 Unpacking libbabl-0.1-0:amd64 (0.1.10-1ubuntu2) ... 
 Selecting previously unselected package libcamd2.3.1:amd64. 
 Preparing to unpack .../libcamd2.3.1_1%3a4.2.1-3ubuntu1_amd64.deb ... 
 Unpacking libcamd2.3.1:amd64 (1:4.2.1-3ubuntu1) ... 
 Selecting previously unselected package libccolamd2.8.0:amd64. 
 Preparing to unpack .../libccolamd2.8.0_1%3a4.2.1-3ubuntu1_amd64.deb ... 
 Unpacking libccolamd2.8.0:amd64 (1:4.2.1-3ubuntu1) ... 
 Selecting previously unselected package libblas3. 
 Preparing to unpack .../libblas3_1.2.20110419-7_amd64.deb ... 
 Unpacking libblas3 (1.2.20110419-7) ... 
 Selecting previously unselected package libgfortran3:amd64. 
 Preparing to unpack .../libgfortran3_4.8.2-19ubuntu1_amd64.deb ... 
 Unpacking libgfortran3:amd64 (4.8.2-19ubuntu1) ... 
 Selecting previously unselected package liblapack3. 
 Preparing to unpack .../liblapack3_3.5.0-2ubuntu1_amd64.deb ... 
 Unpacking liblapack3 (3.5.0-2ubuntu1) ... 
 Selecting previously unselected package libcholmod2.1.2:amd64. 
 Preparing to unpack .../libcholmod2.1.2_1%3a4.2.1-3ubuntu1_amd64.deb ... 
 Unpacking libcholmod2.1.2:amd64 (1:4.2.1-3ubuntu1) ... 
 Selecting previously unselected package libilmbase6:amd64. 
 Preparing to unpack .../libilmbase6_1.0.1-6ubuntu1_amd64.deb ... 
 Unpacking libilmbase6:amd64 (1.0.1-6ubuntu1) ... 
 Selecting previously unselected package libopenexr6:amd64. 
 Preparing to unpack .../libopenexr6_1.6.1-7ubuntu1_amd64.deb ... 
 Unpacking libopenexr6:amd64 (1.6.1-7ubuntu1) ... 
 Selecting previously unselected package libumfpack5.6.2:amd64. 
 Preparing to unpack .../libumfpack5.6.2_1%3a4.2.1-3ubuntu1_amd64.deb ... 
 Unpacking libumfpack5.6.2:amd64 (1:4.2.1-3ubuntu1) ... 
 Selecting previously unselected package libgegl-0.2-0:amd64. 
 Preparing to unpack .../libgegl-0.2-0_0.2.0-4ubuntu1_amd64.deb ... 
 Unpacking libgegl-0.2-0:amd64 (0.2.0-4ubuntu1) ... 
 Selecting previously unselected package libjavascriptcoregtk-1.0-0:amd64. 
 Preparing to unpack .../libjavascriptcoregtk-1.0-0_2.4.8-1ubuntu1/ubuntu14.04.1_amd64.deb ... 
 Unpacking libjavascriptcoregtk-1.0-0:amd64 (2.4.8-1ubuntu1/ubuntu14.04.1) ... 
 Selecting previously unselected package libmng2:amd64. 
 Preparing to unpack .../libmng2_2.0.2-0ubuntu3_amd64.deb ... 
 Unpacking libmng2:amd64 (2.0.2-0ubuntu3) ... 
 Selecting previously unselected package libwebkitgtk-1.0-common. 
 Preparing to unpack .../libwebkitgtk-1.0-common_2.4.8-1ubuntu1/ubuntu14.04.1_all.deb ... 
 Unpacking libwebkitgtk-1.0-common (2.4.8-1ubuntu1/ubuntu14.04.1) ... 
 Selecting previously unselected package libwebkitgtk-1.0-0:amd64. 
 Preparing to unpack .../libwebkitgtk-1.0-0_2.4.8-1ubuntu1/ubuntu14.04.1_amd64.deb ... 
 Unpacking libwebkitgtk-1.0-0:amd64 (2.4.8-1ubuntu1/ubuntu14.04.1) ... 
 Selecting previously unselected package libgimp2.0. 
 Preparing to unpack .../libgimp2.0_2.8.10-0ubuntu1_amd64.deb ... 
 Unpacking libgimp2.0 (2.8.10-0ubuntu1) ... 
 Selecting previously unselected package gimp-data. 
 Preparing to unpack .../gimp-data_2.8.10-0ubuntu1_all.deb ... 
 Unpacking gimp-data (2.8.10-0ubuntu1) ... 
 Selecting previously unselected package gimp. 
 Preparing to unpack .../gimp_2.8.10-0ubuntu1_amd64.deb ... 
 Unpacking gimp (2.8.10-0ubuntu1) ... 
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ... 
 Processing triggers for hicolor-icon-theme (0.13-1) ... 
 Processing triggers for mime-support (3.54ubuntu1.1) ... 
 Processing triggers for gnome-menus (3.10.1-0ubuntu2) ... 
 Processing triggers for desktop-file-utils (0.22-1ubuntu1) ... 
 Processing triggers for bamfdaemon (0.5.1+14.04.20140409-0ubuntu1) ... 
 Rebuilding /usr/share/applications/bamf-2.index... 
 Setting up libamd2.3.1:amd64 (1:4.2.1-3ubuntu1) ... 
 Setting up libbabl-0.1-0:amd64 (0.1.10-1ubuntu2) ... 
 Setting up libcamd2.3.1:amd64 (1:4.2.1-3ubuntu1) ... 
 Setting up libccolamd2.8.0:amd64 (1:4.2.1-3ubuntu1) ... 
 Setting up libblas3 (1.2.20110419-7) ... 
 update-alternatives: using /usr/lib/libblas/libblas.so.3 to provide /usr/lib/libblas.so.3 (libblas.so.3) in auto mode 
 Setting up libgfortran3:amd64 (4.8.2-19ubuntu1) ... 
 Setting up liblapack3 (3.5.0-2ubuntu1) ... 
 update-alternatives: using /usr/lib/lapack/liblapack.so.3 to provide /usr/lib/liblapack.so.3 (liblapack.so.3) in auto mode 
 Setting up libcholmod2.1.2:amd64 (1:4.2.1-3ubuntu1) ... 
 Setting up libilmbase6:amd64 (1.0.1-6ubuntu1) ... 
 Setting up libopenexr6:amd64 (1.6.1-7ubuntu1) ... 
 Setting up libumfpack5.6.2:amd64 (1:4.2.1-3ubuntu1) ... 
 Setting up libgegl-0.2-0:amd64 (0.2.0-4ubuntu1) ... 
 Setting up libjavascriptcoregtk-1.0-0:amd64 (2.4.8-1ubuntu1/ubuntu14.04.1) ... 
 Setting up libmng2:amd64 (2.0.2-0ubuntu3) ... 
 Setting up libwebkitgtk-1.0-common (2.4.8-1ubuntu1/ubuntu14.04.1) ... 
 Setting up libwebkitgtk-1.0-0:amd64 (2.4.8-1ubuntu1/ubuntu14.04.1) ... 
 Setting up libgimp2.0 (2.8.10-0ubuntu1) ... 
 Setting up gimp-data (2.8.10-0ubuntu1) ... 
 Setting up gimp (2.8.10-0ubuntu1) ... 
 Processing triggers for libc-bin (2.19-0ubuntu6.6) ... 
 Temp File /tmp/ptconfigure-temp-script-67656420389.sh Removed 
 ... All done! 
 ******************************* 
 Thanks for installing , visit www.pharaohtools.com for more 
 ****************************** 

 Single App Installer: 
 -------------------------------------------- 
 GIMP: Success 
 ------------------------------ 
 Installer Finished 
 ******************************  




Vorteile
----------

* Die verwendeten Hilfe und andere unterschiedliche Merkmale von apt erklärt Parameter wird nicht zwischen Groß- und Kleinschreibung.
* Es ist gut-to-do in beiden Cent os und als auch in Ubuntu.


GIMP bietet auch "intelligente" Werkzeuge, die einen komplexeren Algorithmus verwenden, um Dinge, die sonst zeitaufwändig oder unmöglich machen. Dazu zählen ein:

* Klonen-Werkzeug, das Kopien Pixel mit einem Pinsel
* Reparatur-Pinsel, die Kopien Pixel aus einem Bereich und Ton und Farbe korrigiert
* Perspective Klon-Werkzeug, das wie das Klon-Werkzeug funktioniert, aber korrigiert Abstandsänderungen
* Unschärfe und schärfen Werkzeug Unschärfen und schärft mit einem Pinsel
* Dodge und Burn-Tool ist ein Pinsel, der Zielbildpunkte heller (Winkelzüge) oder dunkler (Verbrennungen) macht


GIMP verwandeln Tools gehören:

* Richten
* Sich Bewegen
* Crop
* Drehen
* Skala
* Shear
* Perspective
* Flip

