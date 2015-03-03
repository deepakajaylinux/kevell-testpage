=========
RubyBDD
=========

Zusammenfassung
----------------------

Rubin Behaviour Driven Development (BDD) gibt Ihnen das Beste von Test Driven Development, Domain Driven Design und Acceptance Test Driven Planning-Techniken, so dass der Benutzer Rubin BDD für bessere Software mit selbsterklärend, ausführbare Tests, die Anwendern und Entwicklern zusammen zu bringen installieren mit einem PHP-Sprache. Es tröstet mit Ubuntu und Cent OS.

Hilfe Befehl
------------------------

Der Befehl help führt die Benutzer über den Zweck und als auch über die Möglichkeiten, die in den Rubin Bdd Module enthalten sind. Der Befehl help listet einige der alternativen Parameter von Ruby Bdd unter ptconfigure Modul. Es beschreibt auch die Syntax für die Installation updation des Benutzers. Der Befehl help für Ruby Bdd ist nachfolgend dargestellt.

.. code-block:: bash

		ptconfigure Ruby Bdd help

Der folgende Screenshot zeigt den vollen Einsatz von Ruby Bdd.

.. code-block:: bash

 kevell@corp:/# ptconfigure RubyBDD help

 ******************************


  This command allows you to install Ruby RVM.

  RubyBDD, rubybdd, ruby-bdd

        - install
        Installs Ruby BDD Gems
        example: ptconfigure ruby-bdd install

 ------------------------------
 End Help
 ******************************

Installation
-------------------

Die Installation umfasst die Installation von Ruby Bdd erforderlich, um die Installation in einer aktualisierten Version zu machen. Es ist ein Prozess manifest Ruby Bdd Modul unter ptconfigure installieren, indem einfach mit dem Befehl unten angegeben,

.. code-block:: bash

	ptconfigure Ruby Bdd Install

Nach beleben den Befehl geben Sie den Wert katechisieren.

Wenn die Benutzereingaben wie ja es wird automatisch Rubin Bdd mit der Überprüfung aus dem System zu installieren. Wenn nicht beenden Sie die Installation. Der folgende Screenshot zeigt es.

.. code-block:: bash

 kevell@corp:/# ptconfigure ruby-bdd install

 Install Ruby BDD? (Y/N)
 Y
 *******************************
 *        Pharaoh Tools        *
 *          !Ruby BDD!!        *
 *******************************
 ERROR:  Error installing cucumber:
	ERROR: Failed to build gem native extension.

        /usr/bin/ruby1.9.1 extconf.rb
 /usr/lib/ruby/1.9.1/rubygems/custom_require.rb:36:in `require': cannot load such file -- mkmf (LoadError)
	from /usr/lib/ruby/1.9.1/rubygems/custom_require.rb:36:in `require'
	from extconf.rb:1:in `<main>'


 Gem files will remain installed in /var/lib/gems/1.9.1/gems/gherkin-2.12.2 for inspection.
 Results logged to /var/lib/gems/1.9.1/gems/gherkin-2.12.2/ext/gherkin_lexer_ar/gem_make.out
 INFO:  `gem install -y` is now default and will be removed
 INFO:  use --ignore-dependencies to install only the gems you list
 Building native extensions.  This could take a while...
 [Pharaoh Logging] Adding Package cucumber from the Packager Gem did not execute correctly
 ERROR:  Error installing capybara:
	ERROR: Failed to build gem native extension.

        /usr/bin/ruby1.9.1 extconf.rb
 /usr/lib/ruby/1.9.1/rubygems/custom_require.rb:36:in `require': cannot load such file -- mkmf (LoadError)
	from /usr/lib/ruby/1.9.1/rubygems/custom_require.rb:36:in `require'
	from extconf.rb:4:in `<main>'


 Gem files will remain installed in /var/lib/gems/1.9.1/gems/nokogiri-1.6.6.2 for inspection.
 Results logged to /var/lib/gems/1.9.1/gems/nokogiri-1.6.6.2/ext/nokogiri/gem_make.out
 INFO:  `gem install -y` is now default and will be removed
 INFO:  use --ignore-dependencies to install only the gems you list
 Building native extensions.  This could take a while...
 [Pharaoh Logging] Adding Package capybara from the Packager Gem did not execute correctly
 ERROR:  While executing gem ... (Gem::DependencyError)
     Unable to resolve dependencies: calabash-android requires rubyzip (~> 0.9.9); xamarin-test-cloud requires rubyzip (~> 1.1)
 INFO:  `gem install -y` is now default and will be removed
 INFO:  use --ignore-dependencies to install only the gems you list
 [Pharaoh Logging] Adding Package calabash from the Packager Gem did not execute correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************
 

 Single App Installer:
 --------------------------------------------
 RubyBDD: Success
 ------------------------------
 Installer Finished
 ******************************

Option
---------------


.. cssclass:: table-bordered

 +----------------------+---------------------------------------+-------------+------------------------------------------+
 | Parameters           | Alternate Parameters                  | Optionen    | Kommentare                               |
 +======================+=======================================+=============+==========================================+
 |Install RubyBdd?(Y/N) | Anstelle der Verwendung RubyBdd wir   | Y           | es installiert RubyBdd unter ptconfigure |
 |                      | verwenden können, ruby-bdd,rubybdd    |             | in Pharaoh tools                         |
 +----------------------+---------------------------------------+-------------+------------------------------------------+
 |Install RubyBdd?(Y/N) | Anstelle der Verwendung RubyBdd wir   | N           | Das System Ausfahrt die Installation     |
 |                      | verwenden können, ruby-bdd,rubybdd|   |             |                                          |
 +----------------------+---------------------------------------+-------------+------------------------------------------+

Vorteile
----------------


* Rubybdd ist gut-to-do in Ubuntu und CentOS
* Rubybdd unterstützt Nicht Groß- und Kleinschreibung
* Rubybdd ist flexibel
* Ein weiterer großer Vorteil, um mit BDD sind die getriebenen Entwicklung - der Benutzer kann als neueste Version von rubybdd und Patch-Level 
  zu aktualisieren, der Rubin.
* Rubybdd für die Installation verwendet


