==========
Service
==========

Zusammenfassung
--------------------------
          
Dieses Modul ermöglicht die aktuellen Status-Datei in das System. Es kann den Status als Laufen oder nicht erwähnt. Automation möglich. In diesem Modul legen Sie die Konfiguration Ihrer Umgebung. Es ist benutzerfreundlich mit Ubuntu und Cent-OS.

Hilfe Befehl
-------------

Hilfe Befehl verwendet werden, um Informationen zu einem bestimmten Befehl zu finden. Weitere Informationen zu den Funktionsänderungen des Service können wir diese Hilfe Befehl verwenden. Der folgende Screenshot wird dich führen.

.. code-block:: bash

    ptconfigure Service help


.. code-block:: bash

	Kevell@corp:/# ptconfigure Service help

	******************************


	  This command allows you to view or modify service

	  Service, service

        - start
        Start a system service
        example: ptconfigure service start --service-name="apache2"

        - stop
        Stop a system service
        example: ptconfigure service restart --service-name="apache2"

        - restart
        Restart a system service
        example: ptconfigure service restart --service-name="apache2"

        - ensure-running
        Ensure a system service is running. If it is already running, dont attempt to start it
        If it is not running, start it
        example: ptconfigure service ensure-running --service-name="apache2"

        - is-running
        Checks whether a system service is running.
        example: ptconfigure service is-running --service-name="apache2"

        - run-at-reboots
        Ensure a system service will auto start on reboots.
        example: ptconfigure service run-at-reboots --service-name="apache2"

	------------------------------
	End Help
	******************************


Options
------------

.. cssclass:: table-bordered

 +----------------+--------------------------------------------------+-------------------------------------------------------------------+
 | Parameters     | Funktionen                                       | Kommentar                                                         |
 +================+==================================================+===================================================================+
 |start           | Starten Sie einen Systemdienst                   | ptconfigure service start –service-name=”apache2”                 |
 +----------------+--------------------------------------------------+-------------------------------------------------------------------+
 |stop            | Stoppen asystem Service                          | ptconfigure service stop –service-name=”apache2”                  |
 +----------------+--------------------------------------------------+-------------------------------------------------------------------+
 |Restart         | Starten Sie einen Systemdienst                   | ptconfigure service restart –service-name=”apache2”               |
 +----------------+--------------------------------------------------+-------------------------------------------------------------------+
 |Ensure-running  | Sorgen Sie für einen Systemdienst running.In Bei | ptconfigure service ensure-running –service- name=”apache2”       |
 |                | nicht läuft starten Sie es sonst nicht zu        |                                                                   |
 |                | versuchen                                        |                                                                   |
 +----------------+--------------------------------------------------+-------------------------------------------------------------------+
 |Is-running      | Prüfen Sie, ob ein Systemdienst läuft oder nicht | ptconfigure service is-running –service-name=”apache2”            |
 |                | läuft starten Sie es sonst nicht zu versuchen    |                                                                   |
 +----------------+--------------------------------------------------+-------------------------------------------------------------------+
 |Run-at-reboots  | Stellen Sie sicher, einen Systemdienst Autostart | ptconfigure service run-at-reboots –service- name=”apache2        |     
 |                | beim Neustart|                                   |                                                                   |
 +----------------+--------------------------------------------------+-------------------------------------------------------------------+


Die bildliche represenation der Befehl start , stop, restart , Ensure-running, Is-running and Run-at-reboots sind unten aufgeführt ,


.. code-block:: bash

 kevell@corp:/# ptconfigure service start --service-name="apache2"

 [Pharaoh Logging] Starting apache2 service
 * Starting web server apache2
 * 
 ******************************


 Service Modifications:
 --------------------------------------------

 Service: Success

 ------------------------------
 Service Mods Finished
 ******************************

.. code-block:: bash

 kevell@corp:/# ptconfigure service stop --service-name="apache2"

 [Pharaoh Logging] Stopping apache2 service
 * Stopping web server apache2
 * 
 ******************************


 Service Modifications:
 --------------------------------------------

 Service: Success

 ------------------------------
 Service Mods Finished
 ******************************


.. code-block:: bash

 kevell@corp:/# ptconfigure service restart --service-name="apache2"

 [Pharaoh Logging] Restarting apache2 service
 AH00558: apache2: Could not reliably determine the server's fully qualified domain name, using 127.0.1.1. Set the 'ServerName' directive globally to suppress this message
 * Restarting web server apache2
   ...done.
 ******************************


 Service Modifications:
 --------------------------------------------

 Service: Success

 ------------------------------
 Service Mods Finished
 ******************************


.. code-block:: bash


 kevell@corp:/# ptconfigure service ensure-running --service-name="apache2"

 [Pharaoh Logging] Service apache2 is running...
 ******************************


 Service Modifications:
 --------------------------------------------

 Service: Success

 ------------------------------
 Service Mods Finished
 ******************************

.. code-block:: bash


 kevell@corp:/# ptconfigure service is-running --service-name="apache2"

 [Pharaoh Logging] Service apache2 is running...
 ******************************


 Service Modifications:
 --------------------------------------------

 Service: Success

 ------------------------------
 Service Mods Finished
 ******************************

.. code-block:: bash


 kevell@corp:/# ptconfigure service run-at-reboots --service-name="apache2"

 [Pharaoh Logging] Removing current apache2 service startup links
 Removing any system startup links for /etc/init.d/apache2 ...
   /etc/rc0.d/K09apache2
   /etc/rc1.d/K09apache2
   /etc/rc2.d/S91apache2
   /etc/rc3.d/S91apache2
   /etc/rc4.d/S91apache2
   /etc/rc5.d/S91apache2
   /etc/rc6.d/K09apache2
 [Pharaoh Logging] Adding apache2 service startup links
 Adding system startup for /etc/init.d/apache2 ...
   /etc/rc0.d/K20apache2 -> ../init.d/apache2
   /etc/rc1.d/K20apache2 -> ../init.d/apache2
   /etc/rc6.d/K20apache2 -> ../init.d/apache2
   /etc/rc2.d/S20apache2 -> ../init.d/apache2
   /etc/rc3.d/S20apache2 -> ../init.d/apache2
   /etc/rc4.d/S20apache2 -> ../init.d/apache2
   /etc/rc5.d/S20apache2 -> ../init.d/apache2
 ******************************


 Service Modifications:
 --------------------------------------------

 Service: Success

 ------------------------------
 Service Mods Finished
 ******************************



Vorteile
---------

* Der Benutzer kann das System Arbeitsstatus jederzeit überprüfen.
* Service bietet, um Daten zwischen dem System auszutauschen.
* Sie ermöglicht die gemeinsame Nutzung der Ressourcen der Maschine
* Service bietet auch die Funktion von Back-up.
* Service bietet eine flexible Netzwerkumgebung.
* Dies beinhaltet Koordination verteilter Daten.

