Role Name
=========

Role for installation and configuration [InfluxDB](https://github.com/influxdb/influxdb) database.

Requirements
------------

None.

Role Variables
--------------

|Name|Type|Description|Default|
|----|----|-----------|-------|
`influxdb_bind_address`|String|Bind address for InfluxDB service|`127.0.0.1`
`influxdb_host`|String|Address of InfluxDB server|`"{{ influxdb_bind_address }}"`
`influxdb_port`|Integer|Admin port of InfluxDB server|8083
`influxdb_user`|String|User for default project|`default_user`
`influxdb_password`|String|Password for `influxdb_user`|`passw0rd`

Dependencies
------------

None.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: influxdb-server
      roles:
         - { role: undergreen.influxdb, tags: ['influxdb'] }

License
-------

GPLv2

Author Information
------------------

Sergei Antipov, 2GIS LLC
[github page](https://github.com/UnderGreen)
[LinkedIn profile](https://www.linkedin.com/profile/view?id=396228287)
