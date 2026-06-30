# 完善 README、社区引导并发布 v1.0.0 Spec

## Why
当前项目已有完整的评审内容和文档体系（checklists、examples、README），但 README 缺少核心提示词预览、快速体验示例和社区引导，且尚未发布正式 Release 版本。需要进一步提升项目吸引力和社区互动性，并规范版本管理。

## What Changes
1. **README.md 新增「核心提示词预览」章节** — 摘录 SKILL.md 中的关键角色设定片段（200-300 字）
2. **README.md 新增「一分钟体验示例」章节** — 展示完整的输入-输出示例
3. **README.md 新增「分享你的使用体验」章节** — 鼓励用户通过 Issue 分享案例
4. **README.md 顶部增加「欢迎反馈」标识**
5. **README.md 新增「用户案例」章节** — 留空标注"欢迎投稿"
6. **新增 examples/bad-example.md** — 构造存在多处典型错误的论文片段及评审过程
7. **全项目格式一致性检查** — 标题层级、列表样式、代码块格式
8. **创建 GitHub Release v1.0.0** — 编写 Release Notes
9. **Git 提交并推送到远程仓库**

## Impact
- Affected specs: README.md 重写（新增多个章节）
- Affected code: README.md, examples/（新增 bad-example.md）
- New files: examples/bad-example.md
- New Release: v1.0.0

## ADDED Requirements
### Requirement: README 新增章节
README.md SHALL 包含以下新增章节：
- 「核心提示词预览」— 摘录 SKILL.md 角色设定核心片段（200-300 字），放在「这个 Skill 能做什么」之后
- 「一分钟体验示例」— 完整的输入-输出示例，放在「一分钟快速开始」之后
- 「分享你的使用体验」— 鼓励通过 Issue 分享案例、提出检查点、报告问题
- 「欢迎反馈」— 在 README 顶部增加的标识
- 「用户案例」— 留空章节，标注"欢迎投稿"

#### Scenario: 核心提示词预览
- WHEN 用户阅读 README 的「核心提示词预览」章节
- THEN 应展示约 200-300 字的 SKILL.md 角色设定片段
- AND 应包含引导语告知用户完整内容见 SKILL.md

#### Scenario: 一分钟体验示例
- WHEN 用户阅读「一分钟体验示例」章节
- THEN 应展示一个完整的输入-输出示例
- AND 包含真实的提问和回答，展示核心价值

### Requirement: 新增反面教材示例
系统 SHALL 在 examples/ 目录下创建 bad-example.md 文件。

#### Scenario: 反面教材内容完整
- WHEN bad-example.md 被创建
- THEN 文件内容应包含：存在多处典型错误的论文片段或图纸描述 + AI 评委的完整评审过程

### Requirement: 格式一致性检查
所有 markdown 文件 SHALL 检查标题层级统一性、列表样式、代码块格式、错别字。

### Requirement: 创建 Release v1.0.0
系统 SHALL 在 GitHub 上创建 Release v1.0.0。
SHALL 编写 Release Notes 总结核心功能和本次改进内容。

### Requirement: GitHub 推送
系统 SHALL 执行 git add → git commit（Conventional Commits 格式）→ git push 到远程仓库。

## MODIFIED Requirements
### Requirement: 保留现有章节
README.md 保留现有全部章节不变，仅在指定位置新增章节。
examples/ 目录下现有文件不做修改。

## REMOVED Requirements
无