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

 kevell@corp:/# ptdeploy vhe add 
 
 Do you want to add a VHost? (Y/N) 
 y 
 What's the document root? Enter nothing for /home/karunakaran 
 
 What URL do you want to add as server name? 
 kumar 
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
	ServerName kumar 
	DocumentRoot /home/karunakaran 
	<Directory /home/karunakaran> 
		Options Indexes FollowSymLinks MultiViews 
		AllowOverride All 
		Order allow,deny 
		allow from all 
	</Directory> 
 </VirtualHost> 

 Is this Okay? (Y/N) 
 y 
 What is your VHost directory? Found "/etc/apache2/sites-available" - Enter nothing to use this 
 
 Do you want to enable this VHost? (hint - ubuntu probably yes, centos probably no) (Y/N) 
 y 
 Enabling site kumar. 
 To activate the new configuration, you need to run: 
  service apache2 reload 
 a2ensite kumar.conf done 
 ****************************** 

 1Apache VHost Editor Finished 
 ******************************

.. code-block:: bash


 kevell@corp:/# ptdeploy vhe add --yes --vhe-docroot=/var/www/the-app --vhe-url=www.murali.com --vhe-file-ext=".conf" --vhe-apache-command="apache2" --vhe-ip-port="127.0.0.1:80" --vhe-vhost-dir="/etc/apache2/sites-available" --vhe-template="*template data*" 

 *template data* 

 Assuming Okay due to yes parameter 
 Enabling site www.murali.com. 
 To activate the new configuration, you need to run: 
  service apache2 reload 
 a2ensite www.murali.com.conf done 
 ****************************** 

 1Apache VHost Editor Finished 
 ****************************** 

.. code-block:: bash


 kevell@corp:/# ptdeploy vhe add --yes --guess --vhe-url=www.kkkkkkkkk.com 

 What is your VHost Template directory? Enter nothing for default templates 

 Please Choose VHost Template: 
 --- Default Virtual Host Templates: --- 
 (0) docroot-no-suffix 
 (1) docroot-src-suffix 
 (2) docroot-web-suffix 
 (3) docroot-www-suffix 
 (4) docroot-docroot-suffix 
 
 0 
 NameVirtualHost 127.0.0.1:80 
 <VirtualHost 127.0.0.1:80> 
 	ServerAdmin webmaster@localhost 
	ServerName www.kkkkkkkkk.com 
	DocumentRoot /home/karunakaran 
	<Directory /home/karunakaran> 
		Options Indexes FollowSymLinks MultiViews 
		AllowOverride All 
		Order allow,deny 
		allow from all 
	</Directory> 
 </VirtualHost> 

 Assuming Okay due to yes parameter 
 Enabling site www.kkkkkkkkk.com. 
 To activate the new configuration, you need to run: 
   service apache2 reload 
 a2ensite www.kkkkkkkkk.com done 
 ****************************** 

 1Apache VHost Editor Finished 
 ******************************



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

 kevell@corp:/# ptdeploy vhe rm 

 Do you want to delete VHost/s? (Y/N) 
 y 
 Deleting vhost 
 What is your VHost directory? Found "/etc/apache2/sites-available" - Enter nothing to use this 

 Please Choose VHost: 
 --- All Virtual Hosts: --- 
 (0) 000-default.conf 
 (1) ddddddd.conf 
 (2) default-ssl.conf 
 (3) default-ssl.dpkg-remove 
 (4) default.dpkg-remove 
 (5) karuna 
 (6) kumar.conf 
 (7) llllllllllllll.conf 
 (8) mmmmmm.conf 
 (9) ptbuild.conf 
 (10) www.dave.com 
 (11) www.google.com 
 (12) www.kkkkkkkkk.com.conf 
 (13) www.murali.com.conf 
 (14) www.siva.com.conf 
 (15) www.siva1.com 
 
 14 
 Do you want to disable this VHost? (hint - ubuntu probably yes, centos probably no) (Y/N) 
 y 
 Site www.siva.com disabled. 
 To activate the new configuration, you need to run: 
  service apache2 reload 
 a2dissite www.siva.com.conf done 
 VHost www.siva.com.conf Deleted  if existed 
 ****************************** 

 1Apache VHost Editor Finished 
 ****************************** 

