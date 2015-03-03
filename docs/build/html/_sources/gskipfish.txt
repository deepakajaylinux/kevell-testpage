=============
Skipfish
=============

Zusammenfassung
-------------------------

Skipfish-Modul verwendet werden, um Skipfish installieren. Skipfish ist ein aktiver Sicherheit von Webanwendungen Aufklärungswerkzeug. Er bereitet eine interaktive Sitemap zur gezielten Ort durch eine rekursive kriechen und Wörterbuch-Sonden. Die resultierende Karte wird dann mit dem Ausgangssignal aus einer Anzahl von aktiven Sicherheitsüberprüfungen versehen. Der Abschlussbericht mit dem Werkzeug erzeugt wird bedeutet, um als Grundlage für professionelle Web Application Security Assessments dienen. Dieses Modul stärken mit Ubuntu und Cent-OS.

Hilfe Befehl
----------------------

Der Befehl help führt den Anwender über den Zweck und als auch über die Möglichkeiten, die in der Skipfish-Modul enthalten sind. Es listet einige der alternativen Parameter Skipfish-Modul. Es beschreibt auch die Syntax für die Installation des Moduls Skipfish. Der Befehl help für Skipfish Modul wird wie unten dargestellt.

.. code-block:: bash	

		ptconfigure Skipfish help

Die Syntax für die Deklaration den Befehl help ist nicht case sensitive was ein zusätzlicher Vorteil ist. Der folgende Screenshot visualisieren Sie den Befehl help unter Skipfish.

.. code-block:: bash

 kevell@corp:/# ptconfigure Skipfish help

 ******************************


  This command allows you to install Skipfish.
  Skipfish, skipfish

        - install
        Installs Skipfish. 
        example: ptconfigure skipfish install

 ------------------------------
 End Help
 ******************************



Installation
-----------------

Dieser Befehl ermächtigen, Skipfish mit interaktiven Website Karte installieren. Wenn der Benutzer Skipfish dem folgenden Befehl installiert werden soll führt den Benutzer zu installieren.

.. code-block:: bash

                ptconfigure skipfish install

nachdem Sie diesen Befehl fragt das System Benutzer wünschen. Das andere Verfahren wird die Installation durch den Screenshot.

.. code-block:: bash


 kevell@corp:/# ptconfigure Skipfish install
 Install  Skipfish? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *          Skipfish !        *
 *******************************
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following NEW packages will be installed:
  skipfish
 0 upgraded, 1 newly installed, 0 to remove and 15 not upgraded.
 Need to get 233 kB of archives.
 After this operation, 574 kB of additional disk space will be used.
 Get:1 http://us.archive.ubuntu.com/ubuntu/ trusty/universe skipfish amd64 2.10b-1 [233 kB]
 Fetched 233 kB in 29s (7,910 B/s)
 Selecting previously unselected package skipfish.
 (Reading database ... 199429 files and directories currently installed.)
 Preparing to unpack .../skipfish_2.10b-1_amd64.deb ...
 Unpacking skipfish (2.10b-1) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Setting up skipfish (2.10b-1) ...
 [Pharaoh Logging] Adding Package skipfish from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 Skipfish: Success
 ------------------------------
 Installer Finished

 ******************************



Option
-----------

.. cssclass:: table-bordered

 +--------------------+--------------------------------------+--------------+--------------------------------------------------+
 | Parameters         | Alternative Parameters               | Optionen     | Kommentare                                       |
 +====================+======================================+==============+==================================================+
 |Install Skipfish?   | anstelle von Skipfish wir verwenden  | Y(Yes)       | Wenn der Benutzer wünschen, den                  |
 |(Y/N)               | können, skipfish                     |              | Installationsprozess können sie Eingang          |
 |                    |                                      |              | als Y. gehen                                     |
 +--------------------+--------------------------------------+--------------+--------------------------------------------------+
 |Install Skipfish?   | anstelle von Skipfish wir verwenden  | N(No)        | Wenn der Benutzer wünschen, den                  |
 |(Y/N)               | können, skipfish                     |              | Installationsprozess können sie Eingang          |
 |                    |                                      |              | als N. beenden|                                  |
 +--------------------+--------------------------------------+--------------+--------------------------------------------------+


Vorteile
--------------

* Skipfish ist sehr anpassungsfähig und zuverlässig.
* Gut gestaltete Sicherheitskontrollen.
* Graceful Umgang mit Multi-Rahmen-Sites
* Automatische aktualisierte Version der Installation
* High-Speed zu erreichen.
* Nicht Groß- und Kleinschreibung.
* Auch in Ubuntu und Cent OS zu tun.

