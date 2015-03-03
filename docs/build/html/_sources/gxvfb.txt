======
Xvfb
======

Zusammenfassung
-------------------------

Mit diesem Modul können in der Installation des xvfb, die als beliebte Virtual-Machine, bekannt ist. Das Modul stellt eine Lösung für die Arbeit in einer virtuellen Maschine. xvfb als X virtuellen Framebuffer genannt, ist eine Display-Server Implementierung des X11 Display-Server-Protokoll. Im Gegensatz zu anderen Display-Server führt Xvfb alle grafischen Operationen im Speicher ohne einen Bildschirmausgabe. Wir wollen sehen, wie dieses Modul hilft bei der Installation des xvfb über apt-get.

Hilfe Befehl
--------------------

Der Befehl help führt den Anwender über den Zweck und als auch über die Möglichkeiten, die in der xvfb Modul enthalten sind. Der Befehl help Listen aus der alternativen Parameter xvfb Modul. Es beschreibt auch die Syntax für die Installation xvfb Modul Der Befehl help für xvfb Modul wird wie unten dargestellt.

.. code-block:: bash

		ptconfigure Xvfb help

Die Syntax für die Deklaration den Befehl help ist nicht case sensitive was ein zusätzlicher Vorteil ist. Der folgende Screenshot visualisieren Sie den Befehl help unter xvfb Modul.

.. code-block:: bash

 kevell@corp:/# ptconfigure Xvfb help
 ******************************


  This command allows you to install Xvfb, the popular Virtual Machine Solution.

  Xvfb, xvfb

        - install
        Installs Xvfb through apt-get
        example: ptconfigure xvfb install

 ------------------------------
 End Help
 ******************************

Installation
----------------

Der Befehl zum Installieren der xvfb zum Benutzer Maschine verwendet wird unten gezeigt.

.. code-block:: bash

		ptconfigure xvfb install

Nach der Eingabe des Befehls vor, tritt die folgenden Vorgänge wie im Tabellenformat angezeigt.

.. cssclass:: table-bordered

 +------------------------+----------------------------------------+--------------+---------------------------------------------------+
 | Parameters             | Alternative Parameter                  | Option       | Kommentare                                        |
 +========================+========================================+==============+===================================================+
 |Install Xvfb? (Y/N)     | Statt Xvfb kann xvfb kann ebenfalls    | Y(Yes)       | Wenn der Benutzer wünschen, den                   |
 |                        | verwendet werden                       |              | Installationsprozess können sie Eingang als       |
 |                        |                                        |              | Y. gehen                                          |
 +------------------------+----------------------------------------+--------------+---------------------------------------------------+
 |Install Xvfb? (Y/N)     | Statt Xvfb kann xvfb kann ebenfalls    | N(No)        | Wenn der Benutzer wünschen, den                   |
 |                        | verwendet werden                       |              | Installationsprozess können sie Eingang als       |
 |                        |                                        |              | N. beenden|                                       |
 +------------------------+----------------------------------------+--------------+---------------------------------------------------+


Wenn der Benutzer den Installationsprozess fort, während der Ausführung der Installation wird der folgende Prozess durchgeführt:

* Liest Paketlisten.
* Baut Abhängigkeitsbaum.
* Liest Statusinformationen.
* Liste der neuen Pakete installiert.
* Anzahl der Dateien aktualisiert, neu installiert, entfernt wird, nicht aktualisiert.

Schließlich wird der Status eindeutig ausgewiesen und das Hinzufügen von Paket xvfb vom Verpacker Apt korrekt ausgeführt werden. Der folgende Screenshot zeigt Sie den Prozess der Installation xvfb.

Wenn die xvfb Modul ist bereits in der Maschine vorhandenen Benutzer, wird eine Meldung wie die Paket xvfb vom Verpacker Apt bereits installiert ist zu zeigen. Der Screenshot wie folgt ist ein gutes Beispiel für jene Art von Nachrichten.

.. code-block:: bash

 kevell@corp:/# ptconfigure xvfb install
 Install Xvfb? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *          ! Xvfb !        *
 *******************************
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following NEW packages will be installed:
  xvfb
 0 upgraded, 1 newly installed, 0 to remove and 8 not upgraded.
 Need to get 747 kB of archives.
 After this operation, 2,191 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main xvfb amd64 2:1.15.1-0ubuntu2.6 [747 kB]
 Fetched 747 kB in 36s (20.6 kB/s)
 Selecting previously unselected package xvfb.
 (Reading database ... 211203 files and directories currently installed.)
 Preparing to unpack .../xvfb_2%3a1.15.1-0ubuntu2.6_amd64.deb ...
 Unpacking xvfb (2:1.15.1-0ubuntu2.6) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Setting up xvfb (2:1.15.1-0ubuntu2.6) ...
 [Pharaoh Logging] Adding Package xvfb from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 Xvfb: Success
 ------------------------------
 Installer Finished
 ******************************

Vorteile
-----------

* Die Hilfe Befehl deklarieren verwendeten Parameter werden Installation nicht beachtet, welche ein zusätzlicher Vorteil ist, während im 
  Vergleich zu anderen.
* Es ist gut-to-do in beiden Cent OS und als auch in Ubuntu.
* Wenn der xvfb Paket bereits in der Benutzermaschine vorhandenen, wird es nicht überschreibt, statt dass es eine Nachricht zu zeigen, wie 
  bereits existieren.

Xvfb wird hauptsächlich zum Testen verwendet:

* Da es teilt Code mit der realen X-Server, kann es verwendet werden, um die Teile des Codes, die nicht auf die Hardware-Treibern sind zu 
  testen.
* Es kann benutzt werden, um Kunden in verschiedenen Bedingungen wie sonst eine Reihe verschiedener Hardware zu testen; zum Beispiel kann es 
  sein verwendet werden, um zu testen, ob Kunden richtig in Tiefen oder Bildschirmgrößen, die nur selten von der Hardware unterstützt werden.
* Hintergrundlauf der Kunden. (Die xwd Programm oder ein ähnliches Programm für einen Screenshot erfassen kann verwendet werden, um 
  tatsächlich sehen das Ergebnis)
* Laufprogramme, die einen X-Server erfordern, aktiv zu sein, auch wenn sie sie nicht benutzen. (Z Clover HTML-Berichte)


