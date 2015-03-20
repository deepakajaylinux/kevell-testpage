==============
Version
==============


Zusammenfassung
-------------------

Dieser Artikel ist über den Begriff "Version", wie er in verschiedenen Kontexten verwendet wird. Software-Versionsverwaltung ist den Vorgang des Zuweisens von eindeutigen Namen oder einzigartige Versionsnummern einzigartige Zuständen der Computersoftware. Innerhalb einer bestimmten Version Anzahl Kategorie (major, Minor) diese Zahlen sind in der Regel in aufsteigender Reihenfolge zugeordnet und neue Entwicklungen in der Software entsprechen. Auf feinkörnigen Ebene wird Versionsverwaltung oft für die Verfolgung der inkrementell verschiedener Versionen von elektronischen Informationen, ob diese Informationen Computersoftware ist oder nicht.


Hilfe Befehl
----------------------

Dieser Befehl hilft, die Verwendung von Version Modul bestimmen. Der Benutzer wird kommen, über die verschiedenen Möglichkeiten/Format wissen, dieses Modul ausgeführt. Dieser Befehl führt den Endbenutzer, um diesen Befehl zu erfahren. Im folgenden sind mit dem Befehl und der Screenshot von der gleichen.


.. code-block:: bash
        
	jrush  version help

Die bildliche Darstellung der Help-Befehl ist im folgenden aufgeführt,

.. code-block:: bash

 kevell@corp:/# jrush  version help
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

  This command Joomls Version information.

  Version, version

        - available
        Returns available Joomla Versions
        example: jrush version available

        - current
        Returns the current Joomla Version
        example: jrush version current

 ------------------------------
 End Help
 ****************************************


Available
----------------

Wenn der Benutzer wissen über die verfügbaren Joomla-Version muss, die unten mit dem Befehl wird ausgeführt, den Prozess der Installation.


.. code-block:: bash
        
	jrush version available ..config file=”bootstrap file path”


Die bildliche Darstellung des Screenshots ist nachfolgend aufgeführt,


.. code-block:: bash

 kevell@corp:/# jrush version available --config-file="/var/www/html/joomla/configuration.php" 
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

 Joomla Version Info:

 -------------------------

 Version: array(1) {
  ["availableVersions"]=>
  array(2) {
    [0]=>
    string(5) "1.5.0"
    [1]=>
    string(6) "1.5.26"
  }
 }

 ------------------------------
 Joomla Version Info Finished
 ****************************************

Current
----------------

Wenn der Benutzer wissen über die aktuelle Joomla-Version muss, die unten mit dem Befehl wird ausgeführt, den Prozess der Installation.


.. code-block:: bash
        
	jrush version current ..config file=”bootstrap file path”

Die bildliche Darstellung der oben genannte Befehl ist im folgenden aufgeführt,


.. code-block:: bash

 kevell@corp:/# jrush version current --config-file="/var/www/html/joomla/configuration.php" 
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

 Joomla Version Info:

 -------------------------

 Version: array(3) {
  ["shortVersion"]=>
  string(5) "3.3.3"
  ["longVersion"]=>
  string(53) "Joomla! 3.3.3 Stable [ Ember ] 25-July-2014 13:00 GMT"
  ["detailed"]=>
  object(ArrayObject)#47 (1) {
    ["storage":"ArrayObject":private]=>
    object(JVersion)#7 (11) {
      ["PRODUCT"]=>
      string(7) "Joomla!"
      ["RELEASE"]=>
      string(3) "3.3"
      ["DEV_LEVEL"]=>
      string(1) "3"
      ["DEV_STATUS"]=>
      string(6) "Stable"
      ["BUILD"]=>
      string(0) ""
      ["CODENAME"]=>
      string(5) "Ember"
      ["RELDATE"]=>
      string(12) "25-July-2014"
      ["RELTIME"]=>
      string(5) "13:00"
      ["RELTZ"]=>
      string(3) "GMT"
      ["COPYRIGHT"]=>
      string(72) "Copyright (C) 2005 - 2014 Open Source Matters, Inc. All rights reserved."
      ["URL"]=>
      string(107) "<a href="http://www.joomla.org">Joomla!</a> is Free Software released under the GNU General Public License."
    }
  }
 }

 ------------------------------
 Joomla Version Info Finished
 ****************************************


Alternative Parameter
----------------------------

Eines der zwei alternative Parameter einsetzbar in Befehl-

jarticle, JArticle

eg:  jrush version current ..config file=”bootstrap file path”/ jrush Version current ..config file=”bootstrap file path”

Vorteile
--------------

* Hilft, die Informationen über eine Version auf einfache Weise erhalten * hilft dem Benutzer über die Verfügbarkeit der Version Joomla kennen   zu lernen 
* hilft dem Benutzer über die aktuelle Joomla-Version kennen zu lernen

