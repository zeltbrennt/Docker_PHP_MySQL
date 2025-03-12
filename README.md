# Readme

## Create Docker Images

```bash
docker-compose -f ./docker/docker-compose.yml up -d --build
```

## Create Codeigniter Project with composer
```bash
docker exec -it codeigniter composer create-project codeigniter4/appstarter .
```

## Run Dev-Server


```bash
echo "CI_ENVIRONMENT = development" > ./src/.env

docker exec -it codeigniter php spark serve --host 0.0.0.0
```