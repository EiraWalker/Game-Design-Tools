# Excel Style

用于 Excel 表格样式维护的通用 Codex skill，支持策划表、参数表和含数学表达式的工作簿。

技能关注局部编辑、标题层级、输入与结果的视觉区分，以及原生数学公式的保留。调整公式展示区时，根据实际内容设置行高，并同步适配公式框高度和垂直位置，保存后检查裁切与错位。

## 使用

将本目录 `SKILLS/excel-style` 作为名为 `excel-style` 的技能文件夹，放入工具支持的技能目录；保留 `SKILL.md`、`agents/` 与 `references/` 的相对结构。支持 Codex 自动选择，也可显式调用：

```text
使用 $excel-style 调整指定 Excel 文件的公式展示区行高，保留公式内容、字体和其他区域。
```

本技能提供编辑规范，不包含工作簿、字体文件或 Excel 自动化运行时。处理复杂原生数学对象时，需要能够保留这些对象的编辑工具；仅调整布局无需重新生成工作簿。

## 维护位置

- [SKILL.md](SKILL.md)：使用场景与编辑流程。
- [通用样式规则](references/style-guide.md)：跨工作簿的稳定编辑原则。
- [工作簿配置与布局参考](references/workbook-profile.md)：易变的主题、字体、行高、列宽及匿名布局示例。
- [agents/openai.yaml](agents/openai.yaml)：Codex 显示名称和默认调用提示。

具体工作簿信息由使用方维护。参考文档中的布局均为匿名示例，应用前核实当前文件。

## 许可证

[MIT](LICENSE)。
