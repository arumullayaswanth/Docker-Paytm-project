## 🛍️ Docker-Paytm-Project  

A **containerized Paytm-like web service** built using **Docker, Docker Compose, and Jenkins**. This project provides users with **mobile recharges, DTH payments, movie bookings, and train ticket reservations** using a microservices architecture.

---

### 📌 Features  

✅ **Multi-Service Architecture** – Recharge, DTH, Movies, and Train services as independent containers  
✅ **Responsive Design** – Works on all screen sizes  
✅ **Dockerized Deployment** – Runs using Docker and Docker Compose  
✅ **CI/CD Integration** – Jenkins pipeline for automated build, push, and deployment  
✅ **Scalability** – Docker Swarm for high availability  
✅ **Secure Authentication (Optional)** – Can integrate OAuth/Firebase authentication  

---

### 📂 Tech Stack  

| **Category**   | **Technology** |
|--------------|-------------|
| **Frontend**  | HTML, CSS, JavaScript |
| **Backend** (Optional) | Node.js, Express, Firebase |
| **Containerization** | Docker, Docker Compose |
| **CI/CD** | Jenkins, GitHub Actions |
| **Deployment** | Docker Swarm, AWS, DigitalOcean |

---

## 🚀 Setup & Installation  

### **1⃣ Clone the Repository**  
```bash
git clone https://github.com/arumullayaswanth/Docker-Paytm-project.git
cd Docker-Paytm-project
```



# Step 1: Build your Docker image (from Dockerfile in current directory)
docker build -t paytam .

# Step 2: View the list of built images
docker images

# Step 3: Run the container to test it locally
docker run -d -p 80:80 paytam

# Step 4: Tag the image for Docker Hub (replace with your username)
docker tag paytam yaswanth111/paytam:latest

# Step 5: Login to Docker Hub
docker login

# Step 6: Push the image to Docker Hub
docker push yaswanth111/paytam:latest


















### **2⃣ Run Locally with Docker Compose**  
```bash
docker-compose up -d
```
> This will start all services (`Recharge`, `Movies`, `Train`, `DTH`).

### **3⃣ Access Services**  
- **Recharge**: `http://localhost:84`  
- **Movies**: `http://localhost:81`  
- **Train**: `http://localhost:82`  
- **DTH**: `http://localhost:83`  

---

## 🖥️ Docker Deployment  

### **1⃣ Build the Docker Image**  
```bash
docker build -t paytm-service .
```

### **2⃣ Tag & Push to Docker Hub**  
```bash
docker tag paytm-service your-dockerhub-username/paytm-service:latest
docker push your-dockerhub-username/paytm-service:latest
```

### **3⃣ Deploy Using Docker Swarm**  
```bash
docker swarm init
docker stack deploy -c docker-compose.yml paytm
```

---

## 🛠️ Future Enhancements  

✅ Add secure authentication (OAuth/Firebase)  
✅ Implement a fully functional backend with APIs  
✅ Improve UI/UX with Tailwind CSS or Bootstrap  
✅ Integrate Kubernetes for enhanced scaling  

---

## 📞 Contact & Support  

 
🌐 **GitHub**: [arumullayaswanth](https://github.com/arumullayaswanth)  

---

## 📛 License  

This project is open-source and available under the **MIT License**.  

---

### ⭐ If you found this helpful, don’t forget to **star** this repo! 🚀  
