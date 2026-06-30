# 完善文档并推送 GitHub Spec

## Why
项目核心内容（checklists、examples、README）已在上一轮工作中完成深化，但仍有以下改进空间：README 缺少多模态模型使用指导、常见错误速查汇总、贡献指南的直接引用；缺少一个完整的"学生提交→AI评审→追问→结论"全流程模拟案例；且需要将更新推送到远程 GitHub 仓库。

## What Changes
1. **05-defense-presentation.md 文件验证** — 该文件实际已在上一轮工作中补全并深化，内容完整（含三档评分、6个错误案例、追问策略、自查清单），本次仅做格式一致性检查。
2. **新增 examples/full-case-study.md** — 创建一个完整的模拟评审案例，包含：学生提交的完整材料 → AI按五大维度的完整评审输出 → 模拟追问 → 总体结论与修改建议。案例需虚构，不涉及真实个人或课题。注意与已有的 full-review-example.md 区分（后者侧重PLC物料分拣系统评审）。
3. **README.md 新增「配合多模态模型使用」章节** — 说明如何配合 GPT-4V、Claude Vision 等支持图像识别的模型使用，给出上传图纸截图时的最佳实践建议。
4. **README.md 新增「常见错误速查」章节** — 汇总各checklist中的常见错误案例，按维度分类整理。可作为内联章节。
5. **README.md 末尾增加「贡献指南」章节** — 说明如何提交Issue、PR，引用已有的 CONTRIBUTING.md 文件。
6. **全项目格式一致性检查** — 检查所有 markdown 文件使用统一的标题层级，确保链接全部有效。
7. **Git 提交并推送** — 执行 git add、commit、push 到远程仓库 `https://github.com/GZgreywolfy/mechatronics-thesis-defense-skill`

## Impact
- Affected specs: 文档完善相关
- Affected code: 
  - Create: `examples/full-case-study.md`
  - Modify: `README.md`
  - Verify: `checklists/05-defense-presentation.md`
- New files: `examples/full-case-study.md`

## ADDED Requirements
### Requirement: 新增全流程模拟案例
系统 SHALL 在 examples/ 目录下创建 full-case-study.md 文件。

#### Scenario: 案例内容完整
- WHEN full-case-study.md 被创建
- THEN 文件内容应包含：学生提交材料 → AI按五大维度评审 → 模拟追问 → 总体结论与修改建议

### Requirement: README 章节扩展
README.md SHALL 包含以下新增章节：
- 「配合多模态模型使用」— 含图纸/截图上传的最佳实践
- 「常见错误速查」— 按五大维度汇总常见错误
- 「贡献指南」— 引用 CONTRIBUTING.md

### Requirement: 格式一致性
所有 markdown 文件 SHALL 检查标题层级统一性。
所有内部链接 SHALL 验证有效性。

### Requirement: GitHub 推送
系统 SHALL 执行 git add、commit、push 到远程仓库 `https://github.com/GZgreywolfy/mechatronics-thesis-defense-skill`。

#### Scenario: 正常推送
- WHEN 所有文件修改完成
- THEN 执行 git add → git commit（格式：feat: 简要描述）→ git push

## MODIFIED Requirements
### Requirement: 05-defense-presentation.md 保留
该文件已在上一轮工作中补全并深化，本次不做内容修改，仅做格式检查。

## REMOVED Requirements
无