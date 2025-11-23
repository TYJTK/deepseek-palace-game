# 交互式宫廷文字游戏 🏯
  
## 项目简介
基于 n8n 工作流和 DeepSeek AI 开发的交互式宫廷文字游戏，玩家通过选择决定剧情走向。
支持自选性别和出身，npc性格富于变化，在DeepSeek的支持下，有多分支剧情，为每一次游戏带来不一样的体验。

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
   在Credentials中创建Header Auth以及DeepSeek
5. 在palace_game_workflow--Call DeepSeek API节点中的Header Parameters--value自行输入API
6. 创建数据表（data table） `palace_game_sessions`
   add column：sessionId         string
               playerName        string
               choiceHistory     string
               storyProgress     number
               gameEnded         boolean
               currentAge	      string
               timePeriod	      string
               gender            string
               background        string
               npcPersonalities  string
7. 激活工作流即可游玩

## 项目结构
deepseek-palace-game/

├── palace_game_workflow.json  # 主工作流文件

└── README.md                  # 项目说明文档

└── Game over interface.png    # 游戏截图

└── Game star interface.png    # 游戏截图

└── story-scene-1.png          # 游戏截图

└── story-scene-2.png          # 游戏截图

## 使用说明
1. 访问部署后的 Webhook URL
2. 开始游戏，做出选择推动剧情
3. 游戏自动保存进度，支持多轮游玩

## 技术栈
- **后端**: n8n 工作流自动化
- **AI 服务**: DeepSeek 大语言模型
- **存储**: n8n Data Tables
- **前端**: HTML + CSS + JavaScript
