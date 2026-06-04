# TCCC-UX-Lab

TCCC (Tencent Cloud Contact Center) UX Design System & Experiment Lab.

## Repository Structure

```
TCCC-UX-Lab/
├── Docs/                    # 设计文档与规范
│   ├── Information-Architecture/   # 信息架构
│   ├── Design-Rules/              # 设计规则
│   ├── Prompts/                   # AI Prompt 模板
│   └── ChangeLog/                 # 变更记录
│
├── Shared/                  # 共享资源
│   ├── Components/          # 通用组件
│   ├── Assets/              # 静态资源
│   └── Templates/           # 页面模板
│
├── Management/              # 管理端设计
│   ├── Overview/            # 总览模块
│   ├── Extension/           # 扩展模块
│   ├── Agent/               # 智能体模块
│   ├── Staff/               # 坐席模块
│   └── Experiments/         # 实验性设计
│
├── User/                    # 用户端设计
│   ├── Chat/                # 会话
│   ├── Workspace/           # 工作台
│   ├── Knowledge/           # 知识
│   ├── AgentStore/          # 智能体商店
│   ├── Profile/             # 个人中心
│   └── Experiments/         # 实验性设计
│
└── Console/                 # 控制台设计
    ├── Tenant/              # 租户管理
    ├── Billing/             # 计费管理
    ├── Monitor/             # 监控
    ├── Config/              # 配置
    └── Experiments/         # 实验性设计
```

## 页面目录结构

所有页面目录统一遵循以下结构：

```
<PageName>/
├── V1/          # 第一个正式发布版本
├── V2/          # 第二个正式发布版本（如需要）
├── Final/       # 当前确认采用的最终版本
└── Releases/    # 版本说明文档
    ├── V1.md
    ├── V2.md
    └── Final.md
```

- **`V1/`** — 第一个正式发布版本
- **`V2/`** — 第二个正式发布版本（如需要，后续允许 V3、V4、V5…）
- **`Final/`** — 当前确认采用的最终版本
- **`Releases/`** — 存放每次版本变更说明文档

## 版本管理规范

1. **所有页面必须发布到版本目录**。页面设计稿、原型、代码等产物必须放在对应的 `V1/`、`V2/`… 或 `Final/` 目录中，禁止在页面根目录直接放置未归档的文件。
2. **不允许出现 `final-final`、`new`、`copy`、`latest` 等命名**。版本迭代只能通过递增版本号（V3、V4…）表达，禁止使用含义模糊的修饰词。
3. **统一使用 V1、V2、V3… 进行版本编号**。版本号必须连续递增，不可跳号。
4. **`Final/` 永远指向当前确认版本**。当某个版本经评审确认后，将其内容同步到 `Final/`。`Final/` 可随迭代更新，但始终代表当前生效版本。
5. **`Releases/` 记录每次版本变更说明**。每新增一个版本，必须在 `Releases/` 下创建对应的 `.md` 文件（如 `V3.md`），填写变更说明、变更日期和变更人。`Final.md` 在每次 Final 更新时同步更新。

### 示例

```
AgentManagement/
├── V1/
│   └── ... (初版设计)
├── V2/
│   └── ... (修订版设计)
├── V3/
│   └── ... (再次修订)
├── Final/
│   └── ... (当前确认版本，与 V3 内容一致)
└── Releases/
    ├── V1.md     # 初版变更说明
    ├── V2.md     # V2 变更说明
    ├── V3.md     # V3 变更说明
    └── Final.md  # Final 确认说明
```

## License

Internal use only.
