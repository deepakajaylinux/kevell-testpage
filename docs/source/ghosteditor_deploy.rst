======================
Host Editor
======================

Zusammenfassung
------------------

Dieses Modul unterstützt Apache Virtual Host-Editor unter ptdeploy behandeln. Es kann auf zwei Arten funktionieren. Sie werden hinzugefügt und entfernt werden. Vhost Editor ist ein PHP-Tool geschrieben, um das Hinzufügen virtuelle Hosts zu einem Kinderspiel Apache. Vhost Editor ermöglicht es dem Benutzer hinzufügen, bearbeiten oder Virtual Host Informationen über Web-Server des Benutzers zu löschen. Es ist bequem, mit Ubuntu und Cent-OS arbeiten. Mal sehen, wie der Apache Vhost Editor finden Sie unter dapperstarano funktionieren.

Hilfe Befehl
-----------------------

Dieser Befehl help führt den Benutzer zu einem virtuellen Host erstellen. Dies zeigt auch, um einen virtuellen Host einen virtuellen Host hinzufügen, entfernen Sie einen virtuellen Host, aktivieren Sie einen virtuellen Host, und deaktivieren.

Der Befehl help für Apachevhosteditor ist nachfolgend dargestellt.

.. code-block:: bash

	ptdeploy Apachevhosteditor help

Nach Eingang der obige Befehl, beginnt es funktioniert, um einen virtuellen Host-Editor hinzufügen. Es Katechese die Funktionen in den Screenshots.

.. code-block:: bash


 kevell@corp:/# ptdeploy ApacheVHostEditor help
 ******************************


  This command is part of Default Modules and handles Apache VHosts Functions.

  ApacheVHostEditor, apachevhosteditor, vhosteditor, vhe, vhosted

          - add
          create a Virtual Host
          example: sudo ptdeploy vhe add
          example: sudo ptdeploy vhe add --yes --vhe-docroot=/var/www/the-app --vhe-url=www.dave.com --vhe-file-ext="" --vhe-apache-command="apache2" --vhe-ip-port="127.0.0.1:80" --vhe-vhost-dir="/etc/apache2/sites-available" --vhe-template="*template data*"
          example: sudo ptdeploy vhe add --yes --guess --vhe-url=www.dave.com
              # will attempt to guess the following but you can override any
              # --vhe-docroot=*current working dir*
              # --vhe-file-ext="ubuntu none, others .conf"
              # --vhe-apache-command="apache2 or httpd depends on system"
              # --vhe-ip-port="127.0.0.1:80"
              # --vhe-vhost-dir="/etc/apache2/sites-available or /etc/httpd/vhosts.d"
              # --vhe-template="*template data*"
              # --vhe-default-template-name="docroot-src-suffix" // from default templates

          - add-balancer
          create a Virtual Host
          example: sudo ptdeploy vhe add
          example: sudo ptdeploy vhe add --yes --vhe-docroot=/var/www/the-app --vhe-url=www.dave.com --vhe-file-ext="" --vhe-apache-command="apache2" --vhe-ip-port="127.0.0.1:80" --vhe-vhost-dir="/etc/apache2/sites-available" --vhe-template="*template data*"
          example: sudo ptdeploy vhe add --yes --guess --vhe-url=www.dave.com
              # will attempt to guess the following but you can override any
              # --vhe-docroot=*current working dir*
              # --vhe-file-ext="ubuntu none, others .conf"
              # --vhe-apache-command="apache2 or httpd depends on system"
              # --vhe-ip-port="127.0.0.1:80"
              # --vhe-vhost-dir="/etc/apache2/sites-available or /etc/httpd/vhosts.d"
              # --vhe-template="*template data*"
              # --vhe-default-template-name="docroot-src-suffix" // from default templates

          - rm
          example: ptdeploy vhe rm
          example: ptdeploy vhe rm --yes --
          example: ptdeploy vhe rm --yes --guess --vhe-deletion-vhost=www.site.com
          example: ptdeploy vhe rm --yes --guess --vhe-deletion-vhost=www.site.com

          - list
          List current Virtual Hosts
          example: ptdeploy vhe list

          - enable
          enable a Server Block
          example: ptdeploy vhe enable

          - disable
          disable a Server Block
          example: ptdeploy vhe disable

 ------------------------------
 End Help
 ******************************