.. code-block:: bash


 kevell@corp:/# ptdeploy vhe rm --yes --

 Deleting vhost
 What is your VHost directory? Found "/etc/apache2/sites-available" - Enter nothing to use this
 
 Please Choose VHost:
 --- All Virtual Hosts: ---
 (0) 000-default.conf
 (1) ddddddd.conf
 (2) default-ssl.conf
 (3) default-ssl.dpkg-remove
 (4) default.dpkg-remove
 (5) karuna
 (6) kumar.conf
 (7) llllllllllllll.conf
 (8) mmmmmm.conf
 (9) ptbuild.conf
 (10) testrepo.conf
 (11) www.dae.com.conf
 (12) www.dave.com
 (13) www.google.com
 (14) www.kkkkkkkkk.com.conf
 (15) www.murali.com.conf
 
 14
 Site www.kkkkkkkkk.com already disabled
 a2dissite www.kkkkkkkkk.com.conf done
 VHost www.kkkkkkkkk.com.conf Deleted  if existed
 ******************************
 
 1Apache VHost Editor Finished
 ******************************


.. code-block:: bash


 kevell@corp:/# ptdeploy vhe rm --yes --guess --vhe-deletion-vhost=www.da.com.conf

 Deleting vhost
 Site www.da.com disabled.
 To activate the new configuration, you need to run:
  service apache2 reload
 a2dissite www.da.com.conf done
 VHost www.da.com.conf Deleted  if existed
 ******************************
 

 1Apache VHost Editor Finished
 ******************************


.. code-block:: bash

 kevell@corp:/# ptdeploy vhe rm --yes --guess --vhe-deletion-vhost=www.dae.com.conf

 Deleting vhost
 Site www.dae.com disabled.
 To activate the new configuration, you need to run:
   service apache2 reload
 a2dissite www.dae.com.conf done
 VHost www.dae.com.conf Deleted  if existed
 ******************************

 1Apache VHost Editor Finished
 ******************************


Liste
--------

Dieser Befehl verwendet werden, um eine Liste der aktuellen virtuellen Hosts. Der folgende Befehl verwendet werden, um eine Liste der virtuellen Hosts.

.. code-block:: bash

	ptdeploy vhe list

Der Screenshot zeigt die Listenfunktion.

.. code-block:: bash


 kevell@corp:/# ptdeploy vhe list 

 What is your VHost directory? Found "/etc/apache2/sites-available" - Enter nothing to use this 

 You have a sites available dir, so also listing available sites. 
 Current Installed VHosts: 
 --- Enabled Virtual Hosts: --- 
 (0) 000-default.conf 
 (1) ddddddd.conf 
 (2) default-ssl.conf 
 (3) default-ssl.dpkg-remove 
 (4) default.dpkg-remove 
 (5) karuna 
 (6) kumar.conf 
 (7) llllllllllllll.conf 
 (8) mmmmmm.conf 
 (9) ptbuild.conf 
 (10) www.dave.com 
 (11) www.google.com 
 (12) www.kkkkkkkkk.com.conf 
 (13) www.murali.com.conf 
 (14) www.siva.com.conf 
 (15) www.siva1.com 
 --- All Available Virtual Hosts: --- 
 (16) 000-default.conf 
 (17) ddddddd.conf 
 (18) default-ssl.conf 
 (19) default-ssl.dpkg-remove 
 (20) default.dpkg-remove 
 (21) karuna 
 (22) kumar.conf 
 (23) llllllllllllll.conf 
 (24) mmmmmm.conf 
 (25) ptbuild.conf 
 (26) www.dave.com 
 (27) www.google.com 
 (28) www.kkkkkkkkk.com.conf 
 (29) www.murali.com.conf 
 (30) www.siva.com.conf 
 (31) www.siva1.com 
 ****************************** 

 1Apache VHost Editor Finished 
 ****************************** 



ermöglichen
------------------

