=========
Cache
=========


Zusammenfassung
-----------------

JRush Ergänzung zur im temporären Speicher-Cache löschen. Es hat zwei Typen von Caches. Aber beide haben unterschiedliche Funktionen gemäß ihren Namen. Sie sind Website klar und Admin klar. Es ist erfreut mit Ubuntu und Cent OS. Löschen von Dateien, Ordnern und Anwendungen-- und das Löschen der Daten aus dem temporären Speicher--werden nicht ausreichen, wenn du gehst um zu recyceln wird nicht der Inhalt auf Ihrem Computer verfügbar sein.


Hilfe Befehl
--------------------------

Der Help-Befehl verarbeitet die Benutzer über die Bestimmung und auch als zu den Optionen, die im Cache enthalten sind. Es listet die alternative Ausgabeparameter des Caches. Es beschreibt auch die Syntax für die Funktionsweise des Jrush-Moduls. Der Help-Befehl für Cache wird gezeigt wie unten beschrieben.


.. code-block:: bash

	jrush cache help

Nach Eingabe des Befehls führt es die Optionen als Aktion. Das folgende Bild vorstellen es wahrnehmbar.


.. code-block:: bash

 kevell@corp:/# jrush cache help
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

  This command allows you to clear Cache.

  Cache, cache

        - site-clear
        Deletes a user
        example: jrush cache site-clear

        - admin-clear
        Clear the administrator cache
        example: jrush cache admin-clear

 ------------------------------
 End Help
 ****************************************

 
Alternative Parameter
--------------------------------

Auf der anderen Seite Cache des Benutzers verwenden, kann die folgenden Optionen verleihen.


Cache, cache.

Optionen
-------------

Es gibt zwei Optionen zur Verfügung. Sie sind wie folgt.


* Site-clear 
* Admin-clear

Jetzt lassen Sie uns wissen Sie über beide Optionen.


Site-clear
--------------

Website-Clear ist Costoff, den Benutzer zu löschen. Der folgende Befehl wird verwendet, um die Site zu löschen.


.. code-block:: bash

	jrush cache site-clear 

Nach Eingaben wie oben Befehl kommt die Ausgabe wie eine Codierung. Bei der End-Cache kann löschen fertig angezeigt werden. Die Screenshots präsentiert das gleiche.


.. code-block:: bash

 kevell@corp:/# jrush cache site-clear --config-file="/var/www/html/joomla/configuration.php" 
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

 Joomla Cache Clearing Info:

 -------------------------

 Cache: array(2) {
  ["site_cache_clear"]=>
  string(19) "Site Cache Clearing"
  ["site_cache_clear_result"]=>
  array(0) {
  }
 }

 ------------------------------
 Joomla Cache Clearing Finished
 ****************************************

Admin-clear
-------------------

Das Tragen des Administrators Cache löschen. Der Befehl Dienstleistungen den Benutzer Admin wie folgt zu deaktivieren.


.. code-block:: bash

	jrush cache admin-clear

Die folgende Anzeige-Aufnahmen weisen Sie den Benutzer über Admin-Clear-Funktion.


.. code-block:: bash

 kevell@corp:/# jrush cache admin-clear --config-file="/var/www/html/joomla/configuration.php" 
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

 Joomla Cache Clearing Info:

 -------------------------

 Cache: array(2) {
  ["admin_cache_clear"]=>
  string(20) "Admin Cache Clearing"
  ["admin_cache_clear_result"]=>
  array(0) {
  }
 }

 ------------------------------
 Joomla Cache Clearing Finished
 ****************************************


Vorteile
---------------

* It selbstgefällig zu Anstrengung mit Ubuntu und Cent OS. 
* Nicht groß-und Kleinschreibung. 
* Es gebrauchte, um den Benutzer löschen. 
* Es hilft klar admin.


