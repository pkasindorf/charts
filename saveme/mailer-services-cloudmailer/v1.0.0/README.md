# mailer services

## Installing the Chart

To install the chart, use the following:

```console
$ helm install mailer-services-cloudmailer
```

## Configuration

The following table lists the configurable parameters of the mailer-services-cloudmailer chart and
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
