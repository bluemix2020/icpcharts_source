# MQ Helm Chart

## Prerequisites Details
* Kubernetes 1.5 (for `StatefulSets` support)
* Dynamic Storage support on the underlying infrastructure

## StatefulSet Details
* https://kubernetes.io/docs/concepts/abstractions/controllers/statefulsets/

## StatefulSet Caveats
* https://kubernetes.io/docs/concepts/abstractions/controllers/statefulsets/#limitations


## Chart Details
This chart will do the following:

* Implemented a MQ service

## Installing the Chart

To install the chart with the release name `my-release`:

```bash
$ git clone https://github.com/bluemix2020/icpcharts_source.git
$ cd mq
$ helm install mq --name my-release
```

## Configuration

The following tables lists the configurable parameters of the helm chart and their default values.

| Parameter                                  | Description                                | Default                                                    |
| -----------------------                    | ----------------------------------         | ---------------------------------------------------------- |
| `mq_deployment:replicaCount`               | `number of mq instance                     | `1`                                                        |

Specify each parameter using the `--set key=value[,key=value]` argument to `helm install`.

Alternatively, a YAML file that specifies the values for the parameters can be provided while installing the chart. For example,

```bash
$ helm install --name my-release -f values.yaml .
```

## Persistence

The chart mounts a [Persistent Volume](http://kubernetes.io/docs/user-guide/persistent-volumes/) volume at this location. The volume is created using dynamic volume provisioning.
