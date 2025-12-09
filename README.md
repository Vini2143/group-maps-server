# Group Maps API

Group Maps is a backend service that powers a geolocation-based application designed for coordinating real-life group activities. It provides endpoints for authentication, user management, group creation, real-time location updates, and more.

---

##  Technologies Used
- **Python 3.13.5** — Backend language  
- **FastAPI 0.115.12** — High-performance API framework  
- **PostgreSQL 17** — Relational database  
- **Docker & Docker Compose** — Containerized development and deployment

For reference, the specific versions of packages used in this project are listed in requirements.txt. Consult this file if you need to check or match dependency versions.

---

##  Requirements

### Prerequisites
- Python **3.13.5**
- Docker and Docker Compose (optional)

---

##  Environment Setup

Create a `.env` file in the project root.  
You can use the provided `.env.example` as a template.

**Generate the `SECRET_KEY`:**
```bash
openssl rand -hex 32
```

#### Run the project

#### With Docker (recommended):
```bash
docker-compose up --build
```
API:
http://127.0.0.1:8000/docs


#### Without Docker:

#### 1. Create virtual environment
```bash
python -m venv venv
```

Activate (Linux/macOS)
```bash
source venv/bin/activate
```

Activate (Windows)
```bash
venv\Scripts\activate
```

#### 2. Install dependencies
```bash
pip install -r requirements.txt
```

#### 3. Create PostgreSQL database
Run in your PostgreSQL client:
CREATE DATABASE app;

#### 4. Start the FastAPI server
```bash
fastapi dev app/main.py
```

API:
http://127.0.0.1:8000/docs
