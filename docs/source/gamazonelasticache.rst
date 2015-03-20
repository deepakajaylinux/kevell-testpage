===================
Amazon ElastiCache
===================

Zusammenfassung
-----------------

ElastiCache ist ein Webdienst, der vereinfacht die Bereitstellung, den Betrieb und einen in-Memory-Cache in der Wolke zu skalieren. Der Service verbessert die Leistung von Webanwendungen durch die Möglichkeit zum Abrufen von Informationen aus schnell, verwaltete, in-Memory Caches, anstatt ganz auf langsameren Festplatten-basierte Datenbanken. ElastiCache unterstützt zwei Open Source im Arbeitsspeicher zwischenspeichern Motoren:


Memcached - ein weit verbreiteten Speicherobjekt caching-System. ElastiCache ist kompatibel mit Memcached, damit beliebte Tools, mit denen Sie heute mit vorhandenen Memcached-Umgebungen nahtlos mit dem Service funktioniert.


Redis – ein beliebtes Open Source im Arbeitsspeicher Schlüssel-Wert-Geschäft, das Strukturen wie sortiert Datensätze und Listen unterstützt. ElastiCache unterstützt Master / Slave-Replikation und Multi-AZ, die verwendet werden können, um Cross-AZ-Redundanz zu erreichen.


Amazon ElastiCache automatisch erkennt und ersetzt ausgefallene Knoten reduziert den Aufwand beim Selbstmanagement-Infrastrukturen und bietet eine robuste System, die das Risiko einer überladenen Datenbanken, mildert die langsame Website und Anwendung Mal laden. Durch Integration mit Amazon CloudWatch bietet Amazon ElastiCache verstärkten Einblick in wichtige Leistungsmetriken Ihre Memcached oder Redis-Knoten zugeordnet.


Amazon-ElastiCache verwenden, können Sie eine Zwischenspeicherung im Arbeitsspeicher-Schicht für Ihre Infrastruktur in wenigen Minuten hinzufügen, mithilfe der AWS Management Console.



Hilfe Befehl
----------------------

Dieser Befehl hilft, um die Verwendung von Amazon ElastiCache zu bestimmen. Der Benutzer wird kommen, über den anderen Weg/Format wissen, dieses Modul ausgeführt. Dieser Befehl führt den Endbenutzer, um diesen Befehl zu erfahren. Unten gegeben sind, den Befehl und den Screenshot von der gleichen.


.. code-block:: bash

 kevell@corp:/# ptconfigure AWSElastiCache help

 ******************************


    This is an extension provided for Handling AWS ElastiCache.

    AWSElastiCache, awselasticache, aws-elasticache

        - create-cache-cluster
        Lets you add cache Cluster to AWS ElastiCache
        example: ptconfigure AWSElastiCache create-cache-cluster
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
        example: ptconfigure AWSElastiCache delete-cache-cluster
                    --yes
                    --guess

         - delete-replication-group
        Lets you delete replication group to AWS ElastiCache
        example: ptconfigure AWSElastiCache delete-replication-group
                    --yes
                    --guess

        - list
        Will display data about your AWS ElastiCache
        example: ptconfigure AWSElastiCache list
                    --yes
                    --guess

        Note: region must be one of the following...
        us-east-1, ap-northeast-1, sa-east-1, ap-southeast-1, ap-southeast-2, us-west-2, us-gov-west-1, us-west-1, cn-north-1, eu-west-1

 ------------------------------
 End Help
 ******************************

Create-cache-cluster 
---------------------------

Dieser Befehl hilft AWS ElastiCache Cache Cluster hinzu. Die unten mit dem Befehl führt den Prozess.


.. code-block:: bash

	ptconfigure AWSElastiCache create-cache-cluster –yes --guess 


Create-health-check 
---------------------------

Dieser Befehl hilft Gesundheitscheck AWS Route53 hinzu. Die unten mit dem Befehl führt den Prozess.


.. code-block:: bash
	
	ptconfigure AWSRoute53 create-health-check –yes –guess

Reboot-cache-cluster 
---------------------------

Dieser Befehl hilft Cache Cluster AWS ElastiCache neu starten.
 
.. code-block:: bash     

	ptconfigure AWSRoute53 delete-hosted-zone --yes --guess 


Delete-cache-cluster 
-------------------------

Dieser Befehl hilft, Cluster, AWS ElastiCache den Cache löschen. Die unten mit dem Befehl führt den Prozess.


.. code-block:: bash     
	
	ptconfigure AWSElastiCache delete-cache-cluster --yes --guess


Delete-replication-group 
-----------------------------------

Dieser Befehl ermöglicht Replikationsgruppe zu AWS ElastiCache löschen. Die unten mit dem Befehl führt den Prozess.

.. code-block:: bash 
	
	ptconfigure AWSElastiCache delete-replication-group --yes --guess
        

List
---------------------

Dieser Befehl hilft zum Anzeigen von Daten über die AWS-ElastiCache anzeigen. Die unten mit dem Befehl führt den Prozess.


.. code-block:: bash 

	ptconfigure AWSElastiCache list --yes --guess

Alternative Parameter
-----------------------------

Es gibt drei alternative Parameter, die in der Befehlszeile verwendet werden können.

AWSElastiCache, awselasticache, aws-elasticache 

Vorteile
--------------

Fácil de implementar :

