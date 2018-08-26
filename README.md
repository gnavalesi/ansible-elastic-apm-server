# Elastic APM Server Role

Ansible role for downloading and configuring Elastic APM Server. This role creates the ```apm-server.yml```
file with the default values defined.


Role Variables
--------------
#### Default installation values

```yaml
apm_server_version: 6.4.0
```

#### Configuration

The default values are already installed in the ```apm-server.yml``` file.
If you need to define variables or overwrite any default, you should use the ```apm_server_conf_``` prefix, and replace
dashes and dots by underscores as shown below:

```yaml
apm_server_conf_apm_server_host: localhost:8200
apm_server_conf_setup_template_settings_index_number_of_shards: 1
apm_server_conf_setup_template_settings_index_codec: best_compression
apm_server_conf_output_elasticsearch_hosts: ["localhost:9200"]
apm_server_conf_logging_metrics_enabled: false
``` 

License
-------

GNU GPLv3