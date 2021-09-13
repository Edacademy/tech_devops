# Installation de l'outil prometheus

### creation de repertoire prometheus

```bash
mkdir -p ~/devops/prometheus_conf
mkdir -p ~/devops/prometheus_data
mkdir -p ~/devops/grafana_data
mkdir -p ~/devops/grafana/provisioning
```

### copier le fichier prometheus.yml

```bash
cp prometheus.yml ~/devops/prometheus_confprometheus.yml
```

### configuration du domaine local

```bash
sudo nano /etc/hosts
```

### Ajout du domain

```bash
127.0.0.1    prometheus.local
```

### Execution du service

```bash
docker-compose -f "prometheus.yml" up -d --build
```
