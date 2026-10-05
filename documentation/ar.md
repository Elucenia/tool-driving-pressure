<!-- ELUCENIA technical documentation · driving-pressure · ar · no clinical/professional/rights approval -->

# ضغط القيادة والمطاوعة الساكنة

[الشروط والمصادر والأذونات](https://elucenia.org/ar/tools/driving-pressure)

## كيفية الاستخدام

استخدم الأداة في البوابة أو افتح index.html عبر خادم HTTP محلي. اختر اللغة، وأكمل الحقول، ثم أجرِ الحساب.

## المدخلات والوحدات

### الحجم الجاري

`vt`

mL · النطاق: ١٠٠–١٥٠٠

### ضغط الهضبة (وقفة شهيقية)

`pplat`

cmH₂O · النطاق: ٥–٦٠

### PEEP الكلي

`peep`

cmH₂O · النطاق: ٠–٣٠

### الوزن المتوقع

`pbw`

kg · اختياري · النطاق: ٢٠–١٢٠

## إصدار الطريقة

ΔP=Pplat−PEEP؛ Cstat=VT/ΔP؛ سياق أماتو 2015 للتهوية السلبية

## المعادلة الموثقة

الضغط الدافع (ΔP) = ضغط الهضبة − PEEP.

المطاوعة الساكنة = الحجم الجاري ÷ ΔP (mL/cmH₂O).

## الحدود والفئة السكانية

درست دراسة Amato 2015 عددًا قدره 3562 مريضًا بمتلازمة الضائقة التنفسية الحادة (ARDS) من تسع تجارب سابقة، في سياق تهوية دون تنفس نشط. حُلّل ضغط الدفع (driving pressure) بوصفه VT/CRS ومتغيرًا مرتبطًا بالبقاء؛ ولا يثبت هذا الارتباط وحده عتبة عامة أو تدخلًا علاجيًا موجّهًا بالحساب. يجب مراجعة تقنية القياس وظروف التهوية.

## المراجع

- [Amato MBP et al. Driving pressure and survival in the acute respiratory distress syndrome. N Engl J Med, 2015.](https://doi.org/10.1056/NEJMsa1410639)

- [Fan E et al. An Official American Thoracic Society/European Society of Intensive Care Medicine/Society of Critical Care Medicine Clinical Practice Guideline: Mechanical Ventilation in Adult Patients with Acute Respiratory Distress Syndrome. Am J Respir Crit Care Med, 2017.](https://doi.org/10.1164/rccm.201703-0548ST)

## إعادة إجراء الاختبارات التقنية

شغّل node test.cjs في المجلد الجذري لهذا المستودع لتكرار الحالات الاصطناعية المسجلة. تُحفظ المدخلات والنتائج المتوقعة وحدود التفاوت الأصلية. لا تُعدّ الاختبارات التقنية تحققًا سريريًا.

```sh
node test.cjs
```

يحتوي tool.json على المصادر والإصدار ونطاق المراجعة. يحتفظ examples.json بالمدخلات والنتائج المتوقعة للحالات الاصطناعية؛ ويسجل results.json النتائج التي تم الحصول عليها.

[السجل والمراجع](../tool.json) · [شيفرة JavaScript](../calculator.js) · [حالات مرجعية](../examples.json) · [results.json](../results.json)

## المراجعة وشروط الاستخدام

لم تُجرَ مراجعة سريرية مستقلة.

هذه الواجهة ترجمة أعدّها مؤلفوها، وليست إصدارًا رسميًا أو معتمدًا. لم تُجرَ مراجعة سريرية مستقلة أو مراجعة لغوية مهنية، ولم تُستكمل الموافقة على حقوق استخدام الأدوات.

نتيجة المعادلة أو التصنيف. يعتمد التفسير والتصرف ومدى الانطباق على التقييم المهني والمصدر المحدد.

## الترخيص ونسبة العمل إلى أصحابه

ينطبق Apache-2.0 على كود ELUCENIA فقط. تبقى حقوق الأدوات والمنشورات والترجمات والبيانات لأصحابها المعنيين. احتفظ بملفّي LICENSE وNOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
