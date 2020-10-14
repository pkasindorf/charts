# mailer services redux

## Installing the Chart

To install the chart, use the following:

```console
$ helm install digest-q-gen
```

## Configuration

The following table lists the configurable parameters of the digest-q-gen chart and
their default values.

| Parameter                   | Description                                 | Default
|:----------------------------|:--------------------------------------------|:---------------------------------------------------|
| `image.repository`          | Container image to use                      | `blemailservicesregistrydev.azurecr.io/blcloudmailer` |
| `image.tag`                 | Container image tag to deploy               | `latest`                                           |
| `image.pullPolicy`          | Container pull policy                       | `Always`                                           |
| `replicaCount`              | k8s replicas                                | `0`                                                |


Specify each parameter using the `--set key=value[,key=value]` argument to
`helm install`.

