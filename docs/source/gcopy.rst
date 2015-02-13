=======
Copy
=======

Zusammenfassung
-----------------

Kopie ist der Befehl in einer Linux-Shell eingegeben, kopieren eine Datei von einem Ort zum anderen, möglicherweise auf einem anderen Dateisystem. Die Originaldatei bleibt unverändert, und die neue Datei möglicherweise das gleiche oder einen anderen Namen. Kopie ist das Kommando, das eine Kopie Ihrer Dateien oder Verzeichnisse erstellt. Die Möglichkeiten, die Dateien unter Linux kopiert werden, hängt von Ihrem Vertrieb und Datei-System. Alle Versionen von Linux konnte Dateien über die Befehlszeile kopieren. Es gibt auch eine Reihe von Datei-Manager, die sowohl textbasierte und GUI, die verwendet werden könnte.

Z. B. angenommen, Sie haben eine Datei mit dem Namen Bild.jpg im Arbeitsverzeichnis und eine Kopie davon Bild-02.jpg aufgerufen werden soll. Würden Sie den Befehl ausführen und die Datei kopiert werden. Hier Bild.jpg ist die Quelle des Kopiervorgangs und Bild-02.jpg ist das Ziel. Heute existieren beide Dateien in Ihrem Arbeitsverzeichnis.

Die Quell- und Ziel-Dateien können auch in verschiedenen Verzeichnissen befinden. Machen Sie zum Beispiel eine Kopie der Datei /home/chuck/pictures/picture.jpg im Verzeichnis/Home/Chuck/Backup. Die Zieldatei wird auch picture.jpg genannt.


Hilfe Befehl
------------------

Dieser Befehl hilft, die Verwendung von Kopie Modul bestimmen. Der Benutzer wird kommen, über den anderen Weg/Format wissen, dieses Modul ausgeführt. Dieser Befehl führt den Endbenutzer, um diesen Befehl zu erfahren. Unten gegeben sind, den Befehl und den Screenshot von der gleichen.

.. code-block:: bash

       cleopatra copy help

Die bildliche Darstellung der Copy-Befehl-Screenshot ist nachfolgend aufgeführt,

.. code-block:: bash


 kevell@corp:/# cleopatra copy help
 ******************************


 This command handles file copying functions.

 Copy, copy

       - put
       Will ask you for details for servers, then copy a file or directory from local to remote
       example: cleopatra copy put
       example: cleopatra copy put --yes --source="/tmp/file" --target="/home/user/file"

 ------------------------------
 End Help
 ******************************

Setzen
----------

Wenn der Benutzer zum Kopieren einer Datei in unsere Quelle zu anderen Ziel muss, die unten mit dem Befehl führt den Prozess.

.. code-block:: bash

            cleopatra copy put

Das System fragt nach Quellpfad der Datei und Zieldateipfad.

.. code-block:: bash

 kevell@corp:/# cleopatra copy put
 Copy files? (Y/N)
 Y
 Enter source file path
 /kevell.html
 Enter target file path
 /home/desktop
 [Pharaoh Logging] [Copy] Executing cp -r /kevell.html /home/desktop
 ******************************


 Copy Result: Success
 ------------------------------
 Copy Finished
 ******************************


Es gibt eine weitere Möglichkeit, worin Sie den Quell- und Ziel-Pfad in der Befehlszeile geben können.


.. code-block:: bash


 kevell@corp:/# cleopatra copy put --yes --source="/kevell.html" --target="/opt"

 [Pharaoh Logging] [Copy] Executing cp -r /kevell.html /opt
 ******************************


 Copy Result: Success
 ------------------------------
 Copy Finished
 ******************************

Alternative Parameter
------------------------------

Es gibt zwei alternative Parameter, die in der Befehlszeile Copy, Kopie verwendet werden kann.

ZB: Cleopatra Kopie ablegen / Cleopatra kopieren helfen

Vorteile
------------

* Dieser Befehl können Sie eine Kopie Ihrer Dateien oder Verzeichnisse erstellen.
* Kopieren Sie eine Datei oder ein Verzeichnis von Quelle zum Zielort mit einem Befehl
* Wenn Sie eine Datei aus einem Ordner zu einem anderen mit dem gleichen Namen kopieren möchten, reicht nur der Namen des Ziel-Verzeichnisses
* Ein Verzeichnis (und alle seine Inhalte) können zum Ziel die rekursive Option-r von Quelle kopiert werden
 

