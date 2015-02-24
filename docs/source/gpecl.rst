=====
PECL
=====

Zusammenfassung
----------------

PECL steht für "Positive Emitter Coupled Logic". PECL differentielle Logikausgänge allgemein in Hochgeschwindigkeits-Taktverteilungsschaltungen verwendet. Dieser Befehl ermöglicht es dem Benutzer, zu erstellen, zu entfernen, setpassward, existieren. Konzernaktivitäten auch über diesen Befehl möglich. Dieser Befehl Hauptfunktion wird auf dem System. Es eignet sich mit Ubuntu und CentOS.

Hilfe Befehl
----------------------

Pecl macht Paketentwicklung ein Kinderspiel: es funktioniert mit existieren, zu modifizieren, zu erstellen, um das Set für System pecl PASSWORT unterstützen. Mit pecl, Ändern eines Pakets wird so einfach, dass es der Benutzer Standard-Layout, wenn der Benutzer schreibt eine erhebliche Menge an Code.

.. code-block:: bash

		ptconfigure pecl help


Die folgende Abbildung erläutert die Funktion.

.. code-block:: bash

 kevell@corp:/# ptconfigure PECL help

 ******************************


  This command allows you to modify create or modify pecls

  PECL, pecl

        - create
        Create a new system pecl, overwriting if it exists
        example: ptconfigure pecl create --peclname="somename"

        - remove
        Remove a system pecl
        example: ptconfigure pecl remove --peclname="somename"

        - set-password
        Set the password of a system pecl
        example: ptconfigure pecl set-password --peclname="somename" --new-password="somepassword"

        - exists
        Check the existence of a pecl
        example: ptconfigure pecl exists --peclname="somename"

        - show-groups
        Show groups to which a pecl belongs
        example: ptconfigure pecl show-groups --peclname="somename"

        - add-to-group
        Add pecl to a group
        example: ptconfigure pecl add-to-group --peclname="somename" --groupname="somegroupname"

        - remove-from-group
        Remove pecl from a group
        example: ptconfigure pecl remove-from-group --peclname="somename" --groupname="somegroupname"

 ------------------------------
 End Help
 ******************************

schaffen
------------

Dieser Befehl ermöglicht es dem Benutzer, ein neues System pecl erstellen. Überschreiben ist im Falle der Existenz möglich. New pecl Namen können in einem einzigen Befehl selbst zu erwähnen.

Der Befehl zum erstellen verwendet wird, ist wie folgt

.. code-block:: bash

		ptconfigure pecl create 

Nach Eingang als dem oben genannten Befehl, beginnt es zu schaffen pecl. Im Falle einer bestehenden Datei die Anzeige erscheint. Der Befehl und seine Funktion erklärt, mit den Screenshots.

.. code-block:: bash

        - create
        Create a new system pecl, overwriting if it exists
        example: ptconfigure pecl create --peclname="somename"


entfernen
------------

Dieser Befehl ermöglicht dem Benutzer, eine pecl entfernen. Abnehmbare pecl Name kann in einer einzigen Befehlszeile selbst zu erwähnen.
Der Befehl zum erstellen verwendet wird, ist wie folgt

.. code-block:: bash

		ptconfigure pecl remove 

Nach Eingang als dem oben genannten Befehl, beginnt es zu entfernen pecl. Im Falle einer Datei bereits vom pecl die Angabe Meldung erscheint entfernt. Der Befehl und seine Funktion erklärt, mit den Screenshots.

.. code-block:: bash

        - remove
        Remove a system pecl
        example: ptconfigure pecl remove --peclname="somename"

Set PASSWORT
--------------------

Setpassward verwendet werden, um einen bestimmten Befehl mit root-Rechten in pecl laufen. Das Interessante daran ist, dass, wenn der Benutzer den Einsatz für einen bestimmten Befehl PASSWORT, fordert System den Benutzer für das Kennwort des aktuellen Benutzers. Der Befehl zum erstellen verwendet wird, ist wie folgt

.. code-block:: bash

	ptconfigure pecl  set-passward

Pecl Namen und neuen PASSWORT erwähnen auch in der gleichen Befehlszeile. Damit ist ein weiterer Vorteil für dieses Modul. Der folgende Screenshot Funktionen zu visualisieren.

.. code-block:: bash

        - set-password
        Set the password of a system pecl
        example: ptconfigure pecl set-password --peclname="somename" --new-password="somepassword"


vorhanden
-----------

Dieser Befehl verwendet werden, um die Existenz einer pecl überprüfen. Einfache Befehl macht diesen Befehl korrekt arbeiten. Zunächst überprüft er pecl Namen im System zeigt dann, ob sie bestehende oder nicht. Der folgende Befehl verwendet werden, um diese Funktion zu tun

.. code-block:: bash

		ptconfigure pecl Exists

Der folgende Screenshot Funktionen zu visualisieren.

.. code-block:: bash

        - exists
        Check the existence of a pecl
        example: ptconfigure pecl exists --peclname="somename"


Show-Gruppe
------------------

Dieser Befehl verwendet, um die Arbeitsgruppe einer pecl überprüfen. Einfache Befehl macht diesen Befehl korrekt arbeiten. Zunächst überprüft er Gruppennamen dann pecl Namen im System dann ist es zeigt den Namen der Gruppe, zu der ein pecl gehört. Der folgende Befehl verwendet werden, um diese Funktion zu tun.

.. code-block:: bash

        - show-groups
        Show groups to which a pecl belongs
        example: ptconfigure pecl show-groups --peclname="somename"


Add-to-Gruppen
------------------------

Dies ermöglicht dem Benutzer, eine pecl zu einer Gruppe hinzufügen. Beim Hinzufügen kann es fragt pecl und Gruppennamen. Der Benutzer kann die nach ihrem Wunsch geben.

.. code-block:: bash
   
		ptconfigure pecl add-to-group

Nach der Befehlseingabe ist eine pecl hinzufügen in der Gruppe.

.. code-block:: bash

        - add-to-group
        Add pecl to a group
        example: ptconfigure pecl add-to-group --peclname="somename" --groupname="somegroupname"

Entfernen-von-Gruppe
----------------------------

Dieser Befehl ermöglicht es dem Benutzer, eine pecl von Gruppe zu entfernen. Abnehmbare pecl Name kann in einer einzigen Befehlszeile selbst zu erwähnen.

Der Befehl zum erstellen verwendet wird, ist wie folgt

.. code-block:: bash

		ptconfigure pecl remove-from-group 

Nach Eingang als dem oben genannten Befehl, beginnt es zu entfernen pecl aus Gruppe. Im Falle einer Datei bereits vom pecl die Angabe Meldung erscheint entfernt. Der Befehl und seine Funktion erklärt, mit den Screenshots.

.. code-block:: bash

        - remove-from-group
        Remove pecl from a group
        example: ptconfigure pecl remove-from-group --peclname="somename" --groupname="somegroupname"

Vorteile
----------------

* Nicht Groß- und Kleinschreibung.
* Well-to-do in Ubuntu und CentOS.
* Geringerer Stromverbrauch.
* Erstellen Sie ein neues System pecl
* Nehmen Sie die pecl
* In den Gruppen möglich
* Remove Gruppe ist möglich
* Zeigen Gruppe ist möglich

