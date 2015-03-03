========
Port
========

Zusammenfassung
-------------------------

Hafen zertifizieren, um den Status der Ports und Dienstleistungen zu überprüfen. Dieses Modul hilft, die Hafendienste unter ptconfigure überprüfen. Dieses Modul ist am bequemsten mit Ubuntu und Cent-OS.

Hilfe
-------

Dieser Befehl help führen den Benutzer zu Port-Modul. Dies eignet sich für alle Arten von IT-Leute.
.. code-block:: bash

          ptconfigure port help

Der Befehl help zeigt eine kurze Liste der Befehle in das Port-Modul eingebaut.

.. code-block:: bash

	kevell@corp:/# ptconfigure Port  help
	******************************


	  This command allows you to test the status of ports and services running on them

	  Port, port

        - is-responding
        Test if a port is responding
        example: ptconfigure port is-responding --port-number="25"

        - process
        See which process is using a port
        example: ptconfigure port process --port-number="25"

	------------------------------
	End Help
	******************************

Lokaler Host
---------------

Wenn der Benutzer will den Status des Ports in lokalen Host überprüfen dann kann es dem Benutzer die IP-Adresse fragen. Der folgende Screenshot wird es erklären.

.. code-block:: bash


   	kevell@corp:/# ptconfigure port process --port-number="22"

	[Pharaoh Logging] Port 22 is being used by the process sshd
	******************************


	Port Modifications:
	--------------------------------------------

	Port: Success

	------------------------------
	Port Mods Finished
	******************************


Options
--------------- 

.. cssclass:: table-bordered

 +----------------------+--------------------------------------------+----------------------------------------------------+
 | Parameters           | fuctions                                   | Ausgangs                                           |
 +======================+============================================+====================================================+
 |is-responding         | Test-Port reagiert oder nicht              | Es wird den Prozess der Port reagieren             |
 +----------------------+--------------------------------------------+----------------------------------------------------+
 |Process               | Testen Sie den Prozessstatus von Port      | Es wird den Prozess der Port angezeigt|            |
 +----------------------+--------------------------------------------+----------------------------------------------------+
 

Vorteile
-------------

* Der Benutzer kann den aktuellen Betriebsstatus des Ports zu überprüfen.
* Es ist ein benutzerfreundliches Modul.
* Weniger zeitaufwendig.
