
## Download do docker compose
```
curl -LfO 'https://airflow.apache.org/docs/apache-airflow/2.2.4/docker-compose.yaml'
```

## Crie as pastas do Airflow
```
mkdir -p ./dags ./logs ./plugins
```
## Crie o arquivo .env
```
echo -e "AIRFLOW_UID=$(id -u)" > .env
```
## Inicie o Airflow
```
docker-compose up airflow-init
```
## Execute o Airflow
```
docker-compose up
```
