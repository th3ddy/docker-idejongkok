# Docker - Web Server + PostgreSQL

Project ini adalah hasil praktik dari **Modul 1: Fondasi — Cloud, VPS & Mindset Automation** di Kelas Agentic AI Automation — Kelas Otomesyen.

## Stack
- **Nginx** — Web server
- **PostgreSQL 15** — Database
- **Docker Compose** — Container management

## Struktur Project
myproject/
├── docker-compose.yml
├── .env.example
├── .gitignore
└── html/
└── index.html
## Cara Menjalankan

### 1. Clone repo
```bash
git clone git@github.com:th3ddy/docker-idejongkok.git
cd docker-idejongkok
```

### 2. Setup environment
```bash
cp .env.example .env
nano .env  # isi POSTGRES_PASSWORD
```

### 3. Jalankan
```bash
docker compose up -d
```

### 4. Cek status
```bash
docker compose ps
```

Buka browser → `http://IP_SERVER`

## Perintah Docker Berguna
```bash
docker compose up -d      # jalankan semua container
docker compose down       # stop semua container
docker compose logs -f    # lihat log realtime
docker compose ps         # cek status container
```
