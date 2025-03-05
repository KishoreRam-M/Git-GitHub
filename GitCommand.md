Knowing **every** DevOps, backend, and cloud command is a massive topic, but I'll give you a **comprehensive** list categorized by **Git, Linux, Docker, Kubernetes, CI/CD, Cloud (AWS/GCP/Azure), Backend (Spring Boot), Database, Monitoring, and more**.  

---

# 🚀 **DevOps, Backend & Cloud Command Cheat Sheet**

## 🔹 **1. Git & GitHub Commands**
```sh
# Initialize and configure Git
git init                  # Initialize a new repository
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"

# Check status and log
git status                # Show changed files
git log --oneline --graph --all   # View commit history in one line

# Add, commit, push, and pull
git add .                 # Stage all changes
git commit -m "Commit message"   # Commit changes
git push origin main      # Push changes to remote
git pull origin main      # Pull latest changes

# Branching
git branch feature-xyz    # Create a new branch
git checkout feature-xyz  # Switch to a branch
git merge feature-xyz     # Merge branch into main
git push origin feature-xyz  # Push new branch

# Reset & Rebase
git reset --hard HEAD~1   # Undo last commit
git rebase main           # Rebase feature branch onto main

# Stash
git stash                 # Save changes without committing
git stash pop             # Restore stashed changes
```

---

## 🔹 **2. Linux Commands**
```sh
# File Operations
ls -lah                    # List files with details
cd /path/to/directory       # Change directory
mkdir myfolder             # Create a folder
rm -rf myfolder            # Delete a folder

# Disk & Memory
df -h                      # Show disk usage
free -m                    # Show RAM usage

# Process Management
ps aux                     # Show running processes
top                        # Monitor system resources
kill -9 <PID>              # Kill a process

# Networking
ifconfig                   # Show IP addresses
netstat -tulnp             # Show open ports
ping google.com            # Test connectivity

# Users & Permissions
whoami                     # Show current user
chmod 755 file.sh          # Change file permissions
sudo useradd devuser       # Add new user
```

---

## 🔹 **3. Docker Commands**
```sh
# Basic Commands
docker --version           # Check Docker version
docker ps                  # List running containers
docker ps -a               # List all containers

# Container Operations
docker run -d -p 8080:80 nginx    # Run a container
docker stop <container_id>        # Stop a running container
docker rm <container_id>          # Remove a container

# Image Management
docker images               # List all images
docker pull ubuntu          # Download an image
docker build -t myapp .     # Build an image from Dockerfile

# Volume & Networks
docker volume ls            # List volumes
docker network ls           # List networks
```

---

## 🔹 **4. Kubernetes Commands**
```sh
# Basic Cluster Info
kubectl get nodes           # List all nodes
kubectl get pods            # List all pods
kubectl get services        # List all services

# Managing Pods
kubectl run nginx --image=nginx   # Run an nginx pod
kubectl delete pod nginx          # Delete a pod

# Deployments
kubectl create deployment myapp --image=myimage
kubectl get deployments          # List deployments
kubectl delete deployment myapp  # Delete a deployment

# Logs & Debugging
kubectl logs mypod               # View logs of a pod
kubectl exec -it mypod -- /bin/bash  # Access shell inside a pod
```

---

## 🔹 **5. CI/CD (Jenkins, GitHub Actions)**
```sh
# Jenkins CLI
jenkins --version                 # Check Jenkins version
jenkins jobs                       # List all jobs
jenkins build my-job               # Trigger a job

# GitHub Actions
gh workflow list                    # List workflows
gh run list                          # List workflow runs
```

---

## 🔹 **6. Cloud Commands (AWS, GCP, Azure)**

### ☁ **AWS CLI**
```sh
aws configure                  # Set up AWS CLI
aws s3 ls                      # List all S3 buckets
aws ec2 describe-instances     # List EC2 instances
aws lambda list-functions      # List Lambda functions
aws rds describe-db-instances  # List RDS databases
```

### ☁ **GCP CLI**
```sh
gcloud auth login               # Authenticate CLI
gcloud compute instances list   # List all VM instances
gcloud projects list            # List all projects
gcloud sql instances list       # List Cloud SQL instances
```

### ☁ **Azure CLI**
```sh
az login                        # Authenticate CLI
az vm list                      # List all virtual machines
az storage account list         # List all storage accounts
```

---

## 🔹 **7. Spring Boot (Backend) Commands**
```sh
# Start Spring Boot App
mvn spring-boot:run      # Start with Maven
gradle bootRun           # Start with Gradle

# Build the App
mvn clean install        # Build a JAR file
gradle build            # Build with Gradle

# Run Tests
mvn test                # Run unit tests
gradle test             # Run tests with Gradle
```

---

## 🔹 **8. Database (SQL & NoSQL)**
### **PostgreSQL**
```sh
psql -U postgres         # Login to PostgreSQL
\l                      # List databases
\c mydatabase           # Connect to a database
\d                      # List tables
SELECT * FROM users;    # Query a table
```

### **MongoDB**
```sh
mongo                    # Start MongoDB shell
show dbs                 # List databases
use mydb                 # Switch database
db.users.find()          # Query collection
```

---

## 🔹 **9. Monitoring & Logging**
```sh
# ELK Stack (Elasticsearch, Logstash, Kibana)
systemctl start elasticsearch    # Start Elasticsearch
systemctl start kibana           # Start Kibana

# Prometheus & Grafana
docker run -d -p 9090:9090 prom/prometheus   # Run Prometheus
docker run -d -p 3000:3000 grafana/grafana   # Run Grafana

# Logs
tail -f /var/log/syslog       # View logs in real time
journalctl -u nginx --since today   # View service logs
```

---

## **📌 Summary: Essential Commands**
| Category          | Important Commands |
|------------------|------------------|
| **Git**         | `git add .`, `git commit -m`, `git push`, `git pull` |
| **Linux**       | `ls`, `cd`, `rm -rf`, `ps aux`, `top` |
| **Docker**      | `docker ps`, `docker run`, `docker stop` |
| **Kubernetes**  | `kubectl get pods`, `kubectl apply -f` |
| **Cloud (AWS)** | `aws s3 ls`, `aws ec2 describe-instances` |
| **Spring Boot** | `mvn spring-boot:run`, `gradle bootRun` |
| **Database**    | `psql -U postgres`, `mongo` |

---

## 🎯 **Final Thoughts**
This is a **complete DevOps, backend, and cloud command reference** covering **Git, Linux, Docker, Kubernetes, AWS, Spring Boot, Databases, and CI/CD.**  

Want more details on any topic? Let me know! 🚀🔥
