# pgweb Helm Chart

## Prerequisites Details
* Kubernetes 1.5 (for `StatefulSets` support)



## Chart Details
This chart will do the following:

* Implemented a pgweb (Postgres UI) service

## Installing the Chart

To install the chart with the release name `my-release`:

```bash
$ git clone https://github.com/bluemix2020/icpcharts_source.git
$ cd pgweb
$ helm install pgweb --name my-release
```

## Configuration

The following tables lists the configurable parameters of the helm chart and their default values.

| Parameter                                  | Description                                | Default                                                    |
| -----------------------                    | ----------------------------------         | ---------------------------------------------------------- |
| `pgweb_deployment:replicaCount`            | `number of pgweb instance                     | `1`                                                        |

Specify each parameter using the `--set key=value[,key=value]` argument to `helm install`.

Alternatively, a YAML file that specifies the values for the parameters can be provided while installing the chart. For example,

```bash
$ helm install --name my-release -f values.yaml .
```
