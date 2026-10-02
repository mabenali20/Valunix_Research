<h1 align="center">🛡️ Valunix 🛡️</h1>

<p align="center"><b>AI-Powered Web Security & Penetration Testing Platform</b></p>

---

## Table of Contents

- [Project Overview](#project-overview)
- [Similar Projects](#similar-projects)
- [Free Tools](#free-tools)
- [Free AI Models](#free-ai-models)
- [Testing Environments](#testing-environments)
- [References](#references)

---

## Project Overview

<div dir="rtl">

### 💡 ملخص الفكرة

المشروع عبارة عن منصة ذكية بتفحص أمان مواقع الويب وبتستخدم الذكاء الاصطناعي في اكتشاف الثغرات وتحليلها ومساعدة المطور يسدها. المنصة بتفحص الموقع من بره من غير ما تحتاج الكود، وبتعمل هجمات وهمية عشان تشوف فيه ثغرات ولا لأ. وكمان تقدر ترفع الـ Repository أو السورس كود بتاعك فتعدي على الملفات كلها وتفحصها بنفس الطريقة. بعد الفحص، المنصة بتقولك على كل ثغرة نوعها وخطورتها وبترتبهم من الأخطر للأقل خطورة، عشان تعرف تبدأ تسد منين. وفي المنصة شات AI تسأله فيشرحلك الثغرة دي خطورتها إيه، وتسدها إزاي، وتتفاداها بعد كده إزاي، ويديك كمان اقتراحات كود للحل من غير ما يعدل على الكود بتاعك.

### 🎯 الفيتشرز الأساسية (MVP)

- **فحص الموقع من بره:** المنصة تفحص الموقع الشغّال من غير ما تحتاج الكود، وتعمل هجمات وهمية عشان تكتشف الثغرات.
- **فحص الكود المصدري:** المستخدم يرفع الـ Repository أو السورس كود، والمنصة تعدي على الملفات كلها وتحلل الثغرات بنفس الطريقة.
- **تصنيف الثغرات:** كل ثغرة يتحدد نوعها وخطورتها، وتتعرض مرتبة من الأخطر للأقل خطورة، عشان المطور يعرف يبدأ يسد منين.
- **شات AI للشرح والإرشاد:** المستخدم يسأل، والشات يشرحله الثغرة دي خطورتها إيه، وتتسد إزاي، وتتفادى بعد كده إزاي.
- **اقتراحات كود للإصلاح:** المنصة تديك كود مقترح لسد الثغرة، من غير ما تعدل على الكود بتاعك.

### 🚀 الفيتشرز المستقبلية

- **الإصلاح التلقائي:** المنصة تسد الثغرة بنفسها بعد ما تحلل الكود كله وتفهمه.
- **محرر أكواد مدمج بالذكاء الاصطناعي:** محرر جوه المنصة يراجع الكود وانت بتكتب وينبهك للثغرات في نفس اللحظة.
- **تأكيد الثغرة قبل العرض (Validation):** نتأكد من الثغرة قبل ما تظهر للمستخدم، وده يقلل الـ False Positives وهو أكبر شكوى في الأدوات دي.
- **إعادة الفحص بعد الإصلاح (Re-scan):** نتأكد إن الثغرة اتسدت فعلاً.
- **ترتيب ذكي:** مش CVSS بس، ضيفوا EPSS وقائمة CISA KEV (الثغرات المستغلة فعلاً)، وسياق الموقع نفسه.
- **شرح بالعربي:** الأدوات دي كلها بالإنجليزي. شات يشرح بالعربي المصري ويناسب المبتدئين ميزة حقيقية.
- **تقرير PDF:** يتقدم للدكتور أو العميل.
- **فحص تلقائي مع كل Pull Request:** عن طريق GitHub Action أو CI.
- **الإصلاح كـ Pull Request:** مش تعديل مباشر، والمستخدم يراجع ويوافق (ده أأمن وأحسن أكاديمياً).
- **لوحة متابعة (Dashboard):** بتوضح تطور الأمان مع الوقت.
- **وضع تعليمي:** يشرح للطالب إزاي الهجوم بيتم على موقع تجريبي، وتوصيات OWASP Top 10.
- **موديل محلي (Ollama):** للي مش عايز يبعت الكود لأي API خارجي.

</div>

---

## Similar Projects

<div dir="rtl">

اللينكات كلها اتراجعت يوم 2 أكتوبر 2026. أرقام النجوم والـ Commits بتتغير، فمتعتمدش عليها.

</div>

### 1. isitsecure

<div dir="ltr">

- **GitHub:** [jaurakunal/isitsecure](https://github.com/jaurakunal/isitsecure)
- **Website:** https://isitsecure.ai/
- **Stack:** Python · Apache-2.0
- **Architecture doc:** [docs/architecture.md](https://github.com/jaurakunal/isitsecure/blob/main/docs/architecture.md)

</div>

<div dir="rtl">

منصة مفتوحة المصدر لفحص أمان تطبيقات الويب، بتجمع بين SAST وDAST وLLM Code Review في عملية فحص واحدة. بتحلل الكود، وتفحص التطبيق الشغال، وتستخدم نتائج تحليل الكود لتوجيه اختبارات على التطبيق، ثم تستخدم الـ AI لتحليل النتائج وتوليد حلول للإصلاح.

**ملحوظة:**  الـ AI فيه بيشتغل بـ Anthropic أو Gemini API بس، وبتكلف فلوس على حسب حجم الفحص.
</div>

### 2. Shannon

<div dir="ltr">

- **GitHub:** [KeygraphHQ/shannon](https://github.com/KeygraphHQ/shannon)
- **Website:** [keygraph.io](https://keygraph.io/)
- **Stack:** TypeScript · AGPL-3.0 (Shannon Lite)

</div>

<div dir="rtl">

أداة AI Pentester مستقلة لتطبيقات الويب والـ APIs. بتحلل الكود لاكتشاف مسارات الهجوم، وبعدها تستخدم Browser Automation وأدوات اختبار فعلية لمحاولة استغلال الثغرات. الثغرة لا تظهر في التقرير إلا بعد وجود Proof of Concept قابل للتنفيذ، بهدف تقليل النتائج الوهمية.

**ملحوظة:** النسخة المجانية لازم تديها السورس كود مع لينك الموقع (White-box). وفيه نسخة تانية مدفوعة اسمها Shannon Pro.

</div>

### 3. Strix

<div dir="ltr">

- **GitHub:** [usestrix/strix](https://github.com/usestrix/strix)
- **Website:** [strix.ai](https://www.strix.ai/)

</div>

<div dir="rtl">

منصة مفتوحة المصدر تعتمد على AI Agents لتنفيذ Penetration Testing بشكل مستقل. بتشغل التطبيق، وتعمل Reconnaissance واختبارات واستغلال، ثم تتحقق من الثغرات من خلال Proof-of-Concepts حقيقية، وتقدم نتائج قابلة للتنفيذ والإصلاح، مع إمكانية استخدامها داخل CI/CD.

**ملحوظة:** ليها نسخة مفتوحة المصدر ونسخة تجارية مستضافة، وبتقدم إصلاح تلقائي على شكل Pull Request، وده قريب من فيتشر "الإصلاح كـ Pull Request" عندنا.

</div>

### 4. WebPatcher

<div dir="ltr">

- **GitHub:** [OmarHassan-99/WebPatcher](https://github.com/OmarHassan-99/WebPatcher)
- **Website:** Local / GitHub Project

</div>

<div dir="rtl">

منصة بتركز على الربط بين اكتشاف ثغرات الويب وإصلاحها. بتستخدم DAST لاكتشاف المشاكل، وبعدها LLMs عبر LangChain لتوليد Security Patches مناسبة للـ Framework والكود، ثم تعمل Validation للـ Patch للتأكد إنه عالج المشكلة من غير ما يكسر سلوك التطبيق.

</div>

### 5. Diana

<div dir="ltr">

- **GitHub:** [SageSalmon/Diana-Web-Scanner](https://github.com/SageSalmon/Diana-Web-Scanner)
- **Website:** Local / GitHub Project

</div>

<div dir="rtl">

أداة لفحص ثغرات تطبيقات الويب، بتجمع بين تقنيات الفحص التقليدية وتقنيات LLM-driven Security Testing.

الـ AI بيستخدم لفهم الـ Endpoints والـ Responses، وتوليد Payloads مناسبة للسياق، واكتشاف Attack Chains، بالإضافة إلى التحقق من النتائج بهدف تقليل الـ False Positives.

</div>

### 6. Argus

<div dir="ltr">

- **GitHub:** [Kentunji/argus](https://github.com/Kentunji/argus)
- **Website:** Local / GitHub Project

</div>

<div dir="rtl">

Web Application Vulnerability Scanner بيعمل Crawling وفحص للتطبيق بحثًا عن ثغرات زي XSS وSQL Injection ومشاكل الـ Security Headers.

بعد كده بيستخدم LLM لتحليل النتائج، وإعطاء Confidence Rating، وشرح مبسط للثغرات، واقتراح حلول مناسبة للـ Technology Stack، مع إمكانية إنشاء تقارير بصيغة HTML وJSON.

</div>

### 7. VulnIQ

<div dir="ltr">

- **GitHub:** [namanadep/vuln-iq](https://github.com/namanadep/vuln-iq)
- **Website:** Local / GitHub Project

</div>

<div dir="rtl">

منصة Security Assessment بتجمع نتائج عدة أدوات في Dashboard واحدة، منها CodeQL وTrivy وGitleaks وOWASP ZAP، لفحص الكود والـ Containers والـ Secrets وتطبيقات الويب.

المنصة بتستخدم GPT-4 لتحليل النتائج، وعمل Risk Scoring، وترتيب الثغرات حسب الخطورة، وإنشاء تقارير بصيغة PDF.

</div>

### 8. AutoSecScan

<div dir="ltr">

- **GitHub:** [jhammant/AutoSecScan](https://github.com/jhammant/AutoSecScan)
- **Website:** Local / GitHub Project

</div>

<div dir="rtl">

Security Scanner مفتوح المصدر وموجه للـ Continuous Automated Pentesting.

بيجمع نتائج أدوات مختلفة لفحص الـ Network والـ Hosts والكود والـ Dependencies والـ Secrets، وبعدها يستخدم LLM لعمل Triage للنتائج، واكتشاف False Positives، وإعادة ترتيب الخطورة، وشرح المشاكل واقتراح حلول في تقرير موحد.

</div>

### 🔍 إزاي نفهم الـ Architecture بتاعهم

<div dir="rtl">

افتح الـ Repo بتاع كل مشروع من دول (الأهم: isitsecure وShannon وStrix وWebPatcher وArgus) وجاوب على 3 أسئلة:

1. **مكتوب بإيه؟** (Python ولا TypeScript ولا غيره).
2. **بيشغل الأدوات إزاي؟** (ZAP وNuclei وغيرهم)، وبيبعت نتيجتها للـ AI إزاي؟
3. **الـ AI بيعمل إيه بالظبط؟** (بيحلل النتيجة؟ بيولد Payload؟ بيكتب إصلاح؟)

الإجابات هتلاقيها في الـ README وفولدر `docs` أو `architecture`، وكمان في هيكل الفولدرات.

</div>

---

## Free Tools

### Web Scanning — DAST

<div dir="ltr">

**OWASP ZAP** — [Website](https://www.zaproxy.org/) · [GitHub](https://github.com/zaproxy/zaproxy)

</div>
<div dir="rtl">

المحرك الأساسي للـ DAST في المشروع، لفحص تطبيق الويب وإخراج نتائج الفحص.

</div>

<div dir="ltr">

**Nuclei** — [Website](https://nuclei.projectdiscovery.io/) · [GitHub](https://github.com/projectdiscovery/nuclei)

</div>
<div dir="rtl">

فحص إضافي باستخدام قوالب (Templates) لاكتشاف الثغرات المعروفة.

</div>

<div dir="ltr">

**Wapiti** — [Website](https://wapiti-scanner.github.io/) · [GitHub](https://github.com/wapiti-scanner/wapiti)

</div>
<div dir="rtl">

أداة إضافية لفحص تطبيقات الويب ومقارنة النتائج والتحقق منها.

</div>

<div dir="ltr">

**Nikto** — [GitHub](https://github.com/sullo/nikto)

</div>
<div dir="rtl">

فحص خادم الويب وإعداداته. الصفحة القديمة `cirt.net/Nikto2` اتشالت، واللينك ده هو المصدر الحالي.

</div>

<div dir="ltr">

**OpenVAS / Greenbone** — [Website](https://www.greenbone.net/en/community-edition/)

</div>
<div dir="rtl">

فحص الأنظمة والشبكات، كخيار للتوسع مستقبلًا.

</div>

### Source Code — SAST

<div dir="ltr">

**Semgrep CE** — [Website](https://semgrep.dev/) · [GitHub](https://github.com/semgrep/semgrep)

</div>
<div dir="rtl">

تحليل الكود المصدري واكتشاف الثغرات الأمنية.

</div>

<div dir="ltr">

**CodeQL** — [Website](https://codeql.github.com/) · [GitHub](https://github.com/github/codeql)

</div>
<div dir="rtl">

تحليل متقدم للكود المصدري لاكتشاف المشاكل الأمنية.

</div>

<div dir="ltr">

**SonarQube Community** — [Website](https://www.sonarsource.com/products/sonarqube/)

</div>
<div dir="rtl">

تحليل جودة الكود والأمان.

</div>

<div dir="ltr">

**Bandit** — [GitHub](https://github.com/PyCQA/bandit)

</div>
<div dir="rtl">

تحليل أمان الكود الخاص بلغة Python.

</div>

<div dir="ltr">

**Brakeman** — [Website](https://brakemanscanner.org/)

</div>
<div dir="rtl">

تحليل أمان تطبيقات Ruby on Rails.

</div>

<div dir="ltr">

**gosec** — [GitHub](https://github.com/securego/gosec)

</div>
<div dir="rtl">

تحليل أمان الكود الخاص بلغة Go.

</div>

### Secrets & Dependencies

<div dir="ltr">

**Gitleaks** — [GitHub](https://github.com/gitleaks/gitleaks)

</div>
<div dir="rtl">

اكتشاف المفاتيح السرية وبيانات الدخول داخل الكود.

</div>

<div dir="ltr">

**Trivy** — [Website](https://trivy.dev/) · [GitHub](https://github.com/aquasecurity/trivy)

</div>
<div dir="rtl">

فحص المكتبات والحاويات والمفاتيح السرية.

</div>

<div dir="ltr">

**OSV.dev / OSV-Scanner** — [Website](https://osv.dev/) · [GitHub](https://github.com/google/osv-scanner)

</div>
<div dir="rtl">

فحص المكتبات ومقارنتها بقاعدة بيانات الثغرات.

</div>

### AI

<div dir="ltr">

**Ollama** — [Website](https://ollama.com/) · [GitHub](https://github.com/ollama/ollama)

</div>
<div dir="rtl">

تشغيل نماذج الذكاء الاصطناعي محليًا لتحليل نتائج الفحص والكود المصدري.

</div>

<div dir="ltr">

**Cloud AI APIs** — [Free AI Models](#free-ai-models)

</div>
<div dir="rtl">

استخدام نموذج جاهز لتحليل نتائج الفحص، وشرح الثغرات، واقتراح طرق الإصلاح. التفاصيل في قسم Free AI Models.

</div>

<div dir="ltr">

**LangGraph** — [GitHub](https://github.com/langchain-ai/langgraph)

</div>
<div dir="rtl">

بناء Agents بخطوات وقرارات، زي التأكد من الثغرة وإعادة الفحص.

</div>

### AI Security References

<div dir="ltr">

**PentestGPT** — [GitHub](https://github.com/GreyDGL/PentestGPT)

</div>
<div dir="rtl">

دراسة طريقة استخدام نماذج اللغة للمساعدة في عمليات اختبار الاختراق.

</div>

<div dir="ltr">

**Strix** — [GitHub](https://github.com/usestrix/strix)

</div>
<div dir="rtl">

دراسة دمج وكلاء الذكاء الاصطناعي مع أدوات الأمان والتحقق من الثغرات.

</div>

<div dir="ltr">

**CAI** — [GitHub](https://github.com/aliasrobotics/cai)

</div>
<div dir="rtl">

دراسة استخدام وكلاء الذكاء الاصطناعي في مهام الأمن السيبراني.

</div>

<div dir="ltr">

**PentAGI** — [GitHub](https://github.com/vxcontrol/pentagi)

</div>
<div dir="rtl">

دراسة استخدام عدة وكلاء ذكاء اصطناعي (Multi-Agent) في عمليات اختبار الأمان.

</div>

---

## Free AI Models

<div dir="rtl">

حدود الاستخدام المجاني بتتغير كتير. راجع الأرقام الحالية على موقع كل خدمة قبل ما نعتمد عليها في التنفيذ.

### 1. موديلات محلية (عن طريق Ollama)

مجانية تمامًا ومبتبعتش الكود لأي حد، بس محتاجة جهاز كويس (رام وكارت شاشة يفضل). أمثلة:

</div>

<div dir="ltr">

- **Qwen2.5-Coder**
- **DeepSeek-Coder**
- **Llama 3**

</div>

<div dir="rtl">

### 2. خدمات فيها استخدام مجاني

</div>

<div dir="ltr">

- **Google Gemini API** — [ai.google.dev](https://ai.google.dev/)
- **Groq** — [groq.com](https://groq.com/)
- **OpenRouter** — [openrouter.ai](https://openrouter.ai/) (has free models)
- **GitHub Models** — [github.com/marketplace/models](https://github.com/marketplace/models)

</div>

<div dir="rtl">

### 3. ملحوظة

بعض المشاريع المشابهة (زي isitsecure) بتشتغل بـ APIs مدفوعة. إحنا هنعتمد على الأنواع المجانية أو المحلية، وده بيدينا ميزة التكلفة وميزة الخصوصية.

</div>

---

## Testing Environments

<div dir="ltr">

**OWASP Juice Shop** — [Website](https://owasp.org/www-project-juice-shop/) · [GitHub](https://github.com/juice-shop/juice-shop)

</div>
<div dir="rtl">

بيئة قانونية لاختبار أداة الفحص الخاصة بنا.

</div>

<div dir="ltr">

**DVWA** — [GitHub](https://github.com/digininja/DVWA)

</div>
<div dir="rtl">

بيئة قانونية لاختبار اكتشاف الثغرات.

**تنبيه:** الفحص بيتعمل على مواقع التجربة دي أو على مواقع بإذن صاحبها بس. اختبار موقع من غير إذن ممنوع قانونيًا.

</div>

---

## References

<div dir="ltr">

- [OWASP Vulnerability Scanning Tools](https://community.owasp.org/Vulnerability_Scanning_Tools)
- [Pentest-Tools Website Scanner](https://pentest-tools.com/website-vulnerability-scanning/website-scanner)
- [PortSwigger — AI-Powered Scanner Vulnerabilities](https://portswigger.net/web-security/llm-attacks/ai-powered-scanner-vulnerabilities)

</div>

<div dir="rtl">

لينك PortSwigger بيشرح مخاطر الـ AI Scanners نفسها، زي Prompt Injection من محتوى الموقع المفحوص. مهم نحطه في بالنا وإحنا بنصمم الجزء الخاص بالـ AI.

</div>
