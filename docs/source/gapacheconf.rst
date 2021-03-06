============
ApacheConf
============


Zusammenfassung
-------------------------

Dieses Modul hilft bei der Verwaltung und die Apache-Konfiguration installieren. Es gibt die Konfiguration Ihrer Umgebung. Es ist gut situierten in Ubuntu und so gut wie in Cent OS.

Hilfe Befehl
---------------------

Der Befehl Help beschreibt den Zweck und die Befehle, die unter diese Module zur Verfügung. Es erklärt auch den Befehl, das bestimmte Modul zu installieren. Es listet, die alternative Parameter, die für die Deklaration verwendet werden können. Der Befehl werden deklariert Hilfe wird angezeigt, wie unten beschrieben:

.. code-block:: bash

	ptconfigure apacheconf help

In der Bildschirmabbildung so darzustellen, wie unten dargestellt, visuell die Verwendung des Hilfebefehls "unter dieses Modul.

.. code-block:: bash

 kevell@corp:/# ptconfigure apacheconf help
 ******************************


  This module lets you install a configuration for Apache HTTP Server. The only commands available are this help
  and install.

  ApacheConf, apache-configure, apache-configuration, apache-conf, apacheconf

        - install
        Installs a configuration for Apache
        example: ptconfigure apacheconf install

 ------------------------------
 End Help
 ******************************



	
Installation
----------------

Es ist einfacher zu diesem Tool unter ptconfigure zu installieren, indem Sie einfach den nachstehenden Befehl,
 
 
.. code-block:: bash
 
	  ptconfigure apacheconf install

After giving the command above, the tool will ask as

.. code-block:: bash

  Install Apache conf? (Y/N)

wenn Sie einen Eingang als Y geben , wird das Modul erfolgreich installiert.

Es wird auch werfen einige Befehle, um die Nicht- Standardwerte für LockFile , PidFile , Timeout , Keepalive , MaxKeepAliveRequest , Keepalivetimeout angeben. Wenn der Benutzer gibt Eingabe als omatically fix the default value. If the user gives input as N(No) then it will enquire about the values from the user.

Der Screenshot unten angegeben erklärt visuell über die Schritte und Befehle beinhaltet in der Installation.


.. code-block:: bash


 kevell@corp:/# ptconfigure ApacheConf install
 Install Apache Conf? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         Apache Conf!        *
 *******************************
 Set non-default value for LockFile? Default is ${APACHE_LOCK_DIR}/accept.lock (Y/N) 
 y
 What value for LockFile?
 ${APACHE_LOCK_DIR}/accept.lock
 Set non-default value for PidFile? Default is ${APACHE_PID_FILE} (Y/N) 
 y
 What value for PidFile?
 ${APACHE_PID_FILE}
 Set non-default value for Timeout? Default is 300 (Y/N) 
 y
 What value for Timeout?
 300
 Set non-default value for KeepAlive? Default is On (Y/N) 
 y
 What value for KeepAlive?
 On
 Set non-default value for MaxKeepAliveRequests? Default is 100 (Y/N) 
 y
 What value for MaxKeepAliveRequests?
 100
 Set non-default value for KeepAliveTimeout? Default is 5 (Y/N) 
 y
 What value for KeepAliveTimeout?
 5
 ... All done!
 *******************************
 Thanks for installing , visit www.pha  raohtools.com for more
 ******************************
 



Optionen
-----------------

.. cssclass:: table-bordered

 +----------------------------+---------------------------------------------+------------+-----------------------------------------+
 | Parameter                  | Alternative Parameter                       | Pflicht    | Kommentar                               |
 +============================+=============================================+============+=========================================+
 |Install Apache conf? (Y/N)  | anstelle von apachemodules, wir verwenden   | Yes        | Wenn der Benutzer gibt Eingabe als Ja,  |
 |                            | können, ApacheModules, apachemods,          |            | wird das Modul zu installieren.         |
 |                            | apache-modules auch noch                    |            |                                         |
 +----------------------------+---------------------------------------------+------------+-----------------------------------------+
 |Install Apache conf? (Y/N)  | anstelle von apachemodules, wir verwenden   | No         | Wenn der Benutzer gibt als Eingabe Nein |
 |                            | können, ApacheModules, apachemods,          |            | , es wird zu beenden.                   |
 |                            | apache-modules auch noch|                   |            |                                         |
 +----------------------------+---------------------------------------------+------------+-----------------------------------------+



Vorteile
----------------


* Das Modul hilft dem Benutzer bei der Installation und Verwaltung der Konfiguration des Apache.
* Während der Installation des Apache-Tools kann der Endbenutzer entwerfen und verwalten die Konfiguration wie pro ihre Anforderung, die mit 
  diesem Modul.
* Wenn es die Konfiguration bereits gründet gibt es überschreibt vorhandenen.
* Es ist gut situierten in Cent OS und auch wie bei Ubuntu.
* Die Parameter, die in der Deklaration verwendet ist nicht Groß-/Kleinschreibung, die einen zusätzlichen Vorteil.
 

