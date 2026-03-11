# README.md (Template Repository)



````markdown
# Next.js Docker Development Template

Create a **complete web development environment in minutes**.

This template automatically creates a project with:

- **Next.js** (web framework)
- **PostgreSQL** (database)
- **Redis** (cache)
- **pgAdmin** (database management UI)
- **Redis Commander** (Redis UI)
- **Docker** containers for isolated development

Everything runs inside Docker so it **does not affect your system**.

---

# Requirements

Install these first.

## Docker

Download and install:

https://www.docker.com/products/docker-desktop/

Verify installation:

```bash
docker --version
````

Docker must be **running** before starting the environment.

---

## Node.js

Download:

[https://nodejs.org](https://nodejs.org)

Verify installation:

```bash
node --version
```

---

# Step 1 — Create a New Project

Clone this repository:

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

This will automatically:

* create a Next.js project
* configure Docker
* configure PostgreSQL
* configure Redis
* generate environment variables
* prepare the development environment

---

# Step 2 — Start the Development Environment

Build the containers:

```bash
./dev.sh rebuild
```

Start the environment:

```bash
./dev.sh start
```

---

# Step 3 — Open the Applications

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

````

---

# README.project.md (Generated Project)

```markdown
# Project Name

This project was created using the **Next.js Docker Development Template**.

It includes a fully configured development environment with:

- Next.js
- Docker
- PostgreSQL
- Redis
- pgAdmin
- Redis Commander

---

# Development

Start the development environment:

```bash
./dev.sh start
````

---

# Rebuild Containers

If dependencies change or containers fail:

```bash
./dev.sh rebuild
```

---

# Stop the Environment

```bash
./dev.sh stop
```

---

# View Logs

```bash
./dev.sh logs
```

---

# Services

### Web Application

```
http://localhost:3000
```

### pgAdmin

Database management interface.

```
http://localhost:5050
```

### Redis Commander

Redis management interface.

```
http://localhost:8081
```

---

# Environment Variables

Environment configuration is stored in:

```
.env
```

---

# Reset the Environment

If containers break or databases need resetting:

```bash
./dev.sh reset
```

Then rebuild:

```bash
./dev.sh rebuild
```

---

# Project Stack

* Next.js
* Docker
* PostgreSQL
* Redis

---

# Notes

* All services run inside Docker.
* No global database installations are required.
* The development environment is isolated from your system.

```
```
