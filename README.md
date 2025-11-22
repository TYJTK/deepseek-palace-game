# 宫廷文字游戏 🏯

## 项目简介
基于 n8n 工作流和 DeepSeek AI 开发的交互式宫斗文字游戏，玩家通过选择决定剧情走向。

## 功能特色
- 🤖 AI 智能剧情生成
- 💾 游戏状态持久化存储
- 📱 响应式网页界面
- 🎮 多分支剧情选择

## 快速开始

### 环境要求
- n8n 平台账户
- DeepSeek API 密钥

### 部署步骤
1. 下载 `palace_game_workflow.json` 文件
2. 登录 n8n 工作台
3. 导入工作流文件
4. 配置 DeepSeek API 凭据
5. 创建数据表 `palace_game_sessions`
6. 激活工作流即可游玩

## 项目结构
deepseek-palace-game/

├── palace_game_workflow.json  # 主工作流文件

└── README.md                  # 项目说明文档
## 使用说明
1. 访问部署后的 Webhook URL
2. 开始游戏，做出选择推动剧情
3. 游戏自动保存进度，支持多轮游玩

## 技术栈
- **后端**: n8n 工作流自动化
- **AI 服务**: DeepSeek 大语言模型
- **存储**: n8n Data Tables
- **前端**: HTML + CSS + JavaScript
