==================
JConfiguration
==================

Zusammenfassung
------------------

Dieses Modul ist ein Teil eines Standard-Moduls, das Daten stützen Funktionen behandelt. Lassen Sie uns finden Sie unter Konfigurieren und in kommenden Themen zurücksetzen.


Hilfe Befehl
--------------------

Der Help-Befehl führt den Benutzer über den Zweck des Moduls. Es listet, die alternative Parameter, die in der Deklaration verwendet werden können. Es gibt zwei unterschiedliche Syntax zum Konfigurieren und zurücksetzen. Der Befehl für die Hilfe-Option verwendet wird unten gezeigt:


.. code-block:: bash

	jrush jconf help

Der folgende Screenshot zeigt bildhaft über die Tätigkeit der Befehl Help.


.. code-block:: bash

 kevell@corp:/# jrush jconf help
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

  This command is part of Default Modules and handles Databasing Functions.

  JConfiguration, jconfigure, jconfiguration, jconf

      - configure, conf
      set up db user & pw for a project, use admins to create new resources as needed.
      example: ptdeploy jconf conf joomla
      example: ptdeploy jconf conf --yes --platform=joomla30 --mysql-host=127.0.0.1 --mysql-admin-user=""

      - reset
      reset current db to generic values so ptdeploy can write them. may need to be run before db conf.
      example: ptdeploy jconf reset drupal
      example: ptdeploy jconf reset --yes --platform=joomla30

      
 ------------------------------
 End Help
 ****************************************

How to Configure
----------------------

Konfigurieren Sie der Befehl für Joomla ist unten dargestellt:


.. code-block:: bash

	jrush jconf conf joomla

Nach den oben genannten Befehl eingeben, werden sie gefragt


.. cssclass:: table-bordered

 +----------------------------------+---------------------------------------+------------+------------------------------------------------+
 | Parameter			    | Alternative Parameter		    | Optionen	 | Kommentare			                  |
 +==================================+=======================================+============+================================================+
 |Do you want to configure	    | Statt conf können wir auch 	    | Y		 | Wenn der Benutzer wünschen, konfigurieren      |
 |Joomla? (Y/N)			    | configure.                            | 		 | sie können als Eingangs Y.                     |
 +----------------------------------+---------------------------------------+------------+------------------------------------------------+
 |Do you want to configure	    | Statt conf können wir auch   	    | N		 | Wenn der Benutzer nicht wünscht, konfigurieren |
 |Joomla? (Y/N)			    | configure.                            | 		 | sie eingeben kann als N.|                      |
 +----------------------------------+---------------------------------------+------------+------------------------------------------------+


Wenn die Benutzer-Erlöse konfigurieren, dem Benutzer fragt wird, ob sie nicht-Standardwerte für Folgendes festlegen wollen. Es gibt auch den Standardwert:


* Set non-default values for log_path?
* Set non-default values for temp_path?
* Set non-default values for MetaAuthor?
* Set non-default values for MetaDesc?
* Set non-default values for MetaKeys?
* Set non-default values for MetaRights?
* Set non-default values for MetaTitle?
* Set non-default values for MetaVersion?
* Set non-default values for access?
* Set non-default values for cache_handler?
* Set non-default values for cachetime?
* Set non-default values for frontediting?
* Set non-default values for assest_id?
* Set non-default values for user?
* Set non-default values for db?
* Set non-default values for host?
* Set non-default values for password?

Schließlich Ruft die Konfiguration abgeschlossen wie im Screenshot dargestellt.



