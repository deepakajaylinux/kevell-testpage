===================
Amazon CloudWatch
===================

Zusammenfassung
------------------

Amazon CloudWatch ist ein Überwachungsdienst für AWS-Cloud-Ressourcen und die Anwendungen, die Sie auf AWS ausführen. Amazon CloudWatch können Sie sammeln und verfolgen Metriken, sammeln und überwachen log-Dateien und einen Alarm einstellen. Amazon CloudWatch überwacht AWS-Ressourcen wie Amazon EC2-Instanzen, Amazon DynamoDB Tabellen, und Amazon RDS DB-Instanzen sowie benutzerdefinierte Metriken, die durch Ihre Anwendungen und Dienste und alle Protokolldateien, die Ihre Anwendungen generieren generiert. Amazon CloudWatch können systemweite Einblick in betriebliche Gesundheit, Ressourcenauslastung und Anwendungs-Performance zu gewinnen. Diese Erkenntnisse können Sie reagieren und Ihrer Anwendung reibungslos.



Hilfe Befehl
----------------------

Dieser Befehl hilft, um die Verwendung von Amazon CloudWatch zu bestimmen. Der Benutzer wird kommen, über den anderen Weg/Format wissen, dieses Modul ausgeführt. Dieser Befehl führt den Endbenutzer, um diesen Befehl zu erfahren. Unten gegeben sind, den Befehl und den Screenshot von der gleichen.


.. code-block:: bash

 kevell@corp:/# ptconfigure AWSCloudWatch help

 ******************************


  This command allows you to install a few GC recommended Standard Tools
  for productivity in your system.  The kinds of tools we found ourselves
  installing on every box we have, client or server. These include curl,
  vim, drush and zip.

  AWSCloudWatch, aws-cloud-watch, aws-cloudwatch

        - install
        Installs AWSCloudWatch. Note, you'll also need Java installed
        as it is a prerequisite for AWSCloudWatch
        example: ptconfigure aws-cloudwatch install

 ------------------------------
 End Help
 ******************************


Installation
----------------

Falls der Benutzer durchführen, Amazon CloudWatch-Modul in der Maschine muss, die unten mit dem Befehl wird ausgeführt, den Prozess der Installation.


.. code-block:: bash
        
        ptconfigure aws-cloudwatch install

.. code-block:: bash 

	

Vorteile
--------------

Monitor Amazon EC2: Zeigen Sie Metriken für CPU-Auslastung, Datenübertragung und Festplattenaktivität Verwendung von Amazon EC2-Instanzen (Basisüberwachung) ohne Aufpreis. Gegen eine zusätzliche Gebühr bietet CloudWatch detaillierte Überwachung für EC2-Instanzen mit höherer Auflösung und metrische Aggregation. Keine zusätzlicher Software muss installiert werden.


Monitor andere AWS-Ressourcen: Überwachung Metriken auf Amazon DynamoDB Tabellen, Amazon EBS-Volumes, Amazon RDS DB-Instanzen, Amazon Elastic MapReduce Stelle fließt, Elastic Load-Balancern, Amazon SQS Warteschlangen, Amazon SNS-Themen und mehr ohne Aufpreis. Keine zusätzlicher Software muss installiert werden.


Monitor benutzerdefinierte Metriken: Übermitteln Sie benutzerdefinierte Metriken durch eigene Applikationen über eine einfache API-Anforderung generiert und lassen sie von Amazon CloudWatch überwacht. Sie können senden und Speichern von Metriken, die sind wichtig für Ihre Anwendung operative Leistung, Problembehandlung und Trends erkennen zu helfen.


Monitor und Store-Protokolle: CloudWatch Protokolle können Sie überwachen und behandeln Ihre Systeme und Anwendungen, die unter Verwendung Ihres bestehenden Systems, Anwendung und benutzerdefinierte Log-Dateien. Senden Ihren vorhandenen System und die Anwendung benutzerdefinierte Log-Dateien in CloudWatch Protokolle können und diese Protokolle in nahezu in Echtzeit zu überwachen. Dadurch können Sie besser verstehen und betreiben Ihre Systeme und Anwendungen, und Sie können Ihre Protokolle mit hoch belastbare, kostengünstige Speicher für den späteren Zugriff speichern.


Set Alarm: Einen Sie Alarm einstellen, auf Ihre Messdaten senden Sie Mitteilungen oder andere automatisierte Aktionen. Beispielsweise wenn eine bestimmte Amazon EC2-Metrik Ihre Alarm-Schwellenwert überschreitet, können Sie automatische Skalierung dynamisch hinzufügen oder Entfernen von EC2-Instanzen oder senden Ihnen eine Benachrichtigung.


Grafiken und Statistiken anzeigen: Anzeigen von Grafiken und Statistiken für alle Ihre Messdaten auf dem Armaturenbrett Amazon CloudWatch und erhalten einen schnellen Überblick über alle Ihre Alarme und überwacht AWS-Ressourcen an einem Ort.


