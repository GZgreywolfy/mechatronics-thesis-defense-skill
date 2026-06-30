# Tasks

- [x] Task 1: 验证 checklists/05-defense-presentation.md 格式与内容完整性
  - 检查文件是否存在、标题层级是否一致
  - 该文件已在上一轮工作中深化完毕，本次仅做格式验证

- [x] Task 2: 创建 examples/full-case-study.md 全流程模拟评审案例
  - 内容包含：学生提交材料描述 → AI按五大维度评审输出 → 模拟追问 → 总体结论与修改建议
  - 案例必须虚构，不涉及真实个人或课题
  - 与已有的 full-review-example.md 内容不重复（后者是PLC物料分拣系统评审），建议选择不同课题（如机械结构设计类或自动化控制类）

- [x] Task 3: 在 README.md 中新增「配合多模态模型使用」章节
  - 放在「常见问题 FAQ」章节之后
  - 说明如何配合 GPT-4V、Claude Vision 等支持图像识别的模型使用
  - 给出上传图纸截图时的最佳实践建议（如图纸描述模板、标注清晰度要求等）

- [x] Task 4: 在 README.md 中新增「常见错误速查」章节
  - 汇总各checklist中的常见错误案例，按五大维度分类整理
  - 放在「配合多模态模型使用」章节之后

- [x] Task 5: 在 README.md 末尾增加「贡献指南」章节
  - 说明如何提交 Issue、PR
  - 引用已有的 CONTRIBUTING.md 文件
  - 放在「许可证」章节之前

- [x] Task 6: 全项目格式一致性检查
  - 检查所有 markdown 文件的标题层级是否统一（如主题使用 ##，子节使用 ###）
  - 检查 README.md 中的内部链接是否全部有效
  - 修正发现的问题

- [x] Task 7: Git 提交并推送到远程仓库
  - git add 所有变更文件
  - git commit 使用格式：feat: [简要描述]
  - git push 到 `https://github.com/GZgreywolfy/mechatronics-thesis-defense-skill`

# Task Dependencies
- Task 1 独立，可最先执行
- Task 2 独立，可并行执行
- Task 3、4、5 相互独立（均修改 README.md，需顺序执行避免冲突）
- Task 6 依赖 Task 1~5 完成
- Task 7 依赖 Task 6 完成