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



Vorteile
---------

* Der Benutzer kann das System Arbeitsstatus jederzeit überprüfen.
* Service bietet, um Daten zwischen dem System auszutauschen.
* Sie ermöglicht die gemeinsame Nutzung der Ressourcen der Maschine
* Service bietet auch die Funktion von Back-up.
* Service bietet eine flexible Netzwerkumgebung.
* Dies beinhaltet Koordination verteilter Daten.

