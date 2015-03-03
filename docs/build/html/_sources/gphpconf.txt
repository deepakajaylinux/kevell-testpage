============
phpconf
============


Zusammenfassung
-----------------------

Dieses Modul hilft bei der Installation und als auch die Verwaltung der Konfiguration von PHP. Der Benutzer kann seine Konfiguration nach ihrer Anforderung bei der Ausführung von Montagerahmens.


Hilfe Befehl
-------------

Der Befehl help führt den Benutzer bei der Arbeit mit diesem PHP-Konfiguration. Es gibt auch den Befehl für die Installation verwendet. Der Befehl help Liste auch die alternativen Parameter, die verwendet werden können. Der Befehl für die Hilfe-Option im Rahmen der Serverkonfiguration verwendet, wird unten gegeben.

.. code-block:: bash

	ptconfigure PHPConf help

Dieser Screenshot zeigt wie unten angegeben bildliche Darstellung in Bezug auf die Hilfe den Einsatz in PHP-Konfiguration.

.. code-block:: bash

 kevell@corp:/# ptconfigure PHPConf help
 ******************************


  This command is part of Core and provides you  with a method by which you can install Apache HTTP Server

  PHPConf, php-configure, php-configuration, php-conf, phpconf

        - install
        Installs a configuration for PHP
        example: ptconfigure phpconf install

 ------------------------------
 End Help
 ******************************

Installation
-------------

Installation der Serverkonfiguration ist günstiger für die Benutzer, da sie die Konfiguration nach ihren Anforderungen zu gestalten. Der Befehl für die Installation verwendet wird unten gegeben:

.. code-block:: bash

		ptconfigure PHPConf install

Nach der Eingabe des Befehls, wie oben gezeigt, die folgenden Operationen erfolgt wie im Tabellenformat angezeigt.

.. code-block:: bash

 kevell@corp:/# ptconfigure PHPConf install
 Install PHP Conf? (Y/N)
 y
 *******************************
 *        Pharaoh Tools        *
 *         PHP Conf!        *
 *******************************
 Set non-default value for user_ini.filename? Default is .user.ini (Y/N)
 y
 What value for user_ini.filename?

 Set non-default value for user_ini.cache_ttl? Default is 300 (Y/N)
 
 Set non-default value for engine? Default is On (Y/N)

 Set non-default value for short_open_tag? Default is On (Y/N)

 Set non-default value for asp_tags? Default is Off (Y/N)

 Set non-default value for precision? Default is 14 (Y/N)

 Set non-default value for y2k_compliance? Default is On (Y/N)

 Set non-default value for output_buffering? Default is 4096 (Y/N)

 Set non-default value for output_handler? Default is  (Y/N)

 Set non-default value for zlib.output_compression? Default is Off (Y/N)

 Set non-default value for zlib.output_compression_level? Default is -1 (Y/N)

 Set non-default value for zlib.output_handler? Default is  (Y/N)

 Set non-default value for implicit_flush? Default is Off (Y/N)

 Set non-default value for unserialize_callback_func? Default is  (Y/N)

 Set non-default value for serialize_precision? Default is 17 (Y/N)

 Set non-default value for allow_call_time_pass_reference? Default is Off (Y/N)

 Set non-default value for safe_mode? Default is Off (Y/N)

 Set non-default value for safe_mode_gid? Default is Off (Y/N)

 Set non-default value for safe_mode_exec_dir? Default is  (Y/N)

 Set non-default value for safe_mode_allowed_env_vars? Default is PHP_ (Y/N)

 Set non-default value for safe_mode_protected_env_vars? Default is LD_LIBRARY_PATH (Y/N)

 Set non-default value for open_basedir? Default is  (Y/N)

 Set non-default value for disable_functions? Default is pcntl_alarm,pcntl_fork,pcntl_waitpid,pcntl_wait,pcntl_wifexited,pcntl_wifstopped,pcntl_wifsignaled,pcntl_wexitstatus,pcntl_wtermsig,pcntl_wstopsig,pcntl_signal,pcntl_signal_dispatch,pcntl_get_last_error,pcntl_strerror,pcntl_sigpr ocmask,pcntl_sigwaitinfo,pcntl_sigtimedwait,pcntl_exec,pcntl_getpriority,pcntl_setpriority, (Y/N)

 Set non-default value for disable_classes? Default is  (Y/N)

 Set non-default value for ignore_user_abort? Default is On (Y/N)

 Set non-default value for realpath_cache_size? Default is 16k (Y/N)

 Set non-default value for realpath_cache_ttl? Default is 120 (Y/N)

 Set non-default value for zend.enable_gc? Default is On (Y/N)

 Set non-default value for expose_php? Default is On (Y/N)

 Set non-default value for max_execution_time? Default is 30 (Y/N)

 Set non-default value for max_input_time? Default is 60 (Y/N)

 Set non-default value for max_input_nesting_level? Default is 64 (Y/N)

 Set non-default value for max_input_vars? Default is 1000 (Y/N)

 Set non-default value for memory_limit? Default is 128M (Y/N)



 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 PHPConf: Success
 ------------------------------
 Installer Finished
 ******************************


