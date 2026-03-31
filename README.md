# 🏙️ 创意街区探索工具 - 移动端设计

一个专注于发现城市小众街区的移动端设计项目。

## 🌐 在线预览

**GitHub Pages 链接：**
[https://dennydanohoh.github.io/block-exploration-tool/hifi-mobile/](https://dennydanohoh.github.io/block-exploration-tool/hifi-mobile/)

## 📱 设计理念

- **独立手机端设计**：不是桌面稿压缩版，而是为手机单独设计
- **单手操作友好**：所有交互都考虑单手操作场景
- **快速决策**：帮助用户快速找到想去的街区
- **个人化体验**：收藏、历史记录、个性化推荐

## 🎨 设计系统

### 颜色系统
- **主背景**：暖米色 (#f6efe4)
- **面板**：半透明白色 (rgba(255, 250, 242, 0.92))
- **文字**：深灰色 (#1f231d)
- **强调色**：橙色 (#ca6837)
- **辅助色**：橄榄绿 (#48533f)

### 组件系统
- **按钮**：主要按钮、次要按钮、图标按钮
- **卡片**：英雄卡片、列表卡片、结果卡片
- **导航**：底部导航、顶部导航
- **图标**：SVG图标系统

## 📁 项目结构

```
New project/
├── hifi-mobile/          # 移动端高保真设计
│   ├── index.html        # 移动端设计总览
│   ├── home.html         # 移动首页
│   ├── search.html       # 搜索页面
│   ├── place.html        # 地点详情页
│   ├── profile.html      # 个人页面
│   ├── favorites.html    # 收藏页面
│   ├── design-system.html # 设计系统
│   ├── styles.css        # 样式文件
│   └── icons.svg         # 图标系统
├── hifi/                 # 桌面端设计
├── prototype/            # 原型设计
├── 需求文档.md           # 项目需求文档
└── 一期信息架构与页面原型.md
```

## 🚀 快速开始

### 本地预览
```bash
# 进入项目目录
cd /Users/denny/Documents/New\ project

# 启动本地服务器
python3 -m http.server 4173 --bind 127.0.0.1

# 访问地址
http://127.0.0.1:4173/hifi-mobile/
```

### 局域网预览
```bash
# 启动局域网服务器
python3 -m http.server 4173 --bind 0.0.0.0

# 获取本地IP地址
ifconfig | grep "inet " | grep -v 127.0.0.1

# 在手机浏览器访问
http://[你的IP地址]:4173/hifi-mobile/
```

## 📋 页面列表

1. **首页** (`home.html`) - 发现推荐街区
2. **搜索页** (`search.html`) - 搜索和筛选街区
3. **地点详情页** (`place.html`) - 街区详细信息
4. **个人页面** (`profile.html`) - 用户个人中心
5. **收藏页面** (`favorites.html`) - 收藏的街区
6. **设计系统** (`design-system.html`) - 设计规范和组件

## 🛠️ 技术栈

- **HTML5** - 语义化标记
- **CSS3** - 现代布局（Flexbox、Grid）
- **CSS变量** - 设计系统token
- **SVG** - 矢量图标
- **响应式设计** - 移动端优先

## 📄 文档

- [需求文档](./需求文档.md) - 项目需求和功能说明
- [一期信息架构与页面原型](./一期信息架构与页面原型.md) - 信息架构设计
- [前后端框架与系统设计](./前后端框架与系统设计.md) - 技术架构
- [测试用例](./测试用例.md) - 测试方案

## 👤 作者

**dennydanohoh** - [GitHub](https://github.com/dennydanohoh)

## 📄 许可证

本项目仅供学习和设计参考使用。