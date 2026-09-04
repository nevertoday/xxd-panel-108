<div align="center">

# XXD Panel 108｜سجل القصّ الورقي للفن الشعبي الجديد

نحوّل هوية الصورة إلى تكوين ورقي هادئ ذي حسّ ثقافي

[![Codex Skill](https://img.shields.io/badge/Codex-Skill-000000?style=flat-square)](./SKILL.md)

<a href="README.md">简体中文</a> · <a href="README.en.md">English</a> · <a href="README.ja.md">日本語</a> · <a href="README.ko.md">한국어</a> · <strong>العربية</strong>

</div>

## نماذج الأعمال

لا يتضمن هذا المستودع صوراً غير مُراجعة أو نماذج مستعارة من Panel آخر. ستُضاف النماذج بعد توليد ومراجعة الدفعة الأولى مستقلة.

تحمل الصور هوية ومشاعر قوية، لكنها قد تحتاج إلى إعادة تنظيم أكثر قصداً. يحافظ **Panel 108** على واقع الصورة ويترجم النصف الآخر بلغته البصرية المستقلة، لملصقات الفن والنشر المستقل والمعارض والمحتوى الاجتماعي والتصميم الخالص.

يعالج انفصال الصورة عن التصميم، والزخرفة الزائدة، ونقص المساحات البيضاء، وعدم ثبات التسليم بين النسب المختلفة.

- كل صورة تصبح نتيجة مستقلة؛ لا تُدمج الصور.
- المقارنة العمودية أو الأفقية بنسبة 50:50 بدقة ومن دون شريط ثالث.
- تُعالج الصور داخل المجلدات بشكل معزول بلا خلط للموضوع أو النص أو النتائج.
- في `design-only` والخلفيات تُستخدم الصورة كمرجع فقط ولا تظهر الصورة غير المحوّلة.

## الموجّه الأصلي · خمس لغات

[简体中文](references/original-prompt/zh-CN.md) · [English](references/original-prompt/en.md) · [日本語](references/original-prompt/ja.md) · [한국어](references/original-prompt/ko.md) · [العربية](references/original-prompt/ar.md)

يحفظ الملف الصيني الموجّه الأصلي للمشروع وهو المرجع الإبداعي والجمالي الوحيد وقت التشغيل؛ الإصدارات الأخرى للقراءة والتوثيق والمشاركة.

**الكلمات المفتاحية:** قصّ ورقي بفن شعبي جديد · كولاج ورقي مسطّح · ملمس الطباعة · 2–4 ألوان مستخلصة من الصورة · صورة رئيسية بطابع الختم · فراغ واسع

## أوضاع الإخراج الأربعة

- `top-bottom`: تكوين رأسي أصلي 3:4؛ الصورة الواقعية أعلى وتصميم Panel 108 أسفل، بنسبة 50% لكل منهما بدقة.
- `left-right`: الصورة الواقعية يساراً والتصميم يميناً، بنسبة 50% لكل منهما، ولا يُدار إلى تكوين علوي–سفلي.
- `design-only`: تعرض اللوحة كاملة تحويل هذا الـPanel فقط، وتبقى الصورة مرجعاً.
- `wallpaper-pack`: تُنشأ لوحة كاملة مستقلة لكل جهاز بدلاً من قصّ صورة واحدة آلياً.

تدعم نسباً متعددة وبكسلات دقيقة وأنماط نص مولّد／نص حرفي／بلا نص، ومعالجة مجلدات الصور والعلاقة `linked` أو `independent` للخلفيات. ينشئ كل استدعاء مجلد مهمة جديداً واحداً وتسليم PNG.

## الحالات المناسبة والمشكلات التي يحلها

يناسب الصور ذات الهوية القوية التي تضعفها الخلفية المعقدة أو المعالجة العادية. يحتفظ بالموضوع والمحيط والوضع والعلاقة السردية، ثم يحولها إلى قصاصات شعبية معاصرة بظلال مسطحة وخطوط محفورة وأشكال موجبة وسالبة وحبيبات طباعة.

- مناسب للملصقات الفنية والنشر المستقل والمعارض التي تحتاج حساً ثقافياً ويدوياً.
- يختار 2–4 ألوان من الصورة ويصنع مركزاً يشبه الختم وفراغاً ورقياً دافئاً واسعاً.
- يتجنب الرسم الواقعي والمتجهات اللامعة و3D والزخرفة الزائدة والقوالب الحرفية الرخيصة.

## فحص سريع ومنطق التحويل

`قراءة الموضوع والسرد → إبقاء المرتكزات → اختيار 2–4 ألوان من الصورة → الاختزال إلى قصاصات وخطوط محفورة وأشكال موجبة وسالبة → الإنهاء بملمس الطباعة والفراغ`

أنماط المقارنة منطقتان دقيقتان 50:50 بلا شريط ثالث. يعرض التصميم الخالص والخلفيات التحويل فقط. تُنشأ كل صورة مباشرة من أصلها الحالي في مرور واحد، ولا يُعاد إدخال نتيجة وسيطة أو Panel آخر. يعاد تكوين كل نسبة مستقلة، والنص مولّد أو حرفي أو غائب. التسليم النهائي PNG نقطي.

## البدء

```bash
git clone https://github.com/nevertoday/xxd-panel-108.git
mkdir -p ~/.codex/skills
ln -s "$(pwd)/xxd-panel-108" ~/.codex/skills/xxd-panel-108
```

يمكنك أيضاً التثبيت مباشرةً باستخدام `npx skills`:


```bash
npx skills add https://github.com/nevertoday/xxd-panel-108 --skill xxd-panel-108
```

يجلب الأمر المستودع من GitHub ويثبّت الـ Skill ذي الاسم نفسه. لتثبيت Codex للمستخدم أضف `--global --agent codex --yes` ثم أعد تشغيل جلسة الوكيل واستدعِه:

```text
$xxd-panel-108
```

المواصفات الكاملة: [SKILL.md](SKILL.md) · [مهايئ التشغيل](references/xxd-panel-108-prompt.en.md) · [الموجّه الأصلي](references/original-prompt/zh-CN.md)

## الترخيص

يُقدَّم المشروع بموجب **PolyForm Noncommercial License 1.0.0**. النص الكامل في [LICENSE](LICENSE) والصفحة الرسمية <https://polyformproject.org/licenses/noncommercial/1.0.0>.

- يُسمح بالدراسة والبحث والتجارب والاختبار والهوايات والترفيه الشخصي، وباستخدام المنظمات غير التجارية التي يعرّفها الترخيص.
- للأغراض غير التجارية يمكنك الاستخدام والنسخ والتعديل وإنشاء الأعمال المشتقة والتوزيع، مع إرفاق الترخيص وكل `Required Notice:` يقدمه المؤلف.
- تُحظر المنتجات والخدمات التجارية والتسليم بمقابل وبيع الوصول والاستخدامات ذات التطبيق التجاري المتوقع؛ يلزم إذن كتابي منفصل للاستخدام التجاري.
- تُمنح حقوق النشر وحقوق البراءة المحدودة المنصوص عليها فقط، ولا تُمنح العلامات التجارية أو الحقوق الأخرى، ولا يجوز إعادة الترخيص أو النقل.
- يجب تصحيح المخالفة خلال 32 يوماً من الإخطار الكتابي وإلا تنتهي التراخيص. يُقدَّم المشروع كما هو ومن دون ضمان.
<!-- xxd-panel-catalog:start -->
## دليل مشاريع XXD Panel

يحافظ كل واحد من مشاريع Panel الـ108 على موجّهه الأصلي ومنطقه الجمالي المستقل. يسرد الدليل المشاريع متتابعة من 001 إلى 108، ويظهر المشروع الحالي بخط عريض.

| Project | Style |
|---|---|
| [xxd-panel-001](https://github.com/nevertoday/xxd-panel-001) | خط عفوي · ورق قديم · وسائط مختلطة · استعارة ذكية · فراغ دافئ |
| [xxd-panel-002](https://github.com/nevertoday/xxd-panel-002) | محيط سردي · خط متردد · ألوان متجاورة · تكبير انتقائي · حروف مزاحة |
| [xxd-panel-003](https://github.com/nevertoday/xxd-panel-003) | خط أسود متصل · قضية عامة · نقاط قوة · فراغ صامت · تحرر |
| [xxd-panel-004](https://github.com/nevertoday/xxd-panel-004) | واقع محلي · خط دقيق · منظور هندسي · لون الموضوع · كتابة هوية المدينة |
| [xxd-panel-005](https://github.com/nevertoday/xxd-panel-005) | كتل غليظة · حقل بنيوي داكن · كشف جزئي · ترتيب لوني ثلاثي · طباعة حريرية × باستيل |
| [xxd-panel-006](https://github.com/nevertoday/xxd-panel-006) | موضوع 10–20% · ورق 80–90% · خط يدوي رفيع · أربعة ألوان كحد أقصى · أكريليك مسطح |
| [xxd-panel-007](https://github.com/nevertoday/xxd-panel-007) | رسوم مادية صغيرة · تقريب／مقطع／تكرار · فراغ متدرج · ملاحظات سوداء رفيعة · ملمس ورق ممسوح |
| [xxd-panel-008](https://github.com/nevertoday/xxd-panel-008) | إسقاط متساوي القياس · منصات／سلالم／أبواب · مفارقة مكانية · باستيل ديناميكي · ثلاثي أبعاد مطفأ |
| [xxd-panel-009](https://github.com/nevertoday/xxd-panel-009) | مرساة صغيرة · فراغ واسع · علاقة مكانية واحدة · ألوان موضعية · طباعة حريرية بنقاط نصفية |
| [xxd-panel-010](https://github.com/nevertoday/xxd-panel-010) | ظل أسود خشن · سمة بيضاء داخلية · وسيط جاف وملمس ورق · إشارات بيئية قليلة · نص صغير لكتاب أطفال |
| [xxd-panel-011](https://github.com/nevertoday/xxd-panel-011) | صورة جوهرية واحدة · علاقة واحدة · خط أسود متصل · صمت فاعل · لون ذاكرة واحد |
| [xxd-panel-012](https://github.com/nevertoday/xxd-panel-012) | تكاثف كثيف · تشتت خفيف نحو الخارج · ضبط هندسي · لون حيوي واحد · حروف مجهرية سوداء رمادية |
| [xxd-panel-013](https://github.com/nevertoday/xxd-panel-013) | تذكرة أفقية واحدة · تقسيم 74/26 · ألوان مائية مريحة · فراغ عاجي · قسيمة معلومات محلية اللغة |
| [xxd-panel-014](https://github.com/nevertoday/xxd-panel-014) | طي وقطع · طبقات وتعشيق · ثقل يقوده المصدر · ألياف ورق حقيقية · حروف ورقية مقروءة |
| [xxd-panel-015](https://github.com/nevertoday/xxd-panel-015) | تفكيك—اختيار—تقطير—إعادة بناء · أشكال قليلة · أدوار لونية صارمة · فراغ عاجي · نص مجهري لكتاب فني |
| [xxd-panel-016](https://github.com/nevertoday/xxd-panel-016) | موضوع واحد · حركة واحدة · مساحة واسعة من الهواء |
| [xxd-panel-017](https://github.com/nevertoday/xxd-panel-017) | أشكال مستديرة · خط خشن متقطع · تعبئة مسطحة صافية · مساحات مشرقة · لا تماثل حيوي |
| [xxd-panel-018](https://github.com/nevertoday/xxd-panel-018) | مرساة بصرية واحدة · طبقات أمامية ووسطى وخلفية قليلة · فراغ عاجي · ورق مطفأ · ميكروتايب كامل |
| [xxd-panel-019](https://github.com/nevertoday/xxd-panel-019) | تعرّف أولاً · اختزل بقصد · كوّن بالكتابة |
| [xxd-panel-020](https://github.com/nevertoday/xxd-panel-020) | جزيرة طلاء كثيف · مشهد مصغّر مجسّم · آثار سكين حقيقية · فراغ ورقي واسع · كتابة تحريرية رصينة |
| [xxd-panel-021](https://github.com/nevertoday/xxd-panel-021) | مستطيل أسود خالص · معظم الموضوع في الداخل · سمة واحدة تخترق الحد · خط نسخ مهتز · شكل سلبي أبيض ومساحات رمادية ضئيلة |
| [xxd-panel-022](https://github.com/nevertoday/xxd-panel-022) | مستطيل أسود خالص · معظم الموضوع في الداخل · سمة واحدة تخترق الحد · خط سلس ثابت · إشارة لونية واحدة |
| [xxd-panel-023](https://github.com/nevertoday/xxd-panel-023) | نافذة يختارها المصدر · خلفية شاحبة تتنفس · ضوء ملوّن ناعم · حبيبات رش · إسقاط منتشر ونص دقيق |
| [xxd-panel-024](https://github.com/nevertoday/xxd-panel-024) | موضوع فوتوغرافي · نافذة شاحبة ضيقة · اتجاه أفقي／عمودي／مائل من المصدر · فراغ شرقي · تحرير فاخر |
| [xxd-panel-025](https://github.com/nevertoday/xxd-panel-025) | موضوع أولاً · صورة خفية ثانياً · انقلاب الشكل والخلفية · 2–4 ألوان موراندي · طباعة حريرية مادية |
| [xxd-panel-026](https://github.com/nevertoday/xxd-panel-026) | تعرّف بهدوء · اختزل بلطف · دع الورق يتنفس |
| [xxd-panel-027](https://github.com/nevertoday/xxd-panel-027) | ورق عاجي ثقيل · بروز وغور خفيفان · حفر خطي دقيق · بؤرة ذهبية مطفأة · نظام متحفي |
| [xxd-panel-028](https://github.com/nevertoday/xxd-panel-028) | إسقاط متساوي القياس · قاعدة ورقية صغيرة · ألوان من المصدر · حبر دقيق · نموذج تحريري |
| [xxd-panel-029](https://github.com/nevertoday/xxd-panel-029) | حقل أفقي · باستيل شمعي فاتح · ورق يدوي خشن · حبيبات ريسوغراف · كتابة يدوية مسترخية |
| [xxd-panel-030](https://github.com/nevertoday/xxd-panel-030) | مواد طبيعية حقيقية · حقل مستطيل · عبور طبيعي · أقل قدر من الخط الأسود · فراغ تحريري |
| [xxd-panel-031](https://github.com/nevertoday/xxd-panel-031) | رمز مركزي واحد · هندسة مشتقة من المصدر · فهرس شعبي · أثر حبر خشن في الداخل · نظام دقيق في الخارج |
| [xxd-panel-032](https://github.com/nevertoday/xxd-panel-032) | وحدة النص والصورة · حروف أصيلة للخط · دمج سمة المصدر · تباعد بصري · فراغ واسع |
| [xxd-panel-033](https://github.com/nevertoday/xxd-panel-033) | عنصر مميز · كولاج مسطح · تباين المقاييس · لون حي من المصدر · طباعة غلافية |
| [xxd-panel-034](https://github.com/nevertoday/xxd-panel-034) | ختم صغير · لونان إلى أربعة ألوان موضعية · حفر يدوي · ورق دافئ · ملاحظة ميدانية |
| [xxd-panel-035](https://github.com/nevertoday/xxd-panel-035) | موضوع مكعّب واحد · لون حي من المصدر · بلاستيك ABS مطفأ · خلفية هادئة · كتابة معيارية |
| [xxd-panel-036](https://github.com/nevertoday/xxd-panel-036) | علاقة واحدة · خط رفيع متصل · ٢–٤ حقول لونية · حافة مائية · فراغ يتنفس |
| [xxd-panel-037](https://github.com/nevertoday/xxd-panel-037) | شارة واحدة · مينا من المصدر · إطار معدني أبيض · تفصيل مذهّب · ظل حقيقي قصير |
| [xxd-panel-038](https://github.com/nevertoday/xxd-panel-038) | قماش من المصدر · حافة مهدّبة · خياطة يدوية · فراغ فعّال · شعور خفي |
| [xxd-panel-039](https://github.com/nevertoday/xxd-panel-039) | صورة واحدة · جوهر واحد · اتجاه حرير · أرضية نقية · صمت شرقي |
| [xxd-panel-040](https://github.com/nevertoday/xxd-panel-040) | موضوع واقعي · شخصيات بخط أسود · سرد مصغّر · فراغ واسع |
| [xxd-panel-041](https://github.com/nevertoday/xxd-panel-041) | استعارة موضوعية · نظام إيزومتري · مخطوط باهت · لون ياباني صافٍ · فراغ شرقي |
| [xxd-panel-042](https://github.com/nevertoday/xxd-panel-042) | المنظور الأصلي · ٢–٥ طبقات حقيقية · مرساة ثابتة · ألوان مائية شفافة · ملاحظة تحريرية |
| [xxd-panel-043](https://github.com/nevertoday/xxd-panel-043) | رغوة حقيقية · تصوير مسطح أمامي · أرضية داكنة من المصدر · حافة فقاعات دقيقة · فراغ هادئ |
| [xxd-panel-044](https://github.com/nevertoday/xxd-panel-044) | ذهب رقيق · سطح أمامي · أرضية داكنة من المصدر · أثر مطروق · نظام هادئ |
| [xxd-panel-045](https://github.com/nevertoday/xxd-panel-045) | وحدات مدوّرة · لون من المصدر · عمق إيزومتري · ملمس مطفأ · كتابة تحريرية دقيقة |
| [xxd-panel-046](https://github.com/nevertoday/xxd-panel-046) | أرضية بيضاء مشرقة · طلاء كثيف نابض · حجم مصغّر مجسّم · حقل قطري · ضوء دافئ |
| [xxd-panel-047](https://github.com/nevertoday/xxd-panel-047) | مجسّم إيزومتري · طلاء موضوعي كثيف · تماس حقيقي · ورق أبيض دافئ · لون مضيء |
| [xxd-panel-048](https://github.com/nevertoday/xxd-panel-048) | بنية شفافة · رسم علمي · لون أحادي صافٍ · تعليقات دقيقة · فراغ تحريري |
| [xxd-panel-049](https://github.com/nevertoday/xxd-panel-049) | نقش خشبي محدود الألوان · آثار حفر يدوية · حبر مطفأ · ورق دافئ · حواف غير مكتملة |
| [xxd-panel-050](https://github.com/nevertoday/xxd-panel-050) | مشهد سفر مخصّص · أزرق هوائي · متجهات مسطّحة بسيطة · فراغ تحريري · هوية مستقلة لكل صورة |
| [xxd-panel-051](https://github.com/nevertoday/xxd-panel-051) | حرفة ورقية مصغّرة · شريط أفقي عائم · أثر يدوي حقيقي · أزرق هوائي · فراغ واسع |
| [xxd-panel-052](https://github.com/nevertoday/xxd-panel-052) | مجسّم ورقي · شريط أفقي عائم · مادة يدوية أصيلة · أزرق بارد هوائي · فراغ واسع |
| [xxd-panel-053](https://github.com/nevertoday/xxd-panel-053) | خط قلم ملاحظ · تلوين شفاف · إيقاع موسيقي · ورق شبه أبيض · فراغ فعّال |
| [xxd-panel-054](https://github.com/nevertoday/xxd-panel-054) | ذاكرة انتقائية · مشهد رئيس · ست ملصقات · طباعة مطفأة · أزرق هوائي |
| [xxd-panel-055](https://github.com/nevertoday/xxd-panel-055) | سرد الموضوع · ألوان باستيل مريحة · ملمس زيتي خفيف · أزرق هوائي · فراغ تحريري |
| [xxd-panel-056](https://github.com/nevertoday/xxd-panel-056) | صورة جوهرية · فراغ واسع · قفزات دافئة وباردة · يد فطرية · استعارة بصرية |
| [xxd-panel-057](https://github.com/nevertoday/xxd-panel-057) | تكوين هندسي · فسيفساء ذكية · مخطط معماري · خريطة فنية · حقول لونية دافئة وباردة |
| [xxd-panel-058](https://github.com/nevertoday/xxd-panel-058) | قراءة المعنى الضمني · بساطة هندسية · مشهد مفاهيمي · ملمس يدوي ناعم · فراغات فاتحة |
| [xxd-panel-059](https://github.com/nevertoday/xxd-panel-059) | سرد مرسوم يدوياً · استعارة طفولية · ورق دافئ · فكاهة رقيقة · تعليق شاعري |
| [xxd-panel-060](https://github.com/nevertoday/xxd-panel-060) | شكل أسود رئيسي · فراغ هائل · تلاشي هالف تون · تأمل زِنّي · شظايا فكر |
| [xxd-panel-061](https://github.com/nevertoday/xxd-panel-061) | ذاكرة انتقائية · 3–6 شظايا · كتل ورقية · ريزوغراف · تحرير ارتجالي |
| [xxd-panel-062](https://github.com/nevertoday/xxd-panel-062) | خط أسود بسيط · لون تأكيد واحد · عفوية ذكية · ورق فاتح · فراغ احترافي |
| [xxd-panel-063](https://github.com/nevertoday/xxd-panel-063) | قناع مركزي · أشكال بكسل · فراغ سلبي متداخل · خلل خفيف · ألوان محدودة |
| [xxd-panel-064](https://github.com/nevertoday/xxd-panel-064) | ورق ممزق · كولاج قديم · رصاص وحبر · كتابة آلية صغيرة · أرشيف شاعري |
| [xxd-panel-065](https://github.com/nevertoday/xxd-panel-065) | بنية سوداء · خطان من ألوان المصدر · انزياح طباعي · إيقاع طباعة قديمة · كتابة دقيقة |
| [xxd-panel-066](https://github.com/nevertoday/xxd-panel-066) | سرد طفولي · خط أسود عفوي · 3–6 ألوان مسطحة · ألوان مريحة · ملاحظة مكتوبة يدوياً |
| [xxd-panel-067](https://github.com/nevertoday/xxd-panel-067) | حبر أحمر وأزرق ثابت · رسم ثنائي · دعابة طفولية · مراقبة يومية · ورق فاتح |
| [xxd-panel-068](https://github.com/nevertoday/xxd-panel-068) | تنظيم صيني حر · اعتبار البياض حبراً · خط حبر ولون خفيف · كتابة نقشية · تحرير حديث |
| [xxd-panel-069](https://github.com/nevertoday/xxd-panel-069) | نافذة فرشاة عريضة · لون مصدر حي · حدود رفيعة · تجاوز الحواف · فراغ أبيض دافئ |
| [xxd-panel-070](https://github.com/nevertoday/xxd-panel-070) | خطوط يدوية · طلاء مشرق／لون شبه شفاف · موضوع مصغّر · فراغ أبيض دافئ · خط تحريري شبيه بالآلة الكاتبة |
| [xxd-panel-071](https://github.com/nevertoday/xxd-panel-071) | باستيل ناعم · أقلام باستيل شمعية · أقلام مائية ملونة · ورق شبه أبيض · شذرات ذاكرة عائمة · كتابة شاعرية |
| [xxd-panel-072](https://github.com/nevertoday/xxd-panel-072) | نوافذ مصنفرة نصف شفافة · تركيز ناعم مناطقي · هندسة بسيطة · محيط واضح · كتابة حديثة |
| [xxd-panel-073](https://github.com/nevertoday/xxd-panel-073) | عمارة مصغرة متساوية القياس · مكعب مقطوع · مقطع جرف قاري · سقالات عقلانية · ورق محبب |
| [xxd-panel-074](https://github.com/nevertoday/xxd-panel-074) | مربع مستدير قياسي · منظور أمامي شبه3D／2.5D · روح المصدر · حجب متصل · نحت مطفأ · أيقونة علامة |
| [xxd-panel-075](https://github.com/nevertoday/xxd-panel-075) | قلم شمعي داكن · ورق عاجي يدوي · مساحة لونية ناعمة · حبيبات ريسوغراف · فراغ واسع · ملاحظة خاصة |
| [xxd-panel-076](https://github.com/nevertoday/xxd-panel-076) | قلم شمعي داكن خشن · فحم · مساحات ماكرون مشرقة · فراغ متصل 45٪ · ورق طبيعي · ملاحظات رصد |
| [xxd-panel-077](https://github.com/nevertoday/xxd-panel-077) | نحت ورقي بسيط · محيطات قص واضحة · طبقات · ظل ناعم · ماكرون إنساني · طباعة مجلة سفر |
| [xxd-panel-078](https://github.com/nevertoday/xxd-panel-078) | ورق قطني عاجي · ضغط غائر عميق · ذهب شامبانيا داخل الأخدود · علامة خطية دقيقة · ضغط بلا حبر · فخامة هادئة |
| [xxd-panel-079](https://github.com/nevertoday/xxd-panel-079) | خطوط هندسية قوية · منحنيات عضوية حرة · حبر وتلوين مائي · إحساس غير مكتمل · بياض ورق واسع · تركيب تحريري |
| [xxd-panel-080](https://github.com/nevertoday/xxd-panel-080) | هندسة عضوية لينة · غواش رقمي · نسيج شمعي حبيبي · ألوان نباتية · استعارة طبيعية · فراغ عاطفي |
| [xxd-panel-081](https://github.com/nevertoday/xxd-panel-081) | خط أحادي ملوّن · محيط مفتوح · تدرّج الكثافة · 2–4 ألوان خاصة · حبيبات ريزوغراف · سرد تذكاري |
| [xxd-panel-082](https://github.com/nevertoday/xxd-panel-082) | حقل مائي غير منتظم · Naïve + Wonky · Isometric／2.5D · محيط طفولي · لون حي · بطل مجسّم |
| [xxd-panel-083](https://github.com/nevertoday/xxd-panel-083) | خربشة Ugly-cute · محيط Wonky · عدم دقة مضبوطة · بطل فكاهي واحد · شمع خشن · قليل وغريب وأخرق ودقيق |
| [xxd-panel-084](https://github.com/nevertoday/xxd-panel-084) | رسم حضري بسيط · هيكل هندسي · تنقيط كثافي · خطوط منظور قائدة · ألوان محدودة · فراغ شعري |
| [xxd-panel-085](https://github.com/nevertoday/xxd-panel-085) | مسرح مصغّر يدوي · غلاف مجسّم قابل للاقتناء · طين ولباد · ورق مقصوص وخيط · ملمس مطفأ · فراغ فني |
| [xxd-panel-086](https://github.com/nevertoday/xxd-panel-086) | طباعة شاشة حريرية محدودة الألوان بروح منتصف القرن · هندسة ظلية · 2–4 أحبار خاصة · سحب فرشاة جافة · بؤرة واحدة · فراغ واسع |
| [xxd-panel-087](https://github.com/nevertoday/xxd-panel-087) | خريطة علاقات فعلية بالدبابيس والخيط · خيط قرمزي · رسم العلاقات · هندسة ناشئة · ملاحظات يدوية · فراغ جدار بحث |
| [xxd-panel-088](https://github.com/nevertoday/xxd-panel-088) | تكوين تجريبي للصورة الطباعية · النص هو الصورة · صفّ مفكك · محيط نقطي · تدرج كثافة الحروف · شعر بصري |
| [xxd-panel-089](https://github.com/nevertoday/xxd-panel-089) | لقطة من دفتر حياة خاص · بطل واحد · شذرات يومية قليلة · خط يدوي حر · ألوان مائية وأقلام ملونة · فراغ ناضج |
| [xxd-panel-090](https://github.com/nevertoday/xxd-panel-090) | خريطة تفكير بصرية تخطيطية · مركز مفهومي · عقد نصية · هيكل هندسي · أسهم مسار · تدوين بصري · فراغ واسع |
| [xxd-panel-091](https://github.com/nevertoday/xxd-panel-091) | رسم سردي بقلم أزرق أحادي · كوبالت／أزرق قلم／فوق بحري／نيلي · تهشير اتجاهي · خطوط بحث · بياض ورقي طبيعي |
| [xxd-panel-092](https://github.com/nevertoday/xxd-panel-092) | Expressive pen · loose contours · geometric and scribble hatching · negative-space composition |
| [xxd-panel-093](https://github.com/nevertoday/xxd-panel-093) | Independent original aesthetic · photo-grounded transformation · flexible multi-format delivery |
| [xxd-panel-094](https://github.com/nevertoday/xxd-panel-094) | Fine pen-and-ink · selective solid black · source-derived spot colour · vast negative space · vintage book illustration |
| [xxd-panel-095](https://github.com/nevertoday/xxd-panel-095) | Independent original aesthetic · photo-grounded transformation · flexible multi-format delivery |
| [xxd-panel-096](https://github.com/nevertoday/xxd-panel-096) | Independent original aesthetic · photo-grounded transformation · flexible multi-format delivery |
| [xxd-panel-097](https://github.com/nevertoday/xxd-panel-097) | Mid-century vernacular commercial graphic · schematic line drawing · two-colour spot printing · functional humour |
| [xxd-panel-098](https://github.com/nevertoday/xxd-panel-098) | رسم كتاب مصور مائي شبه فطري · خط حبر حر · ألوان مائية／غواش مسطح · أشكال رمزية · منظور بريء · تكوين سردي ناضج |
| [xxd-panel-099](https://github.com/nevertoday/xxd-panel-099) | تميمة علامة مسطحة متجهية · محيط أسود سميك · هندسة مستديرة · نسب مبالغ فيها · 2–4 ألوان علامة · خلفية حروف ضخمة |
| [xxd-panel-100](https://github.com/nevertoday/xxd-panel-100) | سرد شعبي فطري مسطح · أشكال بدائية · ظلال مبسطة · منظور مسطح · حبيبات شمع／باستيل زيتي · ورق دافئ · ألوان حية محدودة |
| [xxd-panel-101](https://github.com/nevertoday/xxd-panel-101) | شبكة 3×3 من أيقونات الذاكرة · إحساس دفتر خاص · خربشات عفوية · ألوان حلوى قديمة · ملاحظات يدوية |
| [xxd-panel-102](https://github.com/nevertoday/xxd-panel-102) | هندسة مريحة · أشكال لينة · تكوين مسطح · ألوان دافئة شافية · فراغ خفيف |
| [xxd-panel-103](https://github.com/nevertoday/xxd-panel-103) | تجميع تجريدي زاهي · كتل لونية كبيرة · تفكيك وإعادة تركيب · لوحة ساطعة · إيقاع قوي |
| [xxd-panel-104](https://github.com/nevertoday/xxd-panel-104) | طباعة نصفية · تدخلات خطية ملونة · مركز بصري واحد · فراغ تأملي |
| [xxd-panel-105](https://github.com/nevertoday/xxd-panel-105) | انتقاء جمالي ذكي · مركز بصري واحد · كولاج ورقي شعري بسيط · ملمس طباعة أحادية／شاشة حريرية／Risograph · لوحة محدودة ناعمة · فراغ واسع |
| [xxd-panel-106](https://github.com/nevertoday/xxd-panel-106) | ذاكرة بكسلية ناعمة · 2–4 مرتكزات بصرية · شبكة منتظمة · كتل معيارية · تهشير نقطي موضعي · مركز بصري واحد · فراغ واسع |
| [xxd-panel-107](https://github.com/nevertoday/xxd-panel-107) | شعر الكلمات المصوّرة · جملة أحجية قابلة للقراءة · كلمات مرسومة يدوياً · كتل مضيئة وناعمة · تقسيم دقيق 50:50 · فراغ واسع |
| **[xxd-panel-108](https://github.com/nevertoday/xxd-panel-108)** | قصاصات ورق بفن شعبي معاصر · ظلال مبسطة · حواف ممزقة · ألوان حية من المصدر · ملمس طباعة · فراغ واسع |
<!-- xxd-panel-catalog:end -->
