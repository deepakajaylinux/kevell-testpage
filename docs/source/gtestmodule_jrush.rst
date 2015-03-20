=============
Test module
=============

Zusammenfassung
-----------------

Testmodule ist die beliebteste Jrush Test, Stand diese Überprüfung über die Erweiterung der Datei und machen Gebrauch davon. Testmodule ist ein Framework aber kann in Absprache mit anderen Tests Artikel verwendet werden. TestModule stellt daher nur die Baseline Tests Funktionen aus anderen Bibliotheken um mehr spezifische und anspruchsvolle Funktionalität zu implementieren. Es zeigt die aktuellen Aktionen. Dies ist komfortabel mit Ubuntu und Cent OS.


Hilfe Befehl
-----------------------

Der Help-Befehl führt die Benutzer über den Zweck und auch als zu den Optionen, die in die Testmodule enthalten sind. Es listet die alternative Ausgabeparameter der Testmodule. Es beschreibt auch die Syntax für die Funktionsweise des Jrush-Moduls. Der Help-Befehl für Testmodule wird angezeigt, wie unten beschrieben.


.. code-block:: bash

	jrush testmodules help

Nach Eingabe des Befehls führt es die Optionen als Aktion. Das folgende Bild visualisieren es offensichtlich.



.. code-block:: bash

 kevell@corp:/# jrush TestModule help
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

  This command allows you to update TestModule.

  TestModule, testmodule, test-module

        - action-one
        An example action. Currently, we get all titles of articles
        example: jrush test-module action-one

        - action-two
        An example action. Currently, we get all titles of articles
        example: jrush test-module action-two

 ------------------------------
 End Help
 ****************************************



Alternative Parameter
--------------------------------

Alternative Verwendung Testmodule der Benutzer kann die folgenden Optionen nutzen.


Test Module, testmodule, test-module.

Optionen
-------------

Es gibt zwei Optionen zur Verfügung. Sie sind wie folgt.

* Action-one
* Action-two

Action-one
-----------------

Es zeigt die aktuellen Titeln von Artikeln. Der Befehl verwendet, um die Aktion-tun ist wie folgt,


.. code-block:: bash

	jrush test-module action-one

Nach gibt der Befehl zeigt es die aktuellen Informationen und die Titel der Artikel. Der Screenshot stellt das gleiche.



.. code-block:: bash

 kevell@corp:/# jrush test-module action-one --config-file="/var/www/html/joomla/configuration.php"
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

 TestModule Action One:
 -------------------------
 array(6) {
  [0]=>
  string(8) "About Us"
  [1]=>
  string(15) "Article 1 Title"
  [2]=>
  string(18) "Creating Your Site"
  [3]=>
  string(9) "article-1"
  [4]=>
  string(9) "article-2"
  [5]=>
  string(9) "article-3"
 }

 ------------------------------
 TestModule Action One Finished
 ****************************************



Action-two
-----------------

Es zeigt die aktuellen Titeln von Artikeln. Der Befehl verwendet, um die Aktion-tun ist wie folgt,


.. code-block:: bash

	jrush testmodule action-two

Nach gibt der Befehl zeigt es die aktuellen Informationen und die Titel der Artikel.


Vorteile
----------------

* Überprüfen Sie die Module korrekt. 
* Nicht Case sensitive. 
* Weniger zeitaufwendig. 
* Billiger, in einfache Website zu aktualisieren.       
* Neueste Update steht 
* geeignet zur Arbeit mit Ubuntu und CentOS.

