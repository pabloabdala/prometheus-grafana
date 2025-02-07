# prometheus-grafana

Crear el prometheus con un volumen:
docker run -d --name prometheus -p 9090:9090  -v c:\prometheus\prometheus.yml:/prometheus/prometheus.yml  -v c:\prometheus\data:/prometheus   prom/prometheus --storage.tsdb.path=/prometheus

Crear el grafana con un volumen:
docker run -d --name grafana -p 3000:3000 -v C:\grafana:/var/lib/grafana grafana/grafana

