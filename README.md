# Fluentd Boshrelease

## Description

This is used to install fluentd for log collection and transport.

### fluentd-server
Deploys a primary server which will forward data to either logstash or directly to elasticsearch. Used in conjunction with `fluentd-plugins`

### fluentd-transporter
In a runtime config, will job will transfer all logs to the defined `fluentd-server` cluster.

### fluentd-plugins
Installs plugins for either `fluentd-server` or `fluentd-transporter`.


## Usage
Inside the `manifests` directory, you should find an example `fluentd.yml` bosh deployment manifest file.

### Example Deployment
```
bosh deploy -d fluentd manifests/fluentd.yml
```

## Properties
### fluented-server
|varliable|description|default|
|---|---|---|
| | | |
To be filled out.
### fluented-transporter
|varliable|description|default|
|---|---|---|
| | | |
To be filled out.
### fluented-plugins
| variable | description | default |
| --- | --- | --- |
| fluentd.plugin | A list of plugins to install.| [] |
