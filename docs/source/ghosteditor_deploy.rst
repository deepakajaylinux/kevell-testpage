======================
Host Editor
======================

Zusammenfassung
------------------

Dieses Modul unterstützt Apache Virtual Host Editor unter Ptdeploy zu behandeln. Es kann auf zwei Arten fungieren. Sie sind hinzufügen und entfernen. Vhost-Editor ist ein PHP-Tool geschrieben, Hinzufügen von virtuellen Hosts zu Apache ein Kinderspiel zu machen. Vhost-Editor ermöglicht es den Benutzer hinzufügen, bearbeiten oder Löschen von virtuellen Hosts auf des Benutzers Webserver. Es ist zweckmäßig, die Arbeit mit Ubuntu und Cent OS.  Mal sehen, wie der Apache Vhost-Editor unter Ptdeploy funktionieren kann.


Hilfe Befehl
-----------------------

Dieses Help-Befehl führt den Benutzer um eine Hosteditor zu erstellen. Der Help-Befehl für Hosteditor ist unten dargestellt.

.. code-block:: bash

	ptdeploy Hosteditor help

Nach Eingaben beginnt der obige Befehl, es funktionieren, um einen virtuellen Host-Editor hinzufügen. Es Katechese die Funktionen in den Screenshots.

.. code-block:: bash

 kevell@corp:/# ptdeploy HostEditor help 

 ****************************** 

  This command is part of Default Modules and handles Host File Management Functions. 

  HostEditor, hosteditor, he, hostEditor 

          - add 
          add a Host File entry 
          example: ptdeploy hosteditor add 
          example: ptdeploy hosteditor add --yes 
              --host-ip=127.0.0.1  # guess will assume 127.0.0.1 
              --host-name=dave.com 

          - rm 
          remove a Host File entry 
          example: ptdeploy hosteditor rm 
          example: ptdeploy hosteditor rm --yes 
              --host-ip=127.0.0.1 # guess will ignore this, and remove any entry matching the host name 
              --host-name=dave.com 

 ------------------------------ 
 End Help 
 ****************************** 



Alternative Parameter
-----------------------------------

Im folgenden sind die alternative Parameter, die in Deklarationen definiert werden können:

HostEditor, hosteditor, he, hostEditor 


Add
-------

Dies ermöglicht den Benutzer um einen Host Editor zu erstellen. Der Benutzer kann eingeben, die laut ihren Wunsch.


.. code-block:: bash

		sudo ptdeploy hosteditor add

Nach Eingang als dem obigen Befehl kann der Benutzer die folgenden Verfahren zu füllen.


.. code-block:: bash

 kevell@corp:/# ptdeploy hosteditor add 

 Do you want to add a hosts file entry? (Y/N) 
 y 
 Do you want a non-default IP? Enter for 127.0.0.1 
 127.0.0.1 
 What URI do you want to affect to the hostfile? 
 karuna 
 Please check host file: 127.0.0.1	localhost 
 127.0.1.1	karuna 
 127.0.1.1       www.kevell.com 
 
 127.0.1.1	www.ptbuild.tld 
 # The following lines are desirable for IPv6 capable hosts 
 ::1     ip6-localhost ip6-loopback 
 fe00::0 ip6-localnet 
 ff00::0 ip6-mcastprefix 
 ff02::1 ip6-allnodes 
 ff02::2 ip6-allrouters 
              --host-ip=127.0.0.1  # guess will assume 127.0.0.1              --host-name=dave.com127.0.0.1          dave.com 
 127.0.0.1          dave.com 
 192.168.1.4          
 127.0.0.1          deepak 
 clear          
 127.0.0.1          www.kevell.com 
 127.0.0.1          
 127.0.0.1          karuna 


 Is this Okay?  (Y/N) 
 y 
 ****************************** 

 1Host Editor Finished 
 ****************************** 

.. code-block::  bash

 kevell@corp:/# ptdeploy hosteditor add --yes 

 Do you want a non-default IP? Enter for 127.0.0.1 
 127.0.0.1 
 What URI do you want to affect to the hostfile? 
 kumar 
 ****************************** 

 1Host Editor Finished 
 ****************************** 




entfernen
--------------

Der terminal-Befehl zum Löschen von Hosteditor ist Rm. Das allgemeine Format dieses Befehls ist Rm. RM entfernt einen Host, wenn Sie für es und wenn nicht dann zeigt eine Fehlermeldung an und gehen Sie zum nächsten Wirt, einen richtigen Pfad angeben.


Den folgenden Befehl zum Löschen des virtuellen Hosts verwendet.

.. code-block:: bash
   
		sudo ptdeploy hosteditor rm

Der folgende Screenshot kann seine Funktionen erklären.

.. code-block:: bash

 kevell@corp:/# ptdeploy hosteditor rm 

 Do you want to remove a hosts file entry? (Y/N) 
 y 
 Do you want a non-default IP? Enter for 127.0.0.1 
 127.0.0.1 
 What URI do you want to affect to the hostfile? 
 karuna 
 Please check host file: 127.0.0.1	localhost 
 127.0.1.1	karuna 
 127.0.1.1       www.kevell.com 

 127.0.1.1	www.ptbuild.tld 
 # The following lines are desirable for IPv6 capable hosts 
 ::1     ip6-localhost ip6-loopback 
 fe00::0 ip6-localnet 
 ff00::0 ip6-mcastprefix 
 ff02::1 ip6-allnodes 
 ff02::2 ip6-allrouters 
              --host-ip=127.0.0.1  # guess will assume 127.0.0.1              --host-name=dave.com127.0.0.1          dave.com 
 127.0.0.1          dave.com 
 192.168.1.4          
 127.0.0.1          deepak 
 clear          
 127.0.0.1          www.kevell.com 
 127.0.0.1          
 127.0.0.1          nithin 
 127.0.0.1          kumar 
 


 Is this Okay?  (Y/N) 
 y 
 ****************************** 

 1Host Editor Finished 
 ****************************** 

.. code-block:: bash


 kevell@corp:/# ptdeploy hosteditor rm --yes 

 Do you want a non-default IP? Enter for 127.0.0.1 
 127.0.0.1 
 What URI do you want to affect to the hostfile? 
 nithin 
 ****************************** 
 
 1Host Editor Finished 
 ****************************** 


Vorteile
---------------

* Multi-User kann gleichzeitig zugreifen. 
* Der Benutzer hinzufügen oder entfernen Sie Host. 
* Nicht groß-und Kleinschreibung.

