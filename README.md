<div align="center">

# XXD Panel 108｜新民艺剪纸志

把照片的识别性，重新剪成一张安静而有文化感的纸上构图

[![Codex Skill](https://img.shields.io/badge/Codex-Skill-000000?style=flat-square)](./SKILL.md)

</div>

## 样张展示 / Sample works

当前仓库暂不放入未经审核或借用其他 Panel 的图片。首批独立生成并完成方向审核后，再将样张补入此处。

有些照片已经有很强的身份和情绪，却还需要一种更有设计感的重新组织方式。**Panel 108** 保留照片的现实部分，再把另一半转译成自己的视觉语言，适合艺术海报、独立出版、展览图像、社交内容和纯设计图。

它重点解决：照片与设计各说各话、主体被过度装饰、版式缺少留白，以及同一套风格无法稳定交付不同画幅的问题。

- 一张照片对应一张独立成品，不多图拼接。
- 上下或左右对照严格 50:50，不增加第三带。
- 目录输入会逐张隔离处理，不混用主体、文案或结果。
- `design-only` 与壁纸模式只把照片作为依据，不把原图照片直接放进可见画面。

## 原始提示词 · 五种语言

[简体中文](references/original-prompt/zh-CN.md) · [English](references/original-prompt/en.md) · [日本語](references/original-prompt/ja.md) · [한국어](references/original-prompt/ko.md) · [العربية](references/original-prompt/ar.md)

简体中文文件逐字保存本项目的原始提示词，并且是运行时唯一的创作与审美权威；其他版本用于阅读、文档与分享。

**关键词：** 新民艺剪纸 · 扁平剪纸拼贴 · 版画肌理 · 2–4 色照片取色 · 章印感主视觉 · 大面积留白

## 四种输出模式

- `top-bottom`：3:4 竖版原生结构，现实照片在上，Panel 108 设计在下，严格各占 50%。
- `left-right`：现实照片在左，设计在右，严格各占 50%，不会旋转成上下结构。
- `design-only`：整张画布只呈现本 Panel 的设计转译，照片只作为参考。
- `wallpaper-pack`：按设备分别生成完整画布，不把一张图机械裁成多台设备。

支持多比例、准确像素、文字自动生成／准确文字／无文字、图片目录批量处理，以及 `linked` 或 `independent` 壁纸关系。每次调用只创建一个新任务目录，最终交付为 PNG。

## 开始使用 / Getting started

```bash
git clone https://github.com/nevertoday/xxd-panel-108.git
mkdir -p ~/.codex/skills
ln -s "$(pwd)/xxd-panel-108" ~/.codex/skills/xxd-panel-108
```

也可以直接使用 `npx skills` 安装：

```bash
npx skills add https://github.com/nevertoday/xxd-panel-108 --skill xxd-panel-108
```

该命令会从 GitHub 获取仓库并安装同名 Skill；需要用户级 Codex 安装时，可追加 `--global --agent codex --yes`。安装后重新启动 Agent 会话，然后调用：

```text
$xxd-panel-108
```

完整规范：[SKILL.md](SKILL.md) · [运行适配器](references/xxd-panel-108-prompt.en.md) · [原始提示词](references/original-prompt/zh-CN.md)

## 许可证

本项目采用 **PolyForm Noncommercial License 1.0.0**。完整法律文本见 [LICENSE](LICENSE)，官方页面：<https://polyformproject.org/licenses/noncommercial/1.0.0>。

- 允许个人学习、研究、实验、测试、兴趣项目、私人娱乐，以及符合协议定义的非商业组织使用。
- 非商业用途可以使用、复制、修改、制作衍生作品和分发，但分发时必须附带许可证及作者提供的 `Required Notice:`。
- 禁止商业产品、商业服务、收费交付、出售访问权或预期商业应用；商业使用需另行取得版权方书面许可。
- 仅授予明确写出的著作权与有限专利权，不授予商标权等其他权利，也不能擅自转授权或转让。
- 违约通知后须在 32 天内纠正，否则许可终止；内容按现状提供，不作担保。
