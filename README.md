# WhatsApp 管理系统

一个功能完整的 WhatsApp 管理系统，支持多端管理、模板市场、群发助手、代理管理等功能。

## 联系方式

- 🌐 TG 群组：https://t.me/whatsappoem
- 👤 联系人：https://t.me/Jeequan
- 📌 开源版本：https://github.com/love414427/WhatsApp-Admin

---

## 🏗️ 系统架构

```
evolution/
├── Service/                    # 后端服务 (Python FastAPI)
├── vue/
│   ├── admin/                 # 管理端 (Vue 3)
│   ├── daili/                 # 代理端 (Vue 3)
│   └── moban/
│       └── vuedemo/           # H5 模板 (Vue 3)
├── 教程/                      # 详细部署教程
└── 展示/                      # 系统演示截图
```

### 架构特点

- **前后端分离**：清晰的前后端职责划分
- **多端管理**：管理端 + 代理端 + H5模板
- **模块化设计**：各模块独立部署，互不影响
- **WebSocket 实时通信**：支持实时消息推送

---

## 📦 模块说明

### 1. Service 服务端

**技术栈**：
- FastAPI (Python Web 框架)
- SQLAlchemy (ORM)
- Uvicorn (ASGI 服务器)
- Playwright (浏览器自动化)
- WebSocket (实时通信)

**核心功能**：
- 用户认证与权限管理 (RBAC)
- WhatsApp 会话管理
- API 管理与密钥控制
- 模板管理与预览
- 代理池管理
- 数据分析与统计
- 文件上传与管理

**主要 API 模块**：
- `system_manage` - 系统管理
- `front_config` - 前端配置
- `waha_api` - WAHA 接口
- `evolution_api` - Evolution 接口
- `baileys_api` - Baileys 接口
- `mass_sender` - 群发助手
- `translation` - 翻译服务
- `proxy_manage` - 代理管理

---

### 2. Admin 管理端

**技术栈**：
- Vue 3 + TypeScript
- Vite 7 (构建工具)
- NaiveUI (UI 组件库)
- UnoCSS (原子化 CSS)
- Pinia (状态管理)
- Vue Router 4 (路由管理)
- AntV/G2/ECharts/VChart (数据可视化)
- Elegant Router (自动路由生成)

**主要功能**：
- 📊 数据概览与统计
- 🤖 API 鱼苗管理（会话管理）
- 🔑 API 密钥管理
- 💬 聊天列表
- 📝 模板中心
- 🔍 关键字监控
- 📱 WhatsApp 号码验证
- 📤 群发助手
- 🛠️ 代理池管理
- 👥 用户与角色管理
- 🏪 代理商管理
- ⚙️ 系统配置

---

### 3. Daili 代理端

**技术栈**：与管理端相同 (Vue 3 + TypeScript + NaiveUI)

**主要功能**：
- 📊 代理统计
- 🤖 API 鱼苗管理
- 🔑 API 使用管理
- 💬 聊天列表
- 🏪 模板市场
- 📝 模板概况
- 🔍 关键字监控
- 📱 WhatsApp 号码验证
- 📤 群发助手
- 📈 数据分析

---

### 4. Vuedemo H5 模板

**技术栈**：
- Vue 3
- Vue Router
- 原生 CSS (简洁风格)

**主要功能**：
- 二维码登录
- 配对码登录
- 会话管理
- 消息发送与接收

---

## 💡 系统亮点

### 1. 多提供商支持
- ✅ WAHA
- ✅ Evolution
- ✅ Baileys

### 2. 完整的权限系统
- ✅ RBAC 角色权限管理
- ✅ 用户与角色分离
- ✅ 菜单级权限控制
- ✅ 代理商层级管理

### 3. 丰富的模板系统
- ✅ 模板市场
- ✅ 我的模板
- ✅ 模板预览
- ✅ 安装与管理

### 4. 强大的消息功能
- ✅ 群发助手
- ✅ 号码验证
- ✅ 关键字监控
- ✅ 实时消息推送

### 5. 代理与安全
- ✅ 代理池管理
- ✅ API 密钥管理
- ✅ 使用记录与统计
- ✅ 访问日志

### 6. 数据可视化
- ✅ 多图表库支持 (G2, ECharts, VChart)
- ✅ 甘特图
- ✅ 数据透视表
- ✅ 实时统计更新

---

