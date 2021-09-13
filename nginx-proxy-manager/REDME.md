# Mise en place de l'outil Nginx Proxy Manager en local

### Creation des repertoires

```bash
mkdir -p ~/devops/nginx/data
mkdir -p ~/devops/nginx/letsencrypt
mkdir -p ~/devops/nginx/storage
```

### Configuration d'un domain en local

```bash
sudo nano /etc/hosts
```

## Configuration du nom du serveur de la machine local
```bash
sudo nano /etc/resolv.conf
nameserver 8.8.8.8
```

### Ajout du domain qui nous permettra d'accéder facilement à notre nginx-prox-manager

```bash
sudo nano /etc/hosts
127.0.0.1  nginxproxymanager.local
```

### Creation du network qui sera utilisé par tous les outils qui seront mis en place

```bash
docker network create devops_web_network
```

### Execution du service

```bash
docker-compose up -d --build
```

### Information de connexion

```bash
- username/password: admin@example.com/changeme

- new password: admin12345
- new login : gobinambale@gmail.com
```

