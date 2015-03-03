==========
Process
==========

Zusammenfassung
-------------------------

Dieses Modul unterstützt die Anwender bei der Handhabung einer erforderlichen Prozessfunktionen, aber auch um einen Prozess zu töten. Der Benutzer kann den bestimmten Prozeß auf der Basis ihrer Anforderungen zu spezifizieren. Der Benutzer kann den Namen des Prozesses, die Datei oder das Verzeichnis entweder lokal oder in einem Remote-Computer angeben. Lassen Sie uns sehen, den Einsatz und Methoden daran beteiligt.

Hilfe Befehl
--------------

Der Befehl help dient den Anwendern darüber, wie zu handhaben und mit Verfahren nach ihren Bedürfnissen zu arbeiten. Es listet auch die alternativen Parameter Prozess. Es beschreibt die Syntax für das Töten eines Prozesses und auch zum Töten eines Prozesses auf der Grundlage der Bedürfnisse an. Der Befehl help zur Prozessmodul wie unten gezeigt.

.. code-block:: bash

		ptconfigure process help

Der folgende Screenshot, wie unten dargestellt, zeigt, wie man einen Prozess zu beenden, und wie Sie definieren einen Prozess zu töten.

Wie zu definieren und um den Prozess zu verwenden
----------------------------------------------------

Um einen Prozess der folgenden Syntax kann verwendet werden, zu töten.

.. code-block:: bash

		ptconfigure process kill

or

.. code-block:: bash

		ptconfigure process kill --yes --name="selenium" --use-psax # default

Die Syntax wie oben gezeigt sucht String in Folge.

.. code-block:: bash

		ptconfigure process kill --yes --name="selenium" --use-pkill #

Die Syntax wie oben gezeigt, wird festgelegt, oder einen String, um getötet zu werden ist.

.. code-block:: bash

		ptconfigure process kill --yes
				--guess
				id="1234 # 

Der Befehl wie oben gezeigt tötet einen Prozess nach der angegebenen ID.

.. code-block:: bash

		ptconfigure process kill --yes
			--level #


Wie oben wird der Befehl verwendet, um ein Verfahren nach dem angegebenen Level zu töten.

.. code-block:: bash

	ptconfigure process kill --yes --guess --name="skype"

Wie oben wird der Befehl verwendet, um einen Prozess, indem Sie seinen Namen zu töten. Der folgende Screenshot zeigt die Arbeitsweise eines Verfahrens zu töten.

Das Töten eines Prozesses mit einem PID
-----------------------------------------------

Wenn der PID # 3486 wird dem lighttpd Prozess zugeordnet. Um den lighttpd-Server zu töten, müssen Sie eine PID übergeben, wie folgt:

.. code-block:: bash

 # kill 3486

or

.. code-block:: bash
 
 $ sudo kill 3486


This will terminate a process with a PID of 3486.

Wie kann ich überprüfen, ob der Prozess ist weg / umgebracht?
----------------------------------------------------------------

Verwenden Sie den Befehl ps oder pidof:

.. code-block:: bash
 
 $ ps aux | grep lighttpd
 $ pidof lighttpd

Wie kann ich töten zwei oder mehr PIDs?
--------------------------------------------

Die Syntax ist wie folgt auf zwei oder mehrere PIDs nach Bedarf können in einem einzigen Befehl verwenden zu töten:

.. code-block:: bash

 kill  pid1 pid2 pid3
 kill -15  pid1 pid2 pid3
 kill -9  pid1 pid2 pid3
 kill  -9 3546 5557 4242

Sag hallo zu allen Befehl zu töten
------------------------------------

Dies ist ein nur Linux-Befehl. um Prozesse namentlich. Befehl | Also keine Notwendigkeit, die PID-Parameter mit den "pidof Prozess" oder "grep Prozess ps aux 'zu finden. Verwenden Sie keine killall Befehl auf Unix-Betriebssystemen. Dies ist eine Linux-spezifischen Befehl.

Die Syntax ist

.. code-block:: bash

 killall Process-Name-Here

To kill the lighttpd server, enter:

.. code-block:: bash
 
 # killall -15 lighttpd

or

.. code-block:: bash

 # killall -9 lighttpd

To kill the Firefox web-browser process, enter:

.. code-block:: bash

 # killall -9 firefox-bin

etwas anderes. Es tötet alle Verfahren und nicht nur bestimmten Prozess. Verwenden Sie niemals töten alle auf UNIX-System.

Vorteile
------------

* Der Benutzer kann ein Verfahren mit unterschiedlichen Parametern wie pro ihre Anforderungen zu töten. Zum Beispiel: mit der ID, Ebene des Prozesses kann festgelegt werden, um zu töten.

