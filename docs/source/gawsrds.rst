=================
AWS RDS 
=================

Zusammenfassung
----------------

Amazon Relational Database Service (Amazon RDS) ist ein Webdienst, der macht es einfach einzurichten, zu betreiben und Skalieren eine relationale Datenbank in der Cloud. Es bietet kostengünstige und veränderbare Kapazität beim Verwalten von zeitraubenden Datenbankverwaltung, damit Sie sich auf Ihre Anwendungen und Geschäft konzentrieren.

Amazon RDS ermöglicht Ihnen online Zugriff auf die Funktionen eines MySQL, Oracle, Microsoft SQL Server, PostgreSQL oder Amazon Aurora-relationalen Datenbank-Management-Systems. Dies bedeutet, dass der Code, Anwendungen und Tools, die Sie bereits heute mit vorhandenen Datenbanken mit Amazon RDS verwendet werden können Amazon RDS automatisch patches die Datenbanksoftware und Ihre Datenbank gesichert, speichern die Sicherungen für einen Benutzer-definierten Aufbewahrungszeitraum und eine Point-in-Time-Recovery. Sie profitieren von der Flexibilität, die Compute-Ressourcen oder die Speicherkapazität Ihrer Datenbank-Instanz (DB-Instanz) über einen einzigen API-Aufruf Skalieren zu können.

Datenbankinstanzen, die mit Amazon RDS-MySQL, Oracle, SQL Server und PostgreSQL-Motoren können mit allgemeinen Zweck (SSD) Speicher, bereitgestellt von IOPS (SSD) Speicher oder magnetische Speicherung bereitgestellt werden. Datenbank-Instanzen, die über die Amazon-Aurora-Engine beschäftigen eine fehlertolerante, Selbstheilungs-SSD gestützten virtualisierten Speicherschicht speziell für Datenbankarbeitslasten.

Darüber hinaus macht es Amazon RDS bedienungsfreundlich Replikation auf Verfügbarkeit und Zuverlässigkeit für Arbeitslasten der Produktion zu verbessern. Mit der Multi-AZ-Bereitstellung-Option, Sie können ausführen, mission kritische Arbeitslasten mit hoher Verfügbarkeit und integrierte automatische Failover-aus der primären Datenbank in einer synchron replizierten sekundären Datenbank im Falle eines Ausfalls. Verwendung von Read-Replika, können damit Amazon RDS für MySQL, PostgreSQL und Amazon Aurora auch übersteigt die Leistungsfähigkeit einer einzelnen Datenbank-Bereitstellung für Lese-Heavy Datenbankauslastungen skalieren. Wie bei allen Amazon Web Services, gibt es keine Vorab-Investitionen erforderlich und Sie zahlen nur für die Ressourcen, die Sie verwenden.

Hilfe Befehl
----------------------

Dieser Befehl hilft, um zu bestimmen, die Verwendung von Amazon RDS. Der Benutzer wird kommen, über den anderen Weg/Format wissen, dieses Modul ausgeführt. Dieser Befehl führt den Endbenutzer, um diesen Befehl zu erfahren. Unten gegeben sind, den Befehl und den Screenshot von der gleichen.

.. code-block:: bash

 kevell@corp:/# ptconfigure Amazon RDS help

 ******************************


    This is an extension provided for Handling AWS ElastiCache.

    Amazon RDS, Amazon RDS, aws-elasticache

        - create-cache-cluster
        Lets you add cache Cluster to AWS ElastiCache
        example: ptconfigure Amazon RDS create-cache-cluster
                    --yes
                    --guess
        - create-health-check
        Lets you add Health Check to AWS Route53
        example: ptconfigure AWSRoute53 create-health-check
                    --yes
                    --guess

          - reboot-cache-cluster
        Lets you reboot cache Cluster to AWS ElastiCache
        example: ptconfigure AWSRoute53 delete-hosted-zone
                    --yes
                    --guess

         - delete-cache-cluster
        Lets you delete cache Cluster to AWS ElastiCache
        example: ptconfigure Amazon RDS delete-cache-cluster
                    --yes
                    --guess

         - delete-replication-group
        Lets you delete replication group to AWS ElastiCache
        example: ptconfigure Amazon RDS delete-replication-group
                    --yes
                    --guess

        - list
        Will display data about your AWS ElastiCache
        example: ptconfigure Amazon RDS list
                    --yes
                    --guess

        Note: region must be one of the following...
        us-east-1, ap-northeast-1, sa-east-1, ap-southeast-1, ap-southeast-2, us-west-2, us-gov-west-1, us-west-1, cn-north-1, eu-west-1

 ------------------------------
 End Help
 ******************************

Describe-instance 
---------------------------

Dieser Befehl hilft, beschreiben Sie die Instanz der AWS RDS. Die unten mit dem Befehl führt den Prozess.

.. code-block:: bash
	
	ptconfigure AWSRDS describe-instance --yes --guess 

Delete-instance 
---------------------------

Dieser Befehl hilft, die um Instanz zu löschen. Die unten mit dem Befehl führt den Prozess.

