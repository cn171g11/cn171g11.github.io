# cn171g11.github.io

个人项目主页，托管在 GitHub Pages 上：**<https://cn171g11.github.io/>**

这一仓库只承载**入口导航页**，各项目的实际代码都在各自的独立仓库里。

## 站点结构

| 路径 | 内容 | 源码仓库 |
|------|------|----------|
| `/` | 项目导航首页（`index.html`） | 本仓库 |
| `/mma-guessr/` | MmaGuessr · 街景猜位置游戏 | [cn171g11/mma-guessr](https://github.com/cn171g11/mma-guessr) |
| `/ad-speedrun-optimizer/` | 反物质维度 · 速通优化器 | [cn171g11/ad-speedrun-optimizer](https://github.com/cn171g11/ad-speedrun-optimizer) |

## 本仓库文件

| 文件 | 说明 |
|------|------|
| `index.html` | 导航首页，卡片式跳转到各子项目 |
| `.nojekyll` | 禁用 GitHub Pages 的 Jekyll 构建 |
| `.gitignore` | 忽略工作区内部目录（如 `.workbuddy/`） |

## 新增一个项目

1. 新建独立仓库，把网页源码放在仓库根（`index.html` 在根目录）
2. 在仓库 Settings → Pages 里把 Source 设为 `main` / `/`
3. 在本仓库 `index.html` 的 `.cards` 容器里加一张卡片，`href` 指向 `/<仓库名>/`

## 变更历史

- 2026-09-14 清理仓库：移除早期原型与已废弃的内嵌游戏副本（`MmaGuessr.html` / `game.html` / `index-prototype.html`），
  主页改为纯导航页并新增「反物质维度 · 速通优化器」入口。回滚点：`12d6484`
- 2026-07-29 改用项目导航首页（项目各自独立成仓）
- 2026-07-28 初始版本：内嵌 MmaGuessr 游戏的单页站点
