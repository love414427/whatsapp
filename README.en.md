<div align="center">
    <img src="https://raw.githubusercontent.com/love414427/demo-kongjiang-didi/main/zhanshi/newlogo%402x.png" />
</div>

<div align="center">

### 📱 Source Code Download: https://t.me/whatsappoem

#### ✨✨ Jianghu Technology » WhatsApp Marketing System ⚡️ Multi-Channel Access / Smart Customer Service / Data Analytics ✨✨

#### ✨✨ Custom development services available! Official Website: www.aprx.me Contact: @jeequan ✨✨

# 👏👏👏 WhatsApp Marketing Management System 👏👏👏

(WhatsApp Marketing, Customer Service Management, Multi-Channel Access, Data Analytics)



</div>

<div align="center">
    If this project helps you, please give it a "Star" ❤️ Thank you for your support!
</div>

***

### 📖 Introduction:

**ContiNew WhatsApp Marketing System** is an enterprise-grade **WhatsApp Marketing and Customer Service Management Platform**, built on the ContiNew Admin high-quality multi-tenant backend framework. It supports enterprise-level features such as multi-channel access, smart customer service, and multi-tenant management.

The system integrates **WhatsApp API Mode**, **Browser Mode**, and **Restore Mode** for number registration, providing complete solutions including unified reception, visitor monitoring, and data analytics to make enterprise WhatsApp marketing more efficient.

Open Source Version: https://github.com/love414427/WhatsApp-Admin

***

### 💡 System Highlights:

> 1. **Multi-Channel Access** - Supports WhatsApp API Mode, Browser Mode, Restore Mode, and other access methods
> 2. **Smart Customer Service** - Real-time visitor monitoring, online customer service, quick replies, WebSocket real-time messaging
> 3. **Data Analytics** - Multi-dimensional statistics, follower analysis, conversion tracking, dashboard visualization
> 4. **Multi-Tenant SaaS** - SaaS deployment, tenant isolation, package management, data permission control
> 5. **Frontend-Backend Separation** - Backend Spring Boot 3.3 + Frontend Vue 3 + Arco Design
> 6. **High Concurrency Support** - Redis caching, WebSocket communication, distributed deployment
> 7. **Template Management** - Supports H5 pages, PC pages, mobile templates, cashier templates, etc.
> 8. **Operations Monitoring** - Online user management, login logs, operation logs, task scheduling

***

### 💻 Environment & Framework Requirements:

```
* JDK 17+
* Spring Boot 3.3.12
* Node.js 20+
* MySQL 8.0+
* Redis 7.0+
* Nginx 1.25+
* PM2 (Node.js Process Manager)
```

