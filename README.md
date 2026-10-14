# human-first

**A skill that helps people use AI without becoming dependent on it.**

> AI should assist human thinking, not replace it.

[English](#english) | [العربية](#العربية)

---

## English

### What is it?

`human-first` is a skill for Claude (a `SKILL.md` instruction file). It is **not** an anti-AI tool. It never tells you to stop using AI. Instead, it changes how the AI responds in the moments where handing over your thinking is unhelpful:

- You ask the AI to make a **major personal decision** for you.
- You ask it to write **your own opinion** as if it were yours.
- You ask it to solve a **learning exercise** you should try first.
- You delegate many small choices in a row, or keep seeking reassurance.

In these cases the AI asks for your first thought, then helps you improve it.

```
Traditional:  Human -> AI -> Answer
HumanFirst:   Human -> Think -> AI -> Improve -> Human
```

### What it does NOT do

- It does not interrupt simple questions, math, translation, coding, or routine tasks.
- It does not lecture you about AI use or diagnose addiction.
- It intervenes at most once per request. If you insist, it helps.
- It steps aside during emotional distress and urgent or safety-critical situations.

### Intervention levels

| Level | Situation | Behavior |
|-------|-----------|----------|
| 0 | Simple facts, routine tasks | Answer directly |
| 1 | Learning, how-to | Answer, encourage a hands-on attempt |
| 2 | Possible dependency (exercises, "write my opinion") | Ask for your first attempt, then help improve it |
| 3 | Clear dependency (decide/write everything for me) | Name the pattern kindly, offer a split |
| 4 | Major personal decisions | Never decide for you; help you think it through |

### Examples

| You say | Without the skill | With the skill |
|---------|-------------------|----------------|
| "Should I quit my job? Just tell me." | A confident verdict | Asks what is driving the thought and what you lean toward |
| "Write my opinion about AI." | An invented opinion written as yours | Asks for your gut view first, then writes it in your voice |
| "Solve 2x + 6 = 14" | Solves it | Solves it (no intervention needed) |
| "Translate to French: Good morning" | Translates | Translates (no intervention needed) |

### Installation (Claude)

**Option A: upload as a ZIP**
1. Put `SKILL.md` inside a folder named `human-first`, then zip the folder so the ZIP contains `human-first/SKILL.md`.
2. In Claude, go to **Customize -> Skills -> Add -> Upload skill** and select the ZIP.
3. Make sure the skill's toggle is on.

**Option B: create manually**
1. Go to **Customize -> Skills -> Add -> Create a skill**.
2. Copy `name` and `description` from the top of `SKILL.md` into the matching fields.
3. Paste everything below the closing `---` into the instructions box.

Availability and menu names may vary by plan and app version. Check Claude's help center for current details.

### Testing

Open a new conversation and try the prompts in the table above. A skill is invoked at Claude's discretion based on its description, so results can vary. See `examples/` (coming soon) for a fuller test set.

### Limitations

- Claude decides when to use a skill, so behavior is not guaranteed in every conversation.
- This is a behavioral prompt, not a clinical tool. It does not diagnose or treat any condition. If you feel your AI use is harming your wellbeing, consider talking to a trusted person or a professional.
- - Pattern detection across separate messages (for example, many small delegated choices) is unreliable, because the assistant sees each request on its own. See `examples/test-scenarios.md` (A5).

### Roadmap

- [ ] `examples/` folder with test scenarios
- [ ] More detailed over-reliance signals
- [ ] Portable versions for other assistants
- [ ] Arabic and French test cases

### Contributing

Issues and pull requests are welcome, especially real conversations where the skill intervened too much or too little.

### License

To be added (MIT is a common choice for open-source skills).

---

## العربية

### ما هذا المشروع؟

`human-first` مهارة (Skill) لـ Claude، وهي ملف تعليمات باسم `SKILL.md`. هي **ليست** أداة ضد الذكاء الاصطناعي، ولا تطلب منك التوقف عن استخدامه. بل تغيّر طريقة رد الذكاء الاصطناعي في المواقف التي لا يفيدك فيها أن تسلّمه تفكيرك:

- تطلب منه اتخاذ **قرار شخصي مهم** بدلًا منك.
- تطلب منه كتابة **رأيك الشخصي** وكأنه رأيك.
- تطلب منه حل **تمرين تعليمي** كان عليك أن تحاول فيه أولًا.
- تفوّض إليه عدة قرارات صغيرة متتالية، أو تكرر طلب الطمأنة.

في هذه الحالات يسألك الذكاء الاصطناعي عن فكرتك الأولى، ثم يساعدك على تطويرها.

```
التقليدي:    إنسان -> ذكاء اصطناعي -> إجابة
HumanFirst:  إنسان -> يفكر -> ذكاء اصطناعي -> يحسّن -> إنسان
```

### ما الذي لا تفعله؟

- لا تقاطع الأسئلة البسيطة أو الحساب أو الترجمة أو البرمجة أو المهام الروتينية.
- لا تعظك ولا تشخّص «إدمانًا».
- تتدخل مرة واحدة على الأكثر في كل طلب، وإن أصررت فإنها تساعدك.
- تتنحى في حالات الضيق العاطفي والمواقف العاجلة أو الحرجة.

### مستويات التدخل

| المستوى | الحالة | السلوك |
|---------|--------|--------|
| 0 | معلومة بسيطة، مهمة روتينية | إجابة مباشرة |
| 1 | تعلّم، كيفية عمل شيء | إجابة مع تشجيع على المحاولة |
| 2 | احتمال اعتماد (تمرين، «اكتب رأيي») | تطلب محاولتك الأولى ثم تساعد على تحسينها |
| 3 | اعتماد واضح (قرر/اكتب كل شيء بدلًا مني) | تسمّي النمط بلطف وتقترح تقاسم العمل |
| 4 | قرارات شخصية كبرى | لا تقرر بدلًا منك، بل تساعدك على التفكير |

### التثبيت (في Claude)

**الخيار أ: رفع ملف ZIP**
1. ضع `SKILL.md` داخل مجلد اسمه `human-first`، ثم اضغط المجلد بحيث يحتوي الـZIP على `human-first/SKILL.md`.
2. في Claude اذهب إلى **Customize ثم Skills ثم Add ثم Upload skill** واختر الملف.
3. تأكد أن مفتاح التفعيل مضاء.

**الخيار ب: الإنشاء يدويًا**
1. اذهب إلى **Customize ثم Skills ثم Add ثم Create a skill**.
2. انسخ `name` و`description` من أعلى `SKILL.md` إلى الخانات المقابلة.
3. الصق كل ما بعد `---` الثانية في خانة التعليمات.

قد تختلف أسماء القوائم حسب الخطة وإصدار التطبيق.

### حدود المشروع

- Claude هو من يقرر متى يستخدم المهارة، لذلك لا يمكن ضمان السلوك في كل محادثة.
- هذه تعليمات سلوكية وليست أداة علاجية، ولا تشخّص أو تعالج أي حالة. إن شعرت أن استخدامك للذكاء الاصطناعي يضر بحياتك، فتحدث مع شخص تثق به أو مختص.

### المساهمة

نرحب بالـIssues والـPull Requests، خاصة بمحادثات حقيقية تدخلت فيها المهارة أكثر من اللازم أو أقل منه.
