<div align="center">

# XXD Panel 108｜新民艺剪纸志

把照片的识别性，重新剪成一张安静而有文化感的纸上构图

[![Codex Skill](https://img.shields.io/badge/Codex-Skill-000000?style=flat-square)](./SKILL.md)

</div>

## Sample works

This repository does not include unreviewed images or samples borrowed from another Panel. Independently generated and reviewed samples will be added here after the first release batch.

Some photographs already carry a strong identity and mood, but need a more deliberate visual reorganisation. **Panel 108** keeps the reality of the photograph and translates the other half through its own independent visual language, for art posters, independent publishing, exhibitions, social content, and design-only outputs.

It addresses the common problems of image and design talking past each other, over-decoration, weak whitespace, and inconsistent delivery across formats.

- One photograph becomes one isolated finished asset; photos are never combined.
- Top-bottom and left-right comparisons are strict 50:50 with no third band.
- Directory inputs are processed independently without cross-source subjects, copy, or results.
- `design-only` and wallpaper modes use the photo as reference only; the untransformed photo is not shown.

## Original prompt · five languages

[简体中文](references/original-prompt/zh-CN.md) · [English](references/original-prompt/en.md) · [日本語](references/original-prompt/ja.md) · [한국어](references/original-prompt/ko.md) · [العربية](references/original-prompt/ar.md)

The Chinese file preserves this project’s original prompt and is the sole creative and aesthetic authority at runtime; the other versions are for reading, documentation, and sharing.

**Keywords:** 新民艺剪纸 · 扁平剪纸拼贴 · 版画肌理 · 2–4 色照片取色 · 章印感主视觉 · 大面积留白

## Four output modes

- `top-bottom`：3:4 竖版原生结构，现实照片在上，Panel 108 设计在下，严格各占 50%。
- `left-right`：现实照片在左，设计在右，严格各占 50%，不会旋转成上下结构。
- `design-only`：整张画布只呈现本 Panel 的设计转译，照片只作为参考。
- `wallpaper-pack`：按设备分别生成完整画布，不把一张图机械裁成多台设备。

支持多比例、准确像素、文字自动生成／准确文字／无文字、图片目录批量处理，以及 `linked` 或 `independent` 壁纸关系。每次调用只创建一个新任务目录，最终交付为 PNG。

## Getting started

```bash
git clone https://github.com/nevertoday/xxd-panel-108.git
mkdir -p ~/.codex/skills
ln -s "$(pwd)/xxd-panel-108" ~/.codex/skills/xxd-panel-108
```

You can also install it directly with `npx skills`:

```bash
npx skills add https://github.com/nevertoday/xxd-panel-108 --skill xxd-panel-108
```

The command fetches the repository from GitHub and installs the same-named Skill. For a user-level Codex installation, append `--global --agent codex --yes`; then restart the agent session and invoke:

```text
$xxd-panel-108
```

完整规范：[SKILL.md](SKILL.md) · [运行适配器](references/xxd-panel-108-prompt.en.md) · [原始提示词](references/original-prompt/zh-CN.md)

## License

This project is released under the **PolyForm Noncommercial License 1.0.0**. See [LICENSE](LICENSE) for the complete legal text and <https://polyformproject.org/licenses/noncommercial/1.0.0> for the official page.

- Personal study, research, experiments, testing, hobbies, private entertainment, and the noncommercial organisations defined by the license are permitted.
- For noncommercial purposes you may use, copy, modify, create derivative works, and distribute, provided you include the license and every `Required Notice:` supplied by the author.
- Commercial products or services, paid delivery, selling access, and anticipated commercial applications are prohibited; obtain separate written permission for commercial use.
- Only the stated copyright and limited patent rights are granted. No trademark or other unstated rights are granted, and you may not sublicense or transfer the license.
- After written notice of a violation, correct it within 32 days or the licenses end. The project is provided as is, without warranties.
