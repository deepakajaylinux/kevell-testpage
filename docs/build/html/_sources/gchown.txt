=======
Chown
=======

Übersicht
----------

Dieses Modul ermöglicht es, die um Erlaubnis des Besitzers zu ändern. Sie können die Berechtigung für einzelne Datei ändern oder Verzeichnis. Davor müssen Sie beachten die Standardberechtigung auf Dateien und Verzeichnisse zum Zeitpunkt ihrer Erstellung zugeordnet. 

Help-Befehl
--------------

Dieser Befehl Help erklärt die Installation eines bestimmten Moduls. Der Befehl Help ist einfach zu bedienen durch den Endbenutzer. Es listet auch out-die alternative Parameter, die in der Deklaration verwendet werden. Der folgende Befehl führt den Benutzer über den Umgang dieses Modul.

.. code-block:: bash
	
	cleopatra chown help

Nachdem er den Befehl gab, listet der Befehl die Hilfeoptionen. Die folgenden Screenshots geben visuellen Effekt für die Nutzung dieses Moduls.


.. code-block:: bash

	Kevell@corp:/# cleopatra chown help
	******************************

	 This command handles file user ownership changing functions.

	  Chown, chown

        - path
        Will change the user ownership of a path
        example: cleopatra chown path --yes --guess --recursive --path=/a/file/path --owner=golden

	------------------------------
	End Help
	******************************


Weg
------

Es ist ein ausgezeichneter Prozess für dieses Modul unter Cleopatra leicht mit dem Befehl unten gegeben,

.. code-block:: bash

	cleopatra chown path –yes—guess—recursive—path=/Cleopatra—owner=Kevells


Dann können wir die Eingabe eingeben.
Geben Sie Besitz Benutzer
Nach der Eingabe des Namens des Besitzers
Chown Ergebnis Erfolg wird angezeigt.


Dies ist optisch von der folgenden Bildschirmabbildung dargestellt.

.. code-block:: bash

	kevell@corp:/# cleopatra chown path --yes --guess --recursive --path=/phj.php --owner=deepak

	Enter ownership user:
	deepak
	[Pharaoh Logging] [Chown] Executing chown -R deepak /phj.php
	******************************


	Chown Result: Success
	------------------------------
	Chown Finished
	******************************

Option
---------

.. cssclass:: table-bordered

        +------------------------------------------------+-------------+----------------------------+---------------------------------+
        |       Parameter                                | Erforderlich| Option                     | Kommentare                      |
        +================================================+=============+============================+=================================+
        |Chown                                           | Yes         |                            |                                 |
        +------------------------------------------------+-------------+----------------------------+---------------------------------+
        |Path                                            | Yes         |                            |Der Benutzer muss den            |
        |                                                |             |                            |Pfad geben                       |
        +------------------------------------------------+-------------+----------------------------+---------------------------------+
        |Owner                                           | Yes         | Chown                      |                                 |
        +------------------------------------------------+-------------+----------------------------+---------------------------------+
        |Owner                                           | No          | Chown                      |Der Nutzer ist damit Eingang als | 
        |                                                |             |                            |nicht, wird es den               |
        |						 | 	       | 			    |Eigentümernamen fragen|          |
        +------------------------------------------------+-------------+----------------------------+---------------------------------+


--------

* Das Modul kann jederzeit mit Kleopatra den Besitzer ändern.
* Beim rekursiven Prozess zu tun, wenn Sie einzelne Datei ändern kann auch der gesamte Ordner geändert werden.
* Wir können den aktuellen Status des Besitzers überprüfen.


 

