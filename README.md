# Claude Code · 10 个必备 Skills 手册

> **内部评选的十大企业级 Skills**：针对全栈开发者，按实际使用价值精选并评分。
> **技术栈参考**：Go · Python · TypeScript · GitHub Actions · Anthropic API

---

## 📊 概览统计
* **精选 Skills**: 10 个
* **直接安装**: 4 个
* **自建定制**: 3 个
* **平均评分**: 9.1

---

## 🏆 Skill 推荐清单

### 01. skill-creator
* **核心评价**: 造 Skill 的 Skill，整个工具库的倍增器。
* **评分**: **9.9** (⭐ 高分推荐)
* **类型**: 直接安装使用
* **详细说明**: 这是一个元技能——它本身不解决任何具体的开发问题，但它让你有能力快速造出解决具体问题的定制 skill。从需求访谈、SKILL.md 起草、测试用例编写、迭代优化到最终打包，全流程都有它辅助。建议第一个安装。
* **适用场景**: 定制团队规范 skill、构建私有工作流、迭代优化现有 skill、打包分享给团队。
* **安装方式**: 直接在 Claude Code 中安装 `skill-creator` skill。

### 02. frontend-design
* **核心评价**: 生产级 Web UI 生成，告别土味 AI 审美。
* **评分**: **9.8** (⭐ 高分推荐)
* **类型**: 直接安装使用
* **详细说明**: 实际使用频率最高、单次提升最显著的一个。它强制 Claude Code 在写前端代码之前先确立完整的设计方向——视觉风格、字体选择、空间构成、交互细节——然后再动手生成代码。
* **适用场景**: React 组件开发、Web 应用全栈、Landing Page、后台管理界面、UI 原型快速验证。
* **安装方式**: 直接在 Claude Code 中安装 `frontend-design` skill。

### 03. prompt-engineer
* **核心评价**: 结构化 system prompt 框架，解决最常见的 LLM 调试痛点。
* **评分**: **9.5** (⭐ 高分推荐)
* **类型**: **需用 skill-creator 自建**
* **详细说明**: 它把你总结出来的 prompt 结构规范固化成 Claude Code 的行为准则，让每次生成的 system prompt 都遵循同一套框架，而不是随机发挥。
* **适用场景**: RAG 问答机器人 prompt 设计、代码生成助手 system prompt、结构化数据抽取、Anthropic API 集成项目。
* **创建命令**: `python -m scripts.package_skill ~/.claude/skills/prompt-engineer/`

### 04. product-self-knowledge
* **核心评价**: 让 Claude Code 永远用最新 Anthropic 文档说话。
* **评分**: **9.4**
* **类型**: 直接安装使用
* **详细说明**: Claude 的训练数据有截止日期，这个 skill 让 Claude Code 在回答任何相关问题之前先查阅最新官方文档，避免凭旧记忆乱说。
* **适用场景**: Anthropic API 调用代码生成、claude SDK 版本相关问题、模型参数查询、定价与 token 计算。
* **安装方式**: 直接在 Claude Code 中安装 `product-self-knowledge` skill。

### 05. code-review-advisor
* **核心评价**: 按团队规范输出带等级标注的标准化 Code Review 报告。
* **评分**: **9.0**
* **类型**: **需用 skill-creator 自建**
* **详细说明**: 核心价值是把你团队约定的规范嵌入进去，让每次输出都是 Critical / Major / Minor 三级标注 + 具体改进建议 + 代码示例的格式。
* **适用场景**: Go 后端服务 CR、TypeScript 前端组件审查、Python 脚本安全审计、PR 合并前质量把关。
* **创建命令**: `python -m scripts.package_skill ~/.claude/skills/code-review-advisor/`

### 06. file-reading
* **核心评价**: 文件处理路由表，彻底消灭「读不了」玄学。
* **评分**: **9.2**
* **类型**: 直接安装使用
* **详细说明**: 告诉 Claude Code 碰到不同格式的文件该用哪种读取策略（如 PDF 走文字提取、扫描件走 OCR 等），让文件处理从玄学变成确定性行为。
* **适用场景**: 上传 PDF API 文档分析、读取 Word 格式需求说明、处理图片中的架构图。
* **安装方式**: 直接在 Claude Code 中安装 `file-reading` skill。

### 07. ci-github-actions
* **核心评价**: 多语言仓库的专属 CI workflow 生成器。
* **评分**: **8.6**
* **类型**: **需用 skill-creator 自建**
* **详细说明**: 核心是把你的仓库结构、部署方式、缓存策略、Secret 命名规范全都固化进去。建议根据语言使用子目录结构存放模板。
* **适用场景**: 多语言 monorepo CI 配置、Go API 服务 Docker 构建、TypeScript 前端 PR 预览部署。
* **创建命令**: `python -m scripts.package_skill ~/.claude/skills/ci-github-actions/`

### 08. docx
* **核心评价**: 正式技术文档的 Word 交付格式，含完整目录和标题层级。
* **评分**: **8.5**
* **类型**: 直接安装使用
* **详细说明**: 让 Claude Code 输出带完整格式的 .docx 文档，包括自动生成目录、标题层级、整齐的表格等。
* **适用场景**: API 接口文档正式版、技术规范书交付、系统设计说明、项目验收文档。
* **安装方式**: 直接在 Claude Code 中安装 `docx` skill。

### 09. pdf + pdf-reading
* **核心评价**: 完整 PDF 工作流：读取解析 + 生成输出的组合包。
* **评分**: **8.4**
* **类型**: 直接安装使用
* **详细说明**: 两个 skill 配对使用：`pdf-reading` 负责深度解析（含 OCR），`pdf` 负责生成、合并、拆分等所有写操作。
* **适用场景**: RFC / 技术论文内容提取、API Spec 分析、扫描版合同解析、技术报告 PDF 生成。
* **安装方式**: 分别安装 `pdf` 和 `pdf-reading` skill。

### 10. pptx
* **核心评价**: 架构评审和技术汇报 PPT，不再手动排版。
* **评分**: **8.2**
* **类型**: 直接安装使用
* **详细说明**: 装了之后可以直接描述架构思路，输出结构清晰、包含 speaker notes 的多 slide 文稿，节省排版时间。
* **适用场景**: 系统架构评审 PPT、技术方案汇报、团队技术分享、项目复盘演示。
* **安装方式**: 直接在 Claude Code 中安装 `pptx` skill。

---
*本文档由 Claude Code 深度用户整理 · 按个人技术栈评分仅供参考*
