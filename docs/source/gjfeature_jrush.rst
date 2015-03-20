==========
JFeature
==========

Zusammenfassung
-----------------

JFeatures ist eines der weltweit beliebtesten Software-Pakete zu erstellen, organisieren, verwalten und Veröffentlichen von Inhalten für Websites, Blogs, Intranets verwendet. Wenn der Benutzer drücken Sie die Zip-Datei in eine andere Datei werden alle Funktionen hinzugefügt werden. Aufgrund seiner skalierbaren Architektur ist es auch ein guter Ausgangspunkt, um Webanwendungen zu erstellen. Es verwendet für die Komponente der Bühne Migration zu verwalten. Es Bequemlichkeit mit Ubuntu und CentOS.


Hilfe Befehl
----------------------

Der Help-Befehl führt die Benutzer über den Zweck und auch als zu den Optionen, die in das JFeatures-Modul enthalten sind. Es listet die alternative Ausgabeparameter des JFeatures-Moduls. Es beschreibt auch die Syntax für die Installation des JFeatures-Moduls. Der Help-Befehl für JFeatures-Modul wird gezeigt wie unten beschrieben.


.. code-block:: bash

	ptconfigure JFeatures help

Die Syntax zum Deklarieren des Help-Befehls ist nicht-Groß-/Kleinschreibung beachtet das ein Vorteil ist. Der folgende Screenshot visualisieren den Benutzer über den Befehl "Help" unter JFeatures.



.. code-block:: bash

 kevell@corp:/# jrush JFeature help
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

  This command manages the JFeature Component for Stage Migration.

  JFeature, jfeature

        - folder-defaults
          Reset the feature file storage folders being used to the default
          example jrush jfeature folder-defaults --config-file="/var/www/website/configuration.php"

        - feature-install
          Install the metadata for a database migration, fileset, or both from the GC Features component
          example jrush jfeature feature-install --feature-file="/var/www/website/XXX_XXX.zip" --config-file="/var/www/website/configuration.php"

        - feature-pull
          perform a pull on an installed feature so it is integrated into the site, db and file changes executed.
          example jrush jfeature feature-pull --pull-unique-time="XXX_XXX" --config-file="/var/www/website/configuration.php"
          example jrush jfeature feature-pull --pull-id="XX" --config-file="/var/www/website/configuration.php"

        - feature-push
          perform a push on an installed feature so it is saved locally.
          example jrush jfeature feature-push --profile-unique="XXX" --config-file="/var/www/website/configuration.php" --push-type="local"

        - group-install
          Install the metadata for a database migration, fileset, or both from the GC Features component
          example jrush jfeature group-install --group-file="/var/www/website/XXXX.group" --config-file="/var/www/website/configuration.php"

        - group-install-all
          Install the metadata for a database migration, fileset, or both from the GC Features component. Will scan the configured metadata
          Directory for group files, and install or update all found groups.
          example jrush jfeature group-install-all --config-file="/var/www/website/configuration.php"

        - group-push
          perform a push of a group profile into a locally saved file.
          example jrush jfeature group-push --group-unique="XXXXXXXXXXXXXXXX" --config-file="/var/www/website/configuration.php"

        - group-pull
          perform a pull on all installed features in the specified group so they are integrated into the site, db and
          file changes executed.
          example jrush jfeature group-pull --group-id="XX" --config-file="/var/www/website/configuration.php"
          example jrush jfeature group-pull --group-name="my group" --config-file="/var/www/website/configuration.php"
          example jrush jfeature group-pull --group-unique="XX1234" --config-file="/var/www/website/configuration.php"

 ------------------------------
 End Help
 ****************************************



Alternative Parameter
-----------------------------------

Im folgenden sind die alternative Parameter, die in Deklarationen definiert werden können:


JFeature, jfeature


Folder-default
----------------------

Dieser Prozeß verwendet, um die Standardeinstellung für Datei-Speicherordner festlegen. Eine Voreinstellung oder Wert, der verwendet wird, wenn keine andere Wahl im Ordner erfolgt. Interaktion mit dem Benutzer sollte verlangt werden. Standardeinstellung für die am häufigsten ausgewählten Optionen dient diesem Zweck.


Der Help-Befehl für Ordner-Standardprozess wird angezeigt, wie unten beschrieben.


.. code-block:: bash

	 Jrush JFeature folder-defaults

Der folgende Screenshot zeigt seine Funktion.


.. code-block:: bash

 	folder-defaults
        Reset the feature file storage folders being used to the default
        example jrush jfeature folder-defaults --config-file="/var/www/website/configuration.php"


Feature-install
----------------------

Dieser Prozeß verwendet, um die Metadaten für eine Datenbankmigration installieren. Hier fragt er die Funktion Datei und konfigurierte Dateiname. Der Benutzer muss die vorstehenden Angaben einzeln eingeben. Andernfalls kann der Benutzer wie alles in derselben Zeile eingeben. Der folgende Befehl wird verwendet, um Jfeature zu installieren.


