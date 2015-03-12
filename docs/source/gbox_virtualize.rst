=======
Box
=======

Zusammenfassung
------------------

Dieses Modul unterstützt die Anwender bei der Handhabung und Verwaltung der Felder, die in der ptvirtualize sind. Wir wollen sehen, wie dieses Modul arbeitet im Umgang mit den Funktionen der Box.

Hilfe Befehl
---------------------

Der Befehl help führt den Anwender über den Zweck und als auch über die Möglichkeiten, die in der Box-Modul enthalten sind. Es listet einige der alternativen Parameter der Box-Modul. Es beschreibt auch die Syntax für die Hinzufügen, Entfernen, Paket, Listenbefehle. Der Befehl help für Box-Modul wird wie unten dargestellt.

.. code-block:: bash
		
	ptvirtualize Box help

Die Syntax für die Deklaration den Befehl help ist nicht case sensitive was ein zusätzlicher Vorteil ist. Der folgende Screenshot visualisieren Sie den Befehl help unter Box.

.. code-block:: bash

 kevell@corp:/# ptvirtualize Box help

 ******************************
 Pharaoh Tools - Virtualize
 ******************************


  This command allows you to manage the Base boxes available to you in ptvirtualize

  Box, box

        - add
        Initialises the Box as usable by ptvirtualize
        example: ptvirtualize box add
        example: ptvirtualize box add --yes --guess
            --source="/home/dave/file.box" # where the box file is
            --target="opt/ptvirtualize/boxes" # will guess the dir next to ptvirtualize install dir
            --name="vanillaubuntu"

        - remove
        Removes the box as usable by ptvirtualize
        example: ptvirtualize box remove

        - package
        Packages a box as usable by ptvirtualize
        example: ptvirtualize box package
        example ptvirtualize box package --yes --guess
            --name="Vanilla Ubuntu 12.04 amd 64"
            --vmname="a4dc638f-2721-40c4-a943-2f2565c83fee" # use name or id of virtual machine
            --provider="virtualbox" # guess will use virtualbox
            --group="ptvirtualize"
            --slug="" # guess can generate this based on name field
            --description="A Vanilla install of Ubuntu..."
            --home_location="http://www.someplace.net/" # guess will set this to http://www.ptvirtualizeboxes.co.uk/
            --target="/opt/ptvirtualize/boxes" # save location, will guess /opt/ptvirtualize/boxes

        - list
        List boxes installed in ptvirtualize
        example: ptvirtualize box list

 ------------------------------
 End Help
 ******************************

Funktionen ptvirtualize Box
----------------------------------

Wie im obigen Befehl help dargestellt werden die Funktionen des ptvirtualize Box beinhaltet folgende Leistungen:

* Add
* Remove
* Package
* List

hinzufügen
--------------

Das Add wird zur Initialisierung der Box als nutzbar ptvirtualize verwendet. Die folgende Syntax kann für das Hinzufügen einer ptvirtualize Box verwendet werden.

.. code-block:: bash

	ptvirtualize box add

or

.. code-block:: bash

	ptvirtualize box add --yes --guess
	--source="/home/dave/file.box	(This line describes where the box is)
	--target="opt/ptvirtualize/boxes"	(This line guess the dir next to ptvirtualize install dir)
	--name="vanillaubuntu"

In der oben genannten Weise kann die Box an einen ptvirtualize hinzugefügt.

entfernen
-----------

Diese Funktion wird zum Entfernen der Box als nutzbar ptvirtualize verwendet. Dies kann mit dem Befehl unten durchgeführt werden:

.. code-block:: bash

	ptvirtualize box remove

In der oben genannten Weise kann die Box aus einem ptvirtualize entfernt werden.

Paket
-----------

Diese Funktion wird verwendet, um zu verpacken die Box als nutzbar ptvirtualize. Dies kann mit dem folgenden Befehl durchgeführt werden:

.. code-block:: bash

	ptvirtualize box package

or

.. code-block:: bash

	ptvirtualize box package --yes --guess
	name="Vanilla Ubuntu 12.04 amd 64"
	vmname="a4.............." (This two lines represents the name and id of virtual machine)
	--provider="virtualbox" (guess will use virtual box)
	--group="ptvirtualize"
	--slug="" (The guess can generate this based on the name field)
	--description="A vanilla install of Ubuntu..."
	--home_location="http://www.someplace.net/" (guess will set this to http://www.ptvirtualizeboxes.co.uk/
	--target="/opt/ptvirtualize/boxes" (The location for saving)



Schließlich ist ein Feld, wie durch die ptvirtualize verwendbaren verpackt.

Liste
-----

Diese Funktion wird zum Auflisten der Felder, die in ptvirtualize installiert werden verwendet. Dies kann mit dem folgenden Befehl durchgeführt werden,

.. code-block:: bash

	ptvirtualize box list

Mit dem Befehl oben, wird die Liste der ptvirtualize Boxen, die neu installiert werden angezeigt.


Alternative Parameter
-----------------------

* Box
* box


Bei der oben genannten Liste, kann jede der alternativen Parameter Erklärung verwendet werden.


Vorteile
-----------

* Die in der Hilfe verwendet wird die Groß- was ein zusätzlicher Vorteil ist, während im Vergleich zu anderen Parametern.
* Es ist gut-to-do sowohl Ubuntu und sowie Cent OS.
* Die Syntax für die Verwendung hinzufügen, entfernen Paket-Liste muss nicht beachtet werden.

