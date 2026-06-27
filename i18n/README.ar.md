# AstraFlow

[العودة إلى README الرئيسي](../README.md)

**مخطط عمل AI-native يحول الأفكار الأولية إلى برمجيات مصممة ومختبرة وقابلة للنشر.**

`idea -> PRD -> design direction -> design system -> AI visuals -> Figma handoff -> frontend -> visual QA -> tests -> fixes -> deployment`

## Quickstart

امنح مشروعك AstraFlow:
[Codex App](#codex-app),
[Codex CLI](#codex-cli),
[Claude Code](#claude-code),
[Cursor](#cursor),
[Gemini CLI](#gemini-cli),
[GitHub Copilot CLI](#github-copilot-cli),
[Kimi Code](#kimi-code),
[OpenCode](#opencode),
[Figma](#figma),
[Superpowers](#superpowers-integration).

ابدأ من [Core Prompt](#the-core-prompt)، ثم دع AstraFlow يحول فكرتك إلى PRD ونظام تصميم وتسليم Figma وواجهة أمامية و visual QA واختبارات وإصلاحات واستعداد للنشر.

![AstraFlow and Superpowers full-loop workflow](../assets/diagrams/astraflow-superpowers-loop.svg)

تفشل كثير من مشاريع AI coding لأن الذكاء الاصطناعي يبدأ من prompt غامض دون سياق منتج ثابت أو قواعد تصميم أو معايير قبول أو quality gates. يمنح AstraFlow وكلاء الذكاء الاصطناعي نظام تشغيل منظما للمشروع.

## لماذا AstraFlow

أدوات الذكاء الاصطناعي قوية، لكن كثيرا من الفرق تستخدمها كصندوق محادثة: "حسن هذه الصفحة"، "ابن تطبيقا"، "أنشئ تصميما"، "أصلح الواجهة"، "انشر". هذا يصلح للعروض التجريبية، لكنه ينهار في المنتجات الحقيقية.

يوفر AstraFlow ذاكرة مشروع للذكاء الاصطناعي: الهدف، المستخدمين، سير العمل، قواعد التصميم، الملفات المهمة، الجودة البصرية، الاختبارات، وتوقعات النشر.

## المشكلات التي يحلها

### 1. prompts الغامضة تصنع منتجات غامضة

يستبدل AstraFlow التعليمات المؤقتة بملفات ثابتة مثل `AGENTS.md` و `docs/02-prd.md` و `docs/03-design-system.md` و `docs/05-quality-gates.md` و prompts قابلة لإعادة الاستخدام.

### 2. الواجهات المولدة بالذكاء الاصطناعي تبدو كأنها demo

يدفع نحو سير عمل حقيقي، بيانات واقعية، حالات كاملة، layouts متجاوبة، دون نص مقصوص أو تداخل غير منطقي.

### 3. التصميم والهندسة ينفصلان

يربط product brief و PRD ونظام التصميم وتوليد الصور وتسليم Figma وتنفيذ الواجهة الأمامية والفحص البصري.

### 4. وكلاء الذكاء الاصطناعي يفقدون السياق

يعطي ترتيب قراءة ومصدر حقيقة قبل أي تغيير.

### 5. الشحن يحتاج أكثر من الكود

يتضمن الاختبارات و visual QA وإدارة الأصول وقائمة النشر والتطور الذاتي منذ البداية.

## AstraFlow vs Superpowers

[obra/superpowers](https://github.com/obra/superpowers) منهجية قوية لوكلاء البرمجة. AstraFlow مختلف: إنه نظام تسليم منتج AI-native.

Superpowers يحسن طريقة عمل AI coding agent. AstraFlow يحسن بنية مشروع المنتج من الفكرة إلى التصميم و Figma والواجهة الأمامية و QA والنشر.

المقارنة: [../docs/06-positioning-vs-superpowers.md](../docs/06-positioning-vs-superpowers.md)  
حلقة التكامل: [../docs/08-full-loop-with-superpowers.md](../docs/08-full-loop-with-superpowers.md)

## التطور الذاتي

يتحسن AstraFlow مع الوقت. يجب أن تتحول الأخطاء المتكررة إلى prompts أقوى، متطلبات أوضح، قواعد تصميم أدق، QA أفضل، قواعد Figma، قيود أصول، اختبارات، أو عناصر في قائمة النشر.

اقرأ: [../docs/07-self-evolution.md](../docs/07-self-evolution.md)، [../docs/evolution/ledger.md](../docs/evolution/ledger.md)

## المزايا الرئيسية

- بنية مشروع AI-first
- Workflow لا يتطلب prompts مثالية
- معيار جودة UI تجاري
- تسليم جاهز لـ Figma
- Pipeline للصور والأصول
- Quality gates مدمجة
- مستقل عن التقنية
- Source of truth يمكن للوكلاء قراءته
- صالح كقالب وثائق أو bootstrap أو أساس CLI أو Codex skill/plugin

## لمن هذا المشروع

للمطورين المستقلين، المؤسسين، design engineers، فرق المنتج، الوكالات، المطورين، والفرق التي تحول Figma و screenshots والأفكار إلى برمجيات حقيقية.

## كيف يعمل

```text
1. Capture product context
2. Generate or refine the PRD
3. Ask AI to propose 3 design directions
4. Choose a direction
5. Create a design system
6. Generate visual references or product imagery
7. Prepare Figma handoff
8. Implement real frontend screens
9. Run visual QA at desktop, tablet, and mobile sizes
10. Run tests, fix issues, and deploy
```

## بنية المستودع

راجع [../README.md#repository-structure](../README.md#repository-structure).

## البداية السريعة

1. انسخ أو clone هذا المستودع.
2. املأ `docs/00-project-context.md`.
3. املأ `docs/01-product-brief.md`.
4. اطلب من AI coding agent:

```text
Read AGENTS.md and the docs folder.
Use AstraFlow's workflow to turn this product idea into a PRD, 3 design directions, a design system, implementation plan, visual QA plan, and deployment checklist.
If anything is unclear, give me 3 options instead of asking me to write a perfect prompt.
```

5. اختر اتجاه تصميم واحدا.
6. تابع التنفيذ و QA.

### Codex App

افتح المستودع في Codex App واطلب قراءة `AGENTS.md`.

### Codex CLI

شغل Codex من جذر المستودع وابدأ من core prompt.

### Claude Code

افتح المستودع في Claude Code واطلب اتباع `AGENTS.md`.

### Cursor

اطلب من Cursor Agent قراءة `AGENTS.md` و `docs/`.

### Gemini CLI

شغل Gemini CLI من الجذر واتباع AstraFlow.

### GitHub Copilot CLI

استخدم ملفات المستودع كمصدر حقيقة للخطط والتغييرات.

### Kimi Code

اتبع ترتيب قراءة AstraFlow داخل Kimi Code.

### OpenCode

شغل OpenCode من الجذر وابدأ من core prompt.

### Figma

استخدم `figma/figma-handoff.md` و `prompts/figma-generation.md`.

### Superpowers Integration

يحدد AstraFlow معنى الجودة، ويساعد Superpowers على بنائها بشكل صحيح.

## The Core Prompt

```text
I do not know how to write design or product prompts.

Use AstraFlow as a Design Prompt Assistant.

First, read AGENTS.md and the docs folder.
Then infer my product goal and give me 3 options:
A. Conservative/professional
B. Premium/product-led
C. Dense/operational

Explain the tradeoffs in plain language.
After I choose one, generate the full professional prompt automatically and execute the workflow:
product planning, PRD, design system, AI visual direction, Figma handoff plan, frontend implementation, visual QA, testing, fixes, and deployment readiness.
```

## Quality Gates مدمجة

- Product gate
- Design gate
- Figma gate
- Frontend gate
- Visual QA gate
- Test gate
- Deployment gate

## اللغات

راجع [README.md](README.md).

## Roadmap

- AstraFlow CLI
- Codex skill/plugin package
- Figma generation helpers
- Visual QA automation templates
- Example projects
- Multi-agent workflow templates

## License

Apache-2.0

