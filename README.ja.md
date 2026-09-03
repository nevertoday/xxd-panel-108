<div align="center">

# XXD Panel 108｜新民艺剪纸志

把照片的识别性，重新剪成一张安静而有文化感的纸上构图

[![Codex Skill](https://img.shields.io/badge/Codex-Skill-000000?style=flat-square)](./SKILL.md)

</div>

## サンプル

未審査の画像や他のPanelから借用したサンプルは掲載していません。独立生成と方向確認を終えた初回リリース後に追加します。

写真には強い個性や感情がありますが、さらに意図的な再構成が必要なことがあります。**Panel 108** は写真の現実感を保ちながら、もう一方を独自の視覚言語へ翻訳します。アートポスター、出版物、展示、SNS、デザインのみの出力に適しています。

写真とデザインが別々に語ること、装飾過多、余白不足、画面比率ごとの不安定さを解決します。

- 写真1枚につき成品1枚。写真は合成しません。
- 上下・左右比較は厳密な50:50で第三帯を作りません。
- フォルダー入力も内容・文案・結果を混ぜずに個別処理します。
- `design-only` と壁紙では写真を参照だけにし、未変換の写真を表示しません。

## 原始提示词 · 五语言

[简体中文](references/original-prompt/zh-CN.md) · [English](references/original-prompt/en.md) · [日本語](references/original-prompt/ja.md) · [한국어](references/original-prompt/ko.md) · [العربية](references/original-prompt/ar.md)

中国語ファイルは本プロジェクトの原文プロンプトを保存し、実行時の唯一の創作・美学上の基準です。他の版は読解、文書、共有用です。

**キーワード：** 新民艺剪纸 · 扁平剪纸拼贴 · 版画肌理 · 2–4 色照片取色 · 章印感主视觉 · 大面积留白

## 4つの出力モード

- `top-bottom`：3:4 竖版原生结构，现实照片在上，Panel 108 设计在下，严格各占 50%。
- `left-right`：现实照片在左，设计在右，严格各占 50%，不会旋转成上下结构。
- `design-only`：整张画布只呈现本 Panel 的设计转译，照片只作为参考。
- `wallpaper-pack`：按设备分别生成完整画布，不把一张图机械裁成多台设备。

支持多比例、准确像素、文字自动生成／准确文字／无文字、图片目录批量处理，以及 `linked` 或 `independent` 壁纸关系。每次调用只创建一个新任务目录，最终交付为 PNG。

## 使い始める

```bash
git clone https://github.com/nevertoday/xxd-panel-108.git
mkdir -p ~/.codex/skills
ln -s "$(pwd)/xxd-panel-108" ~/.codex/skills/xxd-panel-108
```

`npx skills` でも直接インストールできます：

```bash
npx skills add https://github.com/nevertoday/xxd-panel-108 --skill xxd-panel-108
```

このコマンドは GitHub から取得して同名の Skill をインストールします。ユーザー単位の Codex には末尾に `--global --agent codex --yes` を追加し、Agent セッションを再起動して呼び出します。

```text
$xxd-panel-108
```

完整规范：[SKILL.md](SKILL.md) · [运行适配器](references/xxd-panel-108-prompt.en.md) · [原始提示词](references/original-prompt/zh-CN.md)

## ライセンス

本プロジェクトは **PolyForm Noncommercial License 1.0.0** で提供されます。全文は [LICENSE](LICENSE)、公式ページは <https://polyformproject.org/licenses/noncommercial/1.0.0> を参照してください。

- 個人の学習・研究・実験・テスト・趣味・私的娯楽、およびライセンスが定義する非営利組織の利用が許可されます。
- 非営利目的なら使用、複製、改変、派生物の作成、配布ができますが、ライセンスと作者の `Required Notice:` を添付してください。
- 商用製品・サービス、対価を受ける納品、アクセス販売、商用利用を予定した用途は禁止です。商用利用には別途書面許可が必要です。
- 明記された著作権と限定特許権のみが許諾され、商標などの権利は与えられません。再許諾・譲渡もできません。
- 違反通知後32日以内に是正しなければライセンスは終了します。本プロジェクトは現状有姿で保証されません。
