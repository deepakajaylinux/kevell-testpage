============
Sudonopass
============

Zusammenfassung
-----------------------

Sudonopass verwendet werden, um einen bestimmten Befehl mit root-Rechten ausgeführt werden. Das Interessante daran ist, dass, wenn der Benutzer sudo für einen bestimmten Befehl, fordert System den Benutzer für das Kennwort des aktuellen Benutzers. Sobald der Benutzer das Passwort eingeben, wird der Befehl mit Root-Rechten. Dies ist geeignet, um mit Ubuntu und Cent OS arbeiten.

Hilfe Befehl
-----------------------

Dieser Befehl help führen den Benutzer zu sudonopass Modul. Dies eignet sich für alle Arten von Business-Anwender. Der Befehl help zeigt eine kurze Liste der Befehle in das sudonopass Modul gebaut. Der folgende Screenshot aufzuzählen es.

.. code-block:: bash

	kevell@corp:/# ptconfigure SudoNoPass help
	******************************

	This command allows you to add an entry to the system sudo file that will
	 allow your user to have passwordless sudo. This is required for
	 quite a few of the  builds provided by Golden Contact, as
	 will perform test execution, software installs and more, silently.

	 SudoNoPass, sudonopass, sudo-nopass, sudo-passwordless

        - install
        Installs the sudo without password entry
        example: ptconfigure sudo-nopass install

	------------------------------
	End Help
	******************************

Installation
------------------

Dieses Modul ermöglicht sudonopass auf Ubuntu Linux-System-Pakete zu installieren

.. code-block:: bash

          ptconfigure sudonopass install

Install sudonopass ?(Y/N)

Wenn der Benutzer-Eingang, wie ja es wird automatisch installieren Sie die Wurzel Zugang für alle zu konfigurieren. Der folgende Screenshot wird es erklären.

.. code-block:: bash

	kevell@corp:/# ptconfigure sudo-nopass install
	Install Sudo w/o Pass for User? (Y/N) 
	y
	*******************************
	*        Pharaoh Tools        *
	*         Sudo NoPass!        *
	*******************************
	Enter User To Install As:
	Kevells
	The following will be written to /etc/sudoers
	Please check if it looks wrong
	You may not be able to use Sudo if it is incorrect!!!
	Kevells ALL=NOPASSWD: ALL
	Is this okay? (Y/N) 
	y
	... All done!
	*******************************
	Thanks for installing , visit www.pharaohtools.com for more
	******************************
	
	
	Single App Installer:
	--------------------------------------------
	SudoNoPass: Success
	------------------------------
	Installer Finished
	******************************
Option
------------

.. cssclass:: table-bordered

 +-----------------------+-----------+-------------------------------------------------------------------+ 
 | Parameters            | option    | Output                                                            |
 +=======================+===========+===================================================================+
 |Install sudonopass     | yes       | Es wird sudonopass unter ptconfigure installieren                 |
 +-----------------------+-----------+-------------------------------------------------------------------+
 |Install sudonopass     | No        | Sie wird zu beenden| 	                                         |
 +-----------------------+-----------+-------------------------------------------------------------------+



Vorteile
------------

* Sudonopass sorgt dafür, dass Root-Rechte sind für einen bestimmten Befehl (oder für eine bestimmte Zeit) und nicht für die gesamte Sitzung als
  dass eine zufällige Missbrauch von root-Rechten führen.

* Der Benutzer sudonopass selbst verwenden können eingeschränkten Rechten an einen Benutzer gewähren. Dies ist hilfreich, wenn der Benutzer 
  möchte nicht, dass ein Benutzer die Kontrolle über haben alle Wurzel Kräfte, während Sie eine sudonopass.

* Der beste Vorteil ist, dass sudonopass erfordert eigene Login-Passwort des Benutzers und nicht root-Passwort. Dies hilft bei der Führung root-  Passwort Private und es besteht keine Notwendigkeit, es zu ändern, selbst wenn ein Benutzer (sudoer) verlässt.

* Diese Datei enthält Informationen über die Befehle, die ausgeführt werden mit sudo und deren Zeitpunkt der Ausführung wurden. Dies hilft 
  Administratoren behalten Spur von selbst vertrauenswürdige Benutzer

