================
Amazon DynamoDB
================

Zusammenfassung
----------------

Amazon DynamoDB ist eine schnelle und flexible NoSQL-Datenbankdienst für alle Anwendungen, die konsistente, einer einstelligen Millisekunde Latenzzeiten bei jeder Größenordnung. Es ist eine vollständig verwaltete Datenbank und unterstützt sowohl die Dokument als auch die Schlüssel-Wert-Datenmodelle. Seine flexible Datenmodell und zuverlässige Leistung machen es hervorragend für Mobile, Web, Gaming, Ad-Tech, IoT und viele andere Anwendungen.


Hilfe Befehl
---------------------

Dieser Befehl hilft, um die Nutzung von AWS DynamoDB zu bestimmen. Der Benutzer wird kommen, über den anderen Weg/Format wissen, dieses Modul ausgeführt. Dieser Befehl führt den Endbenutzer, um diesen Befehl zu erfahren. Unten gegeben sind, den Befehl und den Screenshot von der gleichen.


.. code-block:: bash


 kevell@corp:/# ptconfigure AWSDynamoDb help

 ******************************


    This is an extension provided for Handling AWSDynamoDb.

    AWSDynamoDb, awsdynamodb,aws-dynamodb

        - describe-table
        Describe a table
        example: ptconfigure AWSDynamoDb describe-table
                    --yes
                    --guess
        - delete-table
        Lets you delete a table
        example: ptconfigure AWSDynamoDb delete-table
                    --yes
                    --guess


        - create-table
          Lets you create a table
          example: ptconfigure AWSDynamoDb create-table
                    --yes
                    --guess




        - list
        Will display data about your AWS AWSDynamoDb
        example: ptconfigure AWSDynamoDb list
                  --yes
                  --guess


        Note: region must be one of the following...
        us-east-1, ap-northeast-1, sa-east-1, ap-southeast-1, ap-southeast-2, us-west-2, us-gov-west-1, us-west-1, cn-north-1, eu-west-1


 ------------------------------
 End Help
 ******************************

Describe-table 
-------------------

Dieser Befehl hilft, um eine Tabelle zu beschreiben. Die unten mit dem Befehl führt den Prozess.


.. code-block:: bash

	 ptconfigure AWSDynamoDb describe-table --yes --guess

Delete-table 
-------------------

Dieser Befehl hilft, um eine Tabelle zu löschen. Die unten mit dem Befehl führt den Prozess.


.. code-block:: bash

	ptconfigure AWSDynamoDb delete-table --yes --guess

Create-table
---------------------

Dieser Befehl hilft, um eine Tabelle zu erstellen. Der wichtigste Teil ist, dass es irreversibel ist.

.. code-block:: bash     

	ptconfigure AWSDynamoDb create-table --yes --guess 


List 
---------------------

Dieser Befehl hilft, Daten über die AWS-AWSDynamoDb anzuzeigen. Die unten mit dem Befehl führt den Prozess.

.. code-block:: bash 
	
	ptconfigure AWSDynamoDb list --yes --guess

Alternative Parameter
-----------------------------

Es gibt zwei alternative Parameter, die in der Befehlszeile verwendet werden können.

AWSDynamoDb, awsdynamodb,aws-dynamodb 

Vorteile
--------------

Sekundäre Index-Scan – eine einfachere Möglichkeit zum Scannen von DynamoDB Tabellen: Amazon-DynamoDB können Sie alle Elemente aus einer Tabelle abrufen, mithilfe des Scan-Vorgangs. Mit sekundären Index-Scan können Sie nun verwenden Sie den Scanvorgang auf sekundären Indizes und rufen alle Daten aus ausgewählten Attribute und Elemente, die auf einen Sekundärindex projiziert werden. Sekundäre Index Scan arbeitet auf globaler und lokaler sekundärer Indizes. Sekundärindizes können gescannt werden, über die DynamoDB-Konsole oder durch Aufrufen der Scan API mit einem zusätzlichen Parameter um den Index angeben.


Online Indizierung – eine flexible Möglichkeit zum Verwalten von globalen Sekundärindizes: Amazon-DynamoDB können Sie globale sekundären Indizes (GSI) am Tisch erstellen erstellen. GSIs können Sie umfangreiche Abfragen mit Filtern zu schreiben. Mit online Indizierung können Sie hinzufügen oder Löschen von GSIs zu einer DynamoDB-Tabelle, jederzeit mithilfe der DynamoDB-Konsole oder über einen einfachen API-Aufruf. Während der GSI wird hinzugefügt oder gelöscht, die DynamoDB Tabelle kann noch behandeln live-Traffic und Dauerbetrieb auf der bereitgestellten Durchsatz-Ebene.


Melden Sie sich für die DynamoDB-Streams-Vorschau: DynamoDB Streams bietet eine Folge von Eintrag Änderungen in einer Tabelle DynamoDB bestellt. Die Änderungen werden dedupliziert und für 24 Stunden gespeichert. Diese Funktion ermöglicht Entwicklern, die Effektivität von DynamoDB mit Kreuz-Region-Replikation, kontinuierliche Analytics mit Redshift Integration, Änderungsbenachrichtigungen und viele andere.