Options
--------

.. cssclass:: table-bordered


 +--------------------------+----------------------------------------+------------------+-----------------------------------------+
 | Parameters               | Alternative Parameters                 | Erforderliche    | Kommentar                               |
 +==========================+========================================+==================+=========================================+
 |Install PHPConf?(Y/N)     | Statt PHP Conf diese alternative Namen | Y(Yes)           | Wenn der Benutzer wünschen, den         |
 |                          | können verwendet werden:php-configure, |                  | Installationsprozess können sie Eingang |
 |                          | php-conf php-configuration, phpconf    |                  | als Y gehen                             |
 +--------------------------+----------------------------------------+------------------+-----------------------------------------+
 |Install PHPConf? (Y/N)    | Statt PHP Conf diese alternative Namen | N(No)            | Wenn der Benutzer wünschen, den         |
 |                          | können verwendet werden:php-configure, |                  | Installationsprozess können sie Eingang | 
 |                          | php-conf php-configuration, phpconf    |                  | als N. beenden|                         |
 +--------------------------+----------------------------------------+------------------+-----------------------------------------+


Wenn der Benutzer den Installationsprozess fort, während der Ausführung der Installation wird das Modul gibt den Standardwert von Konfiguration und fragt den Benutzer auch die Nicht-Standardwerte für die Konfiguration nach ihren Anforderungen zu nennen. Die Spezifikationen für die Konfiguration während der Installation ist unten aufgeführt:

* Preis user_ini.filename
* Wert für user_ini.cache_ttl?
* Preis-Motor.
* Wert für short_open_tag.
* Wert für asp_tags.
* Wert für Präzision.
* Wert für y2k_compliance.
* Wert für output_buffering.
* Wert für output_handler.
* Wert für zlib.output_compression.
* Wert für zlib.output_compression_level.
* Wert für zlib.output_handler.
* Wert für implicit_flush.
* Wert für unserialize_callback_func.
* Wert für serialize Präzision.
* Wert für allow_call_time_pass_reference.
* Wert für safe_mode.
* Wert für safe_mode_gid.
* Wert für safe_mode_exec_dir?
* Wert für safe_mode_allowed_env_vars.
* Wert für Open basedir.
* Wert für Deaktivieren von Funktionen.
* Wert für disable_classes?
* Wert für ignore_user_abort
* Wert für realpath_cache_size?
* Wert für realpath_cache_ttl.
* Wert für zend.enable_gc.
* Wert für expose_php.
* Wert für max_execution_time.
* Wert für max_input_time.
* Wert für max_input_nesting_level.
* Wert für max_input_vars.
* Wert für memory_limits.

Nach einem Blick auf die Standardwerte für die Konfigurationsfunktionen kann der Anwender ihre Aktionen zu entscheiden. Wenn sie eichig mit Standardwerten können sie Eingang als N. Wenn sie benötigen, um die Konfigurationswerte sie eingeben können angeben, wie Y. Der Screenshot wie folgt erklärt die oben beschriebenen Verfahren visuell.

Vorteile
-----------

* Die für die Definition der Installation und Befehl help wird die Groß- verwendeten Parameter.
* Die Benutzer können die Konfigurationsfunktionen in der Laufzeit des Einbaurahmens.
* Es funktioniert gut auf beiden Cent OS und Windows.

