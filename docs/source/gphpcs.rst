==========
PHPCS
==========

Zusammenfassung
------------------------

Dieses Modul hilft bei der Installation von PHP cs von GC Repo. Bei der Installation, holt dieses Modul die neueste Version. Der Benutzer kann den Speicherort für die Programmdatenverzeichnis und Vollstrecker Verzeichnis angeben. Schließlich Ergebnisse sind klar ausgewiesen.

Hilfe Befehl
-------------

Der Befehl help führt die Benutzer über den Zweck und als auch über die Möglichkeiten, die in der PHP-cs-Modul enthalten sind. Es beschreibt auch die Syntax für die Installation von PHP-cs. Der Befehl help für php cs ist unten angegeben.

.. code-block:: bash

	ptconfigure PHPCS help

Die Syntax für die Deklaration den Befehl help ist nicht case sensitive was ein zusätzlicher Vorteil ist. Der folgende Screenshot visualisieren Sie den Befehl help unter PHPCS.

.. code-block:: bash


 kevell@corp:/# ptconfigure PHPCS help 
 ****************************** 

  This command allows you to install PHPCS from a GC Repo. 

  PHPCS 

        - install 
        Installs the latest version of PHPCS 
        example: ptconfigure phpcs install 

        - uninstall 
        Uninstalls the latest version of PHPCS 
        example: ptconfigure phpcs uninstall 

 ------------------------------ 
 End Help 
 ****************************** 


Installation
-------------

Installieren des PHP CS ist einfacher, indem Sie den folgenden Befehl ein, wie gezeigt:

.. code-block:: bash
	
	ptconfigure PHPCS install

Nach der Eingabe des Befehls über die folgenden Vorgänge, wie gezeigt in der Tabellenform auf.

.. cssclass:: table-bordered

 +-----------------------+-------------+---------------------------------------------------------------------+
 | Paramaters            | Optionen    |  Kommentare                                                         |
 +=======================+=============+=====================================================================+
 |Install PHP Code       | Y(Yes)      | Wenn der Benutzer wünschen, den Installationsprozess können         |
 |Sniffer ? (Y/N)        |             | sie Eingang als Y. gehen                                            |
 +-----------------------+-------------+---------------------------------------------------------------------+
 |Install PHP Code       | N(No)       | Wenn der Benutzer wünschen, den Installationsprozess können         |
 |Sniffer ? (Y/N)        |             | sie Eingang als N. beenden|                                         |
 +-----------------------+-------------+---------------------------------------------------------------------+


Wenn der Benutzer den Installationsprozeß schreitet die folgenden Vorgänge stattfindet, wie in der Form einer Tabelle.

.. cssclass:: table-bordered

 +-----------------------+--------------------------+--------------+-----------------------------------------------------+
 | Paramaters            | Weg                      | Optionen     | Kommentare                                          |
 +=======================+==========================+==============+=====================================================+
 |Program data           | opt/phpcs (entsprechend  | Yes          | Wenn der Benutzer der Installation fortzufahren     |
 |directory(Default)     | Modul)”                  |              | mit dem Standard-Programm-Datenverzeichnis können   |
 |                       |                          |              | sie Eingang als Ja                                  |
 +-----------------------+--------------------------+--------------+-----------------------------------------------------+
 |Program data directory | User specific            | No(End       | Wenn der Benutzer mit ihren eigenen                 |
 |                       |                          | Slash)       | Programmdatenverzeichnis fortfahren möchten, können |
 |                       |                          |              | sie Eingang als N, und in die Hand geben sie Ort    |
 |                       |                          |              | besitzen.                                           |
 +-----------------------+--------------------------+--------------+-----------------------------------------------------+
 |Program executor       | “/usr/bin”               | Yes          | Wenn der Benutzer die Installation mit dem          |
 |directory (Default)    |                          |              | Standardprogramm Testamentsvollstrecker Verzeichnis | 
 |                       |                          |              | gehen sie eingeben kann als Ja                      |
 +-----------------------+--------------------------+--------------+-----------------------------------------------------+
 |Program executor       | User specific            | No (End      | Wenn der Benutzer mit ihren eigenen                 |
 |directory              |                          | Slash)       | Programmausführungs Verzeichnis fortfahren möchten, |
 |                       |                          |              | können sie Eingang als N, und in die Hand geben     |
 |                       |                          |              | sie Ort besitzen.|                                  |
 +-----------------------+--------------------------+--------------+-----------------------------------------------------+


Nach diesen Verfahren in der Form einer Tabelle , die Ergebnisse deutlich zusammen mit dem Status berichtet . Der folgende Screenshot erklärt grafisch über den Prozess in die Installation und Deinstallation von PHPCS beteiligt.


.. code-block:: bash


 kevell@corp:/# ptconfigure PHPCS install 
 Install PHP Code Sniffer? (Y/N) 
 y 
 ******************************* 
 *        Pharaoh Tools        * 
 *         PHP CSniffer        * 
 ******************************* 
 Creating /tmp/ptconfigure-temp-script-74085209498.sh 
 chmod 755 /tmp/ptconfigure-temp-script-74085209498.sh 2>/dev/null 
 Changing /tmp/ptconfigure-temp-script-74085209498.sh Permissions 
 Executing /tmp/ptconfigure-temp-script-74085209498.sh 
 Reading package lists... 
 Building dependency tree... 
 Reading state information... 
 php-pear is already the newest version. 
 0 upgraded, 0 newly installed, 0 to remove and 3 not upgraded. 
 downloading PHP_CodeSniffer-2.3.0.tgz ... 
 Starting to download PHP_CodeSniffer-2.3.0.tgz (464,453 bytes) 
 .............................................................................................done: 464,453 bytes 
 install ok: channel://pear.php.net/PHP_CodeSniffer-2.3.0 
 Temp File /tmp/ptconfigure-temp-script-74085209498.sh Removed 
 ... All done! 
 ******************************* 
 Thanks for installing , visit www.pharaohtools.com for more 
 ****************************** 


 Single App Installer: 
 -------------------------------------------- 
 PHPCS: Success 
 ------------------------------ 
 Installer Finished 
 ****************************** 


.. code-block:: bash


 kevell@corp:/# ptconfigure PHPCS uninstall 
 Uninstall PHP Code Sniffer? (Y/N) 
 y 
 ******************************* 
 *        Pharaoh Tools        * 
 *         PHP CSniffer        * 
 ******************************* 
 Creating /tmp/ptconfigure-temp-script-50071430908.sh 
 chmod 755 /tmp/ptconfigure-temp-script-50071430908.sh 2>/dev/null 
 Changing /tmp/ptconfigure-temp-script-50071430908.sh Permissions 
 Executing /tmp/ptconfigure-temp-script-50071430908.sh 
 uninstall ok: channel://pear.php.net/PHP_CodeSniffer-2.3.0 
 Temp File /tmp/ptconfigure-temp-script-50071430908.sh Removed 
 ... All done! 
 ******************************* 
 Thanks for installing , visit www.pharaohtools.com for more 
 ****************************** 


 Single App Uninstaller: 
 ------------------------------ 
 PHPCS: Success 
 ------------------------------ 
 Installer Finished 
 ******************************  


Vorteile
-----------

* Dieses Modul ermöglicht den Anwender bei der Installation von PHP CS mit der aktualisierten Version.
* Der Benutzer kann seinen eigenen Weg für die Programmdatenverzeichnis und Vollstrecker wählen
* Die Parameter Deklaration der Hilfe verwendet und Anlagen muss nicht beachtet werden, die aufgenommen wird, während Vorteil im Vergleich zu 
  anderen.