Secure Boot ist eine Funktion, die Schadsoftware und unerlaubten Medien aus Belastung während des Startvorgangs zu verhindern. Diese ermöglichen Option aktiviert den Server blockieren. In virtuellen Host, wenn das gebrauchte getippt Sie den folgenden Befehl,

.. code-block:: bash
   
	ptdeploy vhe enable

Diese Option ist standardmäßig aktiviert. Diese Option ermöglicht dem virtuellen Host-Server zu aktivieren.

Vorlagen-Modul entwickeln viele der grundlegenden Fähigkeiten benötigt, um hochleistungsfähige Umgebungen durch unser Verständnis der Wechselwirkungen zwischen Menschen, Prozesse und Technologien zu bedienen. Der folgende Screenshot erklärt die gleiche.

.. code-block:: bash

 kevell@corp:/# ptdeploy vhe enable 

 Do you want to enable this VHost? (hint - ubuntu probably yes, centos probably no) (Y/N) 
 y 
 Please Choose VHost: 
 --- All Virtual Hosts: --- 
 (0) 000-default.conf 
 (1) ddddddd.conf 
 (2) default-ssl.conf 
 (3) default-ssl.dpkg-remove 
 (4) default.dpkg-remove 
 (5) karuna 
 (6) kumar.conf 
 (7) llllllllllllll.conf 
 (8) mmmmmm.conf 
 (9) ptbuild.conf 
 (10) www.dave.com 
 (11) www.google.com 
 (12) www.kkkkkkkkk.com.conf 
 (13) www.murali.com.conf 
 (14) www.siva.com.conf 
 (15) www.siva1.com 

 7 
 Enabling site llllllllllllll. 
 To activate the new configuration, you need to run: 
  service apache2 reload 
 a2ensite llllllllllllll.conf done 
 ****************************** 

 1Apache VHost Editor Finished 
 ****************************** 



Deaktivieren
-----------------

Diese disable verwendet, um den Server zu deaktivieren. Inaktive oder Leerlauf befindlichen virtuellen Host-Editor-Verbindungen werden in der Regel durch den Server nach einem bestimmten Zeitraum getrennt wird. Mit dem folgenden Befehl wird verwendet, um den virtuellen Host-Editor zu deaktivieren.

.. code-block:: bash
   
	ptdeploy vhe disable

Nachdem Sie diesen Befehl kann der Benutzer aufgefordert, den Server zu deaktivieren. Wenn die Benutzereingaben, wie es ja den Server zu deaktivieren, dh es wird nicht zulassen, dass jeder Körper in diesem Server zu arbeiten.

Der folgende Screenshot visualisieren offenbar.

.. code-block:: bash


 kevell@corp:/# ptdeploy vhe disable 

 Do you want to disable this VHost? (hint - ubuntu probably yes, centos probably no) (Y/N) 
 y 
 Please Choose VHost: 
 --- All Virtual Hosts: --- 
 (0) 000-default.conf 
 (1) default-ssl.conf 
 (2) default-ssl.dpkg-remove 
 (3) default.dpkg-remove 
 (4) karuna 
 (5) kumar.conf 
 (6) ptbuild.conf 
 (7) www.dave.com 
 (8) www.google.com 
 (9) www.kkkkkkkkk.com.conf 
 (10) www.murali.com.conf 
 (11) www.siva.com.conf 
 (12) www.siva1.com 

 9 
 Site www.kkkkkkkkk.com disabled. 
 To activate the new configuration, you need to run: 
  service apache2 reload 
 a2dissite www.kkkkkkkkk.com.conf done 
 ****************************** 

 1Apache VHost Editor Finished 
 ****************************** 


Vorteile
---------------

* Multi Benutzer gleichzeitig zugreifen können.
* Der Benutzer kann hinzufügen oder entfernen, virtuellen Hosts.
* Der virtuelle Host-Editor aktivieren oder deaktivieren können den virtuellen Host nach Wunsch des Benutzers.
* Nicht Groß- und Kleinschreibung.
* Well-to-do in Ubuntu und CentOS.