Amazon ElastiCache macht es sehr einfach, eine Memcached oder Redis-konforme Cache-Umgebung bereitzustellen. Verwenden Sie die AWS Management Console oder einfache API-Aufrufe, um die Funktionen des einen serienreifen Wolke-Cache-Cluster in Minuten zugreifen, ohne sich Gedanken über die Infrastruktur, die Bereitstellung oder Installation und Wartung von Cache-Software.

Verwaltet: Amazon ElastiCache automatisiert zeitraubende Verwaltungsaufgaben--wie Patch-Management, Fehlererkennung und Wiederherstellung--so dass Sie zu höheren Wert-Anwendungsentwicklung.

Kompatibel: Mit Amazon ElastiCache erhalten Sie nativen Zugriff auf die Memcached oder Redis im Arbeitsspeicher zwischenspeichern-Umgebungen. Dies erleichtert die Kompatibilität mit Ihrem vorhandenen Tools und Anwendungen.

Elastisch: Mit einem einfachen API-Aufruf oder ein paar Klicks der AWS Management Console, können Sie hinzufügen oder Löschen von Cache-Knoten zum Cluster Cache Wolke treffen Ihre Anwendung zu laden. Automatische Erkennung für Memcached ermöglicht automatische Erkennung der Cache-Knoten von ElastiCache Clients, wenn die Knoten hinzugefügt oder aus einem Amazon-ElastiCache-Cluster entfernt.

Zuverlässig: Amazon-ElastiCache verfügt über mehrere Features, die Zuverlässigkeit für kritische Produktionsbereitstellungen, einschließlich automatische Fehlererkennung und Wiederherstellung zu verbessern. Amazon ElastiCache läuft auf die gleiche zuverlässige Infrastruktur, die von anderen Amazon Web Services verwendet.

Integriert: Amazon ElastiCache für nahtlose Verwendung mit anderen Amazon Web Services, einschließlich Amazon Relational Database Service (Amazon RDS), Amazon DynamoDB, Amazon Elastic Compute Cloud (Amazon EC2), Amazon CloudWatch und Amazon Simple Notification Service (Amazon SNS) entwickelt.


Sichere: Amazon-ElastiCache bietet eine Reihe von Mechanismen, die Ihre Cache-Cluster zu sichern.

Amazon ElastiCache bietet Web-Service-Schnittstellen, mit denen Sie Firewalleinstellungen konfigurieren, die Steuerung des Netzwerkzugriffs zum Cache Cluster.

Amazon-ElastiCache können Sie Ihren Cache-Cluster in Amazon Virtual Private Cloud (Amazon VPC) ausführen. Amazon VPC können Sie Ihren Cache-Cluster durch Angabe der IP-Adressbereiche, die Sie möchten für Ihre Cache-Knoten verwenden, und schließen an Ihre vorhandenen Anwendungen in Amazon VPC zu isolieren. Mehr über Amazon ElastiCache in VPC finden Sie in der Bedienungsanleitung des Amazon-ElastiCache.


Kostengünstig: Amazon ElastiCache erspart Ihnen die administrative Kosten der Einrichtung und Verwaltung eines Clusters mit mehreren Knoten Cache. Scale-up und verkleinere die Anzahl der Cache-Knoten in Ihrem Cache-Cluster für optimale Leistung als Ihre Anwendungsnutzung Muster Änderungen, zahlen nur für die Ressourcen, die Sie tatsächlich nutzen können. Die Anforderungs-Preise können Sie für Speicher/Compute-Kapazität pro Stunde mit keine langfristigen Verpflichtungen zu bezahlen. Dies macht die Verwendung von Amazon ElastiCache sehr kostengünstig und erspart Ihnen die Kosten und die Komplexität der Planung, Kauf und Wartung Hardware.


Multi-AZ: Amazon ElastiCache bietet Replikationsfeatures Redis-Motor und dem Multi-AZ-Funktionalität. Sie können nutzen mehrere AWS Availability Zones Verfügbarkeit und darüber hinaus die Kapazitätsengpässe eines einzigen Cache-Knotens zu skalieren. Im Falle von primären Knoten erkennt die ElastiCache automatisch den Ausfall und Failover zu einem gelesenen Replikat höhere Verfügbarkeit ohne die Notwendigkeit manueller Eingriff bereitzustellen.


Sichern und wiederherstellen: Amazon ElastiCache für Redis hilft Ihnen, Ihre Daten zu schützen, indem Erstellen von Snapshots der Cluster. Über ein paar Klicks auf der Konsole oder einfache API-Aufrufe können Sie automatische Snapshots eingerichtet, sowie ein Backup zu starten, wann immer Sie sich entscheiden. Die Snapshots können dann verwendet werden, für das seeding neue ElastiCache für Redis-Cluster.


Wichtige Anwendungsfälle: Amazon ElastiCache kann verwendet werden, um Latenzzeit und Durchsatz für viele Lese-Heavy Anwendungs-Workloads (z. B. soziale Netzwerke, Spiele, Medienfreigabe und Q&A Portale) oder rechenintensive Arbeitsauslastungen (z. B. eine Empfehlungsmaschine) deutlich zu verbessern. Zwischenspeichern verbessert die Anwendungs-Performance durch Speichern von kritischen Teile der Daten im Speicher für Latenzzeiten Zugriff. Zwischengespeicherter Informationen kann die Ergebnisse der I/O-intensiven Datenbankabfragen oder die Ergebnisse der rechenintensive Berechnungen enthalten. Anwendungen benötigen einen Struktur-Datenserver finden die Redis-Engine am nützlichsten.

