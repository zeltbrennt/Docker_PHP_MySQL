
## Create Codeigniter Project with composer
```
docker exec -it codeigniter composer create-project codeigniter4/appstarter .
```

## Run Dev-Server


```
echo "CI_ENVIRONMENT = development" > ./src/.env

docker exec -it codeigniter php spark serve --host 0.0.0.0
```