.. code-block:: bash
	
	ptconfigure AWSRDS delete-instance --yes --guess

Create-db-snapshot 
---------------------------

Dies hilft der Befehl neu starten erstellen Db Snapshot. Die unten mit dem Befehl führt den Prozess.
 
.. code-block:: bash     

	ptconfigure AWSRDS create-db-snapshot --yes --guess 

Delete-db-snapshot 
-------------------------

Dieser Befehl hilft, um Db-Snapshot zu entfernen. Die unten mit dem Befehl führt den Prozess.

.. code-block:: bash     
	
	ptconfigure AWSRDS delete-db-snapshot –yes –guess

Copy-db-snapshot 
-----------------------------------

Dieser Befehl ermöglicht Db Snapshot kopieren. Die unten mit dem Befehl führt den Prozess.

.. code-block:: bash 
	
	ptconfigure AWSRDS copy-db-snapshot --yes --guess
        
Create-instance
------------------------

Dieser Befehl hilft, die um Instanz zu erstellen. Die unten mit dem Befehl führt den Prozess.

.. code-block:: bash 

	ptconfigure AWSRDS create-instance --yes –guess

Reboot-instance
------------------------

Dieser Befehl hilft Instanz neu starten. Die unten mit dem Befehl führt den Prozess.

.. code-block:: bash 

	ptconfigure AWSRDS reboot-instance --yes --guess

Create-instance-read replica
--------------------------------------

Dieser Befehl hilft, um Db-Instanz gelesen Replikat zu erstellen. Die unten mit dem Befehl führt den Prozess.

.. code-block:: bash 

	ptconfigure AWSRDS create-instance-readreplica --yes --guess

List
---------

Dieser Befehl können Sie die anzuzeigenden Daten über Ihre AWS RDS. Die unten mit dem Befehl führt den Prozess.

.. code-block:: bash 

	ptconfigure AWSRDS list --yes --guess

Alternative Parameter
-----------------------------

Es gibt drei alternative Parameter, die in der Befehlszeile verwendet werden können.

AWSRDS, awsrds, aws-rds 

Vorteile
--------------

Einfache Datenbank-Webdienst bereitstellen: Amazon RDS vereinfacht die Bereitstellung von Projekt-Konzeption gehen. Verwenden Sie die AWS Management Console oder einfache API-Aufrufe, um die Funktionen einer serienreifen relationalen Datenbank in Minuten zugreifen, ohne sich Gedanken über Bereitstellung von Infrastruktur oder Installation und Verwaltung von Datenbanksoftware.

Verwaltet: Amazon RDS behandelt zeitaufwändige Datenbankverwaltung, wie Sicherungen, Patch-Management und Replikation, so dass Sie höhere Wert-Anwendungsentwicklung oder Datenbank Verbesserungen einleiten.

Kompatibel: Mit Amazon RDS erhalten Sie nativen Zugriff auf ein relationales Datenbank-Managementsystem. Dies erleichtert die Kompatibilität mit Ihrem vorhandenen Tools und Anwendungen. Darüber hinaus gibt Amazon RDS Sie optionale Steuerung über die Engine Version Befugnisse Ihrer DB-Instanz über DB Engine Version Management unterstützt.

Schnell, vorhersagbare Performance: Datenbankinstanzen können mit Amazon RDS MySQL, Oracle, SQL Server und Oracle-Engines mit allgemeinen Zweck (SSD) Speicher, bereitgestellt von IOPS (SSD) Speicher oder magnetische Speicherung bereitgestellt werden.

Amazon RDS allgemeine Zweck (SSD) Speicher liefert eine konsistente Basisrichtlinie 3 IOPS pro bereitgestellten GB und bietet die Möglichkeit, bis zu 3.000 IOPS platzen.

Amazon RDS bereitgestellt IOPS (SSD) Lagerung ist eine Hochleistungs-Speicheroption entworfen, um schnelle, berechenbar und konsistente Performance für I/O intensive Transaktionsdatenbank Workloads zu liefern. Sie können von 1.000 IOPS auf 30.000 IOPS pro DB-Instanz bereitstellen. (Maximum erkannte, dass IOPS Motortyp variieren wird.)

Magnetspeicher (früher bekannt als Amazon RDS Standard Speicher) eignet sich für kleine Datenbankauslastungen wo weniger häufig auf Daten zugegriffen werden.

Datenbank-Instanzen, die über die Amazon-Aurora-Engine beschäftigen eine fehlertolerante, Selbstheilungs-SSD gestützten virtualisierten Speicherschicht speziell für Datenbankarbeitslasten.

