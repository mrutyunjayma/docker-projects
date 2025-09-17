# MERN Docker Compose Quick Start

## 1. Copy the code
Clone or copy your project folder with `docker-compose.yml` and `mern/`:

```bash
git clone <your-repo-url>
cd mern-docker-compose
2. Build and run containers
bash
Copy code
docker-compose up --build
This builds images and starts containers: MongoDB → Backend → Frontend.

3. Access the app
Frontend: http://localhost:5000

Backend API: http://localhost:5050

MongoDB: localhost:27017

4. Stop containers
bash
Copy code
docker-compose down
5. Quick Notes
Frontend ↔ Backend: use http://backend:5050 inside Docker.

Backend ↔ MongoDB: use mongodb://mongodb:27017/merndatabase.

depends_on ensures proper container start order.

Ports mapping:

Frontend: host 5000 → container 5173

Backend: host 5050 → container 5050

MongoDB: host 27017 → container 27017

Volumes persist MongoDB data.

yaml
Copy code

---

This is all you need to **copy, run, and remember the key points**.  

If you want, I can make an **even shorter “one-command cheat sheet”** for daily use. Do you want me to do that?