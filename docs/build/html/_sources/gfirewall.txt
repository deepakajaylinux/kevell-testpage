===========
Firewall
===========


Zusammenfassung
-------------------------

Eine Firewall ist ein Netzwerk-Sicherheitssystem , das die ein- und ausgehenden Netzwerkverkehr basierend auf einer angelegten Regelsatz steuert. Firewalls gibt es sowohl als Software-Lösung und als Hardware-Appliance.

Hilfe Befehl
----------------

Dieser Befehl help unterstützen den Anwender zu Cleopatra. Es führt den Anwender die Erlaubnis.
Der Benutzer kann die Änderung nach Wunsch zu tun. Hilfe Bild wird den Benutzer zu führen. Lassen Sie uns zu visualisieren.

.. code-block:: bash

  cleopatra Firewall help

Der Screenshot für den obigen Befehl aufgelistet unten,

.. code-block:: bash

 kevell@corp:/# cleopatra Firewall help
 ******************************
 This command allows you to modify create or modify firewalls

  Firewall, firewall

        - enable
        Enable system firewall
        example: cleopatra firewall enable

        - disable
        Disable system firewall
        example: cleopatra firewall disable

        - allow
        Allow a Firewall rule
        example: cleopatra firewall allow --firewall-rule="ssh/tcp"

        - deny
        Deny a Firewall rule. Allow connection attempts to be ignored and time out.
        example: cleopatra firewall deny --firewall-rule="ssh/tcp"

        - reject
        Reject a Firewall rule. Terminate connections attempts with an error to the connector.
        example: cleopatra firewall reject --firewall-rule="ssh/tcp"

        - limit
        Limit a Firewall rule. ufw will deny connections if an IP address has attempted
        to initiate 6 or more connections in the last 30 seconds.
        example: cleopatra firewall limit --firewall-rule="ssh/tcp"

        - delete
        Delete a Firewall rule.
        example: cleopatra firewall delete --firewall-rule="ssh/tcp"

        - insert
        Insert a Firewall rule.
        example: cleopatra firewall insert --firewall-rule="ssh/tcp"

        - reset
        Reset a Firewall rule.
        example: cleopatra firewall reset --firewall-rule="ssh/tcp"

        - default
        Set default policy, should be allow, deny, or reject
        example: cleopatra firewall default --policy="deny"

 ------------------------------
 End Help
 ******************************

Optionen
------------

Firewalls Regeln können nach Ihren Bedürfnissen, Anforderungen und Sicherheitsbedrohungslage angepasst werden. Der Benutzer kann Firewall-Regeln auf Basis von solchen Bedingungen wie zu erstellen oder zu deaktivieren:

.. cssclass:: table-bordered

 +-------------------+-----------------------------------------------------+-------------------------------------------+
 | Parameter         |  Funktion                                           | Kommentar                                 |
 +===================+=====================================================+===========================================+
 |IP address         | Absperren eine bestimmte IP-Adresse oder einen      |                                           |
 |                   | Bereich von IP-Adressen, die Sie denken,            |                                           |
 |                   | sind räuberische                                    |                                           |
 +-------------------+-----------------------------------------------------+-------------------------------------------+
 |Enable             | Aktivieren Sie Firewall-System                      | cleopatra firewall enable                 |
 +-------------------+-----------------------------------------------------+-------------------------------------------+
 |Disable            | Deaktivieren System-Firewall                        | cleopatra firewall disable                |
 +-------------------+-----------------------------------------------------+-------------------------------------------+
 |Allow              | Lassen Sie Firewall-Regel                           | cleopatra firewall allow –firewall-rule   |
 |                   |                                                     | =”ssh/tcp”                                |
 +-------------------+-----------------------------------------------------+-------------------------------------------+
 |Deny               | Lassen Verbindungsversuch ignoriert und Auszeit     | cleopatra firewall deny –firewall-rule    |
 |                   | werden                                              | =”ssh/tcp”                                |
 +-------------------+-----------------------------------------------------+-------------------------------------------+
 |Reject             | Verbindung beenden Versuche mit einem Fehler an dem | cleopatra firewall reject –firewall-rule= |
 |                   | Verbinder                                           | ”ssh/tcp”                                 |
 +-------------------+-----------------------------------------------------+-------------------------------------------+
 |Limit              | Ufw werden Verbindungen zu verweigern, wenn eine    | cleopatra firewall limit –firewall-rule=  |
 |                   | IP-Adresse zu initiieren 6 oder mehr Verbindung in  | ”ssh/tcp”                                 |
 |                   | den letzten 30 Sekunden versucht.                   |                                           |
 +-------------------+-----------------------------------------------------+-------------------------------------------+
 |Delete             | Löschen Sie eine Firewall-Regel                     | cleopatra firewall delete –firewall-rule= |
 |                   |                                                     | ”ssh/tcp”                                 |
 +-------------------+-----------------------------------------------------+-------------------------------------------+
 |Insert             | Setzen Sie eine Firewall-Regel                      | cleopatra firewall insert –firewall-rule= |
 |                   |                                                     | ”ssh/tcp”                                 |
 +-------------------+-----------------------------------------------------+-------------------------------------------+
 |Reset              | Zurücksetzen eine Firewall-Regel                    | cleopatra firewall reset –firewall-rule=  |
 |                   |                                                     | ”ssh/tcp”                                 |
 +-------------------+-----------------------------------------------------+-------------------------------------------+
 |default            | Standardrichtlinie, soll ermöglichen, zu leugnen    | cleopatra firewall default –policy=”deny” |
 |                   | oder ablehnen.|                                     |                                           |
 +-------------------+-----------------------------------------------------+-------------------------------------------+


Vorteile
------------

* Die Firewall verhindert unerwünschten Zugriff auf das System über ein Netzwerk durch die Ermittlung und Verhinderung von Kommunikation über 
  riskante Ports.
* System kommunizieren über viele verschiedene anerkannte Ports, und die Firewall wird dazu neigen, diese ohne Rückfrage oder weist den 
  Benutzer zu ermöglichen.
* Firewalls können auch "verdächtige" Aktivität von außen zu erkennen.
* Der Benutzer kann die Regel, nach ihrem Wunsch eingestellt.
