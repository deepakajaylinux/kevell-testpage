==============
Builderfyer
==============

Zusammenfassung
------------------

Builderfyer bietet dem Anwender einige Standard- Autopiloten für Ihr Projekt zu erstellen. Mit anderen Worten builderfy bietet Ihnen die Möglichkeit, bauen Arbeitsplätze jenkins , die für Ihr Projekt konfiguriert sind, zu implementieren.


Hilfe Befehl
---------------

Der Befehl help ist eine kurze und sowie interessante Zusammenfassung für den Benutzer. Sie bietet Informationen über seine wichtige Rolle , Angaben zum abweichenden Parameter, die in Erklärungen verwendet werden kann. Die Hilfe -Option erklärte Syntax ist unten angegeben ,

.. code-block:: bash

	ptdeploy builderfy help

Die bildliche Darstellung der obigen Befehl aufgelistet unten ,

.. code-block:: bash

 kevell@corp:/# ptdeploy builderfy help
 ******************************


  This is a default Module and provides you a way to deploy build jobs to jenkins that are configured for your project.

  Builderfy, builderfy

        - developer
        Create a developers build for this project
        example: ptdeploy builderfy developer
        example: ptdeploy builderfy developer
                    --yes
                    --guess (optional)
                    --project-description="A description for the project"
                    --github-url="http://www.github.com/phpengine/ptdeploy"
                    --source-branch-spec="origin/master" # guess will assume origin/master
                    --source-scm-url="/var/www/application" # guess will assume the current directory
                    --days-to-keep="10" # guess will assume -1 (to ignore this value)
                    --num-to-keep="100" # guess will assume 15
                    --autopilot-install="/path/to/installer/autopilot" # guess will assume "build/config/ptdeploy/autopilots/autopilot-dev- 
 jenkins-install.php"
                    --autopilot-uninstall="/path/to/uninstaller/autopilot" # guess will assume "build/config/ptdeploy/autopilots/autopilot-dev-
 jenkins-uninstall.php"
                    --target-scm-url="http://www.github.com/phpengine/ptdeploy" #  guess will use your github url
                    --target-branch="master" # guess will default to master

        - manual-staging
        Create a build which will manually deploy to staging and optionally test this project.
        example: ptdeploy builderfy manual-staging

        - continuous-staging
        Create a build which will test and automatically deploy to staging for this project, triggered by SCM Changes.
        example: ptdeploy builderfy continuous-staging

        - manual-production
        Create a build which will manually deploy to production for this project. It deploys straight to production, so
        will not test first.
        example: ptdeploy builderfy manual-staging

        - continuous-staging-to-production
        Create a continuous build job for this project, which will automatically deploy and test SCM Changes to the
        staging server, and upon successful testing will also deploy those changes to production.
        example: ptdeploy builderfy continuous-staging-to-production
        ptdeploy builderfy continuous --yes --jenkins-home="/var/lib/jenkins" --target-job-name="my-project-continuous" --project-
 description="This is the Continuous Delivery build for My Project" --primary-scm-url="http://146.185.129.66:8080/git/root/first-pharaoh-
 cd.git" --source-branch-spec="origin/master" --source-scm-url="http://146.185.129.66:8080/git/root/first-pharaoh-cd.git" --days-to-keep="-1" 
 --amount-to-keep="10" --autopilot-test-invoke-install-file="build/config/ptdeploy/autopilots/tiny-staging-invoke-code-no-dbconf.php" -- 
 autopilot-prod-invoke-install-file="build/config/ptdeploy/autopilots/tiny-prod-invoke-code-no-dbconf.php" --error-
 email="phpengine@hotmail.co.uk" --only-autopilots

        also --no-autopilots to just install the build

        
 --------------
  Drupal Module:

  The Drupal module extends Builderfy by providing Templates for both the build and the autopilot to execute them from

  This module adds the 'drupal' action to builderfy and will let you produce autopilots for it are tailored to Drupal.

  // builderfy - create templates to install build
  sudo ptdeploy builderfy drupal --yes --jenkins-home="/var/lib/jenkins" --target-job-name="my-project-continuous" --project-description="This 
 is the Continuous Delivery build for My Project" --primary-scm-url="http://146.185.129.66:8080/git/root/first-pharaoh-cd.git" --source-branch-
 spec="origin/master" --source-scm-url="http://146.185.129.66:8080/git/root/first-pharaoh-cd.git" --days-to-keep="-1" --amount-to-keep="10" --
 autopilot-test-invoke-install-file="build/config/ptdeploy/autopilots/tiny-staging-invoke-code-no-dbconf.php" --autopilot-prod-invoke-install- 
 file="build/config/ptdeploy/autopilots/tiny-prod-invoke-code-no-dbconf.php" --error-email="phpengine@hotmail.co.uk" --only-autopilots

  // execute the build creator - you'll be using your jenkins/build environment here
  ptdeploy autopilot execute build/config/ptdeploy/builderfy/autopilots/*environment-name*-drupal-invoke-continuous.php

 --------------
  Joomla Module:

  The Joomla module extends Builderfy by providing Templates for both the build and the autopilot to execute them from

  This module adds the 'joomla' action to builderfy and will let you produce autopilots for it are tailored to Joomla.

  // builderfy - create templates to install build
  sudo ptdeploy builderfy joomla --yes --jenkins-home="/var/lib/jenkins" --target-job-name="my-project-continuous" --project-description="This 
 is the Continuous Delivery build for My Project" --primary-scm-url="http://146.185.129.66:8080/git/root/first-pharaoh-cd.git" --source-branch-
 spec="origin/master" --source-scm-url="http://146.185.129.66:8080/git/root/first-pharaoh-cd.git" --days-to-keep="-1" --amount-to-keep="10" --
 autopilot-test-invoke-install-file="build/config/ptdeploy/autopilots/tiny-staging-invoke-code-no-dbconf.php" --autopilot-prod-invoke-install- 
 file="build/config/ptdeploy/autopilots/tiny-prod-invoke-code-no-dbconf.php" --error-email="phpengine@hotmail.co.uk" --only-autopilots

  // execute the build creator - you'll be using your jenkins/build environment here
  ptdeploy autopilot execute build/config/ptdeploy/builderfy/autopilots/*environment-name*-joomla-invoke-continuous.php

 --------------
  Wordpress Module:

  The Wordpress module extends Builderfy by providing Templates for both the build and the autopilot to execute them from

  This module adds the 'wordpress' action to builderfy and will let you produce autopilots for it are tailored to Wordpress.

  // builderfy - create templates to install build
  sudo ptdeploy builderfy wordpress --yes --jenkins-home="/var/lib/jenkins" --target-job-name="my-project-continuous" --project-
 description="This is the Continuous Delivery build for My Project" --primary-scm-url="http://146.185.129.66:8080/git/root/first-pharaoh-
 cd.git" --source-branch-spec="origin/master" --source-scm-url="http://146.185.129.66:8080/git/root/first-pharaoh-cd.git" --days-to-keep="-1" 
 --amount-to-keep="10" --autopilot-test-invoke-install-file="build/config/ptdeploy/autopilots/tiny-staging-invoke-code-no-dbconf.php" --
 autopilot-prod-invoke-install-file="build/config/ptdeploy/autopilots/tiny-prod-invoke-code-no-dbconf.php" --error- 
 email="phpengine@hotmail.co.uk" --only-autopilots

  // execute the build creator - you'll be using your jenkins/build environment here
  ptdeploy autopilot execute build/config/ptdeploy/builderfy/autopilots/*environment-name*-wordpress-invoke-continuous.php

 ------------------------------
 End Help
 ******************************


manual-production
--------------------

Die Produktion builderfy Option Hand wird verwendet, um einen Build , die von Hand bis zur Produktion für dieses Projekt bereitstellen schaffen . Es setzt direkt auf die Produktion , so dass nicht zu testen. Der Befehl für die manuelle Fertigung ist unten angegeben ,

.. code-block:: bash

	ptdeploy builderfy manual-production

Die bildliche Darstellung der obigen Befehl aufgelistet unten ,


.. code-block:: bash


 kevellcorp:/# ptdeploy builderfy manual-production
 Install Builderfy? (Y/N) 
 y
 *******************************
 *   Golden Contact Computing  *
 *           Builderfy!          *
 *******************************
 Enter the data handling type
 (0) code 
 (1) replication 
 (2) capture 
 0
 checkWhat is your Jenkins home? Found "/var/lib/jenkins" - use this?

 What is the target Job Name?
 my-project-continuous
 Enter a description for your project
 This is the continuous delivery for my project
 Enter a Primary SCM URL for your project
 http://146.185.129.66:8080/git/root/first-pharaoh-cd.git
 Enter a Source Branch Spec for your project
 origin/master
 Enter a Source SCM URL for your project
 http://146.185.129.66:8080/git/root/first-pharaoh-cd.git
 Enter the number of days to keep builds for
 1
 Enter the max number of builds results to keep
 10
 Enter the path of the autopilot prod environment invoke install file (Relative to project root)
 build/config/ptdeploy/autopilots/tiny-staging-invoke-code-no-dbconf.php
 Enter the path of the autopilot prod environment invoke with DB Config install file (Relative to project root)
 build/config/ptdeploy/autopilots/tiny-staging-invoke-code-no-dbconf.php
 Enter the path of the autopilot prod environment invoke with DB Install file (Relative to project root)
 build/config/ptdeploy/autopilots/tiny-staging-invoke-code-no-dbconf.php
 Enter the data handling type
 (0) code 
 (1) replication 
 (2) capture 
 0
 Enter build failure Email address. Whitespace-separated list of recipient addresses
 phpengine@hotmail.co.uk
 Copying Files...
 Enter the data handling type
 (0) code 
 (1) replication 
 (2) capture 
 0
 Changing Folder Permissions...
 Changing Folder Owner...
 Changing Folder Group...
 ... All done!
 *******************************
 Thanks for installing , visit www.gcsoftshop.co.uk for more
 ****************************** 


 Success
 In Builderfy
 ******************************



Continuos-staging Wordpress
-------------------------------

Die kontinuierliche Inszenierung wird verwendet, um einen Build , die Probe stellen wird und automatisch an die Inszenierung für dieses Projekt, das von SCM Änderungen ausgelöst Bereitstellung erstellen. Die folgende Befehl zeigt, wie der " Wordpress " Aktion builderfy hinzuzufügen und lassen Sie produzieren Autopiloten für sie werden , um Wordpress zugeschnitten.

.. code-block:: bash

	ptdeploy builderfy continuous-wordpress

Die bildliche Darstellung der obigen Befehl aufgelistet unten ,



.. code-block:: bash


 kevellcorp:/# ptdeploy builderfy continuous-wordpress
 Install Builderfy? (Y/N) 
 y
 *******************************
 *   Golden Contact Computing  *
 *           Builderfy!          *
 *******************************
 Enter the data handling type
 (0) code 
 (1) replication 
 (2) capture 
 0
 checkWhat is your Jenkins home? Found "/var/lib/jenkins" - use this?

 What is the target Job Name?
 my-project-continuous
 Enter a description for your project
 This is the Continuous Delivery build for My Project
 Enter a Primary SCM URL for your project
 http://146.185.129.66:8080/git/root/first-pharaoh-cd.git
 Enter a Source Branch Spec for your project
 origin/master
 Enter a Source SCM URL for your project
 http://146.185.129.66:8080/git/root/first-pharaoh-cd.git
 Enter the number of days to keep builds for
 1
 Enter the max number of builds results to keep
 10
 Enter the path of the autopilot test environment invoke install file (Relative to project root)
 build/config/ptdeploy/autopilots/tiny-staging-invoke-code-no-dbconf.php
 Enter the path of the autopilot prod environment invoke install file (Relative to project root)
 build/config/ptdeploy/autopilots/tiny-staging-invoke-code-no-dbconf.php
 Enter the data handling type
 (0) code 
 (1) replication 
 (2) capture 
 0
 Enter build failure Email address. Whitespace-separated list of recipient addresses
 phpengine@hotmail.co.uk
 Copying Files...
 Enter the data handling type
 (0) code 
 (1) replication 
 (2) capture 
 0
 Changing Folder Permissions...
 Changing Folder Owner...
 Changing Folder Group...
 ... All done!
 *******************************
 Thanks for installing , visit www.gcsoftshop.co.uk for more
 ****************************** 


 Success
 In Builderfy
 ******************************



Continuous-staging Drupal
---------------------------

Die kontinuierliche Inszenierung wird verwendet, um einen Build , die Probe stellen wird und automatisch an die Inszenierung für dieses Projekt, das von SCM Änderungen ausgelöst Bereitstellung erstellen. Die folgende Befehl zeigt, wie die ' Drupal ' Aktion builderfy hinzuzufügen und lassen Sie Autopiloten produzieren dafür sind drupal zugeschnitten.


.. code-block:: bash

        ptdeploy builderfy continuous-wordpress


Die bildliche Darstellung der obigen Befehl aufgelistet unten ,


.. code-block:: bash

 kevellcorp:/# ptdeploy builderfy continuous-drupal
 Install Builderfy? (Y/N) 
 y
 *******************************
 *   Golden Contact Computing  *
 *           Builderfy!          *
 *******************************
 Enter the data handling type
 (0) code 
 (1) replication 
 (2) capture 
 0
 checkWhat is your Jenkins home? Found "/var/lib/jenkins" - use this?

 What is the target Job Name?
 my-project-continuous
 Enter a description for your project
 This is the Continuous Delivery build for My Project
 Enter a Primary SCM URL for your project
 http://146.185.129.66:8080/git/root/first-pharaoh-cd.git
 Enter a Source Branch Spec for your project
 origin/master
 Enter a Source SCM URL for your project
 http://146.185.129.66:8080/git/root/first-pharaoh-cd.git
 Enter the number of days to keep builds for
 1
 Enter the max number of builds results to keep
 10
 Enter the path of the autopilot test environment invoke install file (Relative to project root)
 build/config/ptdeploy/autopilots/tiny-staging-invoke-code-no-dbconf.php
 Enter the path of the autopilot prod environment invoke install file (Relative to project root)
 build/config/ptdeploy/autopilots/tiny-staging-invoke-code-no-dbconf.php
 Enter the data handling type
 (0) code 
 (1) replication 
 (2) capture 
 0
 Enter build failure Email address. Whitespace-separated list of recipient addresses
 phpengine@hotmail.co.uk
 Copying Files...
 Enter the data handling type
 (0) code 
 (1) replication 
 (2) capture 
 0
 Changing Folder Permissions...
 Changing Folder Owner...
 Changing Folder Group...
 ... All done!
 *******************************
 Thanks for installing , visit www.gcsoftshop.co.uk for more
 ******************************


 Success
 In Builderfy
 ******************************


Continuous-staging Joomla
----------------------------

Die kontinuierliche Inszenierung wird verwendet, um einen Build , die Probe stellen wird und automatisch an die Inszenierung für dieses Projekt, das von SCM Änderungen ausgelöst Bereitstellung erstellen. Die folgende Befehl zeigt, wie die " joomla " Aktion builderfy hinzuzufügen und lassen Sie Autopiloten produzieren dafür sind joomla zugeschnitten.

.. code-block:: bash

	ptdeploy builderfy continuous-joomla


Die bildliche Darstellung der obigen Befehl aufgelistet unten ,


.. code-block:: bash

 kevell@corp:/# ptdeploy builderfy continuous-joomla
 Install Builderfy? (Y/N) 
 y
 *******************************
 *   Golden Contact Computing  *
 *           Builderfy!          *
 *******************************
 Enter the data handling type
 (0) code 
 (1) replication 
 (2) capture 
 0
 checkWhat is your Jenkins home? Found "/var/lib/jenkins" - use this?

 What is the target Job Name?
 my-project-continuous
 Enter a description for your project
 This is the Continuous Delivery build for My Project
 Enter a Primary SCM URL for your project
 http://146.185.129.66:8080/git/root/first-pharaoh-cd.git
 Enter a Source Branch Spec for your project
 origin/master
 Enter a Source SCM URL for your project
 http://146.185.129.66:8080/git/root/first-pharaoh-cd.git
 Enter the number of days to keep builds for
 1
 Enter the max number of builds results to keep
 10
 Enter the path of the autopilot test environment invoke install file (Relative to project root)
 build/config/ptdeploy/autopilots/tiny-staging-invoke-code-no-dbconf.php
 Enter the path of the autopilot prod environment invoke install file (Relative to project root)
 build/config/ptdeploy/autopilots/tiny-staging-invoke-code-no-dbconf.php
 Enter the data handling type
 (0) code 
 (1) replication 
 (2) capture 
 0
 Enter build failure Email address. Whitespace-separated list of recipient addresses
 phpengine@hotmail.co.uk
 Copying Files...
 Enter the data handling type
 (0) code 
 (1) replication 
 (2) capture 
 0
 Changing Folder Permissions...
 Changing Folder Owner...
 Changing Folder Group...
 ... All done!
 *******************************
 Thanks for installing , visit www.gcsoftshop.co.uk for more
 ******************************


 Success
 In Builderfy
 ******************************


Alternative Parameter
--------------------------

Es gibt zwei alternative Parameter verwendet werden kann,

Builderfy, builderfy


Vorteile
----------

* Frühere Return on Investment für jedes Feature , nachdem es entwickelt wird , wodurch die Notwendigkeit für große Kapitalinvestitionen 
  reduziert
* Frühere Feedback von den Benutzern über alle neuen Funktionen , wie es um die Produktion freigegeben wird , die Techniken wie parallel 
  (oder A / B) Tests, um festzustellen, welche von zwei möglichen Umsetzung von den Nutzern bevorzugt, bietet
* Minimierung der Durchlaufzeit .