Alternative Parameter
-----------------------------------

Im Folgenden sind die Parameter, die in alternative Erklärungen definiert werden können:

ApacheVHostEditor, apachevhosteditor, vhosteditor, vhe, vhosted.


hinzufügen
---------------

Dies ermöglicht es dem Benutzer, einen virtuellen Host erstellen. Beim Hinzufügen Virtueller Host kann es fragt vhe-docroot, vhe-file-ext, vhe-Apache-Befehl, vhe-IP-Port, vhe-Host-dir, vhe-Vorlagen, vhe-default-Template-Namen. Der Benutzer kann die nach ihrem Wunsch geben.

.. code-block:: bash

	sudo ptdeploy vhe add

Nach Eingang als dem obigen Befehl kann der Benutzer die folgenden Verfahren zu füllen.

.. cssclass:: table-bordered

 +----------------------------+----------------+-----------------------------------------+------------------------------------------------+
 | Parameters                 | Option         | Verzeichnis                             | Kommentare                                     |
 +============================+================+=========================================+================================================+
 |ptdeploy vhe add (Default)  | Yes            | Es kann den Benutzer für Document       | Hinzugefügt virtuellen Host im angegebenen     |
 |                            |                | Root fragen                             | Document-Root unter ptdeploy                   |
 +----------------------------+----------------+-----------------------------------------+------------------------------------------------+
 |What’s the server name      | -              | Es kann den Benutzer zur Servernamen    | Hinzugefügt Servernamen unter ptdeploy         |
 |                            |                | fragen                                  |                                                |
 +----------------------------+----------------+-----------------------------------------+------------------------------------------------+
 |What IP:Port (default)      | 127.0.0.1:80   | Es kann den Benutzer zur IP-Port fragen | Wenn der Benutzer die Eingabe als geben Sie    |
 |                            |                |                                         | das Standardwert für IP: Port                  |
 +----------------------------+----------------+-----------------------------------------+------------------------------------------------+
 |What file extension should  | None           | Es kann fragt den Benutzer nach         | Der Nutzer ist damit Eingang als               |
 |be used? (Default)          |                | Verlängerung                            | Dateierweiterung                               |
 +----------------------------+----------------+-----------------------------------------+------------------------------------------------+
 |ptdeploy vhe add            | No             | Es kann, fragt den Benutzer zur Eingabe | Es kann das Verfahren beendet|                 |
 +----------------------------+----------------+-----------------------------------------+------------------------------------------------+


Schließlich kann das System bittet um vhost Vorlagenverzeichnis. Es gibt 5 Möglichkeiten zur Verfügung in Vorlagen. Sie sind wie folgt.

0 for doc root-no-suffix

1 for doc –src-suffix   used for document screen suffix

2 for doc –web-suffix used for document web suffix

3 for doc –www-suffix used for world wide web suffix

4 for docroot-suffix used for document root suffix

Der Benutzer möchte die Werte nach ihren Bedürfnissen wählen. Dann kann das System die vhost Namen, IP-Adresse und Root etc richtig oder falsch ist. Wenn der Benutzer sagt ja, dann zeigt es die vhost Verzeichnis und aktivieren Sie diese vhost?

Der Teilnehmer meldet sich ja es kann die vhost anderes ermöglichen es verlassen.

