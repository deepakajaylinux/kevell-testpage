=================
AMAZON ROUTE 53 
=================

Zusammenfassung
-----------------

Amazon Route 53 ist eine hoch verfügbare und skalierbare Cloud (DNS = Domain Name System)-Web-Service. Es soll den Entwicklern und Unternehmen eine äußerst zuverlässige und kostengünstige Möglichkeit, Route Endbenutzer auf Internet-Anwendungen durch die Übersetzung der Namen wie www.example.com in die numerischen IP-Adressen wie 192.0.2.1, mit denen Computer miteinander verbinden.

Amazon Route 53 verbindet Benutzeranforderungen an Infrastruktur unter AWS – wie Amazon EC2-Instanzen, Load-balancer Elastic Load Balancing oder Amazon S3 Eimer – effektiv und kann auch verwendet werden, um Route Benutzer Infrastruktur außerhalb der AWS. Amazon Route 53 können DNS Gesundheitskontrollen Route Datenverkehr an gesunden Endpunkte konfigurieren oder unabhängig von der Anwendung und seine Endpunkte überwachen. Amazon Route 53 ermöglicht es Ihnen zur Verwaltung des Datenverkehrs weltweit durch eine Vielzahl von routing-Typen, einschließlich Wartezeit Based Routing, Geo-DNS und Weighted Round Robin – all das ist kombinierbar mit DNS Failover um eine Vielzahl von niedriger Latenz und fehlertolerante Architekturen ermöglichen. Amazon Route 53 bietet auch Domain-Namen-Registrierung – Sie können kaufen und Verwalten von Domain-Namen wie "example.com" und Amazon Route 53 konfiguriert automatisch DNS-Einstellungen für Ihre Domains.

Hilfe Befehl
----------------------

Dieser Befehl hilft, um die Verwendung von Amazon Route 53 zu bestimmen. Der Benutzer wird kommen, über den anderen Weg/Format wissen, dieses Modul ausgeführt. Dieser Befehl führt den Endbenutzer, um diesen Befehl zu erfahren. Unten gegeben sind, den Befehl und den Screenshot von der gleichen.

.. code-block:: bash

 kevell@corp:/# ptconfigure AWSRoute53 help

 ******************************


    This is an extension provided for Handling AWS ROUTE53.

    AWSRoute53, awsroute53, aws-route53

        - create-hosted-zone
        Lets you add Hosted zone to AWS Route53
        example: ptconfigure AWSRoute53 create-hosted-zone
                    --yes
                    --guess
        - create-health-check
        Lets you add Health Check to AWS Route53
        example: ptconfigure AWSRoute53 create-health-check
                    --yes
                    --guess
          - delete-hosted-zone
        Lets you delete Hosted zone to AWS Route53
        example: ptconfigure AWSRoute53 delete-hosted-zone
                    --yes
                    --guess
         - delete-health-check
        Lets you delete Health Check to AWS Route53
        example: ptconfigure AWSRoute53 delete-health-check
                    --yes
                    --guess

        - list
        Will display data about your AWS Route53
        example: ptconfigure AWSRoute53 list
                    --yes
                    --guess

        Note: region must be one of the following...
        us-east-1, ap-northeast-1, sa-east-1, ap-southeast-1, ap-southeast-2, us-west-2, us-gov-west-1, us-west-1, cn-north-1, eu-west-1

 ------------------------------
 End Help
 ******************************

Create-hosted-zone 
---------------------------

Dieser Befehl hilft AWS Route53 gehosteten Zone hinzu. Die unten mit dem Befehl führt den Prozess.

.. code-block:: bash

	ptconfigure AWSRoute53 create-hosted-zone --yes --guess

Create-health-check 
---------------------------

Dieser Befehl hilft Gesundheitscheck AWS Route53 hinzu. Die unten mit dem Befehl führt den Prozess.

.. code-block:: bash
	
	ptconfigure AWSRoute53 create-health-check --yes --guess

Delete-hosted-zone 
---------------------------

Dieser Befehl hilft löschen Hosted Zone für AWS Route53. Die unten mit dem Befehl führt den Prozess.

.. code-block:: bash     

	ptconfigure AWSRoute53 delete-hosted-zone --yes --guess 

Delete-health-check 
-------------------------

