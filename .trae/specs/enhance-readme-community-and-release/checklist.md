# 校验清单

## README 文档校验
- [ ] README.md 顶部包含「欢迎反馈」标识
- [ ] README.md 包含「核心提示词预览」章节（200-300 字 SKILL.md 摘录）
- [ ] README.md 包含「一分钟体验示例」章节（完整输入-输出示例）
- [ ] README.md 包含「分享你的使用体验」章节
- [ ] README.md 包含「用户案例」章节（留空标注）
- [ ] 新增章节不影响原有章节的完整性和可读性
- [ ] README.md 内部链接均有效

## 内容校验
- [ ] examples/bad-example.md 存在且内容完整
- [ ] bad-example.md 包含多处典型错误的论文片段/图纸描述
- [ ] bad-example.md 包含 AI 评委的完整评审过程
- [ ] README.md 的项目文件结构中包含 bad-example.md 的链接

## 格式校验
- [ ] 所有 markdown 文件的标题层级统一（主题 ##，子节 ###）
- [ ] 列表样式统一
- [ ] 代码块格式统一
- [ ] 无明显错别字或语法错误

## GitHub 校验
- [ ] Release v1.0.0 创建成功
- [ ] Release Notes 包含核心功能和本次改进内容

## Git 校验
- [ ] 每个改进任务作为一个独立 commit（Conventional Commits 格式）
- [ ] 所有 commits 成功推送到远程仓库 origin main