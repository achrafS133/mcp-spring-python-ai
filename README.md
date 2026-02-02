# MCP-Spring-Python-AI: Multi-Protocol Chatbot 

![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)  
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.x-brightgreen.svg)  
![Angular](https://img.shields.io/badge/Angular-20.x-red.svg)  
![Python](https://img.shields.io/badge/Python-3.x-blue.svg)  
![NodeJS](https://img.shields.io/badge/NodeJS-18+-green.svg)  

A **Model Context Protocol (MCP)**-based chatbot integrating **Spring Boot (AI + Ollama)**, **Python/NodeJS MCP servers**, and an **Angular frontend**.  

**Author**: [ER-RAHOUTI ACHRAF](https://github.com/your-profile)  

---

##  Table of Contents  
- [Overview](#-overview)  
- [Key Features](#-key-features)  
- [Architecture](#-architecture)  
- [Installation](#-installation)  
- [Usage](#-usage)  
- [Technologies](#-technologies)  
- [Configuration](#-configuration)  
- [Testing](#-testing--debugging)  
- [Screenshots](#-screenshots)  

---

##  Overview  
A modular chatbot demonstrating **MCP protocol** implementation with:  
- **Spring Boot** (SSE-based MCP client/server)  
- **Python/NodeJS** (STDIO-mode MCP tools)  
- **Angular** frontend for interactive chat.  

---

##  Key Features  
- **Multi-Backend Integration**:  
  - Spring AI + Ollama (Qwen3 model)  
  - Python/NodeJS MCP servers for tool execution.  
- **Real-Time Communication**: SSE for streaming responses.  
- **Agent-Based UI**: Angular frontend with thinking/reply distinction.  
- **Tool Ecosystem**: Stock lookup, file ops, employee info, etc.  

---

##  Architecture  
The project consists of four main components:  

- **mcp-client/**: Spring Boot MCP Client  
  - Implements AI agents and REST controllers.  
  - Connects to MCP servers and manages AI interactions.  

- **mcp-server/**: Spring Boot MCP Server  
  - Provides MCP tools and services.  
  - Implements backend logic for tool execution.  

- **mcp-frontend/**: Angular Frontend  
  - Interactive chat UI with agent thinking and reply views.  
  - Built with Angular CLI.  

- **python-mcp-server/**: Python MCP Server  
  - Additional MCP tools implemented in Python.  
  - Provides extended functionality via MCP protocol.  

- **Screenshots/**: Directory containing project screenshots for reference.  
gi
---

##  Installation

### Prerequisites
- [Ollama](https://ollama.ai/) (`ollama pull qwen3`)  
- [Node.js 18+](https://nodejs.org/)  
- Angular CLI (`npm install -g @angular/cli`)  
- [Postman](https://www.postman.com/) (for API testing)  
- Java 17+ and Maven (for Spring Boot projects)  

### Steps
1. Clone the repository and navigate to the project directory:  
   ```bash
   git clone https://github.com/your-username/mcp-spring-python-ai.git  
   cd mcp-spring-python-ai  
   ```  
2. Build and run the Spring Boot client and server:  
   ```bash
   cd mcp-client
   ./mvnw clean install
   ./mvnw spring-boot:run
   ```  
   In a separate terminal:  
   ```bash
   cd mcp-server
   ./mvnw clean install
   ./mvnw spring-boot:run
   ```  
3. Install and run the Angular frontend:  
   ```bash
   cd mcp-frontend
   npm install
   ng serve
   ```  
   Open your browser at `http://localhost:4200/`.  
4. Run the Python MCP server (optional):  
   ```bash
   cd python-mcp-server
   python main.py
   ```  

---

##  Usage

- Use the Angular frontend to interact with the chatbot.  
- The Spring Boot client communicates with MCP servers for AI and tool execution.  
- The Python MCP server provides additional tools accessible via MCP protocol.  

---

##  Technologies

- Java 17+, Spring Boot 3.x  
- Angular 20.x  
- Python 3.x  
- Node.js 18+  
- Ollama Qwen3 AI model  
- Model Context Protocol (MCP)  

---

##  Configuration

- Configure MCP servers in `mcp-client/src/main/resources/mcp-servers.json`.  
- Application properties are in `src/main/resources/application.properties` for client and server.  
- Adjust Angular environment and configuration files as needed.  

---

##  Testing & Debugging

- Run unit tests for Spring Boot projects:  
  ```bash
  ./mvnw test
  ```  
- Run Angular unit tests:  
  ```bash
  ng test
  ```  
- Use Postman or similar tools for API testing.  

---

##  Screenshots

See the `Screenshots/` directory for visual references of the application in action.



---

##  License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
