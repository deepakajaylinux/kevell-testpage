==========
Ping
==========
Zusammenfassung
-----------------------

Als Verb bedeutet PING ", um die Aufmerksamkeit zu bekommen" oder einer anderen Partei online ", um das Vorhandensein von zu überprüfen". PING (Packet Internet Groper) Modul verwendet werden, um das System-Verbindung zu testen. PING verwendet, um Netzwerkdaten zu senden und die Netzwerkdaten empfangen von, anderen Computer in einem Netzwerk. PING häufig verwendet, um zu testen, ob ein weiteres System ist über ein Netzwerk erreichbar ist, und wenn ja, wie lange es dauert, dass die auszutauschenden Daten.

Hilfe Befehl
---------------

Diese Funktion dient, um die Verwendung von PING Modul bestimmen. Dieser Befehl help herauszufinden, die Möglichkeiten, zusammen mit PING-Befehl verwenden. Dieser Befehl wird die Endanwender zu führen, um die Nutzung der verschiedenen Optionen und der Syntax für diese Optionen zu kennen. Da unten sind die Kommando- und der Screenshot der gleiche.

.. code-block:: bash

	ptconfigure ping help

 kevell@corp:/# ptconfigure ping help

 ******************************


  This command allows you to test the status of ports

  Ping, ping

        - once
        ping a target once
        example: ptconfigure ping once --yes --guess
            --target=www.google.com # url/ip to ping test
            --interval=5 # no seconds to wait between requests, will 
 guess 2

        - ten
        ping a target ten times
        example: ptconfigure ping ten --yes --guess
            --target=www.google.com # url/ip to ping test
            --interval=5 # no seconds to wait between requests, will 
 guess 2

        - until-responding
        ping a target for a set amount of time until it responds
        example: ptconfigure ping once --yes --guess
            --target=www.google.com # url/ip to ping test
            --interval=5 # no seconds to wait between requests, will 
 guess 2
            --max-wait=100 # no seconds in total to keep trying, will guess 60

 ------------------------------
 End Help
 ******************************

Optionen
-----------

PING-Modul haben drei verschiedene Möglichkeiten, die Daten gemäß der Option in Befehle abrufen. Tabelle unten erklärt die gleiche

.. cssclass:: table-bordered

 +-------------+---------------------------------------------------+------------------------------------------------------------------+
 | Options     | Befehle                                           | Funktionen                                                       |
 +=============+===================================================+==================================================================+
 |Once         | ptconfigure ping once – yes –guess –target=       | Ping uns ein Ziel einmal. Nach Möglichkeit werden die Daten      |
 |             | google.com – interval=5                           | nur einmal abrufen                                               |
 +-------------+---------------------------------------------------+------------------------------------------------------------------+
 |Ten          | ptconfigure ping ten – yes –guess –target=        | Zehn Option Pull-Daten für das Zehnfache, mit Intervallzeit      |
 |             | google.com – interval=5                           | 5 Sekunden [wartet Sekunden vor dem Senden des nächsten Pakets]  |
 +-------------+---------------------------------------------------+------------------------------------------------------------------+
 |Until-       | ptconfigure ping once – yes –guess                | Ping uns das Ziel für eine bestimmte Zeit until er reagiert mit  |
 |responding   | --target=google.com -- interval=5                 | Intervallzeit 5 Sekunden und höchstens 100 Sekunden, um für die  |
 |             | -- max-wait=100                                   | Ziel versuchen|                                                  |
 +-------------+---------------------------------------------------+------------------------------------------------------------------+


Hinweis:

* Interval - Anzahl der Sekunden, die zwischen jeder Anfrage warten
                              
* Max-Wartezeit - Anzahl der Sekunden, insgesamt zu halten versuchen

* Intervallzeit und Max-Wartezeit Frequenz kann vom Anwender nach der Anforderung entschieden werden



Sobald Option
-----------------

.. code-block:: bash

 kevell@corp:/# ptconfigure ping once --yes --guess --target=www.google.com

 [Pharaoh Logging] Ping Latency is 34 ms
 ******************************


 Ping Modifications:
 --------------------------------------------
 
 Ping: Success

 ------------------------------
 Ping Mods Finished
 ******************************


Ten Option
-------------

.. code-block:: bash

 kevell@corp:/# ptconfigure ping ten --yes --guess --target=www.google.com 

 [Pharaoh Logging] Ping Latency is 36 ms
 [Pharaoh Logging] Ping Latency is 34 ms
 [Pharaoh Logging] Ping Latency is 34 ms
 [Pharaoh Logging] Ping Latency is 34 ms
 [Pharaoh Logging] Ping Latency is 36 ms
 ******************************


 Ping Modifications:
 --------------------------------------------

 Ping: Success

 ------------------------------
 Ping Mods Finished
 ******************************


Until responding
-----------------

.. code-block:: bash

 kevell@corp:/# ptconfigure ping once -- yes --guess --target=google.com -- interval=5 -- max-wait=100

 [Pharaoh Logging] Ping Latency is 37 ms
 ******************************


 Ping Modifications:
 --------------------------------------------

 Ping: Success

 ------------------------------
 Ping Mods Finished
 ******************************

Vorteile
------------


PING hilft dem Benutzer, eine bestimmte IP-Adresse Existenz zu überprüfen und können Anfrage zu akzeptieren. PING-Befehl ist der beste Weg, um die Verbindung zwischen zwei Knoten zu testen. Ob es sich um Local Area Network (LAN) oder Wide Area Network (WAN).

