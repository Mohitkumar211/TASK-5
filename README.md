🚀 Deploying an Nginx App on Local Minikube Cluster
🎯 Goal
Set up a local Kubernetes cluster with Minikube, deploy a simple Nginx web server, and access it through the terminal using curl.

🧰 Tools & Technologies
Kubernetes (via Minikube)

kubectl (Kubernetes CLI)

Docker (as Minikube driver)

Linux Virtual Machine

📂 Directory Layout
![image](https://github.com/user-attachments/assets/f54f748d-4523-4a66-b451-93d4921907ff)

🛠️ Steps to Setup
1. 🚦 Launch Minikube
Initialize Minikube using Docker as the backend:
![image](https://github.com/user-attachments/assets/e4671c89-3531-4a0d-b186-651b8df3235a)

Note: Always run Minikube as a normal (non-root) user.

2. 📦 Deploy Nginx
![image](https://github.com/user-attachments/assets/90403c79-7e6a-4aed-8814-719c43b565f3)

3. 🌐 Expose Nginx Using a Service
![image](https://github.com/user-attachments/assets/84d5e482-4f39-4955-af4d-728991f43fad)

NAME | TYPE | CLUSTER-IP | EXTERNAL-IP | PORT(S) | AGE
nginx-service | NodePort | 10.xxx.xxx.xxx | <none> | 80:32xxx/TCP | 2m

4. 🌍 Access the Application
![image](https://github.com/user-attachments/assets/83d5ce65-09a7-4588-9ef8-49c125318576)

Expected output:

Welcome to nginx!

✅ Summary
Minikube cluster initialized locally

Nginx app deployed with 2 replicas

Exposed using NodePort and verified via curl

✨ Bonus Tip
![image](https://github.com/user-attachments/assets/ce7ec4b3-82bc-49cb-958d-8740b54d6e76)