## � 运行环境及框架

### 服务端环境

| 组件 | 版本要求 |
|------|----------|
| Python | ≥ 3.9 |
| pip | 最新版 |
| SQLite | 内置 |

**依赖库**：
```
fastapi >= 0.100.0
uvicorn >= 0.20.0
sqlalchemy
pymysql
python-jose
passlib[bcrypt]
playwright
googletrans
websockets
```

---

### 前端环境

| 组件 | 版本要求 |
|------|----------|
| Node.js | ≥ 20.19.0 |
| pnpm | ≥ 10.5.0 |

**核心框架**：
```
vue: 3.5.22
vue-router: 4.6.3
naive-ui: 2.43.1
vite: 7.1.12
typescript: 5.9.3
```

---

## 📱 核心功能

### 管理端功能

1. **首页概览**
   - 数据统计卡片
   - 快速操作入口
   - 系统状态显示

2. **API 鱼苗管理**
   - 创建会话
   - 二维码/配对码登录
   - 会话状态管理
   - 会话列表

3. **聊天管理**
   - 聊天列表
   - 消息查看
   - 消息发送

4. **模板管理**
   - 模板中心
   - 我的模板
   - 模板预览
   - 模板配置

5. **代理管理**
   - 代理池管理
   - Rola 代理
   - 代理测试

6. **群发助手**
   - 批量发送
   - 发送任务管理
   - 发送记录

7. **系统管理**
   - 用户管理
   - 角色管理
   - 菜单管理
   - 代理商管理
   - 系统配置

---

### 代理端功能

1. **代理统计**
   - 使用量统计
   - 费用统计
   - 报表展示

2. **API 管理**
   - API 密钥管理
   - 使用记录
   - 配额管理

3. **模板市场**
   - 浏览模板
   - 安装模板
   - 模板使用

---

## 🎬 系统演示

### 管理端截图

| 功能 | 说明 |
|------|------|
| 首页 | 数据概览与统计卡片 |
| 登录 | 用户登录界面 |
| API 鱼苗管理 | 创建和管理 WhatsApp 会话 |
| 聊天列表 | 查看和回复消息 |
| 模板中心 | 模板浏览与管理 |
| 模板预览 | 实时预览模板效果 |
| API 使用管理 | API 调用统计 |
| 群发助手 | 批量消息发送 |
| 关键字监控 | 消息关键字监控 |
| 代理池管理 | 代理服务器管理 |
| 数据分析 | 多维度数据报表 |
| 代理商管理 | 代理商层级管理 |
| 系统配置 | 系统参数配置 |

![首页](展示/后台/首页.png)
![登录](展示/后台/登录.png)
![API 鱼苗管理](展示/后台/API 鱼苗管理（会话）.png)
![API 鱼苗管理新建会话](展示/后台/API 鱼苗管理新建回话.png)
![聊天列表](展示/后台/聊天列表.png)
![模板中心](展示/后台/模板中心.png)
![模板预览01](展示/后台/模板预览01.png)
![模板预览02](展示/后台/模板预览02.png)
![模板预览03](展示/后台/模板预览03.png)
![模板预览04](展示/后台/模板预览04.png)
![我的模板](展示/后台/我的模板.png)
![API使用管理](展示/后台/API使用管理.png)
![API测试](展示/后台/API测试.png)
![WhatsApp 群发助手](展示/后台/WhatsApp 群发助手.png)
![WhatsApp 号码验证工具](展示/后台/WhatsApp 号码验证工具.png)
![关键字监控](展示/后台/关键字监控.png)
![代理池管理](展示/后台/代理池管理.png)
![数据分析](展示/后台/数据分析.png)
![代理商管理](展示/后台/代理商管理.png)
![系统配置](展示/后台/系统配置.png)

---

### 代理端截图

| 功能 | 说明 |
|------|------|
| 首页 | 代理数据概览 |
| 登录 | 代理登录界面 |
| API 使用管理 | API 调用记录 |
| API 鱼苗管理 | 会话管理 |
| 模板市场 | 模板浏览与安装 |
| 模板概况 | 使用统计 |
| 关键字监控 | 消息监控 |
| 数据分析 | 使用数据报表 |