.. code-block:: bash

 kevell@corp:/# ptdeploy vhe add
 Do you want to add a VHost? (Y/N) 
 Y
 What's the document root? Enter nothing for /
 root
 What URL do you want to add as server name?
 www.vh.com
 What IP:Port should be set? Enter nothing for 127.0.0.1:80

 What File Extension should be used? Enter nothing for None (probably .conf on this system)

 What is your VHost Template directory? Enter nothing for default templates

 Please Choose VHost Template: 
 --- Default Virtual Host Templates: ---
 (0) docroot-no-suffix
 (1) docroot-src-suffix
 (2) docroot-web-suffix
 (3) docroot-www-suffix
 (4) docroot-docroot-suffix

 0
 Please check VHost: NameVirtualHost 127.0.0.1:80
 <VirtualHost 127.0.0.1:80>
	ServerAdmin webmaster@localhost
	ServerName www.vh.com
	DocumentRoot root
	<Directory root>
		Options Indexes FollowSymLinks MultiViews
		AllowOverride All
		Order allow,deny
		allow from all
	</Directory>
 </VirtualHost>

 Is this Okay? (Y/N) 

 ******************************


 Apache VHost Editor Finished
 ******************************



entfernen
--------------

Der Terminal-Befehl zum Löschen virtueller Host (s) rm. Das allgemeine Format des Befehls ist rm. rm löscht einen virtuellen Host, wenn Sie einen entsprechenden Pfad angeben, für sie und wenn Sie nicht tun, dann wird eine Fehlermeldung zeigt ihn und fahren Sie mit dem nächsten Host. Manchmal erhalten Sie möglicherweise nicht über die Schreibberechtigungen für einen virtuellen Host, in diesem Fall ist es fordert Sie zur Bestätigung. Geben Sie yes ein, wenn Sie es löschen möchten.

Wenn der Name entfernt war die letzte Verbindung zu einem virtuellen Host und keine Prozesse
der virtuelle Host geöffnet ist, wird der virtuelle Host gelöscht und der Raum, den sie wurde mit zur Wiederverwendung zur Verfügung gestellt.

Wenn der Name war die letzte Verbindung zu einem virtuellen Host, aber alle Prozesse noch
der virtuelle Host geöffnet ist, wird der virtuelle Host existiert, bis der letzte virtuelle Host-Deskriptor, die sich auf sie geschlossen bleiben.

Wenn der Name bezog sich auf einen symbolischen Link, wird der Link entfernt. Der folgende Befehl verwendet werden, um den virtuellen Host löschen.

.. code-block:: bash
   
	sudo ptdeploy vhe rm –yes –guess –vhe-deletion-vhost=www.kevell.com

Der folgende Screenshot kann seine Funktionen zu erklären.

.. code-block:: bash

 - rm
          example: ptdeploy vhe rm
          example: ptdeploy vhe rm --yes --
          example: ptdeploy vhe rm --yes --guess --vhe-deletion-vhost=www.site.com
          example: ptdeploy vhe rm --yes --guess --vhe-deletion-vhost=www.site.com



.. code-block:: bash

 kevell@corp:/# ptdeploy vhe rm
 Do you want to delete VHost/s? (Y/N) 
 y
 Deleting vhost
 What is your VHost directory? Found "/etc/apache2/sites-available" - Enter nothing to use this

 Please Choose VHost:
 --- All Virtual Hosts: ---
 (0) 000-default.conf
 (1) default-ssl.conf

 0
 Do you want to disable this VHost? (hint - ubuntu probably yes, centos probably no) (Y/N) 
 yes
 Site 000-default disabled.
 To activate the new configuration, you need to run:
  service apache2 reload
 a2dissite 000-default.conf done
 VHost 000-default.conf Deleted  if existed
 ******************************


 1Apache VHost Editor Finished
 ******************************




Liste
--------

Liste Informationen über den virtuellen Host (das aktuelle Verzeichnis in Standardeinstellung). Sortieren Einträge alphabetisch. Erforderliche Argumente hat lange Möglichkeiten sowie kurze Optionen zu. Eine Liste mit URL-Angabe sowohl den Listennamen und auch die zugrunde liegende Ansicht, und organisiert die Daten wird aufgerufen. Der folgende Befehl verwendet zur Liste der virtuellen Hosts.

