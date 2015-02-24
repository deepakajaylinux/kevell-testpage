=================
PackageManager
=================

Zusammenfassung
-----------------------

Dieser Befehl verwendet, um die Paketverwaltung zu wickeln. Es wird mit drei Optionen. Sie sind pkg-install, pkg-sicherzustellen, pkg-Entfernen. Dies ermöglicht es dem Benutzer, in einem beliebigen System installiert werden. Es verwaltet die Paket-Manager-Funktionen. Es eignet sich mit Ubuntu und CentOS arbeiten.

Hilfe Befehl
-----------------------

Dieser Befehl help führt den Benutzer zu installieren, stellen Sie sicher, nehmen Sie das Paketmanagement. Dies ermöglicht der Installation sicher, zu entfernen. Der Befehl help für Paket-Manager ist unten dargestellt

.. code-block:: bash

		ptconfigure packagemanager help

Nach Eingang der obige Befehl, beginnt es funktioniert, um zu wickeln. Es Katechese die Funktionen in den Screenshots.

.. code-block:: bash

 kevell@corp:/# ptconfigure packagemanager help
 ******************************


  This command allows you to use a Package Management wrapper.

  PackageManager, package-manager, packagemanager, package-mgr, pkgmgr

        - pkg-install
        Installs a Package through a Package Manager
        example: ptconfigure package-manager install --package-name="mysql" --package-version="5.0" --packager="apt-get"

        - pkg-ensure
        Installs a Package through a Package Manager
        example: ptconfigure package-manager install --package-name="mysql" --package-version="5.0" --packager="apt-get"

        - pkg-remove
        Removes a Package through a Package Manager
        example: ptconfigure package-manager install --package-name="mysql" --package-version="5.0" --packager="apt-get"

  A package manager wrapper that will allow you to install packages on any system

 ------------------------------
 End Help
 ******************************


Alternative Parameter
--------------------------------

Im Folgenden sind die Parameter, die in alternative Erklärungen definiert werden können:

PackageManager, package-manager, packagemanager, pkgmgr, package-mgr.


Pkg-install
---------------

Die Installation umfasst die Installation von Package erforderlich, um die Installation in einer aktualisierten Version zu machen. Es ist eine offensichtliche Prozess Package Modul unter ptconfigure installieren. Packagemanager von nur mit dem Befehl unten angegeben,

.. Code-block:: bash

	ptconfigure PackageManager Install

Nach beleben den Befehl geben Sie den Wert katechisieren.

Wenn die Benutzereingaben wie ja automatisch wird Packagemanager mit der Überprüfung aus dem System zu installieren. Wenn nicht beenden Sie die Installation. Der folgende Screenshot zeigen Packagemanager und seine Funktionen.

.. code-block:: bash

Pkg-sicher
-----------------

Pkg gewährleisten eine Systemdienst ausgeführt wird. Im Falle einer nicht läuft starten Sie es sonst nicht zu versuchen. Durch diesen Befehl kann der Anwender feststellen, ob das System funktioniert oder im Leerlauf. Einfache Befehle sind leicht zu handhaben. Der folgende Befehl verwendet durch Paketmanager zu gewährleisten.

.. code-block:: bash
    
	ptconfigure PackageManager ensure

Pkg-remove
-----------------

Pkg entfernen Befehl verwendet werden, um ein Paket von Paketmanager zu entfernen. Der Paket-Manager überprüft zuerst das Paket wollen von Paketmanager zu entfernen. Dann ist es die Bestätigung verlangen. Dann verwenden Sie die Option Entfernen.
.. code-block:: bash

 		ptconfigure PackageManager remove

Vorteile
-------------

* Nicht Groß- und Kleinschreibung.
* Well-to-do in Ubuntu und CentOS.
* Entfernen Sie die Verpackung ist möglich
* Wickeln Sie den Paket-Manager
* Befehle sind einfach zu bedienen

