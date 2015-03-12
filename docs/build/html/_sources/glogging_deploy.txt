========
Logging
========


Zusammenfassung
-----------------------

Das Logging-Modul wird für die Zwecke der log eine Nachricht auf der Konsole verwendet wird, und ist gegebenenfalls für PHP-Fehlerprotokoll verwendet. Wir wollen sehen, wie die Installation und um das Protokoll für die Deklaration von Nachricht und in PHP-Fehlerprotokoll zu verwenden.


Hilfe Befehl
--------------------

Der Befehl help dient als kurze Bedienungsanleitung, die den Benutzer über ihre Nutzung und Methoden führt. Sie legt die alternativen Parameter, die in der Erklärung verwendet werden kann, und ein Beispiel für die Syntax, um ein Protokoll zu definieren. Der Befehl zur Feststellung der Hilfe-Option verwendet, ist wie folgt:

.. code-block:: bash

	ptdeploy Logging help

Der folgende Screenshot zeigt bildhaft über die Arbeit der Befehl help.

.. code-block:: bash

 kevell@corp:/# ptdeploy Logging help
 ******************************


  Use this to log a message to the Console, and optionally the php error log.

  Logging, logging

        - log
        Logs a message the console or
        example: ptconfigure logging log --php-log --log-message="Here is something logging to the console and error log"

 ------------------------------
 End Help
 ******************************


Installation
---------------

The command used for installing the logging under ptdeploy is given below:

.. code-block:: bash

	ptdeploy logging log


Nach der Eingabe wird der Befehl über das Verfahren der Montage wird in der folgenden tabellarischen Spalte dargestellt.

.. cssclass:: table-bordered

 +----------------------------+--------------------------------------+-----------+--------------------------------------------------------+
 | Parameters                 | Alternative Parameters               | Options   | Kommentare                                             |
 +============================+======================================+===========+========================================================+
 |Install Logging? (Y/N)      | Statt der Protokollierung können wir | Y(Yes)    | Wenn der Benutzer wünschen, den Installationsprozess   |
 |                            | Protokollierung auch.                |           | können sie Eingang als Y. gehen                        |
 +----------------------------+--------------------------------------+-----------+--------------------------------------------------------+
 |Install Logging? (Y/N)      | Statt der Protokollierung können wir | N(No)     | Wenn der Benutzer wünschen, den Installationsprozess   |
 |                            | Protokollierung auch.                |           | können sie Eingang als N. beenden|                     |
 +----------------------------+--------------------------------------+-----------+--------------------------------------------------------+


Wenn der Benutzer den Installationsprozess fort, der Prozess fordern Sie die Benutzer, um die Log-Nachricht mit der Frage spezifizieren


.. code-block:: bash

	"Enter Log Message"
	
	"Good Morning"


Sobald die Benutzereingabe die Nachricht, wird der Give Protokollmeldung auf dem Bildschirm erscheinen, wie gezeigt werden:
"Good Morning"

Schließlich wird die Installation abgeschlossen. Der folgende Screenshot zeigt den Prozess der Installation bildlich.

.. code-block:: bash

 kevell@corp:/#  ptdeploy logging log
 Install Logging? (Y/N) 
 Y
 *******************************
 *   Golden Contact Computing  *
 *           Logging!          *
 *******************************
 Enter Log Message
 Good Morning
 [Pharaoh Logging] Good Morning
 ... All done!
 *******************************
 Thanks for installing , visit www.gcsoftshop.co.uk for more
 ******************************


 Single App Installer:
 --------------------------------------------


 No Data.

 ------------------------------
 Installer Finished



Wie PHP-Fehlerprotokoll definieren
-------------------------------------

Die Syntax für die Deklaration des Protokolls für PHP-Fehlerprotokoll ist unten dargestellt:

.. code-block:: bash

	ptconfigure logging log --php- log --log-message="Here is something logging to the console and error log"

Instead of 

.. code-block:: bash

 	log-message="Here is something logging to the console and error log"


the user can add any text to the portion of log message depending upon their requirements.

Vorteile
-----------

* Der Benutzer kann die häufig verwendeten Protokollmeldung für die PHP-Fehlerprotokoll hinzuzufügen.
* Bei der Installation des Protokoll der Benutzer eingeben können und sorgen für die Anzeige der Protokollmeldung.
* Es ist gut-to-do sowohl ubuntu und als auch in Cent OS.
* Die in der Erklärung verwendeten Parameter wird nicht zwischen Groß- und Kleinschreibung.

