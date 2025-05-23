#  Azure Post-Deployment Manual Configuration Guide

After deploying Azure infrastructure and services, a few manual configuration steps are required to ensure everything functions correctly. This guide provides links to individual `README` files that cover these tasks in detail.

---

### 1. Azure Function App – VNet & Environment Variables Configuration

After deploying the Function App, additional configuration is needed for VNet integration and environment variable setup.  
📄 Refer to: [FAReadme.md](./ReadmeFile/FAReadme.md)

---

### 2. Container & Storage Account – Config File, Volume Mount, and Runtime Setup

Following the deployment of a Container App and Storage Account, you need to upload the config file (e.g., `dab-config.json`), mount the volume, and perform container-level configuration.  
📄 Refer to: [containerconfigreadme.md](./ReadmeFile/containerconfigreadme.md)

---

### 3. Event Grid – Webhook Integration

After deploying the Storage Account, Function App, and Webhook code, you need to create an event Grid System Topic and set up an event subscription for real-time notifications.  
📄 Refer to: [EventGridReadme.md](./ReadmeFile/EventGridReadme.md)

---

### 4. App Registration – OAuth2 & API Security

Once all services and infrastructure are deployed, you must create and configure App Registrations to enable secure OAuth2-based access to APIs.  
📄 Refer to: [appregistrationReadme.md](./ReadmeFile/appregistrationReadme.md)

---

### 5. Diagnostic Settings & Cost Management Dashboard Configuration

Before deploying your dashboard, it’s essential to:

- Enable Diagnostic Settings for all relevant services
- Set up Cost Analysis views in Azure Cost Management

These tasks ensure the dashboard is populated correctly.  
📄 Refer to: [Dashboard&diagnosticsettingReadme.md](./ReadmeFile/Dashboard%26diagnosticsettingReadme.md)

---

##  Subnet Configuration (Post VNet Deployment)

After deploying the **Virtual Network (VNet), you need to create subnets that will be associated with services like Storage Account, Function App, and others during their configuration.

📄 Refer to: [Subnet Configuration Guide](./ReadmeFile/subnetreadme.md)


Make sure to follow each linked guide step-by-step to avoid runtime and visibility issues post-deployment. 


