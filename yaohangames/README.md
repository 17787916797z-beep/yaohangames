# 鼓王·瑶境争锋

一款以瑶族文化为背景的网页游戏。

## 项目结构

```
yaohangames/
├── server.js                 # 后端服务入口
├── package.json              # 项目依赖
├── database/
│    └── game.db             # SQLite 数据库
├── public/
│    ├── index.html          # 主页面
│    ├── css/
│    │    └── style.css     # 样式文件
│    ├── js/
│    │    └── game.js       # 游戏逻辑
│    └── assets/
│         ├── audio/         # 音效文件（需手动添加）
│         │    ├── bgm.mp3
│         │    ├── click.mp3
│         │    ├── win.mp3
│         │    └── fail.mp3
│         ├── drum.png
│         ├── border.png
│         └── rune-bg.png
│         └── music-icon.png
```

## 安装与运行

1. 安装依赖：
```bash
npm install
```

2. 添加音效文件（可选）：
将 MP3 音效文件放入 `public/assets/audio/` 目录

3. 启动服务：
```bash
npm start
```

4. 访问游戏：
打开浏览器访问 `http://localhost:3002`

## 游戏玩法

- 60秒内点击飘动的瑶语符文收集25点"鼓魂能量"
- 连续快速点击可触发连击加分
- 随时间减少，符文移动速度会加快
- 通关后用剩余时间作为积分上传排行榜

## 技术栈

- **后端**：Node.js + Express + SQLite（sql.js）
- **前端**：HTML5 Canvas + 原生 JavaScript
- **安全**：JWT 认证、bcrypt 密码加密

## 近期更新

- ✅ 修复密码加密（bcrypt）
- ✅ 添加 JWT 会话认证
- ✅ 防刷分数验证机制
- ✅ 难度递进系统
- ✅ 连击系统
- ✅ 音效支持
- ✅ 重构项目结构
