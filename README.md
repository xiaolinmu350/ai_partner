# 🤖 AI Partner

一个基于 Streamlit 的 AI 对话助手，支持联网搜索、多轮对话、会话管理，部署在公网可访问。

## 功能亮点

- 🤖 **多轮对话** — 基于 DeepSeek 大模型，支持上下文记忆
- 🔍 **联网搜索** — 集成 Tavily 搜索，实时获取最新信息
- 📱 **手机端适配** — 响应式界面，手机浏览器直接使用
- 💾 **会话管理** — 保存/加载/删除历史会话，支持切换伴侣角色
- 🎭 **自定义伴侣** — 可自由设置伴侣姓名和性格特征
- ⚡ **流式输出** — 实时显示 AI 回复，体验流畅

## 在线体验

👉 [点此访问（公网链接）](https://your-app-link.streamlit.app)

## 技术栈

| 技术 | 用途 |
|------|------|
| Python | 核心开发语言 |
| Streamlit | 前端界面框架 |
| OpenAI SDK | 大模型 API 调用 |
| DeepSeek-chat | 对话模型 |
| Tavily API | 联网搜索工具 |
| Dotenv | 环境变量管理 |

## 本地运行

### 1. 克隆项目

```bash
git clone https://github.com/xiaolinmu350/ai_partner.git
cd ai_partner
```

### 2. 安装依赖

```bash
pip install streamlit openai tavily-python python-dotenv
```

### 3. 配置环境变量

在项目根目录创建 `.env` 文件：

```env
DEEPSEEK_API_KEY=your_deepseek_api_key
DEEPSEEK_BASE_URL=https://api.deepseek.com
TAVILY_API_KEY=your_tavily_api_key
```

### 4. 运行

```bash
streamlit run 03.ai_partner.py
```

## 项目结构

```
├── 03.ai_partner.py      # 主程序
├── session/              # 会话数据存储
├── .env                  # 环境变量配置
├── .gitignore            # Git 忽略规则
└── README.md             # 项目说明
```

## 部署到 Streamlit Cloud

1. 将代码推送到 GitHub
2. 登录 [Streamlit Cloud](https://streamlit.io/cloud)
3. 选择该仓库，设置部署入口为 `03.ai_partner.py`
4. 在 Secrets 中配置 `DEEPSEEK_API_KEY`、`TAVILY_API_KEY` 等环境变量
5. 部署后即可获得公网链接

## 许可证

MIT License