[![](crmeb/crmebimage/crmebimage/demoimage/gitee-广告_java多商户.jpg)](https://www.crmeb.com/ask/thread/46123)

### 🎬 System Demo:

![](展示/admin/01登录界面.png)
![](展示/admin/02首页.png)
![](展示/admin/03产品页面.png)
![](展示/admin/04分析仪.png)
![](展示/admin/05进粉统计.png)

**H5 Frontend Preview:**

Mobile: https://didi.aprxapp.cn/pages/users/login/index
Account/Password: 18788888888/a123456

WEB Admin: https://didi.aprxapp.cn/admin
Account/Password: admin/admin888

Main Site (iOS + Android Download):
https://di.aprxapp.cn/v5/index.html

***

### 📱 Core Features

#### Product Center
![](展示/admin/06APi模式下的%20盗取的账号列表.png)
![](展示/admin/07APi模式下的%20后端出码-8位授权码模式.png)
![](展示/admin/09APi模式下的配置页面.png)

#### Traditional Mode - Browser Restore Mode
![](展示/admin/010传统模式游览器恢复模式-账号列表.png)
![](展示/admin/011传统模式游览器恢复模式-安装这个客户端配合一键恢复模式.png)
![](展示/admin/012传统模式游览器恢复模式-传统的模式单独把出码的做成api部署在另外服务器解决%20风控问题.png)

#### Customer Service Center & Template Management
![](展示/admin/013客服中心.png)
![](展示/admin/014模板管理中心.png)
![](展示/admin/015模板管理中心-手机模板.png)

#### Visitor Monitoring & Data Analytics
![](展示/admin/016前端模板的访问数据-多维度.png)
![](展示/admin/018%20实时监控前端有没有访客的数据.png)
![](展示/admin/019实时监控前端访客详细数据.png)

#### H5 Frontend Templates
![](展示/uinapp前端/004默认手机1.png)
![](展示/uinapp前端/004默认手机2.png)
![](展示/uinapp前端/004默认手机3.png)
![](展示/uinapp前端/004默认手机4.png)
![](展示/uinapp前端/004默认模式1.png)
![](展示/uinapp前端/004默认模式2.png)
![](展示/uinapp前端/005PC模式收银台模式.png)

***

### 🏗️ System Architecture

```
┌─────────────────────────────────────────────────────────────────┐
│                      Client Layer                               │
├─────────────────────────────────────────────────────────────────┤
│  ┌──────────────┐  ┌──────────────┐  ┌──────────────┐           │
│  │   H5 Frontend│  │   Admin Panel│  │   Mobile     │           │
│  │(continew-   │  │(continew-   │  │  UniApp     │           │
│  │ uinapp-ui)  │  │ admin-ui)   │  │  Templates  │           │
│  └──────┬───────┘  └──────┬───────┘  └──────┬───────┘           │
└─────────┼─────────────────┼─────────────────┼────────────────────┘
          │                 │                 │
          ▼                 ▼                 ▼
┌─────────────────────────────────────────────────────────────────┐
│                      Gateway Layer (Nginx)                      │
│              Unified Entry, SSL Encryption, Load Balancing       │
└─────────────────────────────────────────────────────────────────┘
          │                 │                 │
          ▼                 ▼                 ▼
┌─────────────────────────────────────────────────────────────────┐
│                      Java Backend (ContiNew)                    │
│  ┌───────────┐  ┌───────────┐  ┌───────────┐  ┌───────────┐    │
│  │ User Mgmt │  │ Auth Ctrl │  │ Tenant    │  │ Template  │    │
│  │  (RBAC)   │  │(Sa-Token) │  │ (SaaS)    │  │(Template) │    │
│  └───────────┘  └───────────┘  └───────────┘  └───────────┘    │
│  ┌───────────┐  ┌───────────┐  ┌───────────┐                    │
│  │ Visitor   │  │ Analytics │  │ Live Chat │                    │
│  │Monitor)   │  │(Analytics)│  │ (Chat)    │                    │
│  └───────────┘  └───────────┘  └───────────┘                    │
└─────────────────────────────────────────────────────────────────┘
          │                 │                 │
          ▼                 ▼                 ▼
┌─────────────────────────────────────────────────────────────────┐
│                    Node.js Upstream Services                    │
│                                                                 │
│  ┌─────────────────┐  ┌─────────────────┐  ┌─────────────────┐ │
│  │   BaileysApi    │  │Mini-linix-canma │  │  restore-client │ │
│  │  (API Mode)     │  │  (Browser Mode) │  │  (Restore Mode) │ │
│  │ WhatsApp API    │  │  Headless       │  │  Desktop        │ │
│  │  Integration    │  │  Browser Auto   │  │  Client         │ │
│  └─────────────────┘  └─────────────────┘  └─────────────────┘ │
└─────────────────────────────────────────────────────────────────┘
          │
          ▼
┌─────────────────────────────────────────────────────────────────┐
│                       Data Storage Layer                        │
│  ┌───────────┐  ┌───────────┐  ┌───────────┐                    │
│  │   MySQL   │  │   Redis   │  │   Files   │                    │
│  │  Business │  │  Cache/   │  │  Local    │                    │
│  │  Data     │  │  Session  │  │  Storage  │                    │
│  └───────────┘  └───────────┘  └───────────┘                    │
└─────────────────────────────────────────────────────────────────┘
```

***

### 📦 Module Description

| Module Name | Tech Stack | Port | Description |
|------------|-----------|------|-------------|
| **continew** | Java 17 + Spring Boot 3.3 | 8080 | Core Backend Service |
| **continew-admin-ui** | Vue 3 + Arco Design | 8766 | Admin Frontend |
| **continew-uinapp-ui** | Vue 3 + Vite | 8765 | H5 Frontend |
| **BaileysApi** | Node.js + Express | 3005 | WhatsApp API Mode Registration |
| **Mini-linix-canma** | Node.js + Express | 3004 | Browser Mode Registration |
| **restore-client** | Python + PyQt | - | Restore Mode Desktop Client |

***

### 🚀 Deployment Guide

#### 1. Environment Preparation

```bash
# Install JDK 17
apt update && apt install openjdk-17-jdk -y

# Install Node.js 20
curl -fsSL https://deb.nodesource.com/setup_20.x | bash -
apt install nodejs -y

# Install MySQL 8.0
apt install mysql-server -y

# Install Redis
apt install redis-server -y

# Install Nginx
apt install nginx -y

# Install PM2
npm install -g pm2
```

#### 2. Database Deployment

```sql
CREATE DATABASE continew_admin CHARACTER SET utf8mb4 COLLATE utf8mb4_unicode_ci;
CREATE USER 'continew'@'%' IDENTIFIED BY 'your_password';
GRANT ALL PRIVILEGES ON continew_admin.* TO 'continew'@'%';
FLUSH PRIVILEGES;

mysql -u continew -p continew_admin < 新continew_admin.sql
```

#### 3. Backend Deployment

```bash
cd /www/wwwroot/continew
mvn clean package -DskipTests
java -jar continew-server/target/continew-admin.jar --spring.profiles.active=prod
```

#### 4. Upstream Services Deployment

```bash
# BaileysApi
cd /www/wwwroot/BaileysApi && npm install
pm2 start server.js --name "baileys-api"

# Mini-linix-canma
cd /www/wwwroot/Mini-linix-canma && npm install
pm2 start src/index.js --name "mini-canma"

pm2 save && pm2 startup
```

#### 5. Nginx + Cloudflare Configuration

```nginx
server {
    listen 80;
    server_name your-domain.com;

    location / {
        root /www/wwwroot/continew-uinapp-ui/dist;
        try_files $uri $uri/ /index.html;
    }

    location /admin {
        alias /www/wwwroot/continew-admin-ui/dist;
        try_files $uri $admin/ /admin/index.html;
    }

    location /api/ {
        proxy_pass http://127.0.0.1:8080;
        proxy_set_header Host $host;
        proxy_set_header X-Real-IP $remote_addr;
    }

    location /canma/ {
        proxy_pass http://127.0.0.1:3004;
        proxy_http_version 1.1;
        proxy_set_header Upgrade $http_upgrade;
        proxy_set_header Connection "upgrade";
    }

    location /baileys/ {
        proxy_pass http://127.0.0.1:3005;
        proxy_http_version 1.1;
        proxy_set_header Upgrade $http_upgrade;
        proxy_set_header Connection "upgrade";
    }
}
```

**Cloudflare Configuration:**
- DNS A record pointing to server IP, proxy status: "Proxied"
- SSL/TLS Encryption Mode: Full
- Always Use HTTPS: Enabled

***

### 🔗 Contact Information

🌐 **Telegram Group**: https://t.me/whatsappoem

👤 **Contact Person**: https://t.me/Jeequan

***

### 📌 Open Source Version

Free Open Source Version: https://github.com/love414427/WhatsApp-Admin

***

Telegram: https://t.me/jeequan
More Systems: https://t.me/AprxAppoem/

***

### 📚 Related Projects

| Project | URL |
|---------|-----|
| ContiNew Admin Framework | https://github.com/continew-org/continew-admin |
| ContiNew Admin UI | https://github.com/continew-org/continew-admin-ui |
| Jeepay Payment System | https://gitee.com/jeequan/jeepay |

***

### 💟 Jianghu Technology

Successful operation experience, encrypted payment channels, secure fund protection, one-stop maintenance services.

![](crmeb/crmebimage/crmebimage/demoimage/wellcomJavaGroup.jpg)

Telegram: @jeequan https://t.me/jeequan
More Systems: https://t.me/whatsappoem

***