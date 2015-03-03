============
PHPEclipse
============

Zusammenfassung
-----------------------

PHPEclipse ist eine Reihe von Plugins für die Eclipse-Rahmen die integrierten IDE für PHP-Entwickler bietet. Eclipse und PHPEclipse sind in Java geschrieben und läuft auf allen grafischen Desktop-Umgebungen ausgeführt werden. PHPEclipse ist Open Source Software unter der Common Public Licence frei verfügbar.

Die Eclipse-Plattform bietet den Nutzern eine einheitliche Benutzeroberfläche Paradigma. Ein Software Development IDE ist eine der komplexeren Desktopanwendungen die meisten von uns wahrscheinlich zu verwenden sind, so dass die Zeit für einen Entwickler erforderlich ist, damit effizient mit einer bestimmten IDE kann signifikant sein. Eklipse nicht über diese Zeit zu reduzieren, aber es bietet eine einheitliche Schnittstelle Ansatz, der nur einmal, um effizient mit einer Vielzahl von Programmiersprachen und Werkzeuge zu entwickeln lernen. Im Rahmen dieses Ansatzes bietet Eclipse-ausführliche Dokumentation und Tutorials auf alle seine generische Funktionen, so dass Plugin Projekte wie PHPEclipse, nur auf speziell für ihre Domäne ihre Bereiche zu konzentrieren. Indem wir lernen, Eclipse als Entwicklungsplattform verwenden oder zu lernen, Ihre eigenen Plug-in für Eclipse-Tools zu entwickeln, erwerben Sie eine sinnvolle und flexible Fähigkeiten.

Hilfe Befehl
----------------------

Diese Funktion dient, um die Verwendung von PHPEclipse Modul bestimmen. Der Benutzer wird kommen, um über die andere Art und Weise / Format um dieses Modul ausführen kennen. Dieser Befehl leitet den Anwender, um den Zweck dieses Befehls kennen. Da unten sind die Kommando- und der Screenshot der gleiche.

.. code-block:: bash
        
	        ptconfigure PHPeclipse help

Die bildliche Darstellung des obigen Befehls ist nachstehend gezeigt,

.. code-block:: bash

 kevell@corp:/# ptconfigure PHPEclipse help

 ******************************


  This command allows you to update PHPEclipse.

  phpeclipse, PHPEclipse, PHP-Eclipse

        - install
        Installs the latest version of PHPEclipse
        example: ptconfigure phpeclipse install

 ------------------------------
 End Help
 ******************************

Installation
----------------

Dieser Befehl hilft bei der Installation der neuesten Version von PHPEclipse im System. Die unten angegebenen Befehl wird den Prozess der Installation auszuführen.

.. code-block:: bash
        
	        ptconfigure PHPEclipse install

Options
-----------                               


.. cssclass:: table-bordered


 +-----------------------+-------------------------------------------------+-------------+-------------------------------------------+
 | Parameters            | Alternative Parameters                          | Optionen    |  Kommentare                               |
 +=======================+=================================================+=============+===========================================+
 |ptconfigure PHPEclipse | Es gibt drei alternative Parameter, die in der  | Y(Yes)      | System startet Installation               |
 |Install                | Befehlszeile verwendet werden können.           |             |                                           |
 |                       | PHP-Eclipse, PHPEclipse, phpeclipse             |             |                                           |
 |                       | Eg: ptconfigure PHPEclipse install ptconfigure  |             |                                           |
 |                       | PHP-Eclipse install                             |             |                                           |
 +-----------------------+-------------------------------------------------+-------------+-------------------------------------------+
 |ptconfigure PHPEclipse | Es gibt drei alternative Parameter, die in der  | N(No)       | Das System stoppt den                     |
 |Install                | Befehlszeile verwendet werden können.           |             | Installationsprozess                      |
 |                       | PHP-Eclipse, PHPEclipse, phpeclipse             |             |                                           |
 |                       | Eg: ptconfigure PHPEclipse install ptconfigure  |             |                                           |
 |                       | PHP-Eclipse install|                            |             |                                           |
 +-----------------------+-------------------------------------------------+-------------+-------------------------------------------+


Vorteile
--------------

* PHP, HTML, XML und CSS-Syntax-Hervorhebung
* Code-Vervollständigung
* Integrierter Web-Browser-Vorschau
* Integrierte Steuerung von Apache und MySQL-Server
