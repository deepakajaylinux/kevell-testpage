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

        - create
        Create a new system gem, overwriting if it exists
        example: ptconfigure gem create --gemname="somename"

        - remove
        Remove a system gem
        example: ptconfigure gem remove --gemname="somename"

        - set-password
        Set the password of a system gem
        example: ptconfigure gem set-password --gemname="somename" --new-password=                                                                                        "somepassword"

        - exists
        Check the existence of a gem
        example: ptconfigure gem exists --gemname="somename"

        - show-groups
        Show groups to which a gem belongs
        example: ptconfigure gem show-groups --gemname="somename"

        - add-to-group
        Add gem to a group
        example: ptconfigure gem add-to-group --gemname="somename" --groupname="so                                                                                        megroupname"

        - remove-from-group
        Remove gem from a group
        example: ptconfigure gem remove-from-group --gemname="somename" --groupnam                                                                                        e="somegroupname"

 ------------------------------
 End Help
 ******************************


Verschiedene Merkmale der Gem
---------------------------------

Wie aus der obigen Befehl help dargestellt, wird die verschiedenen Merkmale der Edelstein, wie unten aufgeführt,

* Erstellen
* Entfernen
* Set Password
* Vorhanden
* Show_groups
* Add_to_group
* Remove_from_group


Lassen Sie uns im Detail über diese Funktionen finden.

schaffen
--------

Diese Funktion zielt auf die Schaffung eines neuen Systems Juwel, und so gut wie überschreibt bei bereits bestehenden. Diese Funktion von Perle mit diesem Modul kann durch die folgende Syntax erreicht werden,

.. code-block:: bash

	ptconfigure gem create --gemname="somename"

An der Stelle des gemname kann der Benutzer den Namen des Edelsteins, das erzeugt werden soll angeben. Nach der Eingabe des Befehls, wie oben angegeben, wird das neue Schmuckstück mit dem angegebenen Namen erstellt werden.

ENTFERNEN
-----------------

Dies funktioniert zielt darauf ab, eine bestehende gem. Diese Funktion von Perle mit diesem Modul kann durch die folgende Syntax erreicht werden,

.. code-block:: bash

	ptconfigure gem remove --gemname="somename"


An der Stelle des gemname kann der Benutzer den Namen des Edelsteins, die gelöscht werden soll, zu spezifizieren. Nach der Eingabe des Befehls, wie oben angegeben, wird die angegebene Juwel gelöscht.

SET PASS
--------------------

Diese Funktion erleichtert die Einstellung eines neuen Passworts auf ein System, Edelstein gemäß den Anforderungen. Dies kann durch den Befehl, wie unten angegeben durchgeführt werden,

.. code-block:: bash

	ptconfigure gem set-password --gemname="somename" --new-password="somepassword"

Um diese Funktionen zu implementieren, muss der Benutzer, um die beiden Felder geben,

* Gem Namen
* Neues Kennwort

Nachdem Sie die beiden Felder im Format der oben genannten Befehl wird das neue Kennwort für den angegebenen Juwel geschaffen werden.

VORHANDEN
-------------------

Diese Funktion soll die Überprüfung der Existenz einer gem. Dies kann einfach durchgeführt werden, indem Sie unter dem Befehl,

.. code-block:: bash

	ptconfigure gem exists --gemname="somename"

Nach der Anwendung des Befehls, wie oben, wird die Existenz einer genannten gem dem Ergebnis sichergestellt.

Gruppen Zeige
--------------------

Diese Funktion unterstützt die Nutzer wissen zu welcher Gruppe ist der Edelstein gehört. Dies kann einfach durch das unten stehende Befehl erreicht werden,

.. code-block:: bash

	ptconfigure gem show-groups --gemname="somename"

Der Benutzer muss den Namen der Edelstein auf dem Gebiet der gemname angeben, um die Details seiner Gruppe wissen.

ADD _TO_GROUP
-----------------------

Das Hauptziel dieser Funktion ist es, die erforderlichen Juwel in die gewünschte Gruppe, indem einfach der Befehl wie unten angegeben hinzu,

.. code-block:: bash

	ptconfigure gem add-to-group --gemname="somename" --groupname="somegroupname"

Um diese Funktion zu implementieren, muss der Benutzer die beiden folgenden Felder nach ihren Bedürfnissen im Format der oben genannten Befehl angeben,

* Gemname
* Gruppennamen

REMOVE_FROM_GROUP
--------------------------------

Der Hauptzweck dieser Funktion besteht darin, das gem von einer Gruppe, indem einfach den Befehl, wie unten angegeben zu entfernen,

.. code-block:: bash

	ptconfigure gem remove-from-group --gemname="somename" --groupname="somegroupname"

Um diese Funktion zu implementieren, muss der Benutzer die beiden folgenden Felder nach ihren Bedürfnissen im Format der oben genannten Befehl angeben,

* Gemname
* Gruppennamen

Alternative Parameter
-----------------------------

Die alternative Parameter für dieses Modul, die beide in Erklärung verwendet werden,

* Gem
* Edelstein

Vorteile
---------

* Die verwendeten Hilfe und andere unterschiedliche Merkmale von Edel erklärt Parameter wird nicht zwischen Groß- und Kleinschreibung.
* Es ist gut-to-do in beiden Cent os und als auch in Ubuntu.
* Mit diesem Modul kann der Benutzer zu erstellen und zu ändern sowie den Edelstein nach ihren Bedürfnissen.
* Die Existenz einer Perle unter diesem Modul gewährleistet werden.


