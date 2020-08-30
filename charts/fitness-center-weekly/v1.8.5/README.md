## Installing the Chart

Full installation instructions, including details on how to configure extra
functionality in fitness-center-weekly can be found in the [getting started docs](https://fitness-center-weekly.readthedocs.io/en/latest/getting-started/).

More information on the different types of issuers and how to configure them
can be found in our documentation:

https://fitness-center-weekly.readthedocs.io/en/latest/reference/issuers.html

For information on how to configure fitness-center-weekly to automatically provision
Certificates for Ingress resources, take a look at the `ingress-shim`
documentation:

https://fitness-center-weekly.readthedocs.io/en/latest/reference/ingress-shim.html

## Configuration

The following table lists the configurable parameters of the fitness-center-weekly chart and their default values.

| Parameter | Description | Default |
| --------- | ----------- | ------- |
| `image.repository` | Image repository | `quay.io/jetstack/fitness-center-weekly-controller` |
| `image.tag` | Image tag | `v0.3.0` |
| `image.pullPolicy` | Image pull policy | `IfNotPresent` |
| `replicaCount`  | Number of fitness-center-weekly replicas  | `1` |
| `createCustomResource` | Create CRD/TPR with this release | `true` |
| `clusterResourceNamespace` | Override the namespace used to store DNS provider credentials etc. for ClusterIssuer resources | Same namespace as fitness-center-weekly pod
| `leaderElection.Namespace` | Override the namespace used to store the ConfigMap for leader election | Same namespace as fitness-center-weekly pod
| `certificateResourceShortNames` | Custom aliases for Certificate CRD | `["cert", "certs"]` |
| `extraArgs` | Optional flags for fitness-center-weekly | `[]` |
| `rbac.create` | If `true`, create and use RBAC resources | `true` |
| `serviceAccount.create` | If `true`, create a new service account | `true` |
| `serviceAccount.name` | Service account to be used. If not set and `serviceAccount.create` is `true`, a name is generated using the fullname template |  |
| `resources` | CPU/memory resource requests/limits | `requests: {cpu: 10m, memory: 32Mi}` |
| `nodeSelector` | Node labels for pod assignment | `{}` |
| `affinity` | Node affinity for pod assignment | `{}` |
| `tolerations` | Node tolerations for pod assignment | `[]` |
| `ingressShim.defaultIssuerName` | Optional default issuer to use for ingress resources |  |
| `ingressShim.defaultIssuerKind` | Optional default issuer kind to use for ingress resources |  |
| `ingressShim.defaultACMEChallengeType` | Optional default challenge type to use for ingresses using ACME issuers |  |
| `ingressShim.defaultACMEDNS01ChallengeProvider` | Optional default DNS01 challenge provider to use for ingresses using ACME issuers with DNS01 |  |
| `podAnnotations` | Annotations to add to the fitness-center-weekly pod | `{}` |
| `podDnsPolicy` | Optional fitness-center-weekly pod [DNS policy](https://kubernetes.io/docs/concepts/services-networking/dns-pod-service/#pods-dns-policy) |  |
| `podDnsConfig` | Optional fitness-center-weekly pod [DNS configurations](https://kubernetes.io/docs/concepts/services-networking/dns-pod-service/#pods-dns-config) |  |
| `podLabels` | Labels to add to the fitness-center-weekly pod | `{}` |

Specify each parameter using the `--set key=value[,key=value]` argument to `helm install`.

Alternatively, a YAML file that specifies the values for the above parameters can be provided while installing the chart. For example,

## Contributing

This chart is maintained at [github.com/jetstack/fitness-center-weekly](https://github.com/jetstack/fitness-center-weekly/tree/master/contrib/charts/fitness-center-weekly).
