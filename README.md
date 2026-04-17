# Job Tracker - 求职追踪应用

一个现代化的求职追踪管理应用，帮助你高效管理求职过程中的各个环节。

## 功能特性

- **仪表盘** - 展示求职统计数据和图表
- **求职申请管理** - 记录和管理所有求职申请
- **看板视图** - 拖拽式看板，直观展示求职进度
- **个人资料** - 管理个人信息和偏好设置

## 技术栈

- **前端框架**: Next.js 14 (App Router)
- **UI 组件**: shadcn/ui + Radix UI
- **样式方案**: Tailwind CSS + Framer Motion
- **后端服务**: Supabase (认证 + 数据库)
- **图表**: Recharts
- **拖拽排序**: @dnd-kit
- **表单验证**: React Hook Form + Zod
- **开发语言**: TypeScript

## 快速开始

### 1. 克隆项目

```bash
git clone <your-repo-url>
cd job-tracker
```

### 2. 安装依赖

```bash
npm install
```

### 3. 配置环境变量

复制 `.env.example` 为 `.env.local` 并填写配置：

```env
NEXT_PUBLIC_SUPABASE_URL=your_supabase_url
NEXT_PUBLIC_SUPABASE_ANON_KEY=your_supabase_anon_key
```

### 4. 运行开发服务器

```bash
npm run dev
```

访问 [http://localhost:3000](http://localhost:3000)

### 5. 构建生产版本

```bash
npm run build
```

## 项目结构

```
job-tracker/
├── src/
│   ├── app/              # Next.js App Router 页面
│   │   ├── (dashboard)/ # 认证后的页面
│   │   ├── login/        # 登录页面
│   │   ├── signup/       # 注册页面
│   │   └── ...
│   ├── components/       # React 组件
│   │   ├── ui/           # UI 组件库
│   │   └── ...
│   ├── lib/              # 工具函数
│   ├── types/            # TypeScript 类型定义
│   └── utils/            # 工具库
├── public/               # 静态资源
├── .env.local            # 环境变量 (不提交)
└── package.json
```

## 部署

项目已配置 Netlify 部署支持，可直接部署到 Netlify 或 Vercel。

## 许可证

MIT