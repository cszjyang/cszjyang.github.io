# 杨志军中文简历

这是一份根据个人主页内容（包括页面中暂时注释的论文条目）整理的一页式中文求职简历。

## 文件

- `resume.tex`：简历内容，可直接编辑。
- `resume.cls`：排版样式。
- `zh_CN-systemfonts.sty`：中文字体配置。
- `ctexhook.sty`：与本地 XeCJK 配套的官方 CTeX hook 依赖（LPPL 1.3c）。
- `resume.pdf`：编译生成的投递版本。

## 编译

需要 XeLaTeX：

```bash
make
```

或直接运行：

```bash
xelatex -interaction=nonstopmode -halt-on-error resume.tex
```

## 待确认或补充

- 手机号。
- 明确的目标岗位与目标城市。
- 博士入学年月、预计毕业年月及本科起止年月。
- 编程语言、系统工具、开源项目或实习经历。
- 可量化的科研贡献，例如性能提升、测试规模和个人负责模块。

## 模板来源

版式基于 [billryan/resume](https://github.com/billryan/resume) 修改，原模板使用 MIT License；许可证见 `LICENSE`。`ctexhook.sty` 来自 CTeX-kit 2.5.8，文件内保留了 LPPL 1.3c 许可说明。