Skalierbare Datenbank in der Cloud: Sie können die Compute skalieren und Speicherressourcen verfügbar zu Ihrer Datenbank zu Ihrer Anwendung zu erfüllen braucht mit Amazon RDS-API oder der AWS Management Console. Wenn Sie Amazon RDS bereitgestellt IOPS Speicher mit Amazon RDS für MySQL, Oracle oder PostgreSQL verwenden, können Sie bereitstellen und skalieren Sie den Speicher bis zu 3TB und IOPS auf bis zu 30.000. Beachten Sie, dieses Maximum erkannte, dass IOPS Motortyp variieren wird. Zusätzlich für MySQL, PostgreSQL und Amazon Aurora-Datenbank-Engines, können Sie auch eine oder mehrere Read-Replikate mit der Datenbank-Instanz-Bereitstellung zuordnen aktivieren Sie über die Kapazität einer einzelnen Datenbank-Instanz für Lese-Heavy-Arbeitslasten skalieren.

Die Amazon-Aurora-Datenbank-Engine ermöglicht es Ihnen, Ihren Speicher skaliert bis zu 64TB. Sie können Ihre Datenbank-Instanz-Bereitstellung bis zu 15 Amazon-Aurora-Replikate zuordnen. Amazon Aurora Replikate teilen den gleichen zugrunde liegenden Speicher als die Quellinstanz, Senkung der Kosten und die Notwendigkeit zum Kopieren von Daten auf die Replik-Knoten zu vermeiden.

Zuverlässig: Amazon RDS hat mehrere Funktionen, die Zuverlässigkeit für kritische Produktionsdatenbanken, einschließlich automatisierte Backups, DB-Snapshots, automatische Host Ersatz und Multi-AZ-Bereitstellungen zu erweitern. Amazon RDS läuft auf die gleiche zuverlässige Infrastruktur, die von anderen Amazon Web Services verwendet.

Für die Amazon-Aurora-Engine verwendet Amazon RDS RDS Multi-AZ-Technologie, um Failover zu einem der bis zu 15 Aurora Replikate zu automatisieren, die Sie in keinem der drei Availability Zones erstellt haben.
Zur Verwendung mit anderen Amazon Web Services: Amazon RDS ist eng mit anderen Amazon Web Services. Zum Beispiel wird eine Anwendung im Amazon EC2 Latenzzeiten Datenbankzugriff auf eine Amazon RDS-DB-Instanz in der gleichen Region erleben.

Sichere: Amazon RDS bietet eine Reihe von Mechanismen um Ihre DB-Instances.Amazon-RDS sichern können Sie verschlüsseln Ihre MySQL oder PostgreSQL-Datenbanken, die mit Schlüsseln, die Sie durch AWS Key Management Service (KMS) verwalten. Auf eine Datenbankinstanz, die mit Amazon RDS-Verschlüsselung ausgeführt wird werden im Ruhezustand in den zugrunde liegenden Speicher gespeicherte Daten verschlüsselt, wie seine automatisierte Backups, Replikate und Snapshots zu lesen sind.

Amazon RDS unterstützt transparente Datenverschlüsselung in SQL Server und Oracle. Transparente Datenverschlüsselung in Oracle ist AWS CloudHSM, integriert, wodurch Sie sicher erzeugen, speichern und verwalten die kryptografischen Schlüssel in Single-Tenant (Hardware Security Module, HSM) Appliances in der AWS-Cloud.

Amazon RDS umfasst Web-Service-Interfaces um Firewall-Einstellungen konfigurieren, die Netzwerkzugriff auf Ihre Datenbank steuern.
Amazon RDS können Sie Ihre DB-Instanzen in Amazon Virtual Private Cloud (Amazon VPC) ausführen. Amazon VPC können Sie Ihre DB-Instanzen zu isolieren, durch Angabe den IP-Adressbereich, den Sie verwenden möchten, und schließen an Ihre bestehende IT-Infrastruktur durch Industriestandard-verschlüsselte IPsec-VPN. Mehr über Amazon RDS in VPC finden Sie im Amazon RDS-Benutzerhandbuch.

Preiswert: Sie zahlen sehr niedrige Steuersätze und nur für die Ressourcen, die Sie tatsächlich verbrauchen. Darüber hinaus profitieren Sie von der Option der On-Demand Preise und keine Vorauszahlung oder langfristigen Verpflichtungen, oder sogar noch niedriger stündlich Preise über unsere reservierten Mengen Option.

On-Demand-DB Instanzen – On-Demand-DB-Instanzen können Sie für Compute-Kapazität pro Stunde mit keine langfristigen Verpflichtungen zu bezahlen. Dies erspart Ihnen die Kosten und die Komplexität der Planung, Kauf und Wartung Hardware und transformiert, was häufig große Fixkosten in viel kleineren Variable Kosten sind.

Reservierte DB-Instanzen – reservierte DB-Instanzen geben Ihnen die Möglichkeit, eine geringe, einmalige Zahlung für jede DB-Instanz zu machen, die Sie möchten reservieren und erhalten im Gegenzug einen erheblichen Rabatt auf die stündliche Benutzungsgebühr für diese DB-Instanz. Je nach Ihrer Verwendung können Sie die Wahl zwischen drei vorbehalten DB-Instanz (Light, Medium und Belastungstests) und bekommen überall zwischen 30 % und 55 % Rabatt über On-Demand-Preise.

