# Red Hat out of box tools for observability

**[Opentelemetry](https://opentelemetry.io/) is used to collect the telemetry data from applications and send to different backends tools** 

Red Hat build of opentelemetry is used for collecting the telemetry data from the applications by configuring auto instrumentation on applications.

- Deploy the required backend tools listed below
- Deploy the [opentelemetry collector](./1-opentelemetry/collector.yaml)
- Get the service URL of the otel collector to configure in the [auto instrumentation](./1-opentelemetry/collector.yaml)

***Note:  
This demo is tested in openshift environment and all the operators are installed from the openshift operator hub. Setting up these backends in kubernetes maybe different.***

## List of Backends used 

- [**Elastic Search**](./2-elasticsearch/)

    - Operators used :  
      1. Elasticsearch (ECK) Operator - certified

- [**tempo**](./3-tempo/)

    - Operators used:  
      1. Minio Operator - certified
      2. Tempo Operator - Red Hat
    