Dieser Befehl hilft, Gesundheitscheck, AWS Route53 löschen. Die unten mit dem Befehl führt den Prozess.

.. code-block:: bash     
	
	ptconfigure AWSRoute53 delete-health-check --yes --guess

List
---------

Dieser Befehl hilft, Daten über die AWS-Route53 anzuzeigen. Die unten mit dem Befehl führt den Prozess.

.. code-block:: bash 

	ptconfigure AWSRoute53 list --yes --guess

Alternative Parameter
----------------------------

Es gibt drei alternative Parameter, die in der Befehlszeile verwendet werden können.

AWSRoute53, awsroute53, aws-route53 

Vorteile
--------------

Hochverfügbarer und zuverlässiger: Amazon Route 53 basiert auf AWSs hoch verfügbaren und zuverlässigen Infrastruktur. Die verteilte Struktur unserer DNS-Server sorgt für eine konsistente Fähigkeit zum Weiterleiten von den Endbenutzern zur Anwendung. Route 53 soll die Zuverlässigkeit erforderlich für wichtige Anwendungen bereitgestellt. Amazon Route 53 wird von der Amazon Route 53 Service Level Agreement unterstützt.

Skalierbar: Route 53 soll automatisch skaliert werden, um sehr große Abfrage Mengen ohne jeglichen Eingriff ihrerseits zu verarbeiten.

Zur Verwendung mit anderen Amazon Web Services: Amazon Route 53 soll gut mit anderen AWS-Funktionen und Angebote zu arbeiten. Amazon Route 53 können Domain-Namen Ihre Amazon EC2-Instanzen, Amazon S3 Eimer, Amazon CloudFront-Verteilungen und andere AWS-Ressourcen zuordnen. Mithilfe des AWS Identity und Access Management (IAM) Dienstes mit Amazon Route 53 erhalten Sie fein abgestimmte Kontrolle über, die Ihre DNS-Daten zu aktualisieren. Amazon Route 53 können Sie Ihre Instanz Elastic Load Balancing, Amazon CloudFront Verteilung oder Amazon S3 Webseite Eimer verwenden ein Feature namens Aliasressourceneintrag Ihre Zone Apex (example.com versus www.example.com) zuordnen.

Ganz einfach: Mit Selbstbedienung Anmeldebonus, Route 53 beginnen, Ihre DNS-Abfragen innerhalb von Minuten zu beantworten. Sie können die DNS-Einstellungen mit der AWS Management Console oder unsere einfach zu bedienenden API konfigurieren. Sie können auch programmgesteuert die Route 53-API in der gesamten Webanwendung integrieren. Beispielsweise können Sie die Route 53-API verwenden, um einen neuen DNS-Datensatz zu erstellen, wenn Sie eine neue EC2-Instanz erstellen.

Schnell: Mit einem globale Anycast-Netzwerk von DNS-Servern auf der ganzen Welt, Amazon Route 53 soll Ihre Benutzer automatisch auf den optimalen Standort je nach Netzwerkbedingungen zu verlegen. Infolgedessen bietet den Service, niedrige Abfragewartezeit für Endbenutzer sowie niedrige Update Latenz für Ihre DNS-Datensatz-Management-Anforderungen.
Wirtschaftlich: Amazon Route 53 geht auf die Vorteile der AWS Skala Sie. Sie zahlen nur für die Verwaltung von Domains über den Service und die Anzahl der Abfragen, die der Dienst für jede Ihrer Domains, kostengünstig und ohne minimale Nutzung Verpflichtungen oder Gebühren vorab beantwortet.

Sicher: Durch die Integration von Amazon Route 53 mit AWS Identity und Access Management (IAM), können gewähren einzigartige Anmeldeinformationen und Berechtigungen für jeden Benutzer in Ihrem AWS-Konto verwalten und festlegen, wer Zugriff auf welche Teile des Dienstes Amazon Route 53 hat.

Flexibel: Amazon Route 53 bietet Weighted Round Robin (WRR), auch bekannt als DNS Lastverteilung. Dadurch können Sie Ihre DNS-Datensätze Gewichtungen zuweisen, die angeben, welcher Teil Ihres Verkehrs mit verschiedenen Endpunkten weitergeleitet wird.

