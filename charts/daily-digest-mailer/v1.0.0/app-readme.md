# Daily Digest Mailer

This chart installs and configures an instance of the buildinglink 
daily digest mailer service.

## Prerequisites Details

* SQL Server instances (Azure)
  * blazuresql100.buildinglink.local (10.2.1.100) prod r/w
  * blazuresql101.buildinglink.local (10.2.1.101) prod r/o
  * blazuresql102.buildinglink.local (10.2.1.102) dev r/w
  
* Rabbit MQ instance (Azure)
  * 10.2.1.12

* Azure Storage account (blob)
  * blmail / mail (for prod)
  * blmail / dev  (for dev)

* SMTP Relay Servers
  * smtprelay.buildinglink.local  (no attachments)
  * smtprelay2.buildinglink.local (with attachments)

* Sentry

* Localization
  * API Client Id mapped for a service account


## Chart Details

This chart does the following:

* Installs the digestmailer service - a scalable mailer service
  