.. code-block:: bash

 kevell@corp:/# jrush jconf conf joomla
 PHP Notice:  Undefined index: config-file in /opt/jrush/jrush/src/Modules/JConfiguration/Model/JConfigurationDataJoomla3.php on line 141
 PHP Notice:  Undefined index: config-file in /opt/jrush/jrush/src/Modules/JConfiguration/Model/JConfigurationDataJoomla3.php on line 141
 PHP Notice:  Undefined index: config-file in /opt/jrush/jrush/src/Modules/JConfiguration/Model/JConfigurationDataJoomla3.php on line 141
 PHP Notice:  Undefined index: config-file in /opt/jrush/jrush/src/Modules/JConfiguration/Model/JConfigurationDataJoomla3.php on line 141
 Do you want to configure Joomla? (Y/N) 
 Y
 PHP Notice:  Undefined index: config-file in /opt/jrush/jrush/src/Modules/JConfiguration/Model/JConfigurationDataJoomla3.php on line 141
 PHP Notice:  Undefined index: config-file in /opt/jrush/jrush/src/Modules/JConfiguration/Model/JConfigurationDataJoomla3.php on line 141
 Set non-default value for log_path? Default is /logs (Y/N) 

 Set non-default value for tmp_path? Default is /tmp (Y/N) 

 Set non-default value for MetaAuthor? Default is 1 (Y/N) 

 Set non-default value for MetaDesc? Default is  (Y/N) 

 Set non-default value for MetaKeys? Default is  (Y/N) 
 
 Set non-default value for MetaRights? Default is  (Y/N) 

 Set non-default value for MetaTitle? Default is 1 (Y/N) 

 Set non-default value for MetaVersion? Default is 0 (Y/N) 

 Set non-default value for access? Default is 1 (Y/N) 
 
 Set non-default value for cache_handler? Default is file (Y/N) 

 Set non-default value for cachetime? Default is 15 (Y/N) 

 Set non-default value for caching? Default is 0 (Y/N) 

 Set non-default value for captcha? Default is 0 (Y/N) 

 Set non-default value for cookie_domain? Default is  (Y/N) 

 Set non-default value for cookie_path? Default is  (Y/N) 

 Set non-default value for dbprefix? Default is jos_ (Y/N) 

 Set non-default value for dbtype? Default is mysqli (Y/N) 

 Set non-default value for debug? Default is 0 (Y/N) 

 Set non-default value for debug_lang? Default is 0 (Y/N) 

 Set non-default value for display_offline_message? Default is 1 (Y/N) 

 Set non-default value for editor? Default is jce (Y/N) 

 Set non-default value for error_reporting? Default is default (Y/N) 

 Set non-default value for feed_email? Default is author (Y/N) 

 Set non-default value for feed_limit? Default is 10 (Y/N) 

 Set non-default value for force_ssl? Default is 0 (Y/N) 

 Set non-default value for fromname? Default is  (Y/N) 

 Set non-default value for ftp_enable? Default is 0 (Y/N) 

 Set non-default value for ftp_host? Default is  (Y/N) 

 Set non-default value for ftp_pass? Default is  (Y/N) 
 
 Set non-default value for ftp_port? Default is 21 (Y/N) 

 Set non-default value for ftp_root? Default is  (Y/N) 

 Set non-default value for ftp_user? Default is  (Y/N) 

 Set non-default value for gzip? Default is 1 (Y/N) 

 Set non-default value for helpurl? Default is http://help.joomla.org/proxy/index.php?option=com_help&keyref=Help{major}{minor}:{keyref} (Y/N) 

 Set non-default value for lifetime? Default is 60 (Y/N) 

 Set non-default value for list_limit? Default is 20 (Y/N) 

 Set non-default value for live_site? Default is  (Y/N) 

 Set non-default value for mailer? Default is mail (Y/N) 

 Set non-default value for mailfrom? Default is  (Y/N) 

 Set non-default value for memcache_compress? Default is 0 (Y/N) 

 Set non-default value for memcache_persist? Default is 1 (Y/N) 

 Set non-default value for memcache_server_host? Default is localhost (Y/N) 

 Set non-default value for memcache_server_port? Default is 11211 (Y/N) 

 Set non-default value for offline? Default is 0 (Y/N) 

 Set non-default value for offline_image? Default is  (Y/N) 

 Set non-default value for offline_message? Default is This site is down for maintenance.<br /> Please check back again soon. (Y/N) 

 Set non-default value for offset? Default is Europe/London (Y/N) 

 Set non-default value for offset_user? Default is UTC (Y/N) 

 Set non-default value for robots? Default is  (Y/N) 

 Set non-default value for secret? Default is  (Y/N) 

 Set non-default value for sef? Default is 1 (Y/N) 

 Set non-default value for sef_rewrite? Default is 1 (Y/N) 

 Set non-default value for sef_suffix? Default is 0 (Y/N) 

 Set non-default value for sendmail? Default is /usr/sbin/sendmail (Y/N) 

 Set non-default value for session_handler? Default is database (Y/N) 

 Set non-default value for sitename? Default is  (Y/N) 

 Set non-default value for sitename_pagetitles? Default is 1 (Y/N) 

 Set non-default value for smtpauth? Default is 0 (Y/N) 

 Set non-default value for smtphost? Default is localhost (Y/N) 

 Set non-default value for smtppass? Default is  (Y/N) 

 Set non-default value for smtpport? Default is 25 (Y/N) 

 Set non-default value for smtpsecure? Default is none (Y/N) 

 Set non-default value for smtpuser? Default is  (Y/N) 

 Set non-default value for unicodeslugs? Default is 0 (Y/N) 

 Set non-default value for memcached_persist? Default is 1 (Y/N) 

 Set non-default value for memcached_compress? Default is 0 (Y/N) 

 Set non-default value for memcached_server_host? Default is localhost (Y/N) 

 Set non-default value for memcached_server_port? Default is 11211 (Y/N) 

 Set non-default value for proxy_enable? Default is 0 (Y/N) 

 Set non-default value for proxy_host? Default is  (Y/N) 

 Set non-default value for proxy_port? Default is  (Y/N) 

 Set non-default value for proxy_user? Default is  (Y/N) 

 Set non-default value for proxy_pass? Default is  (Y/N) 

 Set non-default value for mailonline? Default is 1 (Y/N) 

 Set non-default value for session_memcache_server_host? Default is localhost (Y/N) 

 Set non-default value for session_memcache_server_port? Default is 11211 (Y/N) 

 Set non-default value for session_memcached_server_host? Default is localhost (Y/N) 

 Set non-default value for session_memcached_server_port? Default is 11211 (Y/N) 

 Set non-default value for frontediting? Default is 1 (Y/N) 

 Set non-default value for asset_id? Default is 1 (Y/N) 

 Set non-default value for user? Default is  (Y/N) 

 Set non-default value for db? Default is  (Y/N) 

 Set non-default value for host? Default is  (Y/N) 

 Set non-default value for password? Default is  (Y/N) 

 PHP Notice:  Undefined index: config-file in /opt/jrush/jrush/src/Modules/JConfiguration/Model/JConfigurationAllOS.php on line 85
 PHP Warning:  file(): Filename cannot be empty in /opt/jrush/jrush/src/Modules/JConfiguration/Model/JConfigurationAllOS.php on line 85
 PHP Warning:  Invalid argument supplied for foreach() in /opt/jrush/jrush/src/Modules/JConfiguration/Model/JConfigurationAllOS.php on line 90
 Please check Joomla 3.x Series Settings file: 

 Is this Okay? (Y/N) 
 Y
 PHP Notice:  Undefined index: config-file in /opt/jrush/jrush/src/Modules/JConfiguration/Model/JConfigurationAllOS.php on line 119
 PHP Notice:  Undefined index: config-file in /opt/jrush/jrush/src/Modules/JConfiguration/Model/JConfigurationAllOS.php on line 120
 Removing old settings file ...
 
 PHP Notice:  Undefined index: config-file in /opt/jrush/jrush/src/Modules/JConfiguration/Model/JConfigurationAllOS.php on line 114
 Moving new settings file  in...
 PHP Notice:  Undefined index: config-file in /opt/jrush/jrush/src/Modules/JConfiguration/Model/JConfigurationAllOS.php on line 115
 PHP Warning:  file_put_contents(): Filename cannot be empty in /opt/jrush/jrush/src/Modules/JConfiguration/Model/JConfigurationAllOS.php on li ne 115
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

 1Joomla Configuration Finished
 ****************************************



while configuring, it will asks the user as 


.. code-block:: bash

	Please check Jomla 3.x Series Settings file:

Is this Okay? (Y/N)

The user have to specify Y or N.


Wie Zurücksetzen
-------------------

Nachfolgend finden Sie der Befehl zum Zurücksetzen:


.. code-block:: bash
 
	jrush jconf reset drupal

Der Screenshot unten zeigt visuell über den Prozess der zurücksetzen


Vorteile 
-----------

* Es ist wohlhabenden in beiden Cent OS und so gut wie Ubuntu. 
* Die Parameter, die in der Deklaration verwendet Groß-/Kleinschreibung keinen zusätzlichen Vorteil, während im Vergleich zu anderen ist. 
* Der Benutzer kann die Nichtstandard-Werte während der Konfiguration angeben.


