## **Mini Project 1 — Full Stack Docker App Setup**

### Project Overview

This project marks the foundation of a **full-stack Dockerized application**.
You set up the folder structure and initialized a React frontend, Express backend, and PostgreSQL database — preparing for containerization in later stages.

### **Objectives**

* Organize a full-stack app with clear folder structure.
* Add initial backend (`app.js`) and frontend (`App.js`) code.
* Initialize Git and push project setup to GitHub.

### **Project Structure**

```
fullstack-docker-app/
├── backend/
│   ├── app.js
│   └── package.json
├── frontend/
│   ├── src/
│   │   └── App.js
│   └── package.json
├── db-data/
├── docker-compose.yml
├── .env
└── README.md
```

### **Technologies Used**

* React
* Node.js & Express
* PostgreSQL
* Git & GitHub

### **Key Learnings**

* Structuring a full-stack app before Dockerization
* Understanding service separation (frontend, backend, DB)
* Using Git effectively to track and share progress

---

## **Mini Project 2 — Dockerize Full Stack App**

###  Project Overview

In this phase, you **containerized the frontend, backend, and database** using Docker and Docker Compose.
You learned to connect all services and verify that they communicate successfully.

### **Objectives**

* Write Dockerfiles for both frontend and backend.
* Use `docker-compose.yml` to define and run multi-container setup.
* Add environment variables for DB connection.
* Verify React ↔ Express ↔ PostgreSQL integration.

### **Technologies Used**

* Docker & Docker Compose
* React (Frontend)
* Node.js + Express (Backend)
* PostgreSQL (Database)
* Environment Variables (`.env`)

### **Steps to Run**

```bash
# Build and run all containers
docker-compose up --build

# Check containers
docker ps

# Stop containers
docker-compose down
```

### **Required Screenshots**

* `docker ps` output showing containers running
* Browser screenshot of working full-stack app (frontend + backend response)

### **Key Learnings**

* Writing Dockerfiles for different services
* Using Docker Compose for orchestration
* Networking between containers
* Managing environment variables securely

---

## **Mini Project 3 — Persistence & Debugging**

### Project Overview

In the final phase, you enhanced your Dockerized app with **data persistence, logging, and debugging**.
You ensured that your PostgreSQL data persists even after containers restart.

### **Objectives**

* Add and verify **volume persistence** for the database.
* Learn to inspect, debug, and view logs from containers.
* Validate that app remains functional after stop/start.

### **Technologies Used**

* Docker Volumes
* Docker Logs & Exec Commands
* Docker Compose
* React, Node.js, PostgreSQL

### **Commands Used**

```bash
# Check running containers
docker ps

# View logs
docker logs <container-name>

# Access container shell (use sh for alpine images)
docker exec -it <container-name> sh

# Stop and restart
docker-compose stop
docker-compose start
```

### **Required Screenshots**

1. Output of `docker ps` (showing all containers running)
2. Working app in browser after stop/start
3. Example of `docker logs` or `docker exec` usage

### **Key Learnings**

* Persisting DB data using Docker volumes
* Container inspection and debugging commands
* Verifying multi-container stability after restarts

---

## **Final GitHub Repository Checklist**

Make sure your repo includes:

```
frontend/
backend/
db-data/
docker-compose.yml
.env
README.md

------
