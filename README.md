# Openflow Local Demo – Oracle + NiFi + Snowflake Bundle

## Setup
1) `.env` anpassen  
2) **Snowflake NARs** in `./nifi-extensions/` legen  
3) **JDBC JARs** in `./nifi-lib/` legen (snowflake-jdbc.jar, optional ojdbc11.jar)  
4) Starten:
   ```bash
   docker compose up -d
