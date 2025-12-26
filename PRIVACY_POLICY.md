# Privacy Policy - WhatsApp Automation Service

**Effective Date: December 26, 2025**

## 1. Information We Collect
- WhatsApp messages (text, media, metadata) received via Meta WhatsApp Business Cloud API
- Sender phone numbers 
- Timestamps and message IDs
- Workflow execution logs [web:82]

## 2. How We Use Your Data
- Process automation workflows triggered by WhatsApp messages
- Store conversation history in n8n database (local Docker volume)
- Execute connected services (APIs, databases) per workflow logic [web:83]

## 3. Data Storage & Security
- **Self-hosted on private Linux server** (no cloud sharing)
- Encrypted at rest in Docker volumes
- Local access only (port 5678, firewall protected)
- No data sharing with third parties [memory:1]

## 4. Data Retention
- Messages stored until manually deleted via n8n workflows
- Docker volume persists data across restarts
- Export/delete: n8n UI → Workflows → Data management

## 5. Your Rights
- **Stop service**: Send `/stop` or contact admin
- **Delete data**: `docker compose down -v` removes all data
- **Access logs**: n8n dashboard → Executions tab

## 6. Contact
For privacy concerns: [your-email@example.com]

**This is a personal automation service. Production use requires legal review.**
