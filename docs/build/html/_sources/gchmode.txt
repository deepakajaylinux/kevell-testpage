============
Chmode
============


Übersicht
-------------

Dateien und Verzeichnisse gehören sowohl für Eigentümer als auch für eine Gruppe. Eine Gruppe besteht meist aus eine Sammlung von Benutzern, alle aus der gleichen Gruppe. Der erste Satz von drei ist das Lesen, schreiben und Ausführen von Berechtigungen für den Besitzer der Datei.

Chmod wird verwendet, um die Berechtigungen für Dateien oder Verzeichnisse ändern. Auf Linux und andere Unix-artige Betriebssysteme gibt es eine Reihe von Regeln für jede Datei, die definiert, wer die Datei zugreifen kann, und wie sie darauf zugreifen können. Diese Regeln werden Dateirechte oder Datei-Modus genannt. Der Befehl Namen Chmod steht für "Modus wechseln", und es wird verwendet, um die Art und Weise zu definieren, die eine Datei zugegriffen werden kann.

Es gibt drei allgemeine Klassen von Benutzern:

* Der Benutzer, der die Datei ("Nutzer") besitzt
* Benutzer gehören der Datei definiert ("Besitzergruppe")
* Alle anderen ("Sonstige")


Wiederum für jede dieser Klassen des Benutzers gibt es drei Arten von Dateizugriff:

* Die Möglichkeit, den Inhalt der Datei ("Read") ansehen
* Die Fähigkeit, den Inhalt der Datei ("schreiben") ändern
* Die Möglichkeit, den Inhalt der Datei als Programm auf dem System ("ausführen") laufen


Für jede der drei Klassen des Benutzers gibt es drei Arten des Zugriffs. 


.. cssclass:: table-bordered  


 +------------+-----------------------------------------------------------------------------------------+
 | Symbole    | Was bedeutet									   	|
 +============+=========================================================================================+
 |rwx	      | der Besitzer der Datei kann lesen, schreiben, oder Führen Sie diese Datei als ein 	|
 |	      | Prozess auf dem System.								        |
 +------------+-----------------------------------------------------------------------------------------+
 |r-x	      | jemand in der Gruppe der Datei gelesen oder Führen Sie diese Datei, aber nicht, 	|
 |	      | es zu schreiben.									|
 +------------+-----------------------------------------------------------------------------------------+
 |r–	      | jeder kann überhaupt diese Datei lesen, aber nicht schreiben oder EXECUTE seinen Inhalt |
 |	      | als einen Prozess.|									|
 +------------+-----------------------------------------------------------------------------------------+



Help-Befehl
----------------------

Dieser Befehl hilft, um die Verwendung von Wechsel-Modus-Modul zu bestimmen. Der Benutzer wird kommen, über den anderen Weg/Format wissen, dieses Modul ausgeführt. Dieser Befehl führt den Endbenutzer, um diesen Befehl zu erfahren. Unten gegeben sind, den Befehl und den Screenshot von der gleichen. 

.. code-block:: bash
        
	        cleopatra Chmod help



Die bildliche Darstellung der oben genannte Befehl ist im folgenden aufgeführt,


.. code-block:: bash

 kevell@corp:/# cleopatra Chmod help
 ******************************


  This command handles file permission functions.

  Chmod, chmod

        - path
        Will change the file permission mode of a path
        example: cleopatra chmod path --yes --guess --recursive --path=/a/file/path --mode=0777


 ------------------------------
 End Help
 ******************************


Weg 
--------

Chmod-Pfad ist der Befehl der die Zugriffsberechtigungen auf Dateisystemobjekte (Dateien und Verzeichnisse) zu ändern.

Die Nummer 1, 2 und 4 stellt ausführen, schreiben und lesen. Diese Zahlen werden verwendet, da eine beliebige Kombination dieser drei Zahlen wird 
eindeutig sein. 

Wenn der Benutzer den Modus der Datei ändern muss die unten mit dem Befehl führt den Prozess.

.. code-block:: bash
        
	        cleopatra chmod path –yes –guess –recursive –path=/”File path” –mode=0777




Alternative Parameter 
--------------------------------                               

Es gibt zwei alternative Parameter, die in der Befehlszeile verwendet werden können. 

Chmod, Chmod

ZB: cleopatra Chmode path/ cleopatra chmod path


Vorteile
--------------


Chmod ändert die Zugriffsrechte der Datei Filename zum angegebenen Berechtigungen Berechtigungen angegeben. Berechtigungen definiert die Berechtigungen für den Besitzer der Datei ("Nutzer"), Mitglieder der Gruppe, die Datei (die "Gruppe") und alle anderen ("andere") besitzt. Es gibt zwei 
Möglichkeiten, diese Berechtigungen darzustellen: mit Symbolen (alphanumerische Zeichen) oder mit Oktalzahlen (die Ziffern 0 bis 7).

 

