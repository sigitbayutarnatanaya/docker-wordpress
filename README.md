# Project Overview
This application consists of three main components:

- Web: wordpress5.1-fpm
- Webserver: Nginx
- Database: MySql

# Project Structure
- docker-learning/
- ├── nginx-conf/
- │   └── nginx.conf
- ├── wordpress/
- │   ├── Dockerfile
- │   └── wp-content
- ├── docker-compose.yml
- ├── .env
- └── README.md

# Prerequisites

- Docker Desktop installed on your machine
- Basic understanding of wordpress & nginx
- Git installed

# Troubleshooting
Common issues and solutions:

- Port Conflicts: Ensure ports 8080, 80, and 9000 are available on your machine
- Database Connection: Check if environment variables in docker-compose.yml match your application settings
- Volume Permissions: Run chmod 755 on the /var/www/html directory if encountering permission issues or chown using registered user

# Next Steps
After mastering this basic setup, consider exploring:

- Adding Redis for caching
- Implementing Nginx as a reverse proxy
- Setting up Docker networks
- Adding monitoring with Prometheus and Grafana
- Implementing CI/CD pipelines

# Command

- Build and start all services
docker-compose up

- Build and start in detached mode
docker-compose up -d

- Stop all services
docker-compose down

- View logs
docker-compose logs

- Rebuild services
docker-compose up --build

- Access container shell
docker exec -it container_name sh


# Contributing
Feel free to submit issues and enhancement requests!
