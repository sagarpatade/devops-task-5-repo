# Kubernetes Minikube Deployment - Task 5

## 📌 Overview
This project demonstrates deploying an application on a Kubernetes cluster using **Minikube**.  
It includes creating a deployment, exposing it via a service, scaling the deployment, and verifying the setup.

---

## 🛠 Technologies Used
- **Kubernetes**
- **Minikube**
- **kubectl**
- **Docker Desktop** (as Kubernetes backend)

---

## 📂 Project Structure
.
├── deployment.yaml # Deployment configuration
├── service.yaml # Service configuration
├── pod_screenshot.png # Screenshot of running pods
├── service_screenshot.png # Screenshot of running services
└── README.md # Project documentation

yaml
Copy
Edit

---

## 🚀 Steps Performed

### 1️⃣ Start Minikube Cluster
```bash
minikube start
2️⃣ Create Deployment
bash
Copy
Edit
kubectl apply -f deployment.yaml
3️⃣ Create Service
bash
Copy
Edit
kubectl apply -f service.yaml
4️⃣ Verify Pods
bash
Copy
Edit
kubectl get pods
5️⃣ Verify Services
bash
Copy
Edit
kubectl get svc
6️⃣ Access the Application
bash
Copy
Edit
minikube service nginx-service
This will open the app in your default browser.

7️⃣ Scale Deployment
bash
Copy
Edit
kubectl scale deployment nginx-deployment --replicas=3
kubectl get pods
8️⃣ Check Pod Logs
bash
Copy
Edit
kubectl logs <pod-name>
📷 Screenshots
Pods

Services

📄 Deliverables
deployment.yaml

service.yaml

Screenshots of kubectl get pods and kubectl get svc

<img width="794" height="249" alt="svc" src="https://github.com/user-attachments/assets/17b1b452-9189-4ff9-bca9-3fb0fa4dc741" />

<img width="815" height="202" alt="pods" src="https://github.com/user-attachments/assets/53888d4a-0a64-4ceb-bba0-378f57a572aa" />

<img width="1919" height="1007" alt="output" src="https://github.com/user-attachments/assets/b8109e38-bc71-461a-a830-0abd323698d5" />

This README file
