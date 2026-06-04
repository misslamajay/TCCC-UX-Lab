# User - 信息架构

用户端（User）面向终端用户，提供 AI 智能体对话、知识查询、工作协作等能力。

## 模块划分

| 模块 | 职责 | 核心页面 |
|------|------|----------|
| Chat | 智能体会话 | 对话列表、对话窗口、多轮对话 |
| Workspace | 个人工作台 | 任务看板、快捷入口、最近访问 |
| Knowledge | 知识中心 | 知识检索、知识详情、收藏 |
| AgentStore | 智能体商店 | Agent 浏览、Agent 详情、安装/启用 |
| Profile | 个人中心 | 账户信息、偏好设置、使用统计 |
| Experiments | 实验性功能 | 探索性交互与原型 |

## 导航层级

```
用户端
├── 会话 (Chat)
├── 工作台 (Workspace)
├── 知识 (Knowledge)
├── 智能体商店 (AgentStore)
├── 我的 (Profile)
└── 实验室 (Experiments)
```

## 角色权限

- **普通用户**：Chat + Knowledge + AgentStore + Profile
- **高级用户**：全部模块 + Workspace 高级功能
- **管理员（用户端视角）**：含组织级配置入口
