# mailer services redux

<br/>

---

### TODO: Move Marc's Notes to confluence

<br/>

#### Dev Reference Links  

 1. [Custom Chart Creation](https://rancher.com/docs/rancher/v2.x/en/catalog/tutorial/)  
 1. [Helm chart developer reference](https://helm.sh/docs/chart_template_guide/)  

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

