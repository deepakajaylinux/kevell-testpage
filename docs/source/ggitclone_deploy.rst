==========
GitClone
==========

Zusammenfassung
------------------------

Das ultimative Ziel dieses Moduls ist es, das Kontrollgriff aus Funktionen. Es kann die Check-Out-Funktionen in den Projektordner des führen
Benutzer.

Die Arbeits Natur dieses Modul beinhaltet Klonen eines Repository in ein neu erstelltes Verzeichnis erstellt Remote-Tracking-Zweige für jeden Zweig im Repository geklont und erstellt, überprüft eine erste Zweig, der von derzeit aktiven Zweig der geklonte Repository gegabelt ist.

Lassen Sie uns über sehen, wie das Modul können die Benutzer im Umgang mit dem Check-out-Funktionen, und auch, wie Sie dieses Modul aus den anstehenden Themen zu verwenden.


Hilfe Befehl
-------------------

Der Befehl help ist eine kurze Anleitung. Sie weist auf die Hauptfunktion dieses Moduls auflistet outs die alternativen Parameter, die in der Erklärung verwendet werden kann, und erklärt auch, über die Syntax und möglichen Optionen für die Verwendung der Check-out-Funktionen unter einer einzigen Option mithilfe Befehl help, wie unten gezeigt,

.. code-block:: bash

	ptdeploy GitClone help


Die Syntax für die Deklaration den Befehl help ist nicht case sensitive was ein zusätzlicher Vorteil ist. Der folgende Screenshot visualisieren Sie den Befehl help unter git clone.

.. code-block:: bash

 kevell@corp:/# ptdeploy GitClone help
 ******************************

 Dieser Befehl ist Teil der Standard-Module und Griffe Kasse Funktionen.
  clone, co

          - perform a checkout into configured projects folder. If you don't want to specify target dir but do want
          to specify a branch, then enter the text "none" as that parameter.
          example: ptdeploy git co https://github.com/phpengine/yourmum {optional target dir} {optional branch}
          example: ptdeploy git co https://github.com/phpengine/yourmum none {optional branch}

 ------------------------------
 End Help
 ******************************


How to Use the checkout functions
-------------------------------------------

The syntax for using the check out functions under git clone is given below.

.. code-block:: bash

	ptdeploy git co https: // github.com/ phpengine/yourmum

Nach der Eingabe des Befehls oben angegeben, beginnt die Ausführung der Kasse Funktion wie in der folgenden Tabelle beschrieben,

.. cssclass:: table-bordered

 +---------------------------+----------------------------------+----------+-----------------------------------------------------+
 | Parameters                | Alternative Parameters           | Options  | Kommentare                                          |
 +===========================+==================================+==========+=====================================================+
 |Perform a clone/download   | Statt,co, wir verwenden können,  | Y(Yes)   | Wenn der Benutzer benötigt, um einen Klon /         |
 |of files? (Y/N)            | checkout, Checkout auch noch     |          | Download von Dateien, die sie eingeben können,      |
 |                           |                                  |          | wie Y. führen                                       |
 +---------------------------+----------------------------------+----------+-----------------------------------------------------+
 |Perform a clone/download   | Statt,co, wir verwenden können,  | N(No)    | Wenn der Benutzer nicht brauchen, um einen Klon /   |
 |of files? (Y/N)            | checkout, Checkout auch noch     |          | Download von Dateien durchführen können sie als N.| |
 +---------------------------+----------------------------------+----------+-----------------------------------------------------+


Der folgende Screenshot zeigt bildlich über den Prozess und die Arbeitsweise überprüfen Funktionen.

.. code-block:: bash


Vorteile
-----------

* Es ist gut-to-do sowohl ubuntu und als auch in Cent OS.
* Die in der Erklärung verwendeten Parameter wird nicht zwischen Groß- und Kleinschreibung.
* Der Benutzer durchführen und die Kassenfunktionen unter git clone überwachen können.
* Während der Durchführung der Check-out-Funktionen kann der Benutzer das Zielverzeichnis angeben, müssen die Ebene angegeben.

