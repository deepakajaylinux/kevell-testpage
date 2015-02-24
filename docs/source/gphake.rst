==============
Phake
==============

Zusammenfassung
------------------------

Phake ist eine spöttische Framework für PHP. Es ermöglicht die Erstellung von Objekten, die ein reales Objekt in einer vorhersagbaren und gesteuerten Weise zu imitieren. Dies ermöglicht Ihnen, externe Methodenaufrufe von Ihrem zu testende System (SUT) gemacht als eine weitere Form der Eingabe, um Ihre SUT und Ausgabe von Ihrem SUT zu behandeln. Dies wird durch Anstoßen Methoden, indirekte Eingabe liefern in Ihre Test- und durch Überprüfung der Parameter, die Methoden, die indirekte Ausgabe von Ihrem Test erhalten getan.

Hilfe Befehl
----------------------

Diese Funktion dient, um die Verwendung von Phake Modul bestimmen. Der Benutzer wird kommen, um über die verschiedenen Möglichkeiten / Format um dieses Modul ausführen kennen. Dieser Befehl leitet den Anwender, um den Zweck dieses Befehls kennen. Da unten sind die Kommando- und der Screenshot der gleiche.

.. code-block:: bash
        
	        ptconfigure Phake help


 kevell@corp:/# ptconfigure Phake help
 ******************************


  This command allows you to install or update Phake.

  Phake, phake

        - install
        Installs the latest version of phake
        example: ptconfigure phake install

        - ensure
        Installs the latest version of phake, only if a version is not installed
        example: ptconfigure phake ensure

 ------------------------------
 End Help
 ******************************

Installation
----------------

Wenn der Benutzer Phake im Rechner installieren muss, wird der unten angegebenen Befehl den Prozess der Installation ausführen

.. code-block:: bash
         
   	        ptconfigure Phake install
 
Das System fragen Sie nach dem Verzeichnisnamen, wenn Sie um Ihre PATH können Sie Ihren Weg zu definieren will. Definieren Sie Ihren Weg, gefolgt von "/" Symbol. Drücken Sie die Eingabetaste, wenn es keine Änderungen durchgeführt werden.

"What is the program data directory? Found "/opt/phake" - use this?

Dann wird das System fragen, für die Ausführung Verzeichnisnamen, wenn Sie um Ihre PATH können Sie Ihren Weg zu definieren will. Definieren Sie Ihren Weg, gefolgt von "/" Symbol. Drücken Sie die Eingabetaste, wenn es keine Änderungen durchgeführt werden

"What is the program executer directory? Found "/usr/bin" - Use this? "

Der folgende Screenshot zeigt die gleiche.

.. code-block:: bash

 kevell@corp:/# ptconfigure Phake install
 Install Phake ? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *          Phake         *
 *******************************
 What is the program data directory? Found "/opt/phake" - use this? (Enter nothing for yes, no end slash)

 What is the program executor directory? Found "/usr/bin" - use this? (Enter nothing for yes, No Trailing Slash)

 git clone 'http://github.com/jaz303/phake.git'  /tmp/phake/phakeCloning into '/tmp/phake/phake'...
 remote: Counting objects: 552, done.
 remote: Total 552 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (552/552), 91.36 KiB | 76.00 KiB/s, done.
 Resolving deltas: 100% (314/314), done.
 Checking connectivity... done.
 Program Data folder populated
 Program Executor Deleted if existed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 Phake: Success
 ------------------------------
 Installer Finished
 ******************************                          



Options
-----------

.. cssclass:: table-bordered




 +---------------------------+-----------------------------------------+------------+------------------------------------------+
 | Parameter                 | Alternative Parameter                   | Optionen   | Kommentare                               |
 +===========================+=========================================+============+==========================================+
 |ptconfigure Phake Install  | Eine der beiden alternativen Parameter  | Y          | Ponce der Benutzer bietet die            |
 |                           | kann in Befehls verwendet werden Phake, |            | Möglichkeit, System startet              |
 |                           | phake eg: ptconfigure phake Install     |            | Installation                             |
 +---------------------------+-----------------------------------------+------------+------------------------------------------+
 |ptconfigure Phake Install  | Eine der beiden alternativen Parameter  | N          | Sobald der Benutzer bietet die           |
 |                           | kann in Befehls verwendet werden Phake, |            | Möglichkeit, stoppt System-Installation  |
 |                           | phake eg: ptconfigure phake Install|    |            |                                          |
 +---------------------------+-----------------------------------------+------------+------------------------------------------+

Vorteile
--------------

* Phake ist eine große spöttische Bibliothek und lässt sich einfach in PHPUnit integriert werden.
* Die neuen Ansätze in Prototypen Mocks und Stubs und die Trennung zwischen Anstoßen und Verifikationsphasen ist sehr erfrischend und leicht zu
  verwenden.
