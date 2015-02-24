========
Mkdir
========

Zusammenfassung
-------------------------

Dieses Modul hilft bei der Erstellung eines Verzeichnisses. Der Nutzer kann den Pfad bei der Erklärung Schaffung Verzeichnis oder zur Laufzeit von ein Verzeichnis. Sie kann entweder in entfernten oder lokalen Maschine durchgeführt werden. Lassen Sie uns darüber, wie dieses Modul hilft bei der Erstellung eines Verzeichnisses zu sehen.

Hilfe Befehl
---------------------

Der Befehl help führt die Benutzer über den Zweck und als auch über die Möglichkeiten, die in der Mk Dir gehören. Der Befehl help listet einige der alternativen Parameter des MK Dir. . Es beschreibt auch die Syntax für das Erstellen eines Verzeichnisses auf zwei verschiedenen Wegen, entweder zum Zeitpunkt der Anmeldung oder während der Laufzeit. . Der Befehl help für MK dir ist nachfolgend dargestellt.

.. code-block:: bash

	ptconfigure  mkdir help

Die Syntax für die Deklaration den Befehl help ist nicht case sensitive was ein zusätzlicher Vorteil ist. Der folgende Screenshot visualisieren Sie den Befehl help unter MK Richt.

.. code-block:: bash

	kevell@corp:/# ptconfigure  Mkdir help
	******************************


        This command handles file copying functions.

         Mkdir, mkdir

        - path
        Will ask you for details for servers, then copy a file or directory from local to remote
        example: ptconfigure  mkdir path
        example: ptconfigure  mkdir path --yes --path="/path/to/new/directory"

	------------------------------
	End Help
	******************************

Alternative Parameter
-------------------------

Bei der Verwendung von Befehlen zur Unterstützung und das Erstellen eines Verzeichnisses anstatt Mkdir Mkdir können ebenfalls verwendet werden.

Erstellen einer Mk Dir
-------------------------

Erstellen einer Mk Dir kann auf zwei verschiedene Arten erfolgen:

.. rubric:: Either at run-time

.. code-block:: bash

	Example: ptconfigure  mkdir path

.. rubric:: Or, at the time of declaration

.. code-block:: bash

	Example: ptconfigure  mkdir path --yes --path="/path/to/new/directory"

Der folgende Screenshot zeigt die zweite Möglichkeit der Erstellung eines Verzeichnisses.

.. code-block:: bash

	kevell@corp:/# ptconfigure  mkdir path --yes --path="/kevellsdoc"
	
	[Pharaoh Logging] [Mkdir] Executing mkdir /kevellsdoc
	******************************


	Mkdir Result: Success
	------------------------------
	Mkdir Finished
	******************************


Vorteile
------------
* Die in Hilfe und ein Verzeichnis-Operationen sind nicht case sensitive was ein zusätzlicher Vorteil ist, während im Vergleich zu anderen 
  verwendeten Parameter.
* Erstellen eines Verzeichnisses kann auf zwei verschiedene Arten, wie der Deklaration oder zur Laufzeit festgelegt werden.
* Es kann sowohl in lokalen oder Remote-Maschine durchgeführt werden.
* Es ist gut-to-do sowohl Ubuntu und sowie Cent OS.

