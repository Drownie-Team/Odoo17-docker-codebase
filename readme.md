# Odoo Docker Compose

## Install docker

Install the docker to the computer.

## Configure the compose and odoo setting
  
1. Go to `compose.yml` file and configure the variable according to your preferences.

2. Go to `config/odoo.conf` to configure the addons path, log, etc. (You must setting the log, port and addons path according to the `compose.yml`) 

## All about docker compose
    
### Run docker compose
To run the docker compose file, you can use the bash code below. The code below will install all the required image if isn't installed on the computer.

```bash
docker compose up -d
```

### Stop docker compose
To stop the running docker file, you can use the bash code below. 
```bash
docker compose down
```

### Refresh docker compose
To stop the docker file, you can use the bash code below. The refresh code is used when you adding new module / upgrading the module.
```bash
docker compose restart
```

## Odoo Development

1. Listening to the logs

    To listen to the real time logs you can consider using the bash code below. The file path and name need to be adjusted according to `config/odoo.conf`
    ```bash
    tail -f logs/odoo-server.log
    ```

## Reference
- [Odoo docker official documentation](https://hub.docker.com/_/odoo)
