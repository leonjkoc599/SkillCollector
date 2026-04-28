Claude Code · 10 个必备 Skills 手册
内部评选的十大企业级 Skills：针对全栈开发者，按实际使用价值精选并评分。
技术栈参考：Go · Python · TypeScript · GitHub Actions · Anthropic API

📊 概览统计
精选 Skills: 10 个

直接安装: 4 个

自建定制: 3 个

平均评分: 9.1

🏆 Skill 推荐清单
01. skill-creator
核心评价: 造 Skill 的 Skill，整个工具库的倍增器。

评分: 9.9 (⭐ 高分推荐)

类型: 直接安装使用

详细说明: 这是一个元技能——它本身不解决任何具体的开发问题，但它让你有能力快速造出解决具体问题的定制 skill。从需求访谈、SKILL.md 起草、测试用例编写、迭代优化到最终打包，全流程都有它辅助。10 个 slot 里有 1 个给它，可以撬动其余所有 skill 的质量上限。建议第一个装。

适用场景: 定制团队规范 skill、构建私有工作流、迭代优化现有 skill、打包分享给团队。

安装方式: 直接在 Claude Code 中安装 skill-creator skill。

02. frontend-design
核心评价: 生产级 Web UI 生成，告别土味 AI 审美。

评分: 9.8 (⭐ 高分推荐)

类型: 直接安装使用

详细说明: 实际使用频率最高、单次提升最显著的一个。它强制 Claude Code 在写前端代码之前先确立完整的设计方向（视觉风格、字体选择、空间构成、交互细节）。输出的是可以直接进 production 的界面。

适用场景: React 组件开发、Web 应用全栈、Landing Page、后台管理界面、UI 原型快速验证。

安装方式: 直接在 Claude Code 中安装 frontend-design skill。

03. prompt-engineer
核心评价: 结构化 system prompt 框架，解决 LLM 调试痛点。

评分: 9.5 (⭐ 高分推荐)

类型: 需用 skill-creator 自建

详细说明: 把你总结出来的 prompt 结构规范（角色定义 → 任务说明 → 输出格式 → 约束边界 → 少样本示例）固化成行为准则，让每次生成的 prompt 都遵循同一套框架。

适用场景: RAG 问答机器人 prompt 设计、代码生成助手 system prompt、结构化数据抽取、Anthropic API 集成项目。

创建命令: python -m scripts.package_skill ~/.claude/skills/prompt-engineer/

04. product-self-knowledge
核心评价: 让 Claude Code 永远用最新 Anthropic 文档说话。

评分: 9.4

类型: 直接安装使用

详细说明: 这个 skill 让 Claude Code 在回答任何 Anthropic 产品相关问题之前，先查最新官方文档（SDK 写法、定价、速率限制）再回答，而不是凭训练时的旧记忆。

适用场景: Anthropic API 调用代码生成、claude SDK 版本查询、模型参数查询、新功能接入。

安装方式: 直接在 Claude Code 中安装 product-self-knowledge skill。

05. code-review-advisor
核心评价: 按团队规范输出带等级标注的标准化 CR 报告。

评分: 9.0

类型: 需用 skill-creator 自建

详细说明: 嵌入团队约定的规范（如 Go 的 error handling、TS 类型安全等），输出 Critical / Major / Minor 三级标注 + 修复方案，不再是泛泛的建议。

适用场景: 后端服务 CR、前端组件审查、安全审计、PR 合并前把关。

创建命令: python -m scripts.package_skill ~/.claude/skills/code-review-advisor/

06. file-reading
核心评价: 文件处理路由表，彻底消灭「读不了」玄学。

评分: 9.2

类型: 直接安装使用

详细说明: 告诉 Claude Code 碰到不同格式（PDF、DOCX、扫描件、图片）时该用哪种读取策略，让文件处理从玄学变成确定性行为。

适用场景: 上传 PDF API 文档分析、读取 Word 需求说明、处理图片中的架构图、解析数据文件。

安装方式: 直接在 Claude Code 中安装 file-reading skill。

07. ci-github-actions
核心评价: 多语言仓库的专属 CI workflow 生成器。

评分: 8.6

类型: 需用 skill-creator 自建

详细说明: 固化仓库结构（Go+TS+Python monorepo）、部署方式、缓存策略和 Secret 规范。建议按语言拆分子目录存放模板。

适用场景: 多语言 monorepo CI 配置、Docker 构建推送、前端预览部署、按需触发 job。

创建命令: python -m scripts.package_skill ~/.claude/skills/ci-github-actions/

08. docx
核心评价: 正式技术文档的 Word 交付格式。

评分: 8.5

类型: 直接安装使用

详细说明: 输出带完整格式的 .docx：自动生成目录、标题层级规范、表格整齐。你只管内容，格式交给它。

适用场景: API 接口文档正式版、技术规范书、系统设计说明、项目验收文档。

安装方式: 直接在 Claude Code 中安装 docx skill。

09. pdf + pdf-reading
核心评价: 完整 PDF 工作流：读取解析 + 生成输出。

评分: 8.4

类型: 直接安装使用

详细说明: 配对使用：pdf-reading 负责深度解析（含 OCR），pdf 负责生成、合并、拆分、加水印等写操作。

适用场景: RFC/论文内容提取、API Spec 分析、扫描版合同解析、技术报告生成。

安装方式: 分别安装 pdf 和 pdf-reading skill。

10. pptx
核心评价: 架构评审和技术汇报 PPT，不再手动排版。

评分: 8.2

类型: 直接安装使用

详细说明: 直接描述架构思路，输出结构清晰、包含 speaker notes 的多 slide 文稿，节省排版时间。

适用场景: 系统架构评审 PPT、技术方案汇报、团队技术分享、项目复盘演示。

安装方式: 直接在 Claude Code 中安装 pptx skill。
