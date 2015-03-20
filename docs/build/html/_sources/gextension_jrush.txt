=============
Extension
=============

Zusammenfassung
----------------

Erweiterung müssen identifiziert werden, so dass das Betriebssystem begegnen können. Diese Dateinamen haben bestimmte Regeln. Der erste Teil des Namens, der Links vom Punkt nennt den Stammnamen. Der Stammname kann keinen Gerätenamen identisch sein. Der zweite Teil auf der rechten Seite der Periode ist die Erweiterung. Es ist optional und ist oft, aber nicht notwendigerweise drei Zeichen lang. Erweiterung kann durch Codierung hinzugefügt werden. Es verstärkt um Schwindel mit Ubuntu und Cent OS.


Hilfe Befehl
-----------------

Der Help-Befehl führt die Benutzer über den Zweck und auch als zu den Optionen, die in der Erweiterung enthalten sind. Es listet die alternative Ausgabeparameter der Erweiterung. Es beschreibt auch die Syntax für die Funktionsweise des Jrush-Moduls. Der Help-Befehl für Erweiterung wird gezeigt wie unten beschrieben.


.. code-block:: bash

	jrush extension help

Nach Eingabe des Befehls führt es die Optionen als Aktion. Das folgende Bild visualisieren es offensichtlich.



.. code-block:: bash

 kevell@corp:/# jrush Extension help
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

  This command allows you to manage Joomla Extensions (Component, Module or Plugin).

  Extension, extension

        - disable
        Deletes a extension
        example: jrush extension disable

        - enable
        Enables a extension
        example: jrush extension enable

        - info
        Display the details of a extension
        example: jrush extension info


 ------------------------------
 End Help
 ****************************************


Alternative Parameter
----------------------------

Als eine Frage der Wahl mit Erweiterung der Benutzer machen kann der folgenden Optionen verwenden.

Extension, extension

Optionen
------------

Es gibt drei Möglichkeiten zur Verfügung. Lassen Sie uns über die Erweiterungs-Option sehen.


* Enable
* Disable
* Info

Disable
-----------

Wenn die Benutzereingabe automatisch es ermöglichen die Erweiterung löscht. Den folgenden Befehl zum Aktivieren verwendet. Wenn die Benutzereingabe automatisch es ermöglichen die Erweiterung löscht. Den folgenden Befehl zum Aktivieren verwendet.


.. code-block:: bash

	jrush extension Disable

Die folgenden Mantel-Shot können seine Funktion visualisieren.


.. code-block:: bash

 kevell@corp:/# jrush Extension disable --config-file="/var/www/html/joomla/configuration.php" 
 Enter a Extension ID. To enter element/extension name use --extension-element or --extension-name parameters
 1
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

 Extension:
 -------------------------

 The following extension was modified:

 Extension ID: 1
 Name: com_mailto
 Element: com_mailto
 Enabled: 0
 ------------------------------
 Extension Manage Finished
 ****************************************


Enable
-----------

Aktivieren wird verwendet, um die Erweiterung zu aktivieren. Der folgende Befehl helfen dem Anwender zu ermöglichen.

.. code-block:: bash

 	jrush extension 


.. code-block:: bash

 kevell@corp:/# jrush Extension enable --config-file="/var/www/html/joomla/configuration.php" 
 Enter a Extension ID. To enter element/extension name use --extension-element or --extension-name parameters
 1
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

 Extension:
 -------------------------

 The following extension was modified:
 
 Extension ID: 1
 Name: com_mailto
 Element: com_mailto
 Enabled: 1
 ------------------------------
 Extension Manage Finished
 ****************************************



Info
--------

Info ist eine Hilfe für den Benutzer zum Anzeigen von Details der Expansion unterstützen. Es fragt nach Erweiterung Id. Nach den Wert eingibt es Erweiterung Details angezeigt. Der folgende Befehl verwendet, um Informationen anzuzeigen.


.. code-block:: bash

	jrush extension info

Es kann sein, visualisiert durch den Screenshot.


.. code-block:: bash

 kevell@corp:/# jrush Extension info --config-file="/var/www/html/joomla/configuration.php" 
 Enter a Extension ID. To enter element/extension name use --extension-element or --extension-name parameters
 1
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

 Extension:
 -------------------------

 The following extension was modified:

 Extension ID: 1
 Name: com_mailto
 Element: com_mailto
 Enabled: 0
 ------------------------------
 Extension Manage Finished
 ****************************************

Vorteile
----------------

* Erweiterungen können eine Art von Metadaten betrachtet werden. 
* Mehrere Anwendungen mit einer bestimmten Erweiterung verbunden werden. * Keine Anfrage sensible * komfortable mit Ubuntu und Cent OS. 
* Verwendet, um die Erweiterung zu löschen 
* Info verwendet, um Informationen zur Erweiterung anzuzeigen.


