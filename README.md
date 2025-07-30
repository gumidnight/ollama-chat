# Ollama-Chat

This project provides a Docker Compose setup to run **Ollama** (a local large language model runtime) with a ChatGPT-style frontend UI (Open WebUI).  
It enables you to host your own private AI chat assistant powered by open-source models with GPU support.

---

## Features

- Run Ollama backend locally with GPU acceleration (NVIDIA CUDA)
- ChatGPT-style UI via Open WebUI on `http://localhost:3000`
- Easy model management with Ollama CLI inside the container
- Fully containerized with Docker Compose for quick setup and deployment
- Customizable UI and backend configurations

---

## Prerequisites

- Ubuntu 20.04 or later
- Docker and Docker Compose installed
- NVIDIA GPU with latest drivers and NVIDIA Container Toolkit installed

---

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/ollama-chat.git
cd ollama-chat
```
### 2. Start the Docker containers
```bash
docker-compose up -d
```
This will start:

Ollama backend API at http://localhost:11434

ChatGPT UI frontend at http://localhost:3000

### 3. Pull a model inside the Ollama container
Enter the Ollama container shell:
```bash
docker exec -it ollama ollama pull llama2
```
You can replace llama2 with other supported models

###  4. Open the UI
Open your browser and visit:
http://localhost:3000

### 5. On my next steps i will try to customise the model
a. Branding & UI Customization
b. Enable Ldap Login
c.Data Privacy & Logging
d. Performance & Scaling
e. Use GPT‑4 API