![首页](展示/代理商/首页.png)
![登录](展示/代理商/登录.png)
![代理统计](展示/代理商/代理统计.png)
![API鱼苗管理](展示/代理商/API鱼苗管理.png)
![API使用管理](展示/代理商/API使用管理.png)
![聊天列表](展示/代理商/聊天列表.png)
![模板市场](展示/代理商/模板市场.png)
![模板概况](展示/代理商/模板概况.png)
![WhatsApp 群发助手](展示/代理商/WhatsApp 群发助手.png)
![WhatsApp 号码验证工具](展示/代理商/WhatsApp 号码验证工具.png)
![关键字监控](展示/代理商/关键字监控.png)
![数据分析](展示/代理商/数据分析.png)

---

## 🚀 部署指南

完整的部署教程请参考 `教程/` 目录下的详细文档。

### 快速部署概览

#### 1. 服务端部署

**安装依赖**：
```bash
cd Service
pip install -r requirements.txt
```

**启动服务**：
```bash
python main.py
```

服务默认运行在 `http://0.0.0.0:8100`

---

#### 2. Admin 管理端部署

**安装依赖**：
```bash
cd vue/admin
pnpm install
```

**本地开发**：
```bash
pnpm dev
```

**生产构建**：
```bash
pnpm build
```

**Nginx 配置**：参考 `教程/ADMIN教程/admin-nginx.conf`

---

#### 3. Daili 代理端部署

部署方式与管理端类似，参考 `教程/代理教程/`

---

#### 4. Vuedemo H5 模板部署

```bash
cd vue/moban/vuedemo
npm install
npm run dev
```

---

### WAHA 上游部署

参考 `教程/WAHA上游配置教程/` 和 `教程/WAHA教程/`

---

### 详细部署教程

- **服务端**：`教程/服务端教程/简单部署教程.md`
- **管理端**：`教程/ADMIN教程/Admin前端部署完整指南.md`
- **代理端**：`教程/代理教程/简单部署教程.md`
- **WAHA**：`教程/WAHA教程/本地Docker部署教程.md`

---

## 📁 目录结构

```
evolution/
├── Service/
│   ├── main.py              # 入口文件
│   ├── requirements.txt     # Python 依赖
│   ├── app/
│   │   ├── api/            # API 路由
│   │   ├── models/         # 数据模型
│   │   ├── core/           # 核心配置
│   │   └── utils/          # 工具函数
│   └── uploads/            # 上传文件目录
├── vue/
│   ├── admin/
│   │   ├── src/
│   │   │   ├── views/     # 页面组件
│   │   │   ├── router/    # 路由配置
│   │   │   ├── service/   # API 服务
│   │   │   └── store/     # 状态管理
│   │   └── package.json
│   ├── daili/             # 代理端（结构同 admin）
│   └── moban/
│       └── vuedemo/       # H5 模板
├── 教程/                  # 部署教程
└── 展示/                  # 演示截图
```

---

## ⚙️ 配置说明

### 服务端配置

服务端使用 SQLite 数据库，无需额外配置数据库服务。

主要配置项在系统管理 → 系统配置中设置。

---

### 前端配置

Admin 端环境变量文件：
- `.env` - 开发环境
- `.env.prod` - 生产环境
- `.env.test` - 测试环境

关键配置：
```env
VITE_BASE_URL=/
VITE_APP_TITLE=WS超级管理系统
VITE_SERVICE_BASE_URL=
VITE_OTHER_SERVICE_BASE_URL=
VITE_ROUTER_HISTORY_MODE=history
VITE_AUTH_ROUTE_MODE=dynamic
```

---

## 🔧 开发说明

### 本地开发

**启动后端**：
```bash
cd Service
python main.py
```

**启动管理端**：
```bash
cd vue/admin
pnpm dev
```

**启动代理端**：
```bash
cd vue/daili
pnpm dev
```

---

### 项目约定

- **代码风格**：遵循项目现有的 ESLint 配置
- **提交规范**：使用 `pnpm commit` 或 `pnpm commit:zh`
- **类型检查**：修改后运行 `pnpm typecheck`
- **路由生成**：新增页面后运行 `pnpm gen-route`

---

## 📞 技术支持

- Telegram 群组：https://t.me/whatsappoem
- 联系人：https://t.me/Jeequan
- 更多系统：https://t.me/AprxAppoem/

---

## 📄 许可证

请参考项目内的 LICENSE 文件。

---

**Star History**

如果这个项目对你有帮助，请给个 Star ⭐

---

*最后更新：2026-06-21*
