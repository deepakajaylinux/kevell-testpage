============
Parallax
============

Zusammenfassung
-----------------------

Die Parallaxe fördert die Multitasking-Funktionen in der Benutzer-Maschine. Die Parameter zu definieren, die Installation und die Hilfe muss nicht beachtet werden, während im Vergleich zu anderen. Es ist einfacher, die Multitasking-Funktion entweder zum Zeitpunkt der Installation oder bei der Ausführung des Installationsprozesses definieren.

Hilfe Befehl
--------------

Der Befehl help führt den Benutzer bei der Arbeit mit diesem Parallaxe. Es gibt auch den Befehl zum Installieren der Parallaxe und die Syntax für zwei Arten erklären Installation verwendet. Der Befehl help Liste auch die alternativen Parameter, die verwendet werden können. Der Befehl für die Hilfe-Option unter der Parallaxe verwendet wird unten gegeben.

.. code-block:: bash

	ptconfigure parallax help

Die Darstellung der Ergebnisse nach der Eingabe des Befehl help wird in der Abbildung unten dargestellt.

Installation
--------------

Es ist einfacher, mit Parallaxe für die Installation als Installation kann auf zwei verschiedene Arten nach den Benutzeranforderungen definiert werden, zu gehen. Diese beiden Wege werden wie nachstehend definiert:

* Mit dem Hinweis auf die Arten von Multi-Tasking, die erforderlich sind, während die Definition der Installationsbefehl.
* Oder durch die Erwähnung der Aufgabentypen während der Ausführung (Run-time) Installation.

Der Befehl zum Festlegen der Mehraufgaben bei der Erklärung der Installationsbefehl verwendet wird unten dargestellt:


.. code-block:: bash

	ptconfigure parallax cli --yes --command-1="pwd" --command-2="who"

Nach denen dieses Befehls führt der Parallaxe sowohl der Aufgaben, wie oben im Befehl-1 und Befehl-2 angegeben. Die beiden Aufgaben werden parallel durchgeführt und das Ergebnis angezeigt. Der Screenshot unten angebracht ist ein sehr gutes Beispiel für die Art von Erklärung oben definiert.
.. code-block:: bash

 kevell@corp:/# ptconfigure parallax cli --yes --command-1="pwd" --command-2="who"
 Completed task: pwd
 Completed task: who
 ******************************


 COMMAND: pwd
 COMPLETE: 1
 EXIT_STATUS: 0
 OUTPUT: /home/kevells


 COMMAND: who
 COMPLETE: 1
 EXIT_STATUS: 0
 OUTPUT: kevells   :0           2015-01-08 12:15 (:0)
 kevells   pts/2        2015-01-08 14:11 (:0)
 kevells   pts/1        2015-01-08 16:36 (:0)
 kevells   pts/10       2015-01-08 16:36 (:0)



 -----------------
 In Cli
 *******************************



Der Befehl für die Deklaration der Mehraufgaben zur Laufzeit verwendet wird, wie folgt dar:

.. code-block:: bash

	ptconfigure parallax cli

Nach der Eingabe des Befehls oben geschieht Folgendes:

.. cssclass:: table-bordered

 +--------------------------+---------------------------------------------+-------------+-----------------------------------------+
 | Parameter                | Alternative Parameter                       | Option      | Kommentare                              |
 +==========================+=============================================+=============+=========================================+
 |Run Commands in           | Trotz parallax, Folgende Alternativen       | Y(Yes)      | Wenn der Benutzer wünschen, den         |
 |Parallel? (Y/N)           | können ebenfalls verwendet werden:          |             | Installationsprozess können sie Eingang |
 |                          | parallax, Parallax                          |             | als Y. gehen                            |
 +--------------------------+---------------------------------------------+-------------+-----------------------------------------+
 |Run Commands in           | Trotz parallax, Folgende Alternativen       | N(No)       | Wenn der Benutzer wünschen, den         |
 |Parallel? (Y/N)           | können ebenfalls verwendet werden:          |             | Installationsprozess können sie Eingang |
 |                          | parallax, Parallax                          |             | als N. Beenden|                         |
 +--------------------------+---------------------------------------------+-------------+-----------------------------------------+

Wenn der Benutzer der Installation fortfahren möchten, kann der Benutzer die mehrere Aufgaben nach ihren Anforderungen festzulegen. Nach Abschluss der Angabe der mehrere Aufgaben, wenn die Benutzer wünschen, hören sie auf, indem Sie einfach niemand stoppen kann.

Schließlich werden die Ergebnisse der abgeschlossenen Aufgaben sowie der Zustand am Ende definiert. Die folgenden Screenshots können Sie eine grafische Darstellung in Bezug auf die oben genannten Verfahren.

.. code-block:: bash

   
	kevell@corp:/# ptconfigure parallax cli 
	
	Run Commands in Parallel? (Y/N) 
	y
	Enter Command to include next. Enter none to end.
	pwd
	Enter Command to include next. Enter none to end.
	who
	Enter Command to include next. Enter none to end.

	Completed task: pwd
	Completed task: who
	******************************


	COMMAND: pwd
	COMPLETE: 1
	EXIT_STATUS: 0
	OUTPUT: /home/kevells


	COMMAND: who
	COMPLETE: 1
	EXIT_STATUS: 0
	OUTPUT: kevells   :0           2015-01-08 12:15 (:0)
	kevells   pts/2        2015-01-08 14:11 (:0)
	kevells   pts/1        2015-01-08 16:36 (:0)
	kevells   pts/10       2015-01-08 16:36 (:0)



	-----------------
	In Cli
	******************************


Vorteile
----------

* Der Benutzer kann die parallele Aufgaben entweder in der Laufzeit oder in einer vordefinierten Weise wie pro ihre Anforderungen zu definieren.
* Schließlich wird nach Vollendung des Multiaufgaben die Ergebnisse und der Status der abgeschlossenen Aufgaben genau berichtet.
* Die für die Deklaration Syntax ist Groß- und Kleinschreibung beim Vergleich zu anderen, die ein zusätzlicher Vorteil ist.
* Es ist gut-to-do in beiden Cent Os und sowie Groß- und Kleinschreibung.

