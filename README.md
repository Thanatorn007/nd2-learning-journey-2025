# ND2 Learning Journey 2025: Industrial Full-Stack Developers

Welcome to my comprehensive learning repository for the **ND2 Industrial Full-Stack Developers** program. This document serves as a detailed roadmap and technical log, capturing the end-to-end process of bridging Operational Technology (OT) with Information Technology (IT).

This repository consolidates my knowledge ranging from **Containerization (Docker)** and **Type-Safe Web Development** to **Real-time Databases** and **Local AI Integration**.

------------------------------------------------------------------------------------------------------------------------------------------------------------------

## 🐳 1. DevOps Concepts for Automation Systems
**Goal:** Establishing a consistent, reproducible, and scalable development environment using Containerization technology to solve "It works on my machine" issues.

![Docker for Developers](images/docker-dev.png)

### 🔹 Containerization Strategy
Understanding the shift from monolithic deployments to microservices:
* **Docker for Developers:**
    * Creating isolated environments for Database, API, and Frontend services.
    * Ensuring consistency across development, testing, and production stages.
* **Service Orchestration:**
    * Managing multi-container applications (MQTT Broker, InfluxDB, Node-RED, Web Server) using **Docker Compose**.
    * Defining networking and volume persistence to ensure data safety during container lifecycles.

### 🔹 Deployment & Automation Workflow
* **Requirement:** Seamless integration of code changes into the industrial production environment.
* **Technique:**
    * **CI/CD Pipelines:** Automating the build and testing process of Docker images.
    * **System Integration:** Connecting the Dockerized Backend, React Frontend, and Local AI services into a unified internal network.

------------------------------------------------------------------------------------------------------------------------------------------------------------------

## 💻 2. Front-End Development (UX/UI & React)
**Goal:** Architecting intuitive and responsive Human-Machine Interfaces (HMI) that enable operators to visualize complex industrial data effectively.

### 🔹 Modern Web Architecture
Moving beyond basic HTML/CSS to robust Single Page Applications (SPA).

![TypeScript Programming](images/typescript.png)

* **Type-Safe Programming (TypeScript):**
    * **Concept:** enforcing static typing to catch errors at compile-time rather than runtime.
    * **Application:** utilized for defining strict interfaces for API responses and sensor data structures, significantly reducing bugs in large-scale applications.
* **React Ecosystem:**
    * **Component-Based Architecture:** Breaking down complex dashboards into reusable, modular components (e.g., Gauge Card, Trend Chart).
    * **State Management:** Efficiently handling real-time data updates without unnecessary re-renders.

### 🔹 UX/UI Design for Industry
Standardizing the design process for clarity and safety.

![UX/UI Design](images/ui-ux-dev.png)

* **Design Workflow:** From wireframing in self-hosted design tools to practical implementation in code.
* **User-Centric Layouts:** Applying UX principles to ensure operators can quickly identify alerts, system status, and anomalies (High Contrast, Clear Hierarchy).
* **Data Visualization:** Implementing **SVG** and charting libraries to render real-time telemetry and historical trends with high performance.

------------------------------------------------------------------------------------------------------------------------------------------------------------------

## 🔌 3. Back-End Development (API & Database)
**Goal:** Building the robust backbone of the system responsible for data management, device control, and security.

![API Server](images/api-server.png)

### 🔹 API Server Architecture
* **RESTful Services:**
    * Designing scalable APIs to manage IoT devices, handle user authentication, and serve configuration data.
    * Implementing **Middleware** for logging, error handling, and request validation.
* **Real-time Interaction:**
    * Bridging the gap between the server and the frontend using **WebSockets** or **MQTT over WebSockets** for instant bi-directional communication.

### 🔹 Database Engineering
![Database Design](images/db-design.png)

* **ORM (Object-Relational Mapping):**
    * Utilizing ORM tools for efficient, secure, and type-safe database queries, abstracting complex SQL commands.
* **Real-time Database Design:**
    * Structuring schemas optimized for high-frequency read/write operations suitable for IoT telemetry data.
    * Balancing between relational data (Users, Devices) and time-series data (Sensor Logs).

------------------------------------------------------------------------------------------------------------------------------------------------------------------

## 🤖 4. Data Processing and AI (Local Intelligence)
**Goal:** Leveraging Artificial Intelligence to create "Smart" Industrial Systems that operate autonomously without relying on external cloud services.

![Local LLM & AI](images/ai-local.png)

### 🔹 Local Intelligence Stack
* **Self-Hosted LLM:**
    * Deploying Large Language Models (like Llama 3, Mistral) on local servers.
    * **Benefit:** Ensuring data privacy (no data leaves the factory) and zero latency response times.
* **AI Agents & Prompt Engineering:**
    * Designing system prompts to turn generic LLMs into specialized assistants (e.g., a "Maintenance Bot" that interprets specific error codes).

### 🔹 Automation Workflows
* **Agent Builders vs. Workflow Tools:**
    * Comparing tools like **n8n** for logic-based automation against AI Agent Builders.
    * **Application:** Triggering physical actions (e.g., turning off a machine) based on complex AI decisions or anomaly detection.

------------------------------------------------------------------------------------------------------------------------------------------------------------------

## 🚀 Future Works/Roadmap
Plans to synthesize these skills into next-generation industrial solutions.

* **Project 1: Self-Hosted AI Maintenance Assistant**
    * **Scope:** A Chatbot interface where technicians can ask "Why is Machine A vibrating?" and the Local LLM analyzes real-time logs to provide diagnostic steps.
    * **Tech Stack:** React (Chat UI), Python API (RAG Pipeline), Local LLM (Ollama).
    * **Status:** *Prototyping & Prompt Testing Phase.*

* **Project 2: Centralized Plant Control Center**
    * **Scope:** A Unified Dashboard visualizing data from 50+ IoT nodes with bi-directional control capabilities.
    * **Tech Stack:** Dockerized Microservices, React + TypeScript, InfluxDB, Nginx.
    * **Status:** *Architecture Design Phase.*

------------------------------------------------------------------------------------------------------------------------------------------------------------------
*Created as part of the ND2-MP5 assignment. A living document of my technical growth in 2025.*
