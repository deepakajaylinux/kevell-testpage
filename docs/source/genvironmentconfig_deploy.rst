====================
EnvironmentConfig
====================

Zusammenfassung
-------------------

Mit diesem Modul können die Benutzer bei der Konfiguration ihrer Umgebung für ihr Projekt erforderlich. Lassen Sie uns sehen, wie man die Umgebung zu konfigurieren, wie man die unerwünschten Umwelt, wie Sie die Optionsliste für die Liste der verfügbaren Umgebungen in kommenden Themen benutzen zu löschen.

Hilfe Befehl
--------------------

Der Befehl help führt den Anwender über den Zweck des Moduls, seine alternative Parameter, die in der Erklärung verwendet. Sie weist auf die drei Funktionen der Umgebungskonfiguration die Liste sind, zu konfigurieren, zu löschen. Er legt auch die Syntax für drei Hauptfunktionen. Die zur Feststellung der Hilfe verwendete Syntax ist wie folgt:

.. code-block:: bash

	ptdeploy envconfig help

Der folgende Screenshot zeigt bildhaft über die Arbeit der Befehl help.

.. code-block:: bash

 kevell@corp:/# ptdeploy EnvironmentConfig help
 **************************************************

  This command is part of a default Module and provides you with a method by which you can
  configure environments for your project from the command line. Currently compliant with
  both ptdeploy and ptconfigure.


  EnvironmentConfig, environmentconfig, environment-config, envconfig, env-config

        - list
        List current environments
        example: ptdeploy envconfig list --yes

        - configure, config
        Configure the environments for your project to use
        example: ptdeploy envconfig config
        example: ptdeploy envconfig config --keep-current-environments

        - delete, del
        Configure the environments for your project to use
        example: ptdeploy envconfig delete
        example: ptdeploy envconfig del --environment-name="staging"

 ------------------------------
 End Help
 ******************************



Wie man die Umgebung konfigurieren
----------------------------------------------

Für den Zweck der Konfiguration der Umgebung kann der Benutzer den folgenden Befehl verwenden:

.. code-block:: bash

	ptdeploy envconfig config

Type text or a website address or translate a document.

Nach der Eingabe des Befehls über die folgenden Operationen erfolgt wie folgt:

Schritt 1: Konfigurieren von Umgebungen hier? (Y / N)

Der Benutzer die Eingabe Y oder N sind

Schritt 2: Verwenden Sie die vorhandene Umgebung Einstellungen? (Y / N)

Der Benutzer die Eingabe Y oder N sind

Wenn die Benutzereingabe als Y wird mit bereits bestehenden fortzufahren.

Wenn sie als Eingang N, wird es in Bezug auf die Umwelt, fragt Informationen

Preis: Name der Umwelt

Preis: Standard temporäre Verzeichnis (Ort)

Nach den obigen Schritten der Benutzer zur Eingabe der folgenden Angaben:

Ziel eingeben?

Geben Sie hier?

Geben Sie das Kennwort?

In einem anderen Server? (Y / N)

Der Benutzer die Eingabe Y oder N sind

Schließlich erhält der Umgebungskonfiguration Erfolg wie in der Abbildung unten dargestellt.
Top of Form

.. code-block:: bash


 kevell@corp:/# ptdeploy envconfig config

 Configure Environments Here? (Y/N) 
 y
 Do you want to add another environment? (Y/N) 
 y
 Environment 3  : 
 Default Settings for Any App not setup for environment  enter them now.
 Value for: Name of this Environment
 deepak
 Value for: Default Temp Dir (should usually be /tmp/)
 /tmp/
 Enter Servers - this is an array of entries
 Enter target ?
 192.168.1.7
 Enter user ?
 deepak
 Enter password ?
 123
 Add Another Server? (Y/N)
 n
 ******************************
 Success
 In Environment Configuration
 ****************************** 



Beim Konfigurieren einer Umgebung, wenn der Benutzer wünschen, mit der aktuellen Umgebung zu konfigurieren, sie den folgenden Befehl verwenden:

.. code-block:: bash

	ptdeploy envconfig config --keep-current-environments


Nach der Eingabe des Befehls vor, werden dazu aufgefordert, die folgenden Details, wie in der Tabellenform dargestellt:


.. cssclass:: table-bordered


 +--------------------------------------+----------+-----------------------------------------------------------------------------+
 | Parameters                           | Options  | Kommentare                                                                  |
 +======================================+==========+=============================================================================+
 |Configure Environments Here? (Y/N)    | Y        | Wenn der Benutzer gegebenenfalls die Umgebungen in der aktuellen            |
 |                                      |          | Umgebung können sie Eingang als Y konfigurieren                             |
 +--------------------------------------+----------+-----------------------------------------------------------------------------+
 |Configure Environments Here? (Y/N)    | N        | Wenn der Benutzer nicht wünscht, um die Umwelt in der aktuellen Umgebung,   |
 |                                      |          | die sie eingeben können, wie N konfigurieren                                |
 +--------------------------------------+----------+-----------------------------------------------------------------------------+
 |Use existing environment settings?    | Y        | Wenn der Benutzer wünschen, die bestehenden Umgebungseinstellungen          |
 |(Y/N)                                 |          | zu verwenden, sie können Eingang als Y.                                     |
 +--------------------------------------+----------+-----------------------------------------------------------------------------+
 |Use existing environment settings?    | N        | Wenn der Benutzer nicht wünscht, um die vorhandenen Umgebungseinstellungen  |
 |(Y/N)                                 |          | verwenden, können sie Eingang als N.                                        |
 +--------------------------------------+----------+-----------------------------------------------------------------------------+
 |Do you want to add another            | Y        | Wenn der Benutzer wünschen, eine andere Umgebung hinzufügen, können         |
 |environment? (Y/N)                    |          | sie Eingang als Y.                                                          |
 +--------------------------------------+----------+-----------------------------------------------------------------------------+
 |Do you want to add another            | N        | Wenn der Benutzer nicht wünscht, eine andere Umgebung, können sie           |
 |environment? (Y/N)                    |          | Eingang als N. hinzufügen|                                                  |
 +--------------------------------------+----------+-----------------------------------------------------------------------------+


Der folgende Screenshot bildlich repräsentiert die oben genannten Verfahren:

.. code-block:: bash



 kevell@corp:/# ptdeploy envconfig config --keep-current-environments

 Configure Environments Here? (Y/N) 
 y
 Use existing environment settings? (Y/N) 
 y
 Do you want to add another environment? (Y/N) 
 n
 ******************************
 Success
 In Environment Configuration
 ****************************** 




Wie Umgebungskonfiguration löschen
-------------------------------------------------------

Wenn der Benutzer, die Umwelt zu Konfiguration zu löschen muss, können sie geben Sie den folgenden Befehl ein:

.. code-block:: bash

	ptdeploy envconfig del --environment-name="kevells"

Der Benutzer kann den Namen der Umgebung, die sie, wie oben gezeigt, die gelöscht werden soll angeben.

Nach der Eingabe des Befehls oben, werden Sie gefragt,

Schritt 1: Environments löschen Hier?

und zeigt eine Warnmeldung

.. code-block:: bash

 WARNING: Deleting an environment from papyrus is final. You may be looking for boxify box-destroy instead (Y/N) 


The user has to specify Y or N


Schritt 2: Umwelt Kevells (Name der angegebenen Umgebung, die angeblich zu löschen) gefunden. Sind Sie sicher, es zu löschen? (Y / N)

Der Benutzer hat auf Y oder N angeben

Schließlich ist der angegebenen Umgebung gelöscht wird, wie im Screenshot zu sehen.

.. code-block:: bash

 kevell@corp:/# ptdeploy envconfig del --environment-name="kevells"

 Delete Environments Here?
 WARNING: Deleting an environment from papyrus is final. You may be looking for boxify box-destroy instead (Y/N) 
 y
 Environment kevells found. Are you sure you want to delete it? (Y/N) 
 y
 [Pharaoh Logging] Removing environment kevells.
 ****************************
 Success
 In Environment Configuration
 ****************************



