===========================
ApacheVHostEditor
===========================

Zusammenfassung
------------------------

Apache Virtual Hosts verwendet werden, um mehr als eine Domäne aus einer einzigen IP-Adresse ausgeführt werden. Dies ist besonders nützlich für Menschen, die Apache vhost Funktionen verarbeiten muss. Die Seiten zeigen unterschiedliche Informationen an die Besucher, abhängig von, mit dem die Benutzer zugreifen der Website. Es gibt keine Begrenzung für die Anzahl von virtuellen Hosts, die zu einem Virtual Private Server hinzugefügt werden können (VPS) .Dies kann für Ubuntu und CentOS sein.

Hilfe Befehl
-----------------------

Der Befehl help führt die Benutzer über den Zweck und als auch über die Möglichkeiten, die in den Apache Virtualhost-Editor-Module enthalten sind. Der Befehl help Listen aus der alternativen Parameter der Apache Virtualhost-Editor
unter ptdeploy Modul. Es beschreibt auch die Syntax für die Installation updation des Benutzers. Der Befehl help für Apache Virtualhost-Editor ist nachfolgend dargestellt.

.. code-block:: bash

	ptdeploy Apache virtualhost editor help

Der folgende Screenshot zeigt den vollen Einsatz von Apache Virtualhost-Editor.

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
--------------

Dieser Befehl verwendet werden, um einen virtuellen Host erstellen. Überschreiben ist möglich. Mit dem folgenden Befehl kann zum Erstellen einer virtuellen Host-Editor übernommen.

.. code-block:: bash

	sudo ptdeploy vhe add

nach Eingabe der obigen Befehl kann folgende fragen:

Vhe Document-Root, Vhe Dateierweiterung, Vhe apache Befehl Vhe IP Port, Vhe Vhost Directory Vhe Template, Vhe Standardvorlagennamen.

Der Benutzer hat die Eingabe alle Details eines nach dem anderen auf andere Weise in der Befehlszeile selbst eingeben. Der folgende Screenshot erklärt darüber

.. code-block:: bash


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


Add-Balancer
---------------------

Dieser Befehl verwendet werden, um einen virtuellen Host erstellen. Überschreiben ist möglich. Es gibt zwei Möglichkeiten, um die Eingangs einzugeben. In einfacher Weise kann der Benutzer vhe Add geben. Der zweite Weg, zusammen mit dem Befehl Hostpfadnamen genannt werden. Mit dem folgenden Befehl kann zum Erstellen einer virtuellen Host-Editor übernommen.

.. code-block:: bash

	sudo ptdeploy vhe add

nach Eingabe der obigen Befehl kann folgende fragen:

Vhe Document-Root, Vhe Dateierweiterung, Vhe apache Befehl Vhe IP Port, Vhe Vhost Directory Vhe Template, Vhe Standardvorlagennamen.

Der Benutzer hat die Eingabe alle Details eines nach dem anderen alles, was in der Befehlszeile selbst eingeben anders. Der folgende Screenshot erklärt
darüber

.. code-block:: bash

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

entfernen
-------------

Dieser Befehl verwendet werden, um eine bestimmte vhost löschen. Es gibt zwei Möglichkeiten, um die Eingangs einzugeben. In einfachen Weg vhe remove (rm) der Benutzer geben kann. Der zweite Weg, zusammen mit dem Befehl Hostpfadnamen genannt werden. Mit dem folgenden Befehl wird verwendet, um den Hostnamen zu entfernen.

.. code-block:: bash

        ptdeploy vhe rm

Der folgende Screenshot zeigt die Funktion rm.

.. code-block:: bash

 - rm
          example: ptdeploy vhe rm
          example: ptdeploy vhe rm --yes --
          example: ptdeploy vhe rm --yes --guess --vhe-deletion-vhost=www.site.com
          example: ptdeploy vhe rm --yes --guess --vhe-deletion-vhost=www.site.com

Liste
--------

Dieser Befehl verwendet werden, um eine Liste der aktuellen virtuellen Hosts. Der folgende Befehl verwendet werden, um eine Liste der virtuellen Hosts.

.. code-block:: bash

	ptdeploy vhe list

Der Screenshot zeigt die Listenfunktion.

.. code-block:: bash

 - list
          List current Virtual Hosts
          example: ptdeploy vhe list


ermöglichen
------------------

Secure Boot ist eine Funktion, die Schadsoftware und unerlaubten Medien aus Belastung während des Startvorgangs zu verhindern. Diese ermöglichen Option aktiviert den Server blockieren. In virtuellen Host, wenn das gebrauchte getippt Sie den folgenden Befehl,

.. code-block:: bash
   
	ptdeploy vhe enable

Diese Option ist standardmäßig aktiviert. Diese Option ermöglicht dem virtuellen Host-Server zu aktivieren.

Vorlagen-Modul entwickeln viele der grundlegenden Fähigkeiten benötigt, um hochleistungsfähige Umgebungen durch unser Verständnis der Wechselwirkungen zwischen Menschen, Prozesse und Technologien zu bedienen. Der folgende Screenshot erklärt die gleiche.

.. code-block:: bash

 - enable
          enable a Server Block
          example: ptdeploy vhe enable


Deaktivieren
-----------------

Diese disable verwendet, um den Server zu deaktivieren. Inaktive oder Leerlauf befindlichen virtuellen Host-Editor-Verbindungen werden in der Regel durch den Server nach einem bestimmten Zeitraum getrennt wird. Mit dem folgenden Befehl wird verwendet, um den virtuellen Host-Editor zu deaktivieren.

.. code-block:: bash
   
	ptdeploy vhe disable

Nachdem Sie diesen Befehl kann der Benutzer aufgefordert, den Server zu deaktivieren. Wenn die Benutzereingaben, wie es ja den Server zu deaktivieren, dh es wird nicht zulassen, dass jeder Körper in diesem Server zu arbeiten.

Der folgende Screenshot visualisieren offenbar.

.. code-block:: bash

 - disable
          disable a Server Block
          example: ptdeploy vhe disable

Vorteile
---------------

* Multi Benutzer gleichzeitig zugreifen können.
* Der Benutzer kann hinzufügen oder entfernen, virtuellen Hosts.
* Der virtuelle Host-Editor aktivieren oder deaktivieren können den virtuellen Host nach Wunsch des Benutzers.
* Nicht Groß- und Kleinschreibung.
* Well-to-do in Ubuntu und CentOS.
