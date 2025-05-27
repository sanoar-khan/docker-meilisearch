# Meilisearch Server in Docker

Run Meilisearch Server in Docker for local development.

### Configs

Create a config file `configs/config.env` by copying from `configs/config.env.example`, and update environment values.

```bash
# create new config file
cp configs/config.env.example configs/config.env

# you may use this command to generate master key
openssl rand -base64 36

# update environment values
MEILI_IMAGE_TAG=v1.14
MEILI_PORT=7700
MEILI_MASTER_KEY=put-your-master-key
```

### Run Commands

```bash
# start mysql server
task dc-up

# stop mysql server
task dc-stop

# remove mysql server
task dc-down

# show container logs
task dc-logs
```
