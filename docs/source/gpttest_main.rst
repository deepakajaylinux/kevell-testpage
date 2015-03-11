=========
PTTest
=========

Zusammenfassung
-----------------------

Die pttest zielt auf Testkonfiguration und Ablaufautomatisierung Management mit Hilfe von php.

Es verwenden, gemeinsame Regeln für eine Reihe von Tools und Technologien für die Handhabung der Testsuite Konfiguration und Ausführung.

Es bietet gemeinsame API, um Tests in einer Vielzahl von Sprachen und Test-Tools auszuführen. Der Anwender kann komplexe Testreihen mit wenig oder ohne zusätzliche Konfiguration erforderlich laufen. Es nährt die Benutzer-Tests manuell oder mit einem Betriebssystem und in der Hand gewährleistet die Stabilität der Umwelt.

Es modulare, objektorientierte und erweiterbar. Also, wenn die Benutzer spürt keine zusätzlichen Module nach Bedarf sie einrahmen und fügen ihre eigenen Modul je nach ihren Anforderungen.

Es ist ein Teil des Pharaos Tool-Suite, die das Konfigurationsmanagement, Test Automation-Management, Automated Deployment, Build und Release-Management und vieles mehr, alles in Code implementiert, und alle in PHP umhüllt.


Hilfe Befehl
-------------------

Wenn Sie den Zweck eines bestimmten Moduls wissen möchten, geben Sie einfach den Befehl wie folgt:

.. code-block:: bash

	pttest ModuleName help

Dieser Befehl liefert die Verwendung dieser speziellen Modul und auch die verfügbaren Optionen in Aktionen, die Sie ausführen können. Die unter gezeigt Screenshot erläutert die Verwendung des Moduls Behat unter pttest mit dem Befehl help.

Der Befehl help listet auch die alternativen Parameter, die in der Erklärung verwendet werden kann.

.. code-block:: bash

 kevell@corp:/# pttest Behat help
 ******************************


  This command allows you to initialize a Behat test suite.

  Behat, behat

        - init, initialize
        Initialises the Behat test suite of this project
        example: pttest behat init
        example: pttest behat initialize

        - execute
        Executes the Behat test suite of this project
        example: pttest behat execute

 ------------------------------
 End Help
 ******************************

Installation
----------------

Installieren des pttest können auf zwei Arten in Abhängigkeit von der Verfügbarkeit und Anforderungen der Anwender durchgeführt werden. Diese beiden Möglichkeiten des Einrichtens pttest sind:

* Installieren pttest über ptconfigure
* Installation des pttest ohne Abhängigkeit von ptconfigure.

Installieren pttest über ptconfigure
---------------------------------------------

Wenn der Benutzer die ptconfigure in ihrer Maschine, dann ist es die einfacheren Weg, um pttest mit dem folgenden Befehl installiert werden:

.. code-block:: bash

	sudo ptconfigure pttest install --yes --guess

Installieren des pttest ohne Abhängigkeit von ptconfigure
------------------------------------------------------------

Wenn der Benutzer wünschen, die pttest ohne abhängig und mit dem ptconfigure sie mit dem folgenden Befehl installieren:

.. code-block:: bash

	sudo apt-get install php5 git

.. code-block:: bash

	git clone https://github.com/phpengine/pttest && sudo php pttest/install-silent

or

Die folgende Befehl ist vorhersehbar für die Benutzer, um die Position während der Installation angeben möchten.

.. code-block:: bash

	git clone https://github.com/phpengine/pttest && sudo php pttest/install

So verwenden und Verfügbare Module
------------------------------------

Lassen Sie uns sehen, wie man die pttest Tool, zuerst, geben Sie einfach als

.. code-block:: bash

	pttest

dieser Befehl die Namen der Module, die unter pttest sind, aus. Der folgende Screenshot zeigt, dass visuell.

.. code-block:: bash

 kevell@corp:/# pttest
 ******************************


 PTTest by Golden Contact Computing
 -------------------

 About:
 -----------------
 PTTest is for Test Automation. It can be used to generate starter test suites for your applications,
 and automated test execution scripts within minutes.

 By providing an common API by which to execute tests in a wide range
 of languages and test tools, you can run complex test suites across a range of platforms with little to no
 extra configuration.

 -------------------------------------------------------------

 Available Commands:
 ---------------------------------------

 Autopilot - PTConfigure Autopilot - User Defined Installations
 Behat - Behat - Initialize or Execute a Behat Test Suite
 Cucumber - Cucumber - Initialize or Execute a Cucumber Test Suite
 EnvironmentConfig - Environment Configuration - Configure Environments for a project
 PHPUnit - PHPUnit - Initialize or Execute a PHPUnit Test Suite
 SystemDetection - System Detection - Detect the Running Operating System
 Templating - Templating
 Testify - Testifyer - Creates default tests for your project

 ******************************



Das Spiel mit PTTest Module

.. toctree::
   :maxdepth: 6


 gbehat_test
 gcucumber_test
 genvironmentconfig_test
 gphpunit_test
 gsystemdetection_test
 gtemplating_test
