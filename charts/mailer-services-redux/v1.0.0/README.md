# mailer services redux

## Installing the Chart

To install the chart, use the following:

```console
$ helm install mailer-services-redux
```

## Configuration

The following table lists the configurable parameters of the mailer-services-redux chart and
their default values.

| Parameter                   | Description                                                                                | Default         |
|:----------------------------|:-------------------------------------------------------------------------------------------|:----------------|
| `image.pullPolicy`          | Container pull policy                                                                      | `Always`  |
| `image.repository`          | Container image to use                                                                     | `blemailservicesregistry.azurecr.io/digestmailer`      |
| `image.tag`                 | Container image tag to deploy                                                              | `latest`         |
| `replicaCount`              | k8s replicas                                                                               | `0`             |
| `updateStrategy`            | update strategy for deployment                                                             | `{}`            |

Specify each parameter using the `--set key=value[,key=value]` argument to
`helm install`.



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

