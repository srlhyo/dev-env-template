# Next.js Docker Development Template

Create a **complete web development environment in minutes**.

This template automatically creates a project with:

* Next.js (web framework)
* PostgreSQL (database)
* Redis (cache)
* pgAdmin (database management UI)
* Redis Commander (Redis UI)
* Docker containers for isolated development

Everything runs inside Docker so it **does not affect your system**.

Estimated setup time: **5–10 minutes**.

---

# Quick Start

If you already have Docker and Node.js installed you can start immediately.

```bash
git clone https://github.com/YOUR-USERNAME/dev-env-template YOUR-PROJECT-NAME
cd YOUR-PROJECT-NAME
chmod +x setup.sh dev.sh

./setup.sh
./dev.sh rebuild
./dev.sh start
```

Then run:

```bash
./dev.sh ports
```

Open the URLs shown in your browser.

---

# Works On

This template has been tested on:

* macOS
* Linux
* Windows (WSL)

---

# Requirements

This template requires **Docker** and **Node.js**.

Before installing anything, check if they are already installed.

---

## 1. Check Your System

Run the following commands in your terminal:

```bash
docker --version
node --version
```

If both commands print a version number, your system is ready.

Example:

```
Docker version 24.x
v20.x
```

If one of these commands fails, install the missing software below.

---

## 2. Install Docker (if needed)

Download Docker Desktop:

[https://www.docker.com/products/docker-desktop/](https://www.docker.com/products/docker-desktop/)

Verify installation:

```bash
docker --version
```

Make sure **Docker is running** before continuing.

---

## 3. Install Node.js (if needed)

Download Node.js LTS:

[https://nodejs.org](https://nodejs.org)

Verify installation:

```bash
node --version
```

Node.js **LTS version** is recommended.

---

# Step 1 — Create a Project From This Template

Clone the template repository. You can choose **any name for your project folder** (replace `YOUR-PROJECT-NAME` with the name you want):

```bash
git clone https://github.com/YOUR-USERNAME/dev-env-template my-project
```

Enter the project folder:

```bash
cd my-project
```

Make scripts executable:

```bash
chmod +x setup.sh dev.sh
```

Run the setup script:

```bash
./setup.sh
```

This script automatically:

* creates a Next.js project
* configures Docker
* configures PostgreSQL
* configures Redis
* generates environment variables
* prepares the development environment

---

# Step 2 — Start the Development Environment

Build containers:

```bash
./dev.sh rebuild
```

Start the environment:

```bash
./dev.sh start
```

---

# Step 3 — Open the Applications

Ports may change automatically if your system already uses the default ones.

Run this command to see the correct URLs:

```bash
./dev.sh ports
```

Example output:

```
Next.js → http://localhost:3000
pgAdmin → http://localhost:5050
Redis Commander → http://localhost:8081
```

Open the URLs shown in your browser.

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

# Create a GitHub Repository for Your Project

After the project is created, you can connect it to GitHub.

Create a new repository on GitHub, then run:

```bash
git init
git add .
git commit -m "Initial project"

git remote add origin https://github.com/YOUR-USERNAME/YOUR-PROJECT.git
git branch -M main
git push -u origin main
```

---

# Troubleshooting

If something breaks:

```bash
./dev.sh reset
./dev.sh rebuild
```

You can also run diagnostics:

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
