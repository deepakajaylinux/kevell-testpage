==========
IntelliJ
==========

Zusammenfassung
-----------------------

Dieses Modul beschleunigt die Installation von IntelliJ, die einen Jet Brains IDE ist mit einer aktuellen Version. Die IntelliJ-Plattform ist eine Plattform für den Aufbau smart, sprachsensitiven IDEs mit einem umfassenden Satz von Komponenten, die das virtuelle Dateisystem, UI-Framework, Text-Editor, lexing, Parsing, abstrakte Syntaxbäume und andere sprachspezifische Infrastruktur, Rahmenbedingungen für die Umsetzung beinhaltet Navigation, Code-Vervollständigung, Inspektionen, Absichten, Refactoring, Versionskontrolle Integration, Debugger Rahmen, grafische Unit-Test-Läufer.

Die IntelliJ-Plattform Sourcecode wird von der Apache-2.0-Lizenz abgedeckt. Das heißt, Sie können Open Source und kommerzielle Produkte auf der Plattform, ohne dass Lizenzgebühren zahlen zu JetBrains bauen. Lassen Sie uns über die Funktionalitäten der IntelliJ unter diesem Modul sehen.

Hilfe Befehl
-----------------

Der Befehl help führt den Anwender über den Zweck und als auch über die Möglichkeiten, die in der IntelliJ-Modul enthalten sind. Es listet einige der alternativen Parameter IntelliJ-Modul. Es beschreibt auch die Syntax für die Installation des IntelliJ Moduls. Der Befehl help für IntelliJ Modul wird wie unten dargestellt.

.. code-block:: bash

 		ptconfigure IntelliJ help

Die Syntax für die Deklaration den Befehl help ist nicht case sensitive was ein zusätzlicher Vorteil ist. Der folgende Screenshot visualisieren Sie den Befehl help unter IntelliJ.

.. code-block:: bash



 kevell@corp:/# ptconfigure IntelliJ help
 ******************************


  This command allows you to install Intellij, the JetBrains IDE

  IntelliJ, intellij

        - install
        Installs the latest version of Developer Tools
        example: ptconfigure gittools install

 ------------------------------
 End Help
 ******************************

Installation
---------------

Der Befehl zum Installieren der JRush zum Benutzer Maschine verwendet wird unten gezeigt.

.. code-block:: bash

		ptconfigure IntelliJ install

Nach der Eingabe des Befehls vor, tritt die folgenden Funktionen:

* Es fordert den Benutzer auf die IntelliJ Version geben.
* Stellt die Verfügbarkeit von Modulen und nicht überprüft die Version.
* Wenn das Modul nicht in der Benutzer-Maschine vorhanden ist, beginnt es installieren.
* Während der Installation wird der Benutzer aufgefordert, um in den Java installieren Directory.

Schließlich ist die Installation von IntelliJ abgeschlossen wird. Der Screenshot siehe unten zeigt den Prozess der Installation von IntelliJ

.. code-block:: bash



 kevell@corp:/# ptconfigure intellij install 

 Install IntelliJ IDE? (Y/N) 
 y 
 ******************************* 
 *        Pharaoh Tools        * 
 *         IntelliJ IDE        * 
 ******************************* 
 Enter IntelliJ Version 
 (0) 12.1 
 0 
 [Pharaoh Logging] Ensure module install is not checking versions 
 [Pharaoh Logging] Module Java reports itself as Installed 
 [Pharaoh Logging] Not installing as already installed 
 Creating /tmp/ptconfigure-temp-script-88128552364.sh 
 chmod 755 /tmp/ptconfigure-temp-script-88128552364.sh 2>/dev/null 
 Changing /tmp/ptconfigure-temp-script-88128552364.sh Permissions 
 Executing /tmp/ptconfigure-temp-script-88128552364.sh 
 Cloning into 'intellij'... 
 remote: Counting objects: 1026, done. 
 remote: Total 1026 (delta 0), reused 0 (delta 0), pack-reused 1026 
 Receiving objects: 100% (1026/1026), 205.06 MiB | 138.00 KiB/s, done. 
 Resolving deltas: 100% (60/60), done. 
 Checking connectivity... done. 
 Checking out files: 100% (744/744), done. 
 Temp File /tmp/ptconfigure-temp-script-88128552364.sh Removed 
 Program Executor Deleted if existed 
 ... All done! 
 ******************************* 
 Thanks for installing , visit www.pharaohtools.com for more 
 ****************************** 


 Single App Installer: 
 -------------------------------------------- 
 IntelliJ: Success 
 ------------------------------ 
 Installer Finished 
 ****************************** 


Parameter
----------------------------

Anstelle von IntelliJ können wir, intellij verwenden

Eg: ptconfigure invoke get/ ptconfigure invoke get

Vorteile
------------


* Dieses Modul erleichtert dem Anwender bei der Installation von IntelliJ mit der neuesten Version.
* Die Parameter Deklaration der Hilfe verwendet und Anlagen muss nicht beachtet werden, die aufgenommen wird, während Vorteil im Vergleich zu 
  anderen.
* Es ist gut-to-do in beiden Cent OS und als auch in Ubuntu.
* Die erforderlichen Status eindeutig bei der Installation überwacht.
* Während der Installation kann der Benutzer geben Sie die gewünschte Version und als auch Java-Installationsverzeichnis.

