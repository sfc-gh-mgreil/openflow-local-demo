# Openflow Local Demo – Oracle + NiFi + Snowflake

This repository provides a **local demo setup** to load data from **Oracle** into **Snowflake** using **Apache NiFi**.  
It bundles all required components into a Docker Compose environment.

---

## 🚀 Setup Guide

### 1. Environment Variables
Create a `.env` file in the project root with your credentials:

```env
# Oracle
ORACLE_PASSWORD=your_oracle_password

# NiFi
NIFI_USER=admin
NIFI_PASS=your_password

2. Extensions & Drivers
Place the Snowflake NARs in:
./nifi-extensions/

Place the JDBC JARs in:
./nifi-lib/
Required:

snowflake-jdbc.jar

For oracle connection:

ojdbc11.jar

3. Start the Demo
Run the following command to start Oracle DB and NiFi:

docker compose up -d
Once running, NiFi can be accessed at:
👉 https://localhost:8443/nifi

📂 Project Structure
├── docker-compose.yml     # Container setup for Oracle & NiFi
├── nifi-extensions/       # Place Snowflake NARs here
├── nifi-lib/              # Place JDBC drivers here
├── nifi-flows/            # Example NiFi flows
└── README.md              # This guide
