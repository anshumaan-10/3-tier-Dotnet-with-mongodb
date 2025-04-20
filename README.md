# 🚀 3-Tier .NET & MongoDB Web Application

![.NET](https://img.shields.io/badge/.NET-8.0-purple?logo=dotnet)
![MongoDB](https://img.shields.io/badge/MongoDB-7.0-green?logo=mongodb)
![License](https://img.shields.io/github/license/yourusername/your-repo)
![Build](https://github.com/yourusername/your-repo/actions/workflows/dotnet.yml/badge.svg)

A modular **3-tier architecture** web application built using **ASP.NET Core (.NET 8.0)** and **MongoDB 7.0**.  
This architecture separates concerns into:
- **Presentation Layer**: UI for user interactions
- **Business Logic Layer**: Core application logic
- **Data Access Layer**: Interfaces with MongoDB

---

## 📚 Table of Contents

- [📋 Prerequisites](#-prerequisites)
- [🛠 Installation](#-installation)
  - [1️⃣ Install .NET SDK & Runtime](#1️⃣-install-net-sdk--runtime)
  - [2️⃣ Install MongoDB](#2️⃣-install-mongodb)
  - [3️⃣ Set Up MongoDB](#3️⃣-set-up-mongodb)
- [▶️ Running the Application](#️-running-the-application)
- [🐳 Docker Support](#-docker-support)
- [🤖 CI/CD - GitHub Actions](#-cicd---github-actions)
- [💻 Using MongoDB Shell](#-using-mongodb-shell)
- [🤝 Contributing](#-contributing)
- [🪪 License](#-license)

---

## 📋 Prerequisites

Ensure your system has the following:

- 🐧 **Ubuntu** (or compatible Linux distro)
- 🟣 [.NET SDK 8.0](https://dotnet.microsoft.com/download/dotnet/8.0)  
- 🍃 [MongoDB 7.0](https://www.mongodb.com/try/download/community)

---

## 🛠 Installation

### 1️⃣ Install .NET SDK & Runtime

```bash
sudo apt-get update
sudo apt-get install -y dotnet-sdk-8.0 aspnetcore-runtime-8.0
