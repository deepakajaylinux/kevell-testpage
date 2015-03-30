============
MediaTools
============

Zusammenfassung
-----------------------

Dieses Modul soll die Installation GC empfohlen Media Tool wie VLC Media Player, der die Produktivität der Benutzer System verbessert. VLC Media Player unterstützt zahlreiche Audio- und Videokompressionsverfahren und Dateiformate, darunter DVD-Video, Video-CD und Streaming-Protokolle. VLC media player (allgemein bekannt als VLC bezeichnet) ist ein tragbares, freie und Open-Source, Cross-Plattform-Media-Player und Streaming-Media-Server, der vom VideoLAN-Projekt geschrieben. Lassen Sie uns darüber, wie dieses Moduls unterstützt die Installation VLC sehen.

Hilfe Befehl
--------------------

Der Befehl help führt die Benutzer über den Zweck und als auch über die Möglichkeiten, die in der Media-Tools Modul enthalten sind. Der Befehl help Listen aus der alternativen Parameter des Media-Tools. Es beschreibt auch die Syntax für die Installation von VLC. Der Befehl help für Media-Tools Modul wird wie unten dargestellt.
.. code-block:: bash
  
 ptconfigure  mediatools help

Die Syntax für die Deklaration den Befehl help ist nicht case sensitive was ein zusätzlicher Vorteil ist. Der folgende Screenshot visualisieren Sie den Befehl help unter Media Tools.

.. code-block:: bash


	Kevell@corp:/# ptconfigure  MediaTools help
	******************************


	This command allows you to install a few GC recommended Media Tools
        for productivity in your system. Currently, we're only including
        VLC Media Player

         MediaTools, media-tools, mediatools, mediatools, media-tools

        - install
        Installs some media tools
        example: ptconfigure  mediatools install

	------------------------------
	End Help


Installation
---------------


Der folgende Befehl verwendet werden, um Media-Tools zu installieren.

.. code-block:: bash

	ptconfigure  mediatools install


Der Screenshot visualisieren seine Funktion.

.. code-block:: bash


        - install
        Installs some media tools
        example: ptconfigure  mediatools install

        ------------------------------
        End Help

If the user proceeds the installation process, the following process occurs during installation.

* Extracts templates from packages
* Reads package lists.
* Builds dependency tree.
* Reads the state information.
* lists out the packages that are automatically installed.
* lists out the extra packages that are installed.
* lists out the suggested packages.
* lists out the new packages that are installed.
* Finally, reports are clearly displayed with the status and results.
* The following screen shot explains the above mentioned process pictorially.


.. code-block:: bash


 kevell@corp:/# ptconfigure mediatools install 
 Install Media Tools? (Y/N) 
 y 
 ******************************* 
 *        Pharaoh Tools        * 
 *         Media Tools!        * 
 ******************************* 
 [Pharaoh Logging] Packages vlc, libdvdread4 from the Packager Apt are already installed, so not installing 
 Creating /tmp/ptconfigure-temp-script-57996813529.sh 
 chmod 755 /tmp/ptconfigure-temp-script-57996813529.sh 2>/dev/null 
 Changing /tmp/ptconfigure-temp-script-57996813529.sh Permissions 
 Executing /tmp/ptconfigure-temp-script-57996813529.sh 
 --2015-03-27 13:21:10--  http://download.videolan.org/pub/debian/stable//Packages 
 Resolving download.videolan.org (download.videolan.org)... 88.191.250.2 
 Connecting to download.videolan.org (download.videolan.org)|88.191.250.2|:80... connected. 
 HTTP request sent, awaiting response... 200 OK 
 Length: 3520 (3.4K) [application/octet-stream] 
 Saving to: â€˜/tmp/dvdcss-2TJ4IX/Packagesâ€™ 

 100%[=======================================================================================================>] 3,520       --.-K/s   in 0s      

 2015-03-27 13:21:11 (77.0 MB/s) - â€˜/tmp/dvdcss-2TJ4IX/Packagesâ€™ saved [3520/3520] 

 --2015-03-27 13:21:12--  http://download.videolan.org/pub/debian/stable/stable/libdvdcss2_1.2.13-0_amd64.deb 
 Resolving download.videolan.org (download.videolan.org)... 88.191.250.2 
 Connecting to download.videolan.org (download.videolan.org)|88.191.250.2|:80... connected. 
 HTTP request sent, awaiting response... 200 OK 
 Length: 44462 (43K) [application/octet-stream] 
 Saving to: â€˜/tmp/dvdcss-2TJ4IX/libdvdcss.debâ€™ 

 100%[=======================================================================================================>] 44,462      65.6KB/s   in 0.7s   

 2015-03-27 13:21:13 (65.6 KB/s) - â€˜/tmp/dvdcss-2TJ4IX/libdvdcss.debâ€™ saved [44462/44462] 

 Selecting previously unselected package libdvdcss2. 
 (Reading database ... 362949 files and directories currently installed.) 
 Preparing to unpack .../dvdcss-2TJ4IX/libdvdcss.deb ... 
 Unpacking libdvdcss2 (1.2.13-0) ... 
 Setting up libdvdcss2 (1.2.13-0) ... 
 Processing triggers for libc-bin (2.19-0ubuntu6.6) ... 
 Temp File /tmp/ptconfigure-temp-script-57996813529.sh Removed 
 ... All done! 
 ******************************* 
 Thanks for installing , visit www.pharaohtools.com for more 
 ****************************** 

 
 Single App Installer: 
 -------------------------------------------- 
 MediaTools: Success 
 ------------------------------ 
 Installer Finished 
 ****************************** 




Options
----------


.. cssclass:: table-bordered

 +----------------------------+----------------------------------------------+-----------+--------------------------------------+
 | Parameter                  |  Alternative Parameter                       | Optionen  | Kommentare                           |
 +============================+==============================================+===========+======================================+
 |Install Media Tools? (Y/N)  | Statt Media Tools, folgende Alternativen     | Y(Yes)    | Wenn der Benutzer wünschen, den      |
 |                            | können ebenfalls verwendet werden            |           | Installationsprozess können sie      |
 |                            | MediaTools, media-tools, mediatools.         |           | Eingang als Y gehen                  |
 +----------------------------+----------------------------------------------+-----------+--------------------------------------+
 |Install Media Tools? (Y/N)  | Statt Media Tools, folgende Alternativen     | N(No)     | Wenn der Benutzer wünschen, den      |
 |                            | können ebenfalls verwendet werden            |           | Installationsprozess können sie      |
 |                            | MediaTools, media-tools, mediatools.         |           | Eingang als N. beenden|              |
 +----------------------------+----------------------------------------------+-----------+--------------------------------------+


Vorteile
------------

* Die in Hilfe und Installation verwendet muss nicht beachtet werden, welche ein zusätzlicher Vorteil ist, während im Vergleich zu anderen 
  Parametern.
* Mit diesem Modul die Produktivität des Systems verbessert werden kann.
* Es ist gut-to-do sowohl Ubuntu und sowie Cent OS.
* Dieses Modul erleichtert die Installation von GC empfohlen Media Tools.

