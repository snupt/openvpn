[![forthebadge](https://forthebadge.com/images/badges/winter-is-coming.svg)](https://forthebadge.com)

## Requirements

### Client

* Mac / Linux
* Ansible

### Server

* Ubuntu Linux
* SSH access

## Configuration

Edit:

1. `group_vars/all.yaml`
1. `inventory.ini`

## Install Docker

```sh
$ make install-docker
```

## Install OpenVPN

### Server & Client

```sh
$ make install-vpn
```

Client file will be in the connections folder

### One more client

```sh
$ make create-client
```

Don't forget to change `client_name` variable in `group_vars/all.yaml`

### Reset

```sh
$ make reset-vpn
```

Remove all configuration files from server
