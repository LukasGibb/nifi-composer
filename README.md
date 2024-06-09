# nifi-composer
Docker Composer files to spin up Apache NiFi and NiFi Registry containers.

The NiFi container uses single user authentication and NiFi Registry has no authentication enabled. This is not intended for production environments.

## Config
Copy the `.env.example` file to `.env` and set your password and key values.

## Starting the cluster
Execute the following command on this directory:

```shell
docker compose up -d
```

## Stopping the cluster

Execute the following command on this directory:

```shell
docker compose down
```
## Configuring the NiFi Registry Client

Once logged in to the NiFi frontend you can add a registry client using the following URL:

```
http://nifi-registry:18080
```