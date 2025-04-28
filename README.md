# Reverse Proxy Project with Docker

This project runs two Flask web applications (`app1` and `app2`) behind a single NGINX reverse proxy using Docker Compose.

## How It Works

- `app1` runs on port 5000 and says "Hello from App 1!"
- `app2` runs on port 5000 and says "Hello from App 2!"
- `nginx` forwards:
  - `/app1` to App 1
  - `/app2` to App 2

## How to Run

```bash
docker-compose up --build -d
```
## Visit in Browser

http://localhost/app1

http://localhost/app2

## Technologies Used

- Docker
- Docker Compose
- NGINX
- Flask (Python)
