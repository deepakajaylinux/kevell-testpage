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

.. code-block:: bash

 kevell@corp:/# ptconfigure File help
 ******************************


  This command allows you to modify files or check their existence

  File, file

        - create
        Create a new system file
        example: ptconfigure file create --file="somename"

        - delete
        Delete a system file
        example: ptconfigure file delete --file="somename"

        - exists
        Check the existence of a file
        example: ptconfigure file exists --filename="somename"

        - append
        Append a line to a file
        example: ptconfigure file append --filename="somename" --line="a line"

        - should-have-line
        Ensure that a file contains a particular line
        example: ptconfigure file should-have-line --filename="somename" --line="a line"

 ------------------------------
 End Help
 ******************************


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


.. code-block:: bash

 kevell@corp:/# ptconfigure file create --file="somename"

 [Pharaoh Logging] [File] Creating File somename
 File somename exists 
 ******************************


 File Modifications:
 --------------------------------------------

 File: Success

 ------------------------------
 File Mods Finished
 ******************************



löschen
----------

Wenn der Benutzer eine Systemdatei zu löschen muss, wird die unten gegebenen Befehl das Verfahren auszuführen.

.. code-block:: bash
	
		ptconfigure file delete --file="somename"


.. code-block:: bash

 kevell@corp:/# ptconfigure file delete --file="somename"

 [Pharaoh Logging] [File] Deleting File somename
 somename Deleted
 File somename not exists 
 ******************************


 File Modifications:
 --------------------------------------------

 File: Success

 ------------------------------
 File Mods Finished
 ******************************




vorhanden
-----------

Wenn der Benutzer benötigt, um die Existenz einer Datei zu überprüfen, wird der unten angegebenen Befehl den Prozess auszuführen.

.. code-block:: bash

		ptconfigure file exists --filename="somename"

.. code-block:: bash

 kevell@corp:/# ptconfigure file exists --filename="somename"

 Enter File Path:
 /home/kevells/Desktop/somename
 File /home/kevells/Desktop/somename exists 
 ******************************


 File Modifications:
 --------------------------------------------

 File: Success

 ------------------------------
 File Mods Finished
 ******************************


anhängen
------------

Wenn der Benutzer eine Zeile in eine Datei angehängt werden muss, wird der unten angegebenen Befehl den Prozess auszuführen.

.. code-block:: bash
	
		ptconfigure file append --filename="somename" --line="a line"

* Line option – you can insert a line to be appended

.. code-block:: bash

 kevell@corp:/# ptconfigure file append --filename="somename" --line="a line"

 Enter File Path:
 /home/kevells/Desktop/somename                             
 Enter the input for append:
 this is for test
 [Pharaoh Logging] [File] Reading File /home/kevells/Desktop/somename
 [Pharaoh Logging] [File] Writing File /home/kevells/Desktop/somename
 ******************************


 File Modifications:
 --------------------------------------------

 File: Success

 ------------------------------
 File Mods Finished
 ******************************





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

