# 🚀 Deploying a Streamlit App with Docker  

This project demonstrates how to containerize a **Streamlit** application using Docker and deploy it efficiently.  

## 📌 Prerequisites  
Before running this project, ensure you have the following installed:  
- [Docker](https://www.docker.com/)  
- [Python 3.x](https://www.python.org/)  
- [Streamlit](https://streamlit.io/)  

---

## 📄 Project Setup  

### **1️⃣ Create a Streamlit App (`app.py`)**  
Create a basic Streamlit application with the following content:

```python
import streamlit as st  

st.title("🚀 Welcome to Streamlit on Docker!")  
st.write("This is a simple Streamlit application running inside a Docker container.")  
```
🐳 Dockerizing the Streamlit App

2️⃣ Create a Dockerfile:
Add a Dockerfile to build an image for the Streamlit app

🛠 Building and Running the Docker Container
3️⃣ Build the Docker Image
Run the following command to build your Docker image:
```bash
docker build -t streamlit-app .
```
4️⃣ Run the Docker Container
Start the container with:
```bash
docker run -p 8501:8501 streamlit-app
```
✅ Accessing the App
Once the container is running, open your browser and go to:
🔗 http://localhost:8501

Your Streamlit app should now be live! 🚀

📌 Verify the Running Container
To check if the container is running, use:
```bash
docker ps
```
If you need to stop the container:
```bash
docker stop <container_id>
```
🎉 Congratulations!
Your Streamlit app is now containerized with Docker and ready to deploy! 🚀
