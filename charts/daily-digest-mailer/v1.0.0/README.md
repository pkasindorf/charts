# Daily Digest Mailer

The daily digest mailer service is use to compose a digests of notification
messages from the buildinglink website. It then sends that digest to subscribers
at a predefined time each day. 


## Installing the Chart

To install the chart, use the following:

```console
$ helm install stable/daily-digest-mailer
```

## Configuration

The following table lists the configurable parameters of the daily-digest-mailer chart and
their default values.

| Parameter                   | Description                                                                                | Default         |
|:----------------------------|:-------------------------------------------------------------------------------------------|:----------------|
| `image.pullPolicy`          | Container pull policy                                                                      | `Always`  |
| `image.repository`          | Container image to use                                                                     | `blemailservicesregistry.azurecr.io/digestmailer`      |
| `image.tag`                 | Container image tag to deploy                                                              | `latest`         |
| `replicaCount`              | k8s replicas                                                                               | `1`             |
| `updateStrategy`            | update strategy for deployment                                                             | `{}`            |

Specify each parameter using the `--set key=value[,key=value]` argument to
`helm install`.