.. code-block:: bash

	 Jrush JFeature feature-install


Der Screenshot zeigt seine Funktionen.


.. code-block:: bash

       feature-install
       Install the metadata for a database migration, fileset, or both from the GC Features component
       example jrush jfeature feature-install --feature-file="/var/www/website/XXX_XXX.zip" --config-file="/var/www/website/configuration.php"


Feature-Pull
-------------------

Feature Pull dient zum einen Zug eines installierten Features durchführen. Durch Integration können Änderungen an der Datei ausgeführt werden.Der folgende Befehl kann verwendet werden, um Konfigurationsdatei zu ziehen.


.. code-block:: bash

	 Jrush JFeature feature-pull


Nach den oben genannten Befehl eingeben, fragt er nach Ip-Adresse und Uhrzeit. Auf dieser Basis Pull ausgeführt werden kann. Der folgende Screenshot erklären seine Funktion.


.. code-block:: bash

	feature-pull
        perform a pull on an installed feature so it is integrated into the site, db and file changes executed.
        example jrush jfeature feature-pull --pull-unique-time="XXX_XXX" --config-file="/var/www/website/configuration.php"
        example jrush jfeature feature-pull --pull-id="XX" --config-file="/var/www/website/configuration.php"

Feature-Push
--------------------

Verfügen Sie über Push verwendet, um einen Druck auf eines installierten Features erreicht. Abschluss drängen kann es lokal gespeichert werden. Der Befehl verwendet, um das Feature zu schieben.


.. code-block:: bash

	 Jrush JFeature feature-push


Nach Eingabe der oben genannten Befehl fragt es Profil einzigartig und Konfigurations-Datei und drücken den. Der Benutzer hat eins nach dem anderen oder alles in derselben Zeile eingeben. Dies kann wie folgt über Snapshots erklärt werden,


.. code-block:: bash

 	feature-push
        perform a push on an installed feature so it is saved locally.
        example jrush jfeature feature-push --profile-unique="XXX" --config-file="/var/www/website/configuration.php" --push-type="local"

Group-install
-------------------

Dieser Prozeß verwendet, um die Metadaten für eine Datenbankmigration installieren. Hier fragt es Feature Gruppe Datei und konfigurierte Dateiname. Der Benutzer muss die vorstehenden Angaben einzeln eingeben. Andernfalls kann der Benutzer wie alles in derselben Zeile eingeben.


.. code-block:: bash

	 Jrush JFeature group-install

Der Screenshot zeigt seine Funktionen.



.. code-block:: bash

	group-install
        Install the metadata for a database migration, fileset, or both from the GC Features component
        example jrush jfeature group-install --group-file="/var/www/website/XXXX.group" --config-file="/var/www/website/configuration.php"


Group-install-all
-----------------------------

Legen Sie diesen Prozess verwendet, um Metadaten für Datenbank-Migration-Datei zu installieren. Gruppe Konfigurationskomponente Funktionen. Installation und Updation ist möglich. Der folgende Befehl verwendet, um die Gruppe zu installieren.


.. code-block:: bash

	 Jrush JFeature group-install-all


Betreten den oben genannten Befehl, dass es fragt Konfigurationsdatei. Der Benutzer kann der Name eingeben. Der folgende Screenshot Führer des Benutzers zum Installieren von Gruppe alle.



.. code-block:: bash

	group-install-all
        Install the metadata for a database migration, fileset, or both from the GC Features component. Will scan the configured metadata
        Directory for group files, and install or update all found groups.
        example jrush jfeature group-install-all --config-file="/var/www/website/configuration.php"



Group-push
-----------------

Dieser Prozeß kann eine Anstrengung eines Gruppe-Profils in lokale Datei ausführen. Hier können die Gruppe einzigartig und der Konfigurationsdateiname genannt werden. Der folgende Befehl verwendet werden, das Profil der Gruppe in lokal-Datei gespeichert.



.. code-block:: bash

	 Jrush JFeature group-push

Der folgende Screenshot Führer des Benutzers zur Gruppe Push Installation.

.. code-block:: bash

	 group-push
         perform a push of a group profile into a locally saved file.
         example jrush jfeature group-push --group-unique="XXXXXXXXXXXXXXXX" --config-file="/var/www/website/configuration.php"


Vorteile
-----------------

* Gut für alle Arten von Benutzern unterstützt 
* einfach zu Upgrades 
* Suche besser, intelligenter Suche 
* leistungsfähige Erweiterbarkeit 
* tun mehr mit weniger Zeit verbringen, die für die Kodierung und tun mehr mit weniger Jfeature Befehle 
* gut zu tun mit Ubuntu und Cent OS 
* nicht Groß-/Kleinschreibung



