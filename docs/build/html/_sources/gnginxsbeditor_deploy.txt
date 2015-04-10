===============
NginxSBEditor
===============

Zusammenfassung
---------------

Dieses Modul ist ein schönes Teil der Standard-Module und Griffe Nginx ServerBlocks Funktionen. Lassen Sie uns über die Methoden für die Verwendung dieser und auch über die Aufgaben im Rahmen dieser nginx Redakteur kommenden Themen zu sehen.

Hilfe Befehl
---------------------

Der Befehl help umhüllt alle notwendigen Informationen über NginxSBEditor wie auch vorrangig, die Liste der alternativen Parameter, die in der Erklärung verwendet werden kann, was sind primäre Funktion NginxSBEditor (Ex: hinzufügen, entfernen, Liste, aktiviert, deaktiviert), und auch die Syntax für die Deklaration diese interessante Funktionen. Der folgende Befehl ist für Hilfe-Option erklärt unter NginxSBEditor verwendet,

.. code-block:: bash

	ptdeploy NginxSBEditor help


Der folgende Screenshot zeigt bildhaft über die Arbeit der Befehl help.

.. code-block:: bash

 kevell@corp:/# ptdeploy NginxSBEditor help
 ******************************


  This command is part of Default Modules and handles Nginx ServerBlocks Functions.

  NginxSBEditor, nginx-sb-editor, nginxsbe

          - add
          create a Server Block
          example: ptdeploy nginxsbe add
          sb-docroot
          sb-url
          sb-ip-port

          - rm
          remove a Server Block
          example: ptdeploy nginxsbe rm

          - list
          List current Server Blocks
          example: ptdeploy nginxsbe list

          - enable
          enable a Server Block
          example: ptdeploy nginxsbe enable

          - disable
          disable a Server Block
          example: ptdeploy nginxsbe disable

 ------------------------------
 End Help
 ******************************

So verwenden
---------------

Wie dargestellt und in der obigen Befehl help erläutert, NginxSBEditor, hat die folgenden Funktionen,

* Add
* Remove
* List
* Enable
* Disable

Lassen Sie uns sehen, wie man diese interessante Funktionen unter NginxSBEditor verwenden.

Add
--------------

Die Rolle dieser Funktion ist zum Erstellen / fügen Sie einen neuen Server-Block. Der Befehl und Bearbeitung von Funktionen hinzuzufügen ist unten dargestellt,

.. code-block:: bash

	ptdeploy NginxSBEditor add

Nach der Eingabe des Befehls oben angegeben, wird die Arbeitsweise dieser Zusatzfunktion unten,


.. cssclass:: table-bordered

 +--------------------------------+--------------------------------------+------------+------------------------------------------------+
 | Parameters                     | Alternative Parameters               | Options    | Kommentare                                     |
 +================================+======================================+============+================================================+
 |Do you want to add a            | Statt NginxSBEditor wir              | Y(Yes)     | Wenn der Benutzer benötigt, um einen neuen     |
 |ServerBlock? (Y/N)              | nginx-sb-Editor, nginxsbe auch       |            | Server Block sie eingeben können, wie Y.       |
 |                                | verwenden können.                    |            | hinzufügen                                     |
 +--------------------------------+--------------------------------------+------------+------------------------------------------------+
 |Do you want to add a            | Statt NginxSBEditor wir              | N(No)      | Wenn der Benutzer nicht in der Notwendigkeit,  |
 |ServerBlock? (Y/N)              | nginx-sb-Editor, nginxsbe auch       |            | einen neuen Server Block sie eingeben kann     |
 |                                | verwenden können.                    |            | als N auf|                                     |
 +--------------------------------+--------------------------------------+------------+------------------------------------------------+


Wenn der Benutzer Erlös Hinzufügen der Server Blöcke während der Zugabe Verfahren die folgenden Schritte beteiligt sind.

Schritt 1:

Was ist Document Root?

Der Benutzer muss das Root, wenn sie nicht wollen, um mit der Standard fortzufahren.

Schritt 2:

Welche URL haben Sie als Servernamen hinzufügen?

Der Benutzer muss die URL, die angeblich hinzuzufügen ist anzugeben.

Schritt 3:

Was IP? Port festgelegt werden sollten?

Der Benutzer muss die IP, wenn sie nicht wollen, um mit der Standard fortzufahren.

Schritt 4:

Was ist Ihre ServerBlock Template-Verzeichnis?

Der Benutzer muss das Verzeichnis, wenn sie nicht wollen, um mit der Standard fortzufahren.

Schritt 5:

Bitte überprüfen Sie die ServerBlock


Der Benutzer muss überprüfen Sie die Ausgabe Anzeige der Server-Block, der hinzugefügt wird, und zu gewährleisten.

Schritt 6:

Ist das okay? (Y / N)

Wenn der Benutzer sind mit dem Ergebnis erzeugt glücklich, sie können als Y-Eingang anderes N.

Schritt 7:

Was ist Ihre ServerBlock Verzeichnis?