.. code-block:: bash
   
	ptdeploy vhe list

Note that whether a list can be used with a variety of views, or might be tailored to produce an elaborate page from a view designed specifically to organize data for it. Lists stored under the lists field of a design document. It can be visualized by the screen shots.

.. code-block:: bash

 - list
          List current Virtual Hosts
          example: ptdeploy vhe list

.. code-block:: bash

 kevell@corp:/# ptdeploy vhe list
 What is your VHost directory? Found "/etc/apache2/sites-available" - Enter nothing to use this

 You have a sites available dir, so also listing available sites.
 Current Installed VHosts:
 --- Enabled Virtual Hosts: ---
 (0) 000-default.conf
 (1) default-ssl.conf
 --- All Available Virtual Hosts: ---
 (2) 000-default.conf
 (3) default-ssl.conf
 ******************************


 1Apache VHost Editor Finished
 ******************************




ermöglichen
---------------

Secure Boot ist eine Funktion, die Schadsoftware und unerlaubten Medien aus Belastung während des Startvorgangs zu verhindern. Diese ermöglichen Option aktiviert den Server blockieren. In virtuellen Host, wenn das gebrauchte getippt Sie den folgenden Befehl,

.. code-block:: bash
   
	ptdeploy vhe enable

Diese Option ist standardmäßig aktiviert. Diese Option ermöglicht dem virtuellen Host-Server zu aktivieren.

Vorlagen-Modul entwickeln viele der grundlegenden Fähigkeiten benötigt, um hochleistungsfähige Umgebungen durch unser Verständnis der Wechselwirkungen zwischen Menschen, Prozesse und Technologien zu bedienen. Der folgende Screenshot erklärt die gleiche.

.. code-block:: bash

 - enable
          enable a Server Block
          example: ptdeploy vhe enable


.. code-block:: bash

 kevell@corp:/# ptdeploy vhe enable
 Do you want to enable this VHost? (hint - ubuntu probably yes, centos probably no) (Y/N) 
 y
 Please Choose VHost:
 --- All Virtual Hosts: ---
 (0) default-ssl.conf
 
 0
 ERROR: Site default-ssl.conf does not exist!
 a2ensite default-ssl.conf.conf done
 ******************************


 1Apache VHost Editor Finished
 ******************************




Disable
-------------

Diese disable verwendet, um den Server zu deaktivieren. Inaktive oder Leerlauf befindlichen virtuellen Host-Editor-Verbindungen werden in der Regel durch den Server nach einem bestimmten Zeitraum getrennt wird. Mit dem folgenden Befehl wird verwendet, um den virtuellen Host-Editor zu deaktivieren.

.. code-block:: bash
   
	ptdeploy vhe disable

Nachdem Sie diesen Befehl kann der Benutzer aufgefordert, den Server zu deaktivieren. Wenn die Benutzereingaben, wie es ja den Server zu deaktivieren, dh es wird nicht zulassen, dass jeder Körper in diesem Server zu arbeiten.

Der folgende Screenshot visualisieren offenbar.

.. code-block:: bash


 - disable
          disable a Server Block
          example: ptdeploy vhe disable

.. code-block:: bash

 kevell@corp:/# ptdeploy vhe disable
 Do you want to disable this VHost? (hint - ubuntu probably yes, centos probably no) (Y/N) 
 y
 Please Choose VHost:
 --- All Virtual Hosts: ---
 (0) default-ssl.conf

 0
 Site default-ssl already disabled
 a2dissite default-ssl.conf done
 ******************************


 1Apache VHost Editor Finished
 ******************************




Vorteile
---------------

* Multi Benutzer gleichzeitig zugreifen können.
* Der Benutzer kann hinzufügen oder entfernen, virtuellen Hosts.
* Der virtuelle Host-Editor aktivieren oder deaktivieren können den virtuellen Host nach Wunsch des Benutzers.
* Nicht Groß- und Kleinschreibung.
