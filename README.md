## 👋 Welcome to poste 🚀

Complete mail server solution in a Docker container

## 📋 Description

Complete mail server solution in a Docker container

## 🚀 Services

- **poste**: analogic/poste.io:latest

## 📦 Installation

### Option 1: Quick Install
```bash
curl -q -LSsf "https://raw.githubusercontent.com/composemgr/poste/main/docker-compose.yaml" -o compose.yml
```

### Option 2: Git Clone
```bash
git clone "https://github.com/composemgr/poste" ~/.local/srv/docker/poste
cd ~/.local/srv/docker/poste
docker compose up -d
```

### Option 3: Using composemgr
```bash
composemgr install poste
```

## 🔧 Configuration

### Environment Variables

```shell
TZ=America/New_York
```

See `docker-compose.yaml` for complete list of configurable options.

## 🌐 Access

- **Web Interface**: http://172.17.0.1:8090

## 📂 Volumes

- `./volumes/config/poste` - Data storage
- `./volumes/data/poste` - Data storage

## 🔍 Logging

```shell
docker compose logs -f poste
```

## 🛠️ Management

```bash
# Start services
docker compose up -d

# Stop services
docker compose down

# Update to latest images
docker compose pull && docker compose up -d

# View logs
docker compose logs -f

# Restart services
docker compose restart
```

## 📋 Requirements

- Docker Engine 20.10+
- Docker Compose V2+

## 🤝 Author

🤖 casjay: [Github](https://github.com/casjay) 🤖  
🦄 composemgr: [Github](https://github.com/composemgr) 🦄
