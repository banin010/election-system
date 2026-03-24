# election-system
Election system developed in a group of 4 using Agile SCRUM and waterfall. 

```bash
# 🚀 Deployment Guide: Docker CLI Java App

# 1️⃣ Build the Docker image locally
docker build -t election-cli .

# 2️⃣ Tag the image for Docker Hub
docker tag election-cli yourusername/election-cli:1.0
# Replace 'yourusername' with your Docker Hub username
# '1.0' = version tag

# 3️⃣ Log in to Docker Hub
docker login
# Enter your Docker Hub username and password

# 4️⃣ Push the image to Docker Hub
docker push yourusername/election-cli:1.0
# Uploads the image publicly or privately (depending on your repo settings)

# 5️⃣ Run the container anywhere
docker run -it yourusername/election-cli:1.0
# '-it' = interactive terminal (needed for CLI input)
# Your program runs exactly like locally, no source code exposed

# 6️⃣ Optional: Update version
docker build -t yourusername/election-cli:1.1 .
docker push yourusername/election-cli:1.1
# Increment version for each update
