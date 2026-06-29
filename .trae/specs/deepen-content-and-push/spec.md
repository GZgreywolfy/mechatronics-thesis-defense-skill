# 完善机电类毕业设计答辩 Skill 项目内容并推送远程仓库 Spec

## Why
当前项目 checklists 文件内容较简略（每份仅 500-800 字），缺少评分标准分档描述和机电类常见错误案例；示例仅有一个 mock-qa.md；README.md 缺少快速开始和 FAQ。需要深化内容使其在实际评审中更具参考价值，并推送到 GitHub 公开仓库。

## What Changes
- 深化 5 个 checklist 文件：每份扩展至 3000+ 字，增加优秀/合格/不合格三档评分参考标准，增加机电类常见错误案例
- 扩充 examples/ 目录：新增 full-review-example.md、drawing-review-example.md、ppt-defense-example.md
- 完善 README.md：增加「一分钟快速开始」、「机电类各专业方向适配说明」、「常见问题 FAQ」章节
- 新增 CONTRIBUTING.md 和 CHANGELOG.md
- 执行 git add、commit、push 到远程仓库 origin main

## Impact
- Affected specs: 所有 5 个 checklist 文件重写，README.md 重写
- Affected code: checklists/01-format.md, checklists/02-logic-structure.md, checklists/03-technical-depth.md, checklists/04-engineering-drawing.md, checklists/05-defense-presentation.md, examples/mock-qa.md, README.md
- New files: examples/full-review-example.md, examples/drawing-review-example.md, examples/ppt-defense-example.md, CONTRIBUTING.md, CHANGELOG.md

## ADDED Requirements
### Requirement: Checklist 内容深化
每个 checklist SHALL 包含：
- 评分参考标准（优秀/合格/不合格三档描述）
- 机电类特有常见错误案例（如电气图纸符号错误、机械公差标注问题、PLC选型不当等）
- 总字数至少 3000 字

### Requirement: 示例扩充
系统 SHALL 新增 3 个示例文件：
- full-review-example.md：包含论文片段 + 评委反馈全文的完整评审示例
- drawing-review-example.md：图纸审查示例
- ppt-defense-example.md：PPT答辩演练示例

### Requirement: 文档完善
README.md SHALL 包含「一分钟快速开始」、「机电类各专业方向适配说明」、「常见问题 FAQ」章节。
系统 SHALL 新增 CONTRIBUTING.md 和 CHANGELOG.md。

### Requirement: GitHub 推送
系统 SHALL 执行 git add、commit、push 到远程仓库 origin main。

#### Scenario: 正常推送
- WHEN 所有文件修改完成
- THEN 执行 git add . → git commit → git push origin main

## MODIFIED Requirements
### Requirement: 现有文件保留
README.md 保留原有 MIT 许可证信息和数据来源隐私声明。
examples/mock-qa.md 保留原有内容不做删除。

## REMOVED Requirements
无