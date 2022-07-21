InfluxDB
=========

Installs [influxdb](https://github.com/influxdata/influxdb) as a docker container.


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
influxdb_container_user: pi
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
influxdb_token: "d1f77bb2-f386-11eb-9a03-0242ac130003"
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

