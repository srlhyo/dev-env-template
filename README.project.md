# Project Name

This project was created using the **Next.js Docker Development Template**.

The development environment includes:

* Next.js
* Docker
* PostgreSQL
* Redis
* pgAdmin
* Redis Commander

---

# Start Development

Start the development environment:

```bash
./dev.sh start
```

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

Web Application

```
http://localhost:3000
```

pgAdmin

```
http://localhost:5050
```

Redis Commander

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

# Stack

* Next.js
* Docker
* PostgreSQL
* Redis

---

# Notes

* All services run inside Docker.
* No global database installations are required.
* The development environment is isolated from your system.