Der Benutzer muss das Verzeichnis.

Schritt 8:

Möchten Sie einen Server-Block aktivieren? (Y / N)

Der Benutzer muss die Eingabe wie Ja oder Nein, je nach ihren Bedürfnissen.

Schritt 9:

Was ist Ihre Aktiviert Symlink ServerBlock Verzeichnis.

Wenn ein Server-Block aktiviert ist, muss der Benutzer seine Verzeichnis angeben.

Der folgende Screenshot zeigt die visuell oben erläuterten Verfahren.


.. code-block:: bash

 kevell@corp:/# ptdeploy nginxsbe add
 Do you want to add a ServerBlock? (Y/N) 
 Y
 What's the document root? Enter nothing for /
 /root/Nginx
 What URL do you want to add as server name?
 www.ngx.com
 What IP:Port should be set? Enter nothing for 127.0.0.1:80

 What is your ServerBlock Template directory? Enter nothing for default templates
 /root/Nginxdir
 Please Choose ServerBlock Template: 
 --- Default Server Block Templates: ---
 (0) docroot-no-suffix
 (1) docroot-src-sfx
 (2) docroot-web-suffix
 (3) docroot-www-suffix
 (4) docroot-docroot-suffix

 3
 Please check ServerBlock: server {
        listen   127.0.0.1:80 ; ## listen for ipv4; this line is default and implied
        #listen   [::]:80 default ipv6only=on; ## listen for ipv6

        root /root/Nginx/www ;
        index index.html index.htm index.php;

        # Make site accessible from http://localhost/
        server_name www.ngx.com ;

        # pass the PHP scripts to FastCGI server listening on 127.0.0.1:9000
        #
        location ~ \.php$ {
                try_files $uri =404;
                fastcgi_split_path_info ^(.+\.php)(/.+)$;
                fastcgi_pass 127.0.0.1:9000;
                fastcgi_index index.php;
                include fastcgi_params;
        }

 }

 Is this Okay? (Y/N) 
 Y
 What is your ServerBlock directory?
 /root/Nginxdir
 Do you want to enable a ServerBlock? (Y/N) 
 Y
 What is your Enabled Symlink ServerBlock directory?
 /home/Nginxsymlink
 Server Block Enabled Symlink Created
 ******************************
 

 1ServerBlock Creator Finished
 ******************************



Remove
----------

Das Entfernen Funktion wird zum Entfernen der unerwünschten Server-Blöcken. Dies kann mit dem Befehl unten angegeben durchgeführt werden,

.. code-block:: bash

	ptdeploy NginxSBEditor rm

Nach der Eingabe des Befehls über das folgende Verfahren zur Löschung beteiligt, wie in der Tabelle dargestellt

.. cssclass:: table-bordered


 +-----------------------------+-------------------------------------------+----------+-------------------------------------------------+
 | Parameters                  | Alternative Parameters                    | Options  | Kommentare                                      |
 +=============================+===========================================+==========+=================================================+
 |Do you want to delete        | Statt NginxSBEditor wir nginx-sb-Editor,  | Y(Yes)   | Wenn der Benutzer auf den Server blockieren     |
 |ServerBlock/s? (Y/N)         | nginxsbe auch verwenden können.           |          | sie eingeben können, wie Y. löschen muss        |
 +-----------------------------+-------------------------------------------+----------+-------------------------------------------------+
 |Do you want to add a         | Statt NginxSBEditor wir nginx-sb-Editor,  | N(No)    | Wenn der Benutzer nicht in der Notwendigkeit,   |
 |ServerBlock/s? (Y/N)         | nginxsbe auch verwenden können.           |          | den Server-Block können sie als Eingangs N      |
 |                             |                                           |          | löschen|                                        |
 +-----------------------------+-------------------------------------------+----------+-------------------------------------------------+
 

Wenn der Benutzer Erlös Löschen der Serverblöcke bei diesem Vorgang die folgenden Schritte beteiligt.

Schritt 1:

Löschen ServerBlock

Was ist Ihre ServerBlock Verzeichnis?

Der Benutzer muss das Verzeichnis angeben.

Schritt 2:

Bitte wählen Sie ServerBlock

--Alle Server Blocks: ---

(0) www.ngn.com

(1) www.ngx.com

(2) www.nx.com

Der Benutzer muss, um die Werte von 0 bis 2 in Abhängigkeit von deren Anforderungen angeben.

Schritt 3:

!! Sicher? Definitiv ServerBlock löschen? (Y / N) !!

Der Benutzer muss angeben, Ja oder Nein, je nach ihren Bedürfnissen.

Schritt 4:

Möchten Sie einen ServerBlock deaktivieren? (Y / N)

Der Benutzer muss angeben, Ja oder Nein, je nach ihren Bedürfnissen.

Schritt 5:

Was ist Ihre Aktiviert Symlink ServerBlock Verzeichnis?

Der Benutzer muss das Verzeichnis angeben.

