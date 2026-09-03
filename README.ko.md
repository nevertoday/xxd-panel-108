<div align="center">

# XXD Panel 108｜新民艺剪纸志

把照片的识别性，重新剪成一张安静而有文化感的纸上构图

[![Codex Skill](https://img.shields.io/badge/Codex-Skill-000000?style=flat-square)](./SKILL.md)

</div>

## 샘플 작품

검토되지 않았거나 다른 Panel에서 빌린 이미지는 포함하지 않습니다. 독립 생성과 방향 검토를 마친 첫 릴리스 후 샘플을 추가합니다.

사진은 이미 강한 정체성과 분위기를 담고 있지만, 더 의도적인 재구성이 필요할 때가 있습니다. **Panel 108**은 사진의 현실감을 유지하고 다른 절반을 독립적인 시각 언어로 번역합니다. 아트 포스터, 독립 출판, 전시 이미지, 소셜 콘텐츠와 디자인 전용 출력에 적합합니다.

사진과 디자인이 따로 노는 문제, 과도한 장식, 부족한 여백, 비율별 불안정한 결과를 해결합니다.

- 사진 한 장은 독립적인 결과 한 장이 됩니다. 사진을 합치지 않습니다.
- 위아래·좌우 비교는 제3 영역 없이 엄격한 50:50입니다.
- 폴더 입력도 주체·문구·결과를 섞지 않고 개별 처리합니다.
- `design-only`와 배경화면 모드에서는 사진을 참고로만 사용하고 변환되지 않은 사진을 보여주지 않습니다.

## 원본 프롬프트 · 5개 언어

[简体中文](references/original-prompt/zh-CN.md) · [English](references/original-prompt/en.md) · [日本語](references/original-prompt/ja.md) · [한국어](references/original-prompt/ko.md) · [العربية](references/original-prompt/ar.md)

중문 파일은 이 프로젝트의 원본 프롬프트를 보존하며 런타임의 유일한 창작·미학 기준입니다. 다른 버전은 읽기·문서·공유용입니다.

**키워드:** 新民艺剪纸 · 扁平剪纸拼贴 · 版画肌理 · 2–4 色照片取色 · 章印感主视觉 · 大面积留白

## 네 가지 출력 모드

- `top-bottom`：3:4 竖版原生结构，现实照片在上，Panel 108 设计在下，严格各占 50%。
- `left-right`：现实照片在左，设计在右，严格各占 50%，不会旋转成上下结构。
- `design-only`：整张画布只呈现本 Panel 的设计转译，照片只作为参考。
- `wallpaper-pack`：按设备分别生成完整画布，不把一张图机械裁成多台设备。

支持多比例、准确像素、文字自动生成／准确文字／无文字、图片目录批量处理，以及 `linked` 或 `independent` 壁纸关系。每次调用只创建一个新任务目录，最终交付为 PNG。

## 시작하기

```bash
git clone https://github.com/nevertoday/xxd-panel-108.git
mkdir -p ~/.codex/skills
ln -s "$(pwd)/xxd-panel-108" ~/.codex/skills/xxd-panel-108
```

`npx skills`로도 바로 설치할 수 있습니다:

```bash
npx skills add https://github.com/nevertoday/xxd-panel-108 --skill xxd-panel-108
```

이 명령은 GitHub에서 저장소를 가져와 같은 이름의 Skill을 설치합니다. 사용자 전역 Codex 설치는 끝에 `--global --agent codex --yes`를 추가한 뒤 Agent 세션을 다시 시작해 호출하세요.

```text
$xxd-panel-108
```

完整规范：[SKILL.md](SKILL.md) · [运行适配器](references/xxd-panel-108-prompt.en.md) · [原始提示词](references/original-prompt/zh-CN.md)

## 라이선스

이 프로젝트는 **PolyForm Noncommercial License 1.0.0**에 따라 제공됩니다. 전체 법적 전문은 [LICENSE](LICENSE), 공식 페이지는 <https://polyformproject.org/licenses/noncommercial/1.0.0>에서 확인하세요.

- 개인 학습·연구·실험·테스트·취미·비공개 오락과 라이선스가 정의한 비상업 조직의 사용을 허용합니다.
- 비상업적 목적이면 사용·복사·수정·2차 저작물 작성·배포가 가능하지만 라이선스와 저자의 모든 `Required Notice:`를 함께 제공해야 합니다.
- 상업 제품·서비스, 유료 납품, 접근권 판매와 예상되는 상업적 적용은 금지되며 별도 서면 허가가 필요합니다.
- 명시된 저작권과 제한적 특허권만 부여되며 상표 등 다른 권리는 부여되지 않습니다. 재허여·양도도 금지됩니다.
- 위반 서면 통지 후 32일 안에 시정하지 않으면 라이선스가 종료됩니다. 프로젝트는 있는 그대로 제공되며 보증하지 않습니다.
