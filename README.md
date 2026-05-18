<div align="center">

# 🐹 微信打地鼠

**萌趣十足的微信小程序打地鼠游戏**

[![GitHub](https://img.shields.io/badge/GitHub-Project-blue?logo=github)](https://github.com/aiyangtongxue/wechat-whack-a-mole)
[![WeChat](https://img.shields.io/badge/WeChat-Mini_Program-07C160?logo=wechat)](https://developers.weixin.qq.com/miniprogram/dev/framework/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

</div>

---

## 📌 项目简介

微信打地鼠是一款基于微信小程序平台开发的休闲益智游戏。玩家需要在 3×3 的地鼠洞网格中，快速点击随机冒出的地鼠来获取分数。游戏拥有精美的视觉设计——渐变天空、飘动白云、浮动太阳、装饰花朵，搭配治愈系背景音乐和萌趣音效，带来轻松愉悦的游戏体验。

---

## ✨ 核心特性

- 🐹 **经典打地鼠玩法** — 3×3 网格，地鼠随机出现，点击得分
- 🎨 **精美视觉设计** — 渐变天空与草地、动态浮动太阳、飘动白云、装饰性花朵
- 🎵 **沉浸式音效** — 治愈系背景音乐 + 萌趣击打音效 + 欢乐开始音效
- 🔇 **音效控制** — 一键静音/开启，贴心不打扰
- 🏆 **最高分记录** — 本地持久化存储最高分，挑战自我
- 💫 **流畅动画** — 地鼠弹跳出现动画、按钮光泽效果、云朵飘动动画
- 🎯 **随机难度** — 地鼠出现时长与间隔随机变化，越玩越刺激

---

## 🛠️ 技术栈

| 技术 | 用途 |
|------|------|
| 微信小程序框架 | 应用架构与页面管理 |
| WXML | 页面结构（数据绑定、列表渲染） |
| WXSS | 样式与动画（CSS 动画、渐变、阴影） |
| JavaScript (Component) | 游戏逻辑（Component 组件化开发） |
| wx.createInnerAudioContext | 音频播放控制 |
| wx.setStorageSync | 本地数据持久化 |

---

## 🚀 快速开始

### 前置条件

- [微信开发者工具](https://developers.weixin.qq.com/miniprogram/dev/devtools/download.html) 最新版
- 微信小程序 AppID（或使用测试号）
- 基础库版本 ≥ 2.19.4

### 安装步骤

```bash
git clone https://github.com/aiyangtongxue/wechat-whack-a-mole.git
cd wechat-whack-a-mole
```

### 运行命令

1. 打开**微信开发者工具**
2. 选择「导入项目」，指向项目根目录
3. 填入 AppID（或选择「测试号」）
4. 点击「编译」即可在模拟器中预览
5. 点击「预览」可扫码在手机端体验

---

## 📂 项目结构

```
wechat-whack-a-mole/
├── app.js                             # 小程序入口（背景音乐管理）
├── app.json                           # 全局配置（页面路由、窗口样式）
├── project.config.json                # 项目配置
├── project.private.config.json        # 私有项目配置
├── pages/
│   └── index/
│       ├── index.js                   # 游戏核心逻辑（Component）
│       ├── index.wxml                 # 游戏页面模板
│       └── index.wxss                 # 游戏样式与动画
├── audio/
│   ├── background.mp3                 # 背景音乐
│   ├── hit.mp3                        # 击打音效
│   └── start.mp3                      # 开始音效
├── images/
│   └── mole.png                       # 地鼠图片
├── CNAME                              # 自定义域名配置
├── WeChat_20250117025054.mp4          # 演示视频
├── 微信截图_20250117025625.png         # 截图
├── 微信截图_20250126061043.png         # 截图
└── README.md                          # 项目说明文档
```

---

## 🎮 游戏玩法

1. 点击 **「开始游戏」** 按钮启动
2. 地鼠会从 9 个洞中随机冒出
3. 快速点击地鼠获得 +1 分
4. 地鼠出现时长随机（800ms-1500ms），越快点击越好
5. 挑战最高分记录！

---

## 🤝 贡献与许可证

欢迎提交 Issue 和 Pull Request 来帮助改进项目！

本项目采用 **MIT License** 开源协议，详情请见 [LICENSE](LICENSE) 文件。
