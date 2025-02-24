# SELFHOST YOUR AI AGENT 🤖🌐

This repository provides a simple way to self-host your own AI agent using Docker and Docker Compose. It's designed for developers who want to quickly spin up their own AI-powered services.

---

## 🚀 Overview

Easily deploy your AI agent by setting up the necessary Docker containers and environment variables. After running the containers, you’ll import a template workflow to get your AI agent up and running.

---

## 📋 Prerequisites

Before you begin, make sure you have the following:

- Docker installed on your system 🐳
- Docker Compose installed 🛠️
- Basic knowledge of Docker and environment variables
- Access to the `n8n` web interface to import workflows 🌐

### Setup Environment

1. Copy the `.env.example` file to `.env`.
    ```bash
    cp .env.example .env
    ```
2. Modify the `.env` file to suit your environment, such as adding API keys or other configuration details.

---

## ⚙️ How to Start

To get your AI agent up and running:

1. **Start Docker**:
   If Docker isn't running, start it now.

2. **Run Docker Compose**:
    ```bash
    docker-compose up -d
    ```
    This will build and start the necessary containers in detached mode.

3. **Access `n8n` Web Interface**:
    Once the containers are up, you can access the `n8n` web interface at `http://localhost:5678` (or the appropriate address if you customized it).

4. **Import the Template Workflow**:
    - Download or navigate to the `workflow-template/agent_template.json` file in this repository.
    - In the `n8n` interface, go to the **Workflow** menu and select **Import**.
    - Upload the `agent_template.json` file to import the template workflow.
    - Save and activate the workflow to start using your AI agent.

---

## 🛑 How to Shutdown

When you're finished, you can shut down the containers with:

```bash
docker-compose down
```

This will stop and remove the containers, freeing up resources on your system.

---

## 🧑‍💻 Customization

Feel free to customize the `.env` file and the Docker setup to fit your specific needs. You can integrate different AI models, change ports, or add more services.

Additionally, you can modify the imported workflow or create new ones to enhance the functionality of your AI agent.

---

## 📚 Resources

- [Docker Documentation](https://docs.docker.com/)
- [Docker Compose Documentation](https://docs.docker.com/compose/)
- [n8n Documentation](https://n8n.io/docs/)

---

## 🤝 Contributing

If you'd like to contribute to this project, feel free to submit a pull request! Contributions are always welcome.

---

## 👨‍💻 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.