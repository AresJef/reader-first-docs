# reader-first-docs

把软件用法写得让第一次使用的人也能看懂，并验证示例实际会得到文中所说的结果。适用于 README、开发者指南、API 帮助、IDE 存根、示例与排错说明，也可以检查安装包与同版本文档站是否一致。

- **只审查**：找出读者得不到答案的地方，交判断和修改建议，不改稿。
- **局部改写**：只追相关读者任务、共享模板和受影响的位置，分别验证技术事实和可读性。
- **全项目或正式交付**：从内容清点走到同版包与文档站对账，并区分作者自查、独立复核和未验事项。

## 安装与使用

在支持从 GitHub 安装 Skill 的宿主中，可交给安装器以下请求：

```text
请从 https://github.com/AresJef/reader-first-docs 安装 reader-first-docs，仓库根路径是 .，固定到 v1.0.0。
```

也可以从 GitHub Release 下载固定版本源码，将目录作为 `reader-first-docs` 放到宿主实际支持的个人或项目 Skill 路径。保持 `SKILL.md` 位于该目录根部，不多套一层目录。已有同名 Skill 时先确认差异，不静默覆盖。安装后，在宿主中确认能发现并调用它。

```text
使用 $reader-first-docs，只审查这个 README。找出第一次使用的人会卡住的地方，指出原因并建议修改，不改文件。
```

完整流程见 [SKILL.md](SKILL.md)。[agents/openai.yaml](agents/openai.yaml) 仅提供可选的 OpenAI 界面元数据，流程不依赖它。使用此 Skill 不授予修改产品行为或对外发布的权限。

[MIT License](LICENSE)
