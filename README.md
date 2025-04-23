# PNPM + NX Monorepo

这是一个使用 PNPM 和 NX 管理的 Monorepo 项目示例。

## 项目结构

```
.
├── apps/           # 应用程序目录
│   └── web/        # 网页应用示例
├── packages/       # 共享包目录
│   └── common/     # 通用工具包
├── nx.json         # NX配置文件
├── package.json    # 根项目配置
└── pnpm-workspace.yaml # PNPM工作空间配置
```

## 开始使用

### 安装依赖

```bash
pnpm install
```

### 构建所有包

```bash
pnpm build
```

### 启动开发模式

```bash
pnpm dev
```

### 查看项目依赖关系图

```bash
pnpm graph
```

## NX 命令

- 构建特定项目：`nx build web`
- 运行特定项目的测试：`nx test common`
- 查看受影响的项目：`nx affected:graph`
