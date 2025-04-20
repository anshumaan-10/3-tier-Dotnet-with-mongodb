# 3-Tier .NET & MongoDB Web Application
![.NET](https://img.shields.io/badge/.NET-8.0-purple?logo=dotnet)
![MongoDB](https://img.shields.io/badge/MongoDB-7.0-green?logo=mongodb)

A modular **3-tier architecture** web application built using **ASP.NET Core (.NET 8.0)** for the backend and **MongoDB 7.0** as the NoSQL database. This architecture separates concerns into:
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
- [💻 Using MongoDB Shell](#-using-mongodb-shell)
- [🪪 License](#-license)

---

## 📋 Prerequisites

Ensure your system has the following:

- 🐧 **Ubuntu** (or compatible Linux distribution)
- 🟣 [.NET SDK 8.0](https://dotnet.microsoft.com/download/dotnet/8.0)  
- 🍃 [MongoDB 7.0](https://www.mongodb.com/try/download/community)

---

## 🛠 Installation

### 1️⃣ Install .NET SDK & Runtime

```bash
sudo apt-get update
sudo apt-get install -y dotnet-sdk-8.0 aspnetcore-runtime-8.0
```

---

### 2️⃣ Install MongoDB

1. **Add MongoDB GPG key and repo:**

```bash
curl -fsSL https://www.mongodb.org/static/pgp/server-7.0.asc | \
sudo gpg -o /usr/share/keyrings/mongodb-server-7.0.gpg --dearmor
```

```bash
echo "deb [ arch=amd64,arm64 signed-by=/usr/share/keyrings/mongodb-server-7.0.gpg ] https://repo.mongodb.org/apt/ubuntu jammy/mongodb-org/7.0 multiverse" | \
sudo tee /etc/apt/sources.list.d/mongodb-org-7.0.list
```

2. **Install MongoDB:**

```bash
sudo apt update
sudo apt install -y mongodb-org
```

3. **Enable and start MongoDB service:**

```bash
sudo systemctl enable mongod
sudo systemctl start mongod
```

---

### 3️⃣ Set Up MongoDB

1. **Install MongoDB Shell:**

📖 [Official MongoDB Shell Installation Guide](https://www.mongodb.com/docs/mongodb-shell/install/)

2. **Open MongoDB Shell:**

```bash
mongosh
```

3. **Sample MongoDB Shell Commands:**

```bash
show dbs;                         # List all databases
use your_database;               # Switch to a specific DB
show collections;                # List collections
db.Products.find().pretty();     # View documents in Products
```

---

## ▶️ Running the Application

1. **Navigate to the directory** where `Program.cs` is located.

```bash
cd path/to/project/
```

2. **Build the application:**

```bash
dotnet build
```

3. **Run the application:**

```bash
dotnet run
```

🌐 The application will be available in your browser, typically at `http://localhost:5000`.

---

## 💻 Using MongoDB Shell

```bash
mongosh
```

Here are a few essential commands:

| Action | Command |
|--------|---------|
| List databases | `show dbs;` |
| Use database | `use db_name;` |
| List collections | `show collections;` |
| Query a collection | `db.Products.find().pretty();` |

---

## 🪪 License

This project is licensed under the **MIT License**.  
See the [LICENSE](LICENSE) file for details.

---

