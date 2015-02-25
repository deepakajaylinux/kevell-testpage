==========
File
==========

Zusammenfassung
----------------------

Die Datei ist ein Standardprogramm zum Erkennen der Art von Daten in einer Computerdatei enthalten sind. Die Datei Befehl versucht, jedes Dateisystemobjekt (dh Datei, ein Verzeichnis oder Link), die als Argument (dh Eingang) vorgesehen ist, zu klassifizieren. Datei testet jedes Argument in einem Versuch, sie zu klassifizieren. Es gibt drei Arten von Tests, in dieser Reihenfolge durchgeführt: Dateisystem-Tests, magische Zahl Tests und Sprachtests.

Das erste ist ein Dateisystem-Test, der den Systemaufruf stat verwendet, um Informationen aus der Objekt inode (die Informationen zu einer Datei enthält) zu erhalten.

Der zweite Test überprüft, ob es eine magische Zahl, die eine Reihe an oder nahe der Anfang von vielen Arten von Dateien, die das Dateiformat anzeigt (dh die Art der Datei) eingebettet ist.


Im Falle, dass die ersten beiden Tests fehlschlagen, um den Typ einer Datei zu ermitteln, werden Sprachtests verwendet werden, um festzustellen, ob es Klartext (dh ausschließlich aus Menschen lesbare Zeichen besteht), und, wenn ja, welche Art von Klartext , wie beispielsweise HTML (Hypertext Markup Language) oder Quellcode

Hilfe Befehl
-----------------

Diese Funktion dient, um die Verwendung von Dateimodul zu bestimmen. Der Benutzer wird kommen, um über die verschiedenen Möglichkeiten / Format um dieses Modul ausführen kennen. Dieser Befehl leitet den Anwender, um den Zweck dieses Befehls kennen. Da unten sind die Kommando- und der Screenshot der gleiche.

.. code-block:: bash
        
	        ptconfigure file help

schaffen
------------

Wenn der Benutzer braucht, um eine neue Systemdatei erstellen, wird der unten angegebenen Befehl den Prozess auszuführen.

.. code-block:: bash

                ptconfigure file create --file="somename"

Die unten angegebenen Befehle überschreiben Dateien, die es gibt

.. code-block:: bash
         
	       ptconfigure file create --file="somename” --overwrite-existing

The below given command for write the data in the file

.. code-block:: bash
           
		ptconfigure file create –file="somename” --data="things to put in the file" 

löschen
----------

Wenn der Benutzer eine Systemdatei zu löschen muss, wird die unten gegebenen Befehl das Verfahren auszuführen.

.. code-block:: bash
	
		ptconfigure file delete --file="somename"

vorhanden
-----------

Wenn der Benutzer benötigt, um die Existenz einer Datei zu überprüfen, wird der unten angegebenen Befehl den Prozess auszuführen.

.. code-block:: bash

		ptconfigure file exists --filename="somename"

anhängen
------------

Wenn der Benutzer eine Zeile in eine Datei angehängt werden muss, wird der unten angegebenen Befehl den Prozess auszuführen.

.. code-block:: bash
	
		ptconfigure file append --filename="somename" --line="a line"

* Line option – you can insert a line to be appended

Should-have-line
-------------------

When the user needs to ensure that a file contains a particular line, the below given command will execute the process

.. code-block:: bash
	
		ptconfigure file should-have-line --filename="somename" --line="a line"

* Line option – Statement that needs to be checked


Options
-----------  

.. cssclass:: table-bordered

 +-------------------------+----------------------------------------------------------+
 | Parameter               | Alternative Parameter                                    |
 +=========================+==========================================================+
 |ptconfigure file help    | Eine der beiden alternativen Parameter können            |
 |                         | verwendet werden, in Befehl - File, file                 |
 |                         | eg: ptconfigure File Install/ ptconfigure file Install|  |
 +-------------------------+----------------------------------------------------------+

                             
Vorteile
-----------

* Geben Sie einen Datei speziell formatierte, die positionsempfindlichen Tests; Standardpositionsempfindlichen Tests und kontextsensitive
  Tests nicht durchgeführt werden.

