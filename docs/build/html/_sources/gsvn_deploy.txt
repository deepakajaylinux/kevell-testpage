=======
SVN
=======

Zusammenfassung
-----------------------

Dieses Modul unterstützt die Anwender bei der Handhabung Kasse Funktionen. Apache Subversion (oft abgekürzt SVN, hinter den Befehlen svn) ist ein Software-Versionierung und Versionskontrollsystem verteilt als freie Software unter der Apache-Lizenz. [1] Entwickler benutzen Subversion auf aktuelle und frühere Versionen von Dateien wie Quellcode zu erhalten, Web-Seiten und Dokumentation. Ziel ist es, ein weitgehend kompatibel Nachfolger des weit verbreiteten Concurrent Versions System (CVS) sein. Wir wollen sehen, wie dieses Modul können im Umgang mit Kassenfunktionen.

Hilfe Befehl
---------------------

Der Befehl help führt den Anwender über den Zweck und als auch über die Möglichkeiten, die in der SVN enthalten sind. Es listet einige der alternativen Parameter SVN. Es beschreibt auch die Syntax für die Verwendung der Kassenfunktionen. Der Befehl help zur SVN-Modul wird wie unten dargestellt.

.. code-block:: bash

	ptdeploy svn help

Die Syntax für die Deklaration den Befehl help ist nicht case sensitive was ein zusätzlicher Vorteil ist. Der folgende Screenshot visualisieren Sie den Befehl help unter SVN.

.. code-block:: bash

 kevell@corp:/# ptdeploy svn help
 ******************************


  This command is part of Default Modules and handles Checkout Functions.

  Checkout, checkout, co

          - perform a checkout into configured projects folder. If you don't want to specify target dir but do want
          to specify a branch, then enter the text "none" as that parameter.
          example: ptdeploy svn co https://svnhub.com/phpengine/yourmum {optional target dir} {optional branch}
          example: ptdeploy svn co https://svnhub.com/phpengine/yourmum none {optional branch}

 ------------------------------
 End Help
 ******************************

Wie man die Kasse Funktionen verwenden
-------------------------------------------

Die Syntax für das Check-out-Funktionen unter svn ist unten angegeben.

.. code-block:: bash

	ptdeploy svn co https: // svnhub.com/ phpengine/yourmum



Nach der Eingabe des Befehls oben angegeben, beginnt die Ausführung der Kasse Funktion wie in der folgenden Tabelle beschrieben,

.. cssclass:: table-bordered

 +------------------------------+------------------------------------+-------------+-----------------------------------------------+
 | Parameters                   | Alternative Parameters             | Options     | Kommentare                                    |
 +==============================+====================================+=============+===============================================+
 |Perform a clone/download      | anstelle von co, Die wir verwenden | Y(Yes)      | Wenn der Benutzer benötigt, um einen Klon /   |
 |of files? (Y/N)               | können checkout, Checkout also.    |             | Download von Dateien, die sie eingeben        |
 |                              |                                    |             | können, wie Y. führen                         |
 +------------------------------+------------------------------------+-------------+-----------------------------------------------+
 |Perform a clone/download of   | anstelle von co, Die wir verwenden | N(No)       | Wenn der Benutzer nicht in der Notwendigkeit, |
 |files? (Y/N)                  | können checkout, Checkout also.    |             | einen Klon / Herunterladen von Dateien führen |
 |                              |                                    |             | sie eingeben kann als N.|                     |
 +------------------------------+------------------------------------+-------------+-----------------------------------------------+


Wenn der Benutzer geht der Kasse Funktion durch Eingabe als Y sind die folgenden Schritte erforderlich, wie unten beschrieben.

Schritt 1:

Auch ändern die Berechtigungen / Eigentümer? (Y / N)

Der Benutzer muss die Eingabe wie Y oder N, abhängig von ihrer Bereitschaft in Ändern von Berechtigungen / Eigentümer.

Schritt 2:

Welche Benutzer Apache Web Server als?

Der Benutzer muss die Eingabe des Namens von Benutzer, der den Apache-Web-Server.

Schritt 3:

Es geht um den Prozess der Veränderung Ordner-Berechtigungen und Ordner Besitzer.

Der folgende Screenshot zeigt bildlich über den Prozess und die Arbeitsweise überprüfen Funktionen.


.. code-block:: bash

 kevell@corp:/# ptdeploy  svn co --repository-url="http://core.svn.wordpress.org/trunk" --custom-clone-dir="/opt/"
 Perform a clone/download of files? (Y/N) 
 y
 Also change permissions/owner? (Y/N) 
 n
 View Template SvnView.tpl.php for  Not Found




Vorteile
-----------

* Es ist gut-to-do sowohl ubuntu und als auch in Cent OS.
* Die in der Erklärung verwendeten Parameter wird nicht zwischen Groß- und Kleinschreibung.
* Der Benutzer durchführen und die Kassenfunktionen überwachen, indem Sie diese SVN kann.

