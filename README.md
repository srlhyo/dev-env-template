# Next.js Docker Development Template

Create a **complete web development environment in minutes** using Docker.

This template automatically creates a project with:

* **Next.js** (web framework)
* **PostgreSQL** (database)
* **Redis** (cache)
* **pgAdmin** (database UI)
* **Redis Commander** (Redis UI)
* **Docker** containers for isolated development

Everything runs inside Docker so it **does not affect your system**.

---

# Step 1 — Create Your Project From This Template

On the GitHub page of this repository click:

```
Use this template
```

Then:

1. Choose a **repository name** (this will be your project name)
2. Choose **public or private**
3. Click **Create repository**

GitHub will create a **new repository based on this template**.

---

# Step 2 — Clone Your New Project

Clone the repository you just created.

Example:

```bash
git clone https://github.com/YOUR-USERNAME/YOUR-PROJECT
cd YOUR-PROJECT
```

Make scripts executable:

```bash
chmod +x setup.sh dev.sh
```

---

# Step 3 — Verify System Requirements

Before running the setup, verify that required tools are installed.

### Docker

Check Docker:

```bash
docker --version
```

If Docker is not installed:

[https://www.docker.com/products/docker-desktop/](https://www.docker.com/products/docker-desktop/)

Docker must be **running** before starting the environment.

---

### Node.js

Check Node:

```bash
node --version
```

If Node.js is not installed:

[https://nodejs.org](https://nodejs.org)

---

# Step 4 — Run Project Setup

Run the setup script:

```bash
./setup.sh
```

This will automatically:

* create a Next.js project
* configure Docker
* configure PostgreSQL
* configure Redis
* generate environment variables
* prepare the development environment

---

# Step 5 — Start the Development Environment

Build the containers:

```bash
./dev.sh rebuild
```

Start the environment:

```bash
./dev.sh start
```

---

# Step 6 — Open the Applications

Once running, open these in your browser.

### Web Application

```
http://localhost:3000
```

### Database Interface (pgAdmin)

```
http://localhost:5050
```

### Redis Interface

```
http://localhost:8081
```

---

# Useful Commands

Start containers

```bash
./dev.sh start
```

Stop containers

```bash
./dev.sh stop
```

Rebuild containers

```bash
./dev.sh rebuild
```

View logs

```bash
./dev.sh logs
```

Check environment health

```bash
./dev.sh doctor
```

Reset the environment

```bash
./dev.sh reset
```

---

# Troubleshooting

If something breaks:

```bash
./dev.sh reset
./dev.sh rebuild
```

You can also check your system setup:

```bash
./dev.sh doctor
```

---

# What This Template Creates

Your generated project will include:

* Next.js application
* Docker development environment
* PostgreSQL database
* Redis cache
* pgAdmin interface
* Redis Commander interface
* automated environment configuration

---

# License

MIT License