Eine weitere Möglichkeit des Löschens wird eine Umgebung, ohne den Namen der Umgebung wird, wie durch Verwendung des Befehls angezeigt:

.. code-block:: bash

	ptdeploy envconfig delete

Nach der Eingabe des Befehls oben, werden Sie gefragt,

Schritt 1: Environments löschen Hier?

und zeigt eine Warnmeldung

.. code-block:: bash

 WARNING: Deleting an environment from papyrus is final. You may be looking for boxify box-destroy instead (Y/N) 

Der Benutzer hat auf Y oder N angeben

Schließlich ist die Umgebung gelöscht wird, wie im Screenshot gezeigt:

.. code-block:: bash

 kevell@corp:/# ptdeploy envconfig delete

 Delete Environments Here?
 WARNING: Deleting an environment from papyrus is final. You may be looking for boxify box-destroy instead (Y/N) 
 y
 Enter Environment Name To delete
 deepak
 Environment deepak found. Are you sure you want to delete it? (Y/N) 
 y
 [Pharaoh Logging] Removing environment deepak.
 ******************************
 Success
 In Environment Configuration
 ****************************** 


Wie Umgebungskonfiguration Liste
--------------------------------------------------

Wenn der Benutzer die Liste der Details in Bezug auf Umwelt-Konfiguration sehen möchten, können sie Eingang wie dargestellt:

.. code-block:: bash

	ptdeploy envconfig list

Nach der Eingabe des Befehls vor, werden dazu aufgefordert,

Liste Environment hier? (Y / N)

wenn der Benutzer als Y gibt, wird die Anzeige der Ausgabe zu erzeugen, wie im Bild gezeigt:

.. code-block:: bash


 kevell@corp:/# ptdeploy envconfig list --yes
 ************************************************

 array(3) {
  [0]=>
  array(2) {
    ["any-app"]=>
    array(2) {
      ["gen_env_name"]=>
      string(13) "default-local"
      ["gen_env_tmp_dir"]=>
      string(5) "/tmp/"
    }
    ["servers"]=>
    array(1) {
      [0]=>
      array(3) {
        ["target"]=>
        string(9) "127.0.0.1"
        ["user"]=>
        string(5) "local"
        ["password"]=>
        string(5) "local"
      }
    }
  }
  [1]=>
  array(2) {
    ["any-app"]=>
    array(2) {
      ["gen_env_name"]=>
      string(18) "default-local-8080"
      ["gen_env_tmp_dir"]=>
      string(5) "/tmp/"
    }
    ["servers"]=>
    array(1) {
      [0]=>
      array(3) {
        ["target"]=>
        string(14) "127.0.0.1:8080"
        ["user"]=>
        string(5) "local"
        ["password"]=>
        string(5) "local"
      }
    }
  }
  [2]=>
  array(2) {
    ["any-app"]=>
    array(2) {
      ["gen_env_name"]=>
      string(6) "deepak"
      ["gen_env_tmp_dir"]=>
      string(5) "/tmp/"
    }
    ["servers"]=>
    array(1) {
      [0]=>
      array(3) {
        ["target"]=>
        string(11) "192.168.1.7"
        ["user"]=>
        string(6) "deepak"
        ["password"]=>
        string(3) "123"
      }
    }
  }
 }

 In Environment Configuration
 ******************************



Alternative Parameter
--------------------------------
 
Statt envconfig können die folgenden Parameter in der Erklärung verwendet werden:

* EnvironmentConfig
* environmentconfig
* environment-config
* env-config


Vorteile
------------

* Es ist gut-to-do in beiden Cent OS und als auch in Ubuntu.
* Die in der Erklärung verwendet muss nicht beachtet werden, welche ein zusätzlicher Vorteil ist, während im Vergleich zu anderen Parametern.
* Dieses Modul führt die Benutzer, wie man die Umgebung zu konfigurieren, wie man die unerwünschten Umgebung zu löschen, wie Sie die Liste 
  Option nutzen Liste der verfügbaren Umgebungen.