Der folgende Screenshot zeigt visuell über den Prozess der Löschung.

.. code-block:: bash

 kevell@corp:/# ptdeploy nginxsbe rm
 Do you want to delete ServerBlock/s? (Y/N) 
 Y
 Deleting ServerBlock
 What is your ServerBlock directory?
 /root/Nginxdir
 Please Choose ServerBlock:
 ---All Server Blocks: ---
 (0) www.ngn.com
 (1) www.ngx.com
 (2) www.nx.com

 2
 !! Sure? Definitely delete ServerBlock? (Y/N) !!
 Y
 Do you want to disable a ServerBlock? (Y/N) 
 Y
 What is your Enabled Symlink ServerBlock directory?
 /root/home/Nginxsymlink
 Server Block www.nx.com Disabled if existed
 Server Block www.nx.com Deleted if existed
 *******************************


 1ServerBlock Creator Finished
 ******************************

List
-------

Die Funktion der Liste Option ist die Bereitstellung der aktuellen installierten Server blockiert. Der Befehl für die Liste verwendet, ist unten angegeben,

.. code-block:: bash

	ptdeploy NginxSBEditor list

Nach der Eingabe des Befehls über die folgenden Verfahren in der Liste die Option beteiligt.

Schritt 1:

Was ist Ihre ServerBlock Verzeichnis?

Der Benutzer muss das Verzeichnis angeben.

Schritt 2:

Was ist Ihre Aktiviert Symlink ServerBlock Verzeichnis?

Der Benutzer muss das Verzeichnis angeben.

Nach diesen Schritten sind er Liste der aktuell installierten ServerBlocks angezeigt.

Der folgende Screenshot zeigt die Funktionsweise der Liste Option visuell.

.. code-block:: bash


 kevell@corp:/# ptdeploy nginxsbe list
 What is your ServerBlock directory?
 /root/Nginxdir
 What is your Enabled Symlink ServerBlock directory?

 Current Installed ServerBlocks:
 --- Enabled Server Blocks: ---
 (0) www.ngn.com
 (1) www.ngx.com
 --- All Available Server Blocks: ---
 (2) www.ngn.com
 (3) www.ngx.com
 ******************************


 1ServerBlock Creator Finished
 ******************************

Enable
----------

Mit der Freigabefunktion verwendet, um eine serverblock ermöglichen . Der Befehl zum Aktivieren verwendet wird unten gezeigt ,

.. code-block:: bash

	ptdeploy nginxsbe enable

.. code-block:: bash

 kevell@corp:/# ptdeploy nginxsbe enable

 Do you want to enable a ServerBlock? (Y/N) 
 y
 What is your Enabled Symlink ServerBlock directory? Found "/etc/nginx/sites-enabled" - Enter nothing to use this

 Please Choose ServerBlock:
 --- All Server Blocks: ---
 (0) ServerBlocktemp
 (1) aaaaaa
 (2) as
 (3) ddd
 (4) default
 (5) default.dpkg-old
 (6) dfdkdfsd.com
 (7) dfsdfssfdfdfdf.com
 (8) google
 (9) karuna
 (10) kkkkkkk
 (11) kumark
 (12) sites-available
 (13) vijay
 (14) www.amazon.com
 (15) www.deepak.com
 (16) www.google.com
 (17) www.kkk.com

 1
 Server Block Enabled Symlink Created
 ******************************
 ServerBlock Creator Finished
 ******************************


Disable
----------

Die Sperrfunktion wird verwendet, um eine Server- Block deaktivieren. Der Befehl zum Deaktivieren aufgelistet unten ,

.. code-block:: bash

	ptdeploy nginxsbe disable

.. code-block:: bash


 kevell@corp:/# ptdeploy nginxsbe disable

 Do you want to disable a ServerBlock? (Y/N) 
 y
 What is your Enabled Symlink ServerBlock directory? Found "/etc/nginx/sites-enabled" - Enter nothing to use this

 Please Choose ServerBlock:
 --- All Server Blocks: ---
 (0) ServerBlocktemp
 (1) aaaaaa
 (2) as
 (3) ddd
 (4) default
 (5) default.dpkg-old
 (6) dfdkdfsd.com
 (7) dfsdfssfdfdfdf.com
 (8) google
 (9) karuna
 (10) kkkkkkk
 (11) kumark
 (12) sites-available
 (13) vijay
 (14) www.amazon.com
 (15) www.deepak.com
 (16) www.google.com
 (17) www.kkk.com

 1
 Server Block aaaaaa Disabled  if exist
 ******************************
 ServerBlock Creator Finished
 ******************************



Vorteile
----------

* Es ist gut-to-do sowohl ubuntu und als auch in Cent OS.
* Die in der Erklärung verwendeten Parameter wird nicht zwischen Groß- und Kleinschreibung.
* Die Benutzer können Liste der Server-Blöcke zur Verfügung und sind derzeit installiert, noch bevor das Hinzufügen oder Löschen einer 
  Serverblock anzuzeigen.
