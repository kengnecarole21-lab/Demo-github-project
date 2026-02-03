# 🖥️ Infrastructure Status Board

A beautiful, real-time status dashboard for monitoring infrastructure and application health.

![Status Board](https://img.shields.io/badge/status-operational-brightgreen)
![GitHub Pages](https://img.shields.io/badge/GitHub-Pages-blue)

## 🌐 Live Dashboard

**Access the live dashboard at:**
👉 **https://kengnecarole21-lab.github.io/Demo-github-project/**

## 📋 Features

- ✅ **Visual Status Cards** - Color-coded cards with up/down/maintenance indicators
- 📊 **Real-time Summary** - Quick overview of operational vs down systems
- 🎨 **Beautiful UI** - Modern, responsive design with gradient backgrounds
- 📱 **Mobile Friendly** - Works perfectly on all devices
- ⚡ **Fast Updates** - Simple JSON configuration for status changes
- 🔄 **Auto Timestamp** - Shows last update time automatically

## 🚀 Quick Start

### View the Dashboard

Simply open: https://kengnecarole21-lab.github.io/Demo-github-project/

### Update System Status

1. Click on `index.html` in this repository
2. Click the pencil icon (✏️) to edit
3. Find the `applications` array (around line 263)
4. Change the status:
   - `"up"` - System is operational (green)
   - `"down"` - System is offline (red)
   - `"maintenance"` - System under maintenance (orange)
5. Commit changes
6. Dashboard updates automatically in 1-2 minutes!

## 📖 Monitored Systems

### Infrastructure Services
- Vulcan Gitlab
- APP CI Pipelines
- Splunk-AWS-DTRA
- Grafana-On-Prem & Grafana-DTRA
- PrismaCloud-On-Prem & PrismaCloud-DTRA
- Rancher-AWS
- Coder-On-Prem
- Sonarqube-DEPOT

### MINES Environments
- env3, env2, env1
- TEST, STAGING, PROD

### Keycloak Environments
- env3, env2, env1
- test, coresvcs, prod

### Network Infrastructure
- Firewall-0
- Firewall-1

## 🔧 Configuration

All system statuses are defined in the `applications` array in `index.html`:

```javascript
const applications = [
    { name: "Vulcan Gitlab", status: "up" },
    { name: "Rancher-AWS", status: "down" },
    { name: "MINES-PROD", status: "maintenance" },
    // ... add more systems
];
```

## 📥 Embed in Confluence

### Using iframe:

```html
<iframe 
  src="https://kengnecarole21-lab.github.io/Demo-github-project/" 
  width="100%" 
  height="1400" 
  frameborder="0"
  style="border: none;">
</iframe>
```

### In Confluence:
1. Edit your Confluence page
2. Type `/iframe` or insert "HTML" macro
3. Paste the URL: `https://kengnecarole21-lab.github.io/Demo-github-project/`
4. Set width: `100%`, height: `1400px`
5. Publish!

## 🎨 Status Colors

- 🟢 **Green** - System operational (↑)
- 🔴 **Red** - System down (↓)
- 🟠 **Orange** - Under maintenance (⚠)

## 📊 Dashboard Sections

1. **Header** - Title and subtitle
2. **Timestamp** - Last update time
3. **Status Cards** - Visual grid of all systems
4. **Summary** - Count of operational/down/maintenance systems
5. **Legend** - Status indicator guide

## 🔄 Auto-Update

The timestamp refreshes automatically every minute. The status cards update immediately when you commit changes to `index.html`.

## 📱 Responsive Design

The dashboard automatically adapts to:
- Desktop (3-column grid)
- Tablet (2-column grid)
- Mobile (1-column stack)

## 🛠️ Maintenance

### To add a new system:
1. Edit `index.html`
2. Add to the `applications` array:
   ```javascript
   { name: "New System", status: "up" }
   ```
3. Commit changes

### To remove a system:
1. Edit `index.html`
2. Delete the line from the `applications` array
3. Commit changes

## 📄 License

This project is open source and available for use by the team.

## 👥 Team

Created and maintained by the Infrastructure Team.

For questions or issues, contact the DevSecOps team.

---

**Last Updated:** November 2025
**Version:** 1.0
**Status:** Production Ready ✅

