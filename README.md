# Skills Collection

Claude Code 技能集合，包含各类开发辅助和内容生成工具。

## 目录

- [vue2.6.14](#vue2614) - Vue 2.6.14 开发指南
- [guanrentang-writer](#guanrentang-writer) - 观仁堂中医公众号文章生成器

---

## vue2.6.14

> Vue 2.6.14 Options API 最佳实践、响应式系统、组件模式和生态系统集成。

### 功能特性

- **响应式系统** - Object.defineProperty 响应式原理与陷阱
- **全局 API** - Vue.config、自定义指令、插件开发
- **生命周期** - Vue 2 特定生命周期钩子
- **组件选项** - Props、Events、Slots、Provide/Inject
- **指令** - v-model/v-on/v-bind 修饰符、v-if vs v-show
- **内置组件** - transition、keep-alive、transition-group
- **TypeScript** - Vue.extend、PropType、类型安全
- **生态系统** - Vue Router 3.x、Vuex 3.x、Composition API

### 文档结构

\`\`\`
vue2.6.14/
├── reference/
│   ├── reactivity/          # 响应式系统
│   ├── global-api/          # 全局 API
│   ├── lifecycle/           # 生命周期
│   ├── component-options/   # 组件选项
│   ├── directives/          # 指令
│   ├── instance-api/        # 实例 API
│   ├── components/          # 内置组件
│   ├── render-functions/    # 渲染函数
│   ├── types/               # TypeScript 集成
│   ├── build-tooling/       # 构建工具
│   ├── ecosystem/           # 生态系统
│   └── comparison/          # Vue 2 vs Vue 3 差异
└── SKILL.md                 # 完整索引
\`\`\`

### 使用场景

- 维护 Vue 2 项目时查阅 API 用法
- 解决 Vue 2 响应式系统相关问题
- Vue 2 + TypeScript 开发
- Vue Router 3 / Vuex 3 配置

---

## guanrentang-writer

> 观仁堂中医公众号文章生成器。一站式完成：选题 → 写文章 → 配图 → 输出成品。

### 功能特性

- **智能选题** - 根据当前季节/节气自动选择主题
- **文章生成** - 符合观仁堂风格的中医养生文章（1000-1500字）
- **自动配图** - AI 生成封面、配图、食疗图
- **固定结尾** - 自动添加装饰图和关注二维码

### 配置要求

| 配置项 | 说明 |
|-------|------|
| \`ZHIPU_API_KEY\` | 智谱 API Key（环境变量或 .env 文件） |
| \`assets/\` | 固定素材目录（结尾装饰图、二维码图） |

### 使用方式

| 用户说 | 效果 |
|-------|------|
| "帮我写一篇文章" | 自动选题，输出到默认目录 |
| "写个春季养生的" | 指定主题 |
| "随机写一篇" | 随机选题 |
| "输出到 ~/Desktop" | 指定输出目录 |

### 输出结构

\`\`\`
articles/
├── 春季养肝全攻略.md
├── images/
│   └── 春季养肝全攻略/
│       ├── cover.jpg      # 封面（AI 生成）
│       ├── content-1.jpg  # 配图（AI 生成）
│       └── recipe.jpg     # 食疗图（AI 生成）
└── assets/
    ├── ending-decorative.jpg  # 结尾装饰图（固定）
    └── ending-qrcode.jpg      # 关注二维码（固定）
\`\`\`

---

## 安装使用

将需要的 skill 目录复制到你的 Claude Code skills 目录：

\`\`\`bash
# 复制单个 skill
cp -r vue2.6.14 ~/.agents/skills/

# 或复制全部
cp -r * ~/.agents/skills/
\`\`\`

---

## License

MIT
