# Airflow

有Web UI 介面

排成表示式 https://crontab.guru/

官網

https://airflow.apache.org/

🔧 實作範例：建立一個 Airflow 專案

1. 下載官方 Docker Compose 範例

curl -LfO 'https://airflow.apache.org/docs/apache-airflow/2.9.1/docker-compose.yaml'

2. 建立資料夾結構

mkdir airflow-docker

cd airflow-docker

建立結構（官方建議）：

mkdir -p ./dags ./logs ./plugins ./config

3. 建立 .env 檔案
   
AIRFLOW_UID=50000 (用來指定容器中的 user id，避免權限問題）

5. 啟動 Airflow

docker compose up airflow-init

docker compose up

接著打開瀏覽器：http://localhost:8080

預設帳密是：

使用者名稱：airflow

密碼：airflow
