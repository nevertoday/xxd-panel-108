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

## 适用场景与解决的问题

当照片主体很有辨识度，却被复杂背景、过度装饰或普通滤镜削弱时，108 用新民艺剪纸重新组织信息：上方保留真实照片，下方只留下主体、轮廓、姿态和叙事关系，转成扁平剪纸、章印感主视觉与版画肌理。

### 适合这些情况

- 想保留照片身份，又需要文化感和手工感的艺术海报、出版封面或展览图像。
- 不想要写实插画、光滑矢量或 3D，而偏好剪影、色块、刻线、正负形与纸张颗粒。
- 需要同一套风格稳定输出上下、左右、纯设计、壁纸、多比例和目录批处理。

### 它替你解决什么

- 删除无关背景和重复物件，避免主体被装饰吞没。
- 从照片提炼 2–4 种辨识度最高的颜色，形成鲜明但克制的民艺色块。
- 统一每张成品的双区逻辑：严格 50:50，不增加标题栏、底栏或第三带。

### 快速判断：Panel 108 适合你吗？

| 你关心的问题 | 这套风格给你的回答 |
|---|---|
| 结果是什么 | 上方真实照片＋下方新民艺剪纸设计的一张完整海报 |
| 一眼特点 | 小尺度章印感主体、平面剪纸色块、版画颗粒、大面积暖白留白 |
| 如何尊重原图 | 保留身份、结构、姿态、光色；下方只做删减与符号化重构 |

## 它如何把输入变成成品

```text
识别主体与叙事关系 → 选择 2–4 个关键颜色 → 删除无关细节 → 概括为剪纸轮廓、色块、刻线与正负形 → 加入版画颗粒与留白 → 完成新民艺纸上构图
```

## 能力与边界

- `top-bottom` 默认 3:4，上下各 50%；`left-right` 左右各 50%，永不旋转成另一方向。
- `design-only` 与 `wallpaper-pack` 全画布只显示设计转译；照片只是不可见参考。
- 每张图从当前原图一次直达生成，禁止把中间结果、样张或其他 Panel 作品送入第二轮。
- 所有交付都是完整 PNG 位图；不以 SVG、HTML、Canvas 或程序绘图替代成品。

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
<!-- xxd-panel-catalog:start -->
## XXD Panel 全系列项目

108 个 Panel 各自保留独立的原始提示词与审美逻辑。下面连续列出 001–108 的全部项目地址和核心风格特点；当前项目以粗体标出。

