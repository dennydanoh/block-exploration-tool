# OpenClaw 交接说明

## 项目定位

这是一个移动端优先的街区发现产品原型，核心目标是帮助用户发现中国城市里小众、有调调、适合逛街、咖啡、慢走的街区，不做传统景点导览。

当前设计重点：

- 公开内容知识汇总，不直接做平台内容搬运
- 支持搜索、地点详情、收藏、登录、个人中心
- 收藏页与个人中心已拆分
- 未登录状态下，收藏和我的入口统一先进入登录流程
- 移动端正在做高保真细节打磨

## 当前工作目录

`/Users/denny/Documents/New project`

## 当前最重要的文件

产品与方案文档：

- `/Users/denny/Documents/New project/需求文档.md`
- `/Users/denny/Documents/New project/一期信息架构与页面原型.md`
- `/Users/denny/Documents/New project/测试用例.md`
- `/Users/denny/Documents/New project/前后端框架与系统设计.md`

移动端高保真设计：

- `/Users/denny/Documents/New project/hifi-mobile/index.html`
- `/Users/denny/Documents/New project/hifi-mobile/home.html`
- `/Users/denny/Documents/New project/hifi-mobile/search.html`
- `/Users/denny/Documents/New project/hifi-mobile/place.html`
- `/Users/denny/Documents/New project/hifi-mobile/login.html`
- `/Users/denny/Documents/New project/hifi-mobile/favorites.html`
- `/Users/denny/Documents/New project/hifi-mobile/profile.html`
- `/Users/denny/Documents/New project/hifi-mobile/styles.css`
- `/Users/denny/Documents/New project/hifi-mobile/icons.svg`

## 当前设计状态

已经完成：

- 移动端首页、城市页、搜索页、详情页、登录页、收藏页、个人中心、空状态页
- 二级页统一左侧返回按钮
- 底部导航统一为 4 个核心入口：发现 / 搜索 / 收藏 / 我的
- 未登录状态下，收藏和我的统一跳登录流程
- 收藏页按 城市 > 具体街区 展示，并补了缩略图和更多街区信息
- 按钮高度已统一到 44px 体系
- 底部导航标签被压住的问题已经通过样式修过
- 页面中原先使用的字符 icon 已基本替换为统一 SVG icon system

## 当前预览入口

如果本地静态服务正常运行，直接打开：

- `http://127.0.0.1:4173/hifi-mobile/index.html`

如果打不开，在项目根目录重新启动：

```bash
cd "/Users/denny/Documents/New project"
python3 -m http.server 4173 --bind 127.0.0.1
```

然后再访问：

- `http://127.0.0.1:4173/hifi-mobile/index.html`

## 最近一轮正在打磨的重点

用户刚刚要求：

1. 所有 icon 参考主流设计站常见矢量库风格，统一大小和风格
2. 顶部右上角按钮、底部导航 icon、页面内各种操作 icon 全部统一

已经完成的处理：

- 新建 `/Users/denny/Documents/New project/hifi-mobile/icons.svg`
- 用统一 SVG sprite 替换主要 icon
- styles.css 中补了 `.ui-icon`、`.btn-icon`、底部导航 icon 尺寸规则

## 下一步最建议继续做的事

优先顺序建议如下：

1. 逐页检查移动端 icon 的视觉对齐，确认描边、留白、active 态是否一致
2. 统一所有 chip、tag、stat-pill 的尺寸、圆角、字重和间距
3. 进一步打磨底部导航 active 态，让它更像成熟 iOS 工具产品
4. 补未登录收藏时的底部弹层，而不是整页跳转

## 和用户继续沟通时要保持的产品约束

- 产品是街区发现工具，不是点评社区
- 重点是国内一线城市和有代表性的城市漫游片区
- 不聚焦传统游客景点，优先有氛围、有街景、有咖啡和小店的街区
- 收藏、账号、个人信息都要严格区分登录态
- 收藏页和个人中心不要再混在一起
- 所有页面避免出现“点了没反应”的按钮

