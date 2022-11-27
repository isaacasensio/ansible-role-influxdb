InfluxDB
=========

Installs [influxdb](https://github.com/influxdata/influxdb) docker container as a daemon.


Role Variables
--------------

Available variables are listed below, along with default values (see defaults/main.yml):

```
influxdb_image: "influxdb:2.0.7-alpine"
```
The version of the docker image to run as a container.

```
influxdb_host_data_path: /var/lib/influxdb2
```
Host path which stores influxdb data.

```
influxdb_host_config_path: /etc/influxdb2
```
Host path which stores influxdb config.

```
influxdb_container_user: influxdb
```
User running the container 

```
influxdb_host_port: 8086
```
Host port exposed

```
influxdb_username: "test"
```
Username

```
influxdb_password: "passw)rd!"
```
Password

```
influxdb_org: "home"
```
System inital organization

```
influxdb_bucket: "bucket"
```
System inital bucket

```
influxdb_token: "ffe8006b-9bc0-4421-aa09-942ad8ebcb9a"
```
Admin token


Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - iasensio.influxdb

License
-------

MIT