| 项目地址 | 风格特点 |
|---|---|
| [xxd-panel-001](https://github.com/nevertoday/xxd-panel-001) | 稚拙线条 · 复古纸感 · 混合媒材 · 轻巧隐喻 · 暖色留白 |
| [xxd-panel-002](https://github.com/nevertoday/xxd-panel-002) | 叙事轮廓 · 迟疑手线 · 近似色调 · 局部夸张 · 套印文字 |
| [xxd-panel-003](https://github.com/nevertoday/xxd-panel-003) | 连续黑线 · 公共议题 · 受力结点 · 留白沉默 · 向外释放 |
| [xxd-panel-004](https://github.com/nevertoday/xxd-panel-004) | 在地现实 · 精准单线 · 几何透视 · 主题配色 · 城市品牌文字 |
| [xxd-panel-005](https://github.com/nevertoday/xxd-panel-005) | 钝拙体块 · 暗色结构场 · 局部显形 · 三层色阶 · 丝网印刷 × 粉蜡笔 |
| [xxd-panel-006](https://github.com/nevertoday/xxd-panel-006) | 小主体 · 80%–90% 纸面留白 · 纤细手线 · 四色以内 · 丙烯平涂 |
| [xxd-panel-007](https://github.com/nevertoday/xxd-panel-007) | 实物小图 · 局部／剖面／重复 · 错位留白 · 细黑手写 · 扫描纸感 |
| [xxd-panel-008](https://github.com/nevertoday/xxd-panel-008) | 正交等距 · 平台／台阶／门洞 · 空间悖论 · 动态粉彩 · 极净哑光 3D |
| [xxd-panel-009](https://github.com/nevertoday/xxd-panel-009) | 极小主体 · 巨大留白 · 单一空间关系 · 专色体系 · Halftone 丝网印刷 |
| [xxd-panel-010](https://github.com/nevertoday/xxd-panel-010) | 粗黑剪影 · 内部白色特征区 · 干媒介纸感 · 极少环境记号 · 童书编辑小字 |
| [xxd-panel-011](https://github.com/nevertoday/xxd-panel-011) | 一个核心意象 · 一组关系 · 连续黑线 · 主动留白 · 一抹记忆点色 |
| [xxd-panel-012](https://github.com/nevertoday/xxd-panel-012) | 高密聚合 · 外围稀释 · 几何约束 · 一种生命主线色 · 黑灰微排版 |
| [xxd-panel-013](https://github.com/nevertoday/xxd-panel-013) | 一张横向票体 · 74/26 分区 · 治愈水彩 · 象牙白留白 · 本地化信息票根 |
| [xxd-panel-014](https://github.com/nevertoday/xxd-panel-014) | 折叠与切面 · 层叠与嵌套 · 源图重心构图 · 真实纸纤维 · 可读纸艺文字 |
| [xxd-panel-015](https://github.com/nevertoday/xxd-panel-015) | 解构—筛选—提炼—重构 · 少量形体 · 严格色彩角色 · 象牙色留白 · 艺术书微排版 |
| [xxd-panel-016](https://github.com/nevertoday/xxd-panel-016) | ONE SUBJECT · ONE MOTION · A LARGE FIELD OF AIR |
| [xxd-panel-017](https://github.com/nevertoday/xxd-panel-017) | 圆润形体 · 粗糙断线 · 纯色平涂 · 明亮色场 · 轻快不对称 |
| [xxd-panel-018](https://github.com/nevertoday/xxd-panel-018) | 一个视觉锚点 · 前中后少量纸层 · 暖象牙留白 · 哑光纸触感 · 完整微排版 |
| [xxd-panel-019](https://github.com/nevertoday/xxd-panel-019) | RECOGNISE FIRST · REDUCE WITH INTENT · COMPOSE WITH TYPE |
| [xxd-panel-020](https://github.com/nevertoday/xxd-panel-020) | 厚涂颜料岛 · 立体微缩场景 · 真实刀痕 · 大面积纸面留白 · 克制编辑排版 |
| [xxd-panel-021](https://github.com/nevertoday/xxd-panel-021) | 纯黑矩形 · 主体大部入场 · 一个特征越界 · 抖动复印线 · 白色负形与微灰面 |
| [xxd-panel-022](https://github.com/nevertoday/xxd-panel-022) | 纯黑矩形 · 主体大部入场 · 一个特征越界 · 流畅稳定线 · 唯一单点彩色 |
| [xxd-panel-023](https://github.com/nevertoday/xxd-panel-023) | 源图择窗 · 浅色呼吸背景 · 柔和有色光影 · 喷绘颗粒 · 虚实投影与微排版 |
| [xxd-panel-024](https://github.com/nevertoday/xxd-panel-024) | 真实摄影主体 · 窄长浅色窗口 · 横／竖／斜向自适应 · 东方留白 · 高级商业编辑 |
| [xxd-panel-025](https://github.com/nevertoday/xxd-panel-025) | 一眼主体 · 第二眼隐藏意象 · 正负形反转 · 2–4 色莫兰迪 · 真实丝网触感 |
| [xxd-panel-026](https://github.com/nevertoday/xxd-panel-026) | RECOGNISE QUIETLY · REDUCE GENTLY · LET THE PAPER BREATHE |
| [xxd-panel-027](https://github.com/nevertoday/xxd-panel-027) | 乳白厚纸 · 浅凸浅凹 · 极简线刻 · 哑金焦点 · 博物馆展陈 |
| [xxd-panel-028](https://github.com/nevertoday/xxd-panel-028) | 正交等距 · 微缩基座 · 源图限定色盘 · 精细墨线 · 纸上编辑插画 |
| [xxd-panel-029](https://github.com/nevertoday/xxd-panel-029) | 横向色域 · 浅色蜡粉笔 · 粗纤维手工纸 · Risograph 颗粒 · 松弛手写 |
| [xxd-panel-030](https://github.com/nevertoday/xxd-panel-030) | 真实自然材料 · 矩形色域 · 自然越界 · 极少黑线 · 编辑留白 |
| [xxd-panel-031](https://github.com/nevertoday/xxd-panel-031) | 一个核心母题 · 源图几何母体 · 民俗图录 · 内部粗粝印痕 · 外部精确秩序 |
| [xxd-panel-032](https://github.com/nevertoday/xxd-panel-032) | 图文一体 · 原生文字结构 · 源图特征嵌入 · 视觉字距 · 高级留白 |
| [xxd-panel-033](https://github.com/nevertoday/xxd-panel-033) | 可识别母题 · 平面拼贴 · 尺度对比 · 源图鲜明配色 · 封面排版 |
| [xxd-panel-034](https://github.com/nevertoday/xxd-panel-034) | 小尺度章印 · 2–4 种专色 · 手刻线 · 暖色纸张 · 田野注释 |
| [xxd-panel-035](https://github.com/nevertoday/xxd-panel-035) | 单一积木主体 · 明艳源图色 · 哑光 ABS · 安静背景 · 模块文字 |
| [xxd-panel-036](https://github.com/nevertoday/xxd-panel-036) | 一个关系 · 纤细连续线 · 二至四色域 · 水彩渗化 · 柔软留白 |
| [xxd-panel-037](https://github.com/nevertoday/xxd-panel-037) | 一枚徽章 · 源图珐琅色 · 白金属外框 · 流金细节 · 实体短影 |
| [xxd-panel-038](https://github.com/nevertoday/xxd-panel-038) | 源图布色 · 真实毛边 · 手缝针脚 · 主动留白 · 隐藏情绪 |
| [xxd-panel-039](https://github.com/nevertoday/xxd-panel-039) | 一图一核 · 中国丝线 · 针向层次 · 洁净底色 · 东方留白 |
| [xxd-panel-040](https://github.com/nevertoday/xxd-panel-040) | 真实主体 · 黑线小人 · 微型叙事 · 大量留白 |
| [xxd-panel-041](https://github.com/nevertoday/xxd-panel-041) | 主题隐喻 · 等距秩序 · 淡手稿 · 日系清透色 · 东方留白 |
| [xxd-panel-042](https://github.com/nevertoday/xxd-panel-042) | 原始视角 · 二至五层 · 稳定锚点 · 透明水彩 · 编辑注释 |
| [xxd-panel-043](https://github.com/nevertoday/xxd-panel-043) | 真实皂沫 · 正面平视 · 源图深底 · 细密泡缘 · 安静空间 |
| [xxd-panel-044](https://github.com/nevertoday/xxd-panel-044) | 薄层纯金 · 正面平面 · 源图深底 · 锤纹压痕 · 安静秩序 |
| [xxd-panel-045](https://github.com/nevertoday/xxd-panel-045) | 圆润模块 · 源图色彩 · 等距纵深 · 哑光触感 · 编辑微排版 |
| [xxd-panel-046](https://github.com/nevertoday/xxd-panel-046) | 明亮白底 · 鲜活厚涂 · 微缩实体 · 斜向色带 · 温暖光感 |
| [xxd-panel-047](https://github.com/nevertoday/xxd-panel-047) | 等距微缩 · 主题厚涂 · 真实接触 · 暖白纸面 · 明亮色彩 |
| [xxd-panel-048](https://github.com/nevertoday/xxd-panel-048) | 透明结构 · 科学图解 · 清透单色 · 精确注释 · 编辑留白 |
| [xxd-panel-049](https://github.com/nevertoday/xxd-panel-049) | 限色木刻 · 手工刀痕 · 哑光套印 · 温暖纸面 · 不完整边缘 |
| [xxd-panel-050](https://github.com/nevertoday/xxd-panel-050) | 定制旅行场景 · 空气蓝 · 极简平涂矢量 · 编辑留白 · 一图一身份 |
| [xxd-panel-051](https://github.com/nevertoday/xxd-panel-051) | 微缩纸艺 · 横向悬浮景观带 · 真实手工材质 · 空气蓝 · 大量留白 |
| [xxd-panel-052](https://github.com/nevertoday/xxd-panel-052) | 纸艺微缩 · 横向浮岛 · 真实手作 · 空气感冷蓝 · 大量留白 |
| [xxd-panel-053](https://github.com/nevertoday/xxd-panel-053) | 观察线稿 · 透明淡彩 · 音乐性节奏 · 近白纸面 · 大胆留白 |
| [xxd-panel-054](https://github.com/nevertoday/xxd-panel-054) | 选择性记忆 · 主视觉 · 六枚贴纸 · 哑光印刷 · 空气感蓝 |
| [xxd-panel-055](https://github.com/nevertoday/xxd-panel-055) | 主体叙事 · 治愈粉彩 · 浅油画笔触 · 空气感蓝 · 编辑留白 |
| [xxd-panel-056](https://github.com/nevertoday/xxd-panel-056) | 核心意象 · 巨大留白 · 暖冷跳色 · 稚拙手绘 · 视觉隐喻 |
| [xxd-panel-057](https://github.com/nevertoday/xxd-panel-057) | 几何构成 · 智能马赛克 · 建筑图解 · 艺术地图 · 暖冷色块 |
| [xxd-panel-058](https://github.com/nevertoday/xxd-panel-058) | 潜台词解读 · 几何极简 · 观念景观 · 柔和手工质感 · 淡色留白 |
| [xxd-panel-059](https://github.com/nevertoday/xxd-panel-059) | 手绘叙事 · 童真隐喻 · 温暖纸感 · 轻微诙谐 · 诗性旁白 |
| [xxd-panel-060](https://github.com/nevertoday/xxd-panel-060) | 黑色主形 · 极大留白 · 网点消散 · 禅意思考 · 哲思碎片 |
| [xxd-panel-061](https://github.com/nevertoday/xxd-panel-061) | 选择性记忆 · 3–6 个片段 · 剪纸色块 · Risograph · 即兴编辑排版 · 治愈色盘 |
| [xxd-panel-062](https://github.com/nevertoday/xxd-panel-062) | 极简黑线 · 单一强调色 · 聪明笨拙 · 浅色纸底 · 专业留白 |
| [xxd-panel-063](https://github.com/nevertoday/xxd-panel-063) | 核心 Mask · 像素形体 · 负形嵌套 · 轻微 glitch · 有限色盘 · 大留白 |
| [xxd-panel-064](https://github.com/nevertoday/xxd-panel-064) | 手撕纸边 · 旧纸拼贴 · 铅笔墨线 · 打字机小字 · 档案感 · 诗性留白 |
| [xxd-panel-065](https://github.com/nevertoday/xxd-panel-065) | 黑色结构线 · 两种源图彩线 · 错位叠压 · 旧印刷节奏 · 微型排版 |
| [xxd-panel-066](https://github.com/nevertoday/xxd-panel-066) | 童真叙事 · 笨拙黑线 · 3–6 色平涂 · 治愈色彩 · 手写观察 · 大留白 |
| [xxd-panel-067](https://github.com/nevertoday/xxd-panel-067) | 固定红蓝 · 手绘双墨 · 童真幽默 · 生活观察 · 极浅纸底 · 手写短句 |
| [xxd-panel-068](https://github.com/nevertoday/xxd-panel-068) | 经营位置 · 计白当黑 · 墨线淡彩 · 东方题跋 · 现代编辑 · 清雅留白 |
| [xxd-panel-069](https://github.com/nevertoday/xxd-panel-069) | 粗笔绘画视窗 · 鲜活取色 · 纤细描边 · 越界关系 · 暖白留白 · 自由图文混排 |
| [xxd-panel-070](https://github.com/nevertoday/xxd-panel-070) | 手绘描边 · 明亮厚涂／半透明色块 · 微缩主体 · 暖白留白 · 打字机式编辑字体 |
| [xxd-panel-071](https://github.com/nevertoday/xxd-panel-071) | 柔和粉彩 · 粉蜡笔 · 水溶性色铅笔 · 近白纸面 · 漂浮记忆片段 · 诗性手写 |
| [xxd-panel-072](https://github.com/nevertoday/xxd-panel-072) | 半透明磨砂视窗 · 区域差异化柔焦 · 极简几何 · 清晰识别轮廓 · 明艳治愈色 · 现代编辑排版 |
| [xxd-panel-073](https://github.com/nevertoday/xxd-panel-073) | 等距微缩建筑 · 剖切立方体 · 大陆架空间 · 理性脚手架 · 手绘建筑图解 · 白色纹理纸 |
| [xxd-panel-074](https://github.com/nevertoday/xxd-panel-074) | 标准圆角方形 · 正面伪 3D／2.5D · 原图灵魂提炼 · 连续空间遮挡 · 哑光雕塑感 · 品牌图标提案 |
| [xxd-panel-075](https://github.com/nevertoday/xxd-panel-075) | 深色蜡笔速写 · 米白手工纸 · 柔和不规则色域 · Risograph 颗粒 · 大面积留白 · 打字机私人注记 |
| [xxd-panel-076](https://github.com/nevertoday/xxd-panel-076) | 粗粝深色蜡笔 · 炭笔彩铅 · 明亮马卡龙色块 · 45% 连续留白 · 天然纸面 · 打字机观察注记 |
| [xxd-panel-077](https://github.com/nevertoday/xxd-panel-077) | 极简纸雕拼贴 · 清晰剪纸轮廓 · 前后层叠 · 柔和投影 · 人文马卡龙 · 旅行杂志排版 |
| [xxd-panel-078](https://github.com/nevertoday/xxd-panel-078) | 暖米白棉纸 · 深压凹印 · 凹槽香槟金箔 · 纤细线性标识 · 无墨压痕 · 低调奢华 |
| [xxd-panel-079](https://github.com/nevertoday/xxd-panel-079) | 强几何直线 · 自由有机曲线 · 钢笔淡彩 · 未完成感 · 大面积纸白 · 编辑式图文混排 |
| [xxd-panel-080](https://github.com/nevertoday/xxd-panel-080) | 柔性有机几何 · 数字水粉蜡笔 · 颗粒肌理 · 植物系配色 · 自然隐喻 · 情绪留白 |
| [xxd-panel-081](https://github.com/nevertoday/xxd-panel-081) | 等粗彩色单线 · 开放轮廓 · 线密度层级 · 2–4 色专印 · Risograph 颗粒 · 私人纪念叙事 |
| [xxd-panel-082](https://github.com/nevertoday/xxd-panel-082) | 不规则水彩色域 · Naïve + Wonky · Isometric／2.5D · 稚拙轮廓 · 鲜活配色 · 立体主角 |
| [xxd-panel-083](https://github.com/nevertoday/xxd-panel-083) | Ugly-cute 丑萌涂鸦 · Wonky 发抖轮廓 · 故意失准 · 单一幽默主角 · 粗糙蜡笔 · 少怪笨准 |
| [xxd-panel-084](https://github.com/nevertoday/xxd-panel-084) | 极简城市线描 · 几何线性骨架 · 点描密度层次 · 透视引导线 · 限制性色彩 · 诗意留白 |
| [xxd-panel-085](https://github.com/nevertoday/xxd-panel-085) | 手工微缩舞台 · 收藏级立体封面 · 黏土毛毡纸板 · 手剪线绳 · 哑光触感 · 艺术留白 |
| [xxd-panel-086](https://github.com/nevertoday/xxd-panel-086) | 中世纪现代主义限色丝网版画 · 剪影几何 · 2–4 色专印 · 干刷拖墨 · 一个焦点 · 大面积留白 |
| [xxd-panel-087](https://github.com/nevertoday/xxd-panel-087) | 实体线绳关系系统地图 · 图钉节点 · 朱红线绳 · 关系映射 · 涌现几何 · 研究墙式留白 |
| [xxd-panel-088](https://github.com/nevertoday/xxd-panel-088) | 实验字体图像构成 · 文字即图像 · 解构排版 · 点阵轮廓 · 文字密度梯度 · 视觉诗 |
| [xxd-panel-089](https://github.com/nevertoday/xxd-panel-089) | 私人生活手账小品 · 一个主角 · 少量生活碎片 · 松散手绘线 · 水彩彩铅与粉蜡笔 · 成熟留白 |
| [xxd-panel-090](https://github.com/nevertoday/xxd-panel-090) | 图式化视觉思维地图 · 概念中心 · 文字节点 · 几何骨架 · 轨迹箭头 · 视觉记谱 · 大面积留白 |
| [xxd-panel-091](https://github.com/nevertoday/xxd-panel-091) | 单色蓝笔叙事速写 · 钴蓝／钢笔蓝／群青／靛蓝 · 方向排线 · 寻找线 · 选择性细化 · 自然纸白 |
| [xxd-panel-092](https://github.com/nevertoday/xxd-panel-092) | Expressive pen · loose contours · geometric and scribble hatching · negative-space composition |
| [xxd-panel-093](https://github.com/nevertoday/xxd-panel-093) | Independent original aesthetic · photo-grounded transformation · flexible multi-format delivery |
| [xxd-panel-094](https://github.com/nevertoday/xxd-panel-094) | Fine pen-and-ink · selective solid black · source-derived spot colour · vast negative space · vintage book illustration |
| [xxd-panel-095](https://github.com/nevertoday/xxd-panel-095) | Independent original aesthetic · photo-grounded transformation · flexible multi-format delivery |
| [xxd-panel-096](https://github.com/nevertoday/xxd-panel-096) | Independent original aesthetic · photo-grounded transformation · flexible multi-format delivery |
| [xxd-panel-097](https://github.com/nevertoday/xxd-panel-097) | Mid-century vernacular commercial graphic · schematic line drawing · two-colour spot printing · functional humour |
| [xxd-panel-098](https://github.com/nevertoday/xxd-panel-098) | 拟朴素水彩绘本插画 · 松散墨线 · 平面水彩／类水粉 · 符号化造型 · 天真透视 · 明快照片取色 · 成熟叙事构图 |
| [xxd-panel-099](https://github.com/nevertoday/xxd-panel-099) | 品牌吉祥物平面矢量插画 · 粗黑轮廓 · 圆润几何 · 夸张比例 · 2–4 色品牌化取色 · 超大文字背景 |
| [xxd-panel-100](https://github.com/nevertoday/xxd-panel-100) | 稚拙民艺感平面叙事 · primitive forms · 简化剪影 · flattened perspective · 蜡笔／油画棒颗粒 · 暖白纸面 · 鲜活限制色 |
| [xxd-panel-101](https://github.com/nevertoday/xxd-panel-101) | 九宫记忆簿 · 3×3 记忆图标 · 私人手帐感 · 稚拙涂鸦 · 复古糖果色 · 手写批注 |
| [xxd-panel-102](https://github.com/nevertoday/xxd-panel-102) | 治愈几何志 · 柔和几何形 · 扁平构成 · 温暖治愈色 · 轻松留白 |
| [xxd-panel-103](https://github.com/nevertoday/xxd-panel-103) | 鲜彩抽象拼 · 大色块 · 抽象拆分与拼合 · 高明度配色 · 醒目视觉节奏 |
| [xxd-panel-104](https://github.com/nevertoday/xxd-panel-104) | 网点禅意志 · 网点印刷 · 彩色线性介入 · 单一视觉重心 · 禅意留白 |
| [xxd-panel-105](https://github.com/nevertoday/xxd-panel-105) | 智能筛选最美一幕 · 单一视觉重心 · 诗意极简纸本拼贴 · 单版画／丝网／Risograph 质感 · 柔和有限色盘 · 大面积留白 |
| [xxd-panel-106](https://github.com/nevertoday/xxd-panel-106) | 柔彩像素记 · 2–4 个视觉锚点 · 规则网格 · 模块色块 · 局部 dithering · 单一视觉核心 · 大面积留白 |
| [xxd-panel-107](https://github.com/nevertoday/xxd-panel-107) | 图像替词诗 · 可读 Rebus 句子 · 现代手绘图像词 · 明快柔和色块 · 严格 50:50 双区 · 大量留白 |
| **[xxd-panel-108](https://github.com/nevertoday/xxd-panel-108)** | 当代民艺剪纸 · 简化剪影 · 手撕边 · 鲜活照片取色 · 印刷肌理 · 大面积留白 |
<!-- xxd-panel-catalog:end -->
