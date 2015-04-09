====
Gem
====

Zusammenfassung
-----------------------

Dieses Modul umschließt alle Bedürfnisse der Nutzer für die Arbeit mit GEM. Es umfaßt verschiedene Funktionen, und Kassen fördert verschiedene Funktionen durchgeführt werden.

RubyGems ist ein Paketmanager für die Programmiersprache Ruby, die ein Standardformat für die Verteilung von Ruby-Programme und Bibliotheken bietet (in einem eigenständigen Format namens ein "Juwel"), ein Werkzeug entwickelt, die einfache Verwaltung den Einbau von Edelsteinen und einen Server für verteilen sie.

Lassen Sie uns die verschiedenen Funktionen und wie man dieses Modul aus den kommenden Themen verwenden.

Hilfe Befehl
-------------------

Der Befehl help weist die Benutzer über den Zweck und verschiedene Funktionen und die Syntax für die Durchführung dieser verschiedenen Funktionen. Außerdem werden outs die alternativen Parameter, die in Erklärungen verwendet werden kann. Die Syntax-Format zur Anwendung Hilfe-Option im Rahmen dieses Moduls ist unten angegeben,

.. code-block:: bash

	ptconfigure gem help

Der folgende Screenshot visualisieren die Ausgabe und Bearbeitung der Hilfe-Option im Rahmen dieses Moduls.

.. code-block:: bash

 kevell@corp:/# ptconfigure gem help
 ******************************


  This command allows you to modify create or modify gems

  Gem, gem

        - install
        Install
        example: ptconfigure gem pkg-install --package-name="somename"

        - remove
        Remove
        example: ptconfigure gem pkg-remove --package-name="somename"

        - ensure
        Ensure
        example: ptconfigure gem pkg-ensure --package-name="somename"

        - update
        Update
        example: ptconfigure gem update


 ------------------------------
 End Help
 ******************************


Verschiedene Merkmale der Gem
---------------------------------

Wie aus der obigen Befehl help dargestellt, wird die verschiedenen Merkmale der Edelstein, wie unten aufgeführt,

* Install
* Remove
* Ensure
* Update


Lassen Sie uns im Detail über diese Funktionen finden.


Install
-----------

Diese Funktion ermöglicht es Ihnen, das Paket, das die Bedürfnisse der Nutzer zu installieren. Der folgende Screenshot visualisieren die Ausgabe ,

.. code-block:: bash

 kevell@corp:/# ptconfigure gem pkg-install --package-name=cucumber
 Successfully installed cucumber-2.0.0
 1 gem installed
 Installing ri documentation for cucumber-2.0.0...
 Installing RDoc documentation for cucumber-2.0.0...
 ******************************


 Gem Modifications:
 --------------------------------------------

 Gem: Success

 ------------------------------
 Gem Mods Finished
 ******************************




Remove
-----------------

Dies funktioniert zielt darauf ab, eine bestehende gem. Diese Funktion von Perle mit diesem Modul kann durch die folgende Syntax erreicht werden,

.. code-block:: bash

	ptconfigure gem remove --gemname="somename"


An der Stelle des gemname kann der Benutzer den Namen des Edelsteins, die gelöscht werden soll, zu spezifizieren. Nach der Eingabe des Befehls, wie oben angegeben, wird die angegebene Juwel gelöscht.

.. code-block:: bash

 kevell@corp:/# ptconfigure gem pkg-remove --package-name=cucumber
 Removing cucumber
 Successfully uninstalled cucumber-2.0.0
 ******************************


 Gem Modifications:
 --------------------------------------------

 Gem: Failure

 ------------------------------
 Gem Mods Finished
 ****************************** 



Ensure
--------------------

Diese Funktion stellt sicher, das Paket in der Maschine korrekt installiert ist.

.. code-block:: bash

	ptconfigure gem pkg-ensure --package="ssh"

.. code-block:: bash


 kevell@corp:/# ptconfigure gem pkg-ensure
 Enter Package:
 cucumber
 true
 [Pharaoh Logging] Package cucumber from the Packager Gem is Installed
 ******************************


 Gem Modifications:
 --------------------------------------------

 Gem: Success

 ------------------------------
 Gem Mods Finished
 ******************************


.. code-block:: bash

 kevell@corp:/# ptconfigure gem pkg-ensure
 Enter Package:
 cucumber
 false
 [Pharaoh Logging] Package cucumber from the Packager Gem is not Installed
 ******************************


 Gem Modifications:
 --------------------------------------------

 Gem: Success

 ------------------------------
 Gem Mods Finished
 ******************************


Alternative Parameter
-----------------------------

Die alternative Parameter für dieses Modul, die beide in Erklärung verwendet werden,

* Gem
* gem

Vorteile
---------

* Die verwendeten Hilfe und andere unterschiedliche Merkmale von Edel erklärt Parameter wird nicht zwischen Groß- und Kleinschreibung.
* Es ist gut-to-do in beiden Cent os und als auch in Ubuntu.
* Mit diesem Modul kann der Benutzer zu erstellen und zu ändern sowie den Edelstein nach ihren Bedürfnissen.
* Die Existenz einer Perle unter diesem Modul gewährleistet werden.


