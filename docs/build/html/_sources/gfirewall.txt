===========
Firewall
===========


Zusammenfassung
-------------------------

Eine Firewall ist ein Netzwerk-Sicherheitssystem , das die ein- und ausgehenden Netzwerkverkehr basierend auf einer angelegten Regelsatz steuert. Firewalls gibt es sowohl als Software-Lösung und als Hardware-Appliance.

Hilfe Befehl
----------------

Dieser Befehl help unterstützen den Anwender zu ptconfigure. Es führt den Anwender die Erlaubnis.
Der Benutzer kann die Änderung nach Wunsch zu tun. Hilfe Bild wird den Benutzer zu führen. Lassen Sie uns zu visualisieren.

.. code-block:: bash

  ptconfigure Firewall help

Der Screenshot für den obigen Befehl aufgelistet unten,

.. code-block:: bash

 kevell@corp:/# ptconfigure Firewall help
 ******************************
 This command allows you to modify create or modify firewalls

  Firewall, firewall

        - enable
        Enable system firewall
        example: ptconfigure firewall enable

        - disable
        Disable system firewall
        example: ptconfigure firewall disable

        - allow
        Allow a Firewall rule
        example: ptconfigure firewall allow --firewall-rule="ssh/tcp"

        - deny
        Deny a Firewall rule. Allow connection attempts to be ignored and time out.
        example: ptconfigure firewall deny --firewall-rule="ssh/tcp"

        - reject
        Reject a Firewall rule. Terminate connections attempts with an error to the connector.
        example: ptconfigure firewall reject --firewall-rule="ssh/tcp"

        - limit
        Limit a Firewall rule. ufw will deny connections if an IP address has attempted
        to initiate 6 or more connections in the last 30 seconds.
        example: ptconfigure firewall limit --firewall-rule="ssh/tcp"

        - delete
        Delete a Firewall rule.
        example: ptconfigure firewall delete --firewall-rule="ssh/tcp"

        - insert
        Insert a Firewall rule.
        example: ptconfigure firewall insert --firewall-rule="ssh/tcp"

        - reset
        Reset a Firewall rule.
        example: ptconfigure firewall reset --firewall-rule="ssh/tcp"

        - default
        Set default policy, should be allow, deny, or reject
        example: ptconfigure firewall default --policy="deny"

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
 |Enable             | Aktivieren Sie Firewall-System                      | ptconfigure firewall enable               |
 +-------------------+-----------------------------------------------------+-------------------------------------------+
 |Disable            | Deaktivieren System-Firewall                        | ptconfigure firewall disable              |
 +-------------------+-----------------------------------------------------+-------------------------------------------+
 |Allow              | Lassen Sie Firewall-Regel                           | ptconfigure firewall allow –firewall-rule |
 |                   |                                                     | =”ssh/tcp”                                |
 +-------------------+-----------------------------------------------------+-------------------------------------------+
 |Deny               | Lassen Verbindungsversuch ignoriert und Auszeit     | ptconfigure firewall deny –firewall-rule  |
 |                   | werden                                              | =”ssh/tcp”                                |
 +-------------------+-----------------------------------------------------+-------------------------------------------+
 |Reject             | Verbindung beenden Versuche mit einem Fehler an dem | ptconfigure firewall reject –firewall-    |
 |                   | Verbinder                                           | rule=”ssh/tcp”                            |
 +-------------------+-----------------------------------------------------+-------------------------------------------+
 |Limit              | Ufw werden Verbindungen zu verweigern, wenn eine    | ptconfigure firewall limit –firewall      |
 |                   | IP-Adresse zu initiieren 6 oder mehr Verbindung in  | -rule=”ssh/tcp”                           |
 |                   | den letzten 30 Sekunden versucht.                   |                                           |
 +-------------------+-----------------------------------------------------+-------------------------------------------+
 |Delete             | Löschen Sie eine Firewall-Regel                     | ptconfigure firewall delete –firewall     |
 |                   |                                                     | -rule=”ssh/tcp”                           |
 +-------------------+-----------------------------------------------------+-------------------------------------------+
 |Insert             | Setzen Sie eine Firewall-Regel                      | ptconfigure firewall insert –firewall     |
 |                   |                                                     | -rule=”ssh/tcp”                           |
 +-------------------+-----------------------------------------------------+-------------------------------------------+
 |Reset              | Zurücksetzen eine Firewall-Regel                    | ptconfigure firewall reset –firewall      |
 |                   |                                                     | -rule=”ssh/tcp”                           |
 +-------------------+-----------------------------------------------------+-------------------------------------------+
 |default            | Standardrichtlinie, soll ermöglichen, zu leugnen    | ptconfigure firewall default –policy      |
 |                   | oder ablehnen.                                      | =”deny”|                                  |
 +-------------------+-----------------------------------------------------+-------------------------------------------+


Die bildliche Darstellung für den Befehl allow, deny , ablehnen und Reset ist unten aufgeführt ,

.. code-block:: bash

 kevell@corp:/# ptconfigure firewall allow --firewall-rule="ssh/tcp"

 Rules updated
 Rules updated (v6)
 ******************************


 Firewall Modifications:
 --------------------------------------------

 Firewall: Success

 ------------------------------
 Firewall Mods Finished
 ******************************

.. code-block:: bash


 kevell@corp:/# ptconfigure firewall deny --firewall-rule="ssh/tcp"


 Skipping adding existing rule
 Skipping adding existing rule (v6)
 ******************************


 Firewall Modifications:
 --------------------------------------------

 Firewall: Success

 ------------------------------
 Firewall Mods Finished
 ******************************

.. code-block:: bash


 kevell@corp:/# ptconfigure firewall reject --firewall-rule="ssh/tcp"

 Rules updated
 Rules updated (v6)
 ******************************


 Firewall Modifications:
 --------------------------------------------

 Firewall: Success

 ------------------------------
 Firewall Mods Finished
 ******************************


.. code-block:: bash


 kevell@corp:/# ptconfigure firewall reset --firewall-rule="ssh/tcp"

 Resetting all rules to installed defaults. Proceed with operation (y|n)? Backing up 'user.rules' to '/lib/ufw/user.rules.20150324_190113'
 Backing up 'after.rules' to '/etc/ufw/after.rules.20150324_190113'
 Backing up 'after6.rules' to '/etc/ufw/after6.rules.20150324_190113'
 Backing up 'before6.rules' to '/etc/ufw/before6.rules.20150324_190113'
 Backing up 'user6.rules' to '/lib/ufw/user6.rules.20150324_190113'
 Backing up 'before.rules' to '/etc/ufw/before.rules.20150324_190113'
 
 ******************************


 Firewall Modifications:
 --------------------------------------------

 Firewall: Success

 ------------------------------
 Firewall Mods Finished
 ******************************



Vorteile
------------

* Die Firewall verhindert unerwünschten Zugriff auf das System über ein Netzwerk durch die Ermittlung und Verhinderung von Kommunikation über 
  riskante Ports.
* System kommunizieren über viele verschiedene anerkannte Ports, und die Firewall wird dazu neigen, diese ohne Rückfrage oder weist den 
  Benutzer zu ermöglichen.
* Firewalls können auch "verdächtige" Aktivität von außen zu erkennen.
* Der Benutzer kann die Regel, nach ihrem Wunsch eingestellt.
