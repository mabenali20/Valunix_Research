<h1 align="center">🛡️ Valunix 🛡️</h1>

<p align="center"><b>AI-Powered Web Security & Penetration Testing Platform</b></p>

---

## Table of Contents

- [Project Overview](#project-overview)
- [Similar Projects](#similar-projects)
- [How We Can Build It](#how-we-can-build-it)
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

- **فحص الموقع من بره (Web Pentest):** المنصة تفحص الموقع الشغّال من غير ما تحتاج الكود، وتعمل هجمات وهمية عشان تكتشف الثغرات.
- **فحص الكود المصدري:** المستخدم يرفع الـ Repository أو السورس كود، والمنصة تعدي على الملفات كلها وتحلل الثغرات بنفس الطريقة.
- **تصنيف الثغرات:** كل ثغرة يتحدد نوعها وخطورتها، وتتعرض مرتبة من الأخطر للأقل خطورة، عشان المطور يعرف يبدأ يسد منين.
- **شات AI للشرح والإرشاد:** المستخدم يسأل، والشات يشرحله الثغرة دي خطورتها إيه، وتتسد إزاي، وتتفادى بعد كده إزاي.
- **اقتراحات كود للإصلاح:** المنصة تديك كود مقترح لسد الثغرة، من غير ما تعدل على الكود بتاعك.

### 🚀 الفيتشرز المستقبلية

- **الإصلاح التلقائي:** المنصة تسد الثغرة بنفسها بعد ما تحلل الكود كله وتفهمه.
- **محرر أكواد مدمج بـ AI:** محرر جوه المنصة يراجع الكود وانت بتكتب وينبهك للثغرات في نفس اللحظة.
- **Validation قبل العرض:** تأكيد الثغرة قبل ما تظهر للمستخدم، وده يقلل الـ False Positives وهو أكبر شكوى في الأدوات دي.
- **Re-scan بعد الإصلاح:** يتأكد إن الثغرة اتسدت فعلاً.
- **ترتيب ذكي:** مش CVSS بس، ضيفوا EPSS وقائمة CISA KEV (الثغرات المستغلة فعلاً)، وسياق الموقع نفسه.
- **شرح بالعربي:** الأدوات دي كلها بالإنجليزي. شات يشرح بالعربي المصري ويناسب المبتدئين ميزة حقيقية.
- **تقرير PDF:** يتقدم للدكتور أو العميل.
- **GitHub Action / CI:** فحص تلقائي مع كل Pull Request.
- **Fix كـ Pull Request:** مش تعديل مباشر، والمستخدم يراجع ويوافق (ده أأمن وأحسن أكاديمياً).
- **Dashboard:** بتطور الأمان مع الوقت.
- **وضع تعليمي:** يشرح للطالب إزاي الهجوم بيتم على موقع تجريبي، وتوصيات OWASP Top 10.
- **LLM محلي (Ollama):** للي مش عايز يبعت الكود لأي API خارجي.

</div>

---

## Similar Projects

<div dir="rtl">

> اللينكات كلها اتراجعت يوم 2 أكتوبر 2026. أرقام الـ Stars والـ Commits بتتغير، فمتعتمدش عليها.

</div>

### 1. isitsecure

<div dir="rtl">

- **GitHub:** [jaurakunal/isitsecure](https://github.com/jaurakunal/isitsecure)
- **Website:** مفيش موقع رسمي للمشروع. الدومين `isitsecure.ai` بيفتح منتج تاني مالوش علاقة بالمشروع ده، فاتشال من هنا.
- **التقنيات:** Python، والـ License هو Apache-2.0.

منصة مفتوحة المصدر لفحص أمان تطبيقات الويب، بتجمع بين SAST وDAST وLLM Code Review في عملية فحص واحدة. بتحلل الـ Source Code، وتفحص الـ Web App الشغال، وتستخدم نتائج تحليل الكود لتوجيه اختبارات على التطبيق، ثم تستخدم الـ AI لتحليل النتائج وتوليد حلول للإصلاح.

**ملحوظة مهمة:** الـ LLM فيها بيشتغل بـ Anthropic أو Gemini API بس، وبتكلف فلوس على حسب حجم الفحص. أحسن مرجع للـ Architecture عندنا: [docs/architecture.md](https://github.com/jaurakunal/isitsecure/blob/main/docs/architecture.md).

</div>

### 2. Shannon

<div dir="rtl">

- **GitHub:** [KeygraphHQ/shannon](https://github.com/KeygraphHQ/shannon)
- **Website:** [keygraph.io](https://keygraph.io/)
- **التقنيات:** TypeScript، والنسخة المجانية (Shannon Lite) الـ License بتاعها AGPL-3.0.

أداة AI Pentester مستقلة لتطبيقات الويب والـ APIs. بتحلل الـ Source Code لاكتشاف مسارات الهجوم، وبعدها تستخدم Browser Automation وأدوات اختبار فعلية لمحاولة استغلال الثغرات. الـ Finding لا يظهر في التقرير إلا بعد وجود Proof of Concept قابل للتنفيذ، بهدف تقليل النتائج الوهمية.

**ملحوظة مهمة:** النسخة المجانية White-box، يعني لازم تديها السورس كود مع لينك الموقع. وفيه نسخة تانية مدفوعة (Shannon Pro) فيها SAST وSCA وSecrets.

</div>

### 3. Strix

<div dir="rtl">

- **GitHub:** [usestrix/strix](https://github.com/usestrix/strix)
- **Website:** [strix.ai](https://www.strix.ai/)

منصة مفتوحة المصدر تعتمد على AI Agents لتنفيذ Penetration Testing بشكل مستقل. بتشغل التطبيق، وتعمل Reconnaissance واختبارات واستغلال، ثم تتحقق من الثغرات من خلال Proof-of-Concepts حقيقية، وتقدم نتائج قابلة للتنفيذ والإصلاح، مع إمكانية استخدامها داخل CI/CD.

**ملحوظة مهمة:** ليها نسخة Open Source ونسخة تجارية مستضافة، وبتقدم Auto-Fix على شكل Pull Request، وده قريب من فيتشر "Fix كـ Pull Request" عندنا.

</div>

### 4. WebPatcher

<div dir="rtl">

- **GitHub:** [OmarHassan-99/WebPatcher](https://github.com/OmarHassan-99/WebPatcher)
- **Website:** Local / GitHub Project

منصة بتركز على الربط بين اكتشاف ثغرات الويب وإصلاحها. بتستخدم DAST لاكتشاف المشاكل، وبعدها LLMs عبر LangChain لتوليد Security Patches مناسبة للـ Framework والـ Code، ثم تعمل Validation للـ Patch للتأكد إنه عالج المشكلة من غير ما يكسر سلوك التطبيق.

</div>

### 5. Diana

<div dir="rtl">

- **GitHub:** [SageSalmon/Diana-Web-Scanner](https://github.com/SageSalmon/Diana-Web-Scanner)
- **Website:** Local / GitHub Project

المشروع عبارة عن أداة لفحص ثغرات تطبيقات الويب، وبيجمع بين تقنيات فحص الويب التقليدية وتقنيات LLM-driven Security Testing.

الـ AI بيستخدم لفهم الـ Endpoints والـ Responses، وتوليد Payloads مناسبة للسياق، واكتشاف Attack Chains، بالإضافة إلى التحقق من النتائج بهدف تقليل الـ False Positives.

</div>

### 6. Argus

<div dir="rtl">

- **GitHub:** [Kentunji/argus](https://github.com/Kentunji/argus)
- **Website:** Local / GitHub Project

المشروع عبارة عن Web Application Vulnerability Scanner بيعمل Crawling وفحص للـ Web App بحثًا عن ثغرات زي XSS وSQL Injection ومشاكل الـ Security Headers.

بعد كده بيستخدم LLM لتحليل النتائج، وإعطاء Confidence Rating، وشرح مبسط للثغرات، واقتراح حلول مناسبة للـ Technology Stack، مع إمكانية إنشاء تقارير بصيغ HTML وJSON.

</div>

### 7. VulnIQ

<div dir="rtl">

- **GitHub:** [namanadep/vuln-iq](https://github.com/namanadep/vuln-iq)
- **Website:** Local / GitHub Project

المشروع عبارة عن منصة Security Assessment بتجمع نتائج عدة أدوات Security في Dashboard واحدة، منها CodeQL وTrivy وGitleaks وOWASP ZAP لفحص الـ Source Code والـ Containers والـ Secrets والـ Web Applications.

المنصة بتستخدم GPT-4 لتحليل النتائج، وعمل Risk Scoring، وترتيب الـ Vulnerabilities حسب الخطورة، وإنشاء تقارير بصيغة PDF.

</div>

### 8. AutoSecScan

<div dir="rtl">

- **GitHub:** [jhammant/AutoSecScan](https://github.com/jhammant/AutoSecScan)
- **Website:** Local / GitHub Project

المشروع عبارة عن Security Scanner مفتوح المصدر وموجه للـ Continuous Automated Pentesting.

بيجمع نتائج أدوات مختلفة لفحص الـ Network والـ Hosts والـ Code والـ Dependencies والـ Secrets، وبعدها يستخدم LLM لعمل Triage للنتائج، واكتشاف False Positives، وإعادة ترتيب الخطورة، وشرح المشاكل واقتراح حلول في تقرير موحد.

</div>

### 🔍 إزاي نفهم الـ Architecture بتاعهم

<div dir="rtl">

افتح الـ Repo بتاع كل مشروع من دول (الأهم: isitsecure وShannon وStrix وWebPatcher وArgus) وجاوب على 3 أسئلة:

1. **مكتوب بإيه؟** (Python ولا TypeScript ولا غيره).
2. **بيشغل الأدوات إزاي؟** (ZAP وNuclei وغيرهم) وبيبعت نتيجتها للـ AI إزاي؟
3. **الـ AI بيعمل إيه بالظبط؟** (بيحلل النتيجة؟ بيولد Payload؟ بيكتب Fix؟)

الإجابات هتلاقيها في الـ README وفولدر `docs` أو `architecture`، وكمان في هيكل الفولدرات.

</div>

---

## How We Can Build It

<div dir="rtl">

الفكرة إننا **مش بنكتب Scanner من الصفر**. إحنا بنربط أدوات جاهزة ومجانية، وبنحط الـ AI فوقها عشان يحلل النتائج ويشرحها ويقترح الحل.

### الـ Architecture المبسط

</div>

<div dir="ltr">

```
Target (URL / Repo)
        |
        v
+-----------------------------+
|  Backend (Orchestrator)     |
+-----------------------------+
        |
        +--> DAST tools   : ZAP, Nuclei, Wapiti, Nikto
        +--> SAST tools   : Semgrep, Bandit, CodeQL
        +--> Secrets/Deps : Gitleaks, Trivy, OSV-Scanner
        |
        v
  Raw results (JSON)
        |
        v
+-----------------------------+
|  Normalizer + Ranking       |  (one format, sort by severity)
+-----------------------------+
        |
        v
+-----------------------------+
|  LLM (Ollama / Cloud API)   |  (explain, triage, suggest fix)
+-----------------------------+
        |
        v
  Frontend (Report + AI Chat)
```

</div>

<div dir="rtl">

### الأدوات بتتشغل إزاي وبتطلع إيه

| الأداة | بتتشغل إزاي | الناتج |
|---|---|---|
| OWASP ZAP | REST API أو Docker | JSON / HTML / XML |
| Nuclei | CLI | JSON |
| Wapiti | CLI | JSON / HTML |
| Nikto | CLI | JSON / HTML |
| Semgrep | CLI | JSON |
| Bandit | CLI | JSON |
| Gitleaks | CLI | JSON |
| Trivy | CLI | JSON |
| OSV-Scanner | CLI | JSON |
| Ollama | REST API على الجهاز | نص (Response من الموديل) |

### خطوات الربط

1. الـ Backend يشغل الأداة المناسبة حسب نوع الفحص (موقع شغال ولا كود).
2. يجمع النتايج JSON ويوحدها في شكل واحد (النوع، الخطورة، المكان، الوصف).
3. يرتبها من الأخطر للأقل.
4. يبعت كل ثغرة للـ LLM عشان يشرحها ويقترح حل، والشات يرد على أسئلة المستخدم.
5. الـ Frontend يعرض التقرير والشات.

### أطر لربط الـ AI بالأدوات

- **LangChain:** لو محتاجين نربط الموديل بخطوات وأدوات بسيطة، وWebPatcher بيستخدمه.
- **LangGraph:** لو عايزين Agents بتاخد قرارات على خطوات (زي Validation وRe-scan).
- **PentestGPT** (موجود تحت في AI Security References): مثال كويس لفكرة استخدام LLM في الـ Pentesting.

</div>

---

## Free Tools

### Web Scanning — DAST

<div dir="rtl">

- **OWASP ZAP:** [zaproxy.org](https://www.zaproxy.org/) | [GitHub](https://github.com/zaproxy/zaproxy)
  - الاستخدام: المحرك الأساسي للـ DAST في المشروع، لفحص تطبيق الويب وإخراج نتائج الفحص.
- **Nuclei:** [nuclei.projectdiscovery.io](https://nuclei.projectdiscovery.io/) | [GitHub](https://github.com/projectdiscovery/nuclei)
  - الاستخدام: فحص إضافي باستخدام قوالب (Templates) لاكتشاف الثغرات المعروفة.
- **Wapiti:** [wapiti-scanner.github.io](https://wapiti-scanner.github.io/) | [GitHub](https://github.com/wapiti-scanner/wapiti)
  - الاستخدام: أداة إضافية لفحص تطبيقات الويب ومقارنة النتائج والتحقق منها.
- **Nikto:** [GitHub](https://github.com/sullo/nikto)
  - الاستخدام: فحص خادم الويب وإعداداته (Web Server & Configuration).
  - ملحوظة: الصفحة القديمة `cirt.net/Nikto2` اتشالت، واللينك ده هو المصدر الحالي.
- **OpenVAS / Greenbone:** [greenbone.net](https://www.greenbone.net/en/community-edition/)
  - الاستخدام: فحص الأنظمة والشبكات (Systems & Networks)، كخيار للتوسع مستقبلًا.

</div>

### Source Code — SAST

<div dir="rtl">

- **Semgrep CE:** [semgrep.dev](https://semgrep.dev/) | [GitHub](https://github.com/semgrep/semgrep)
  - الاستخدام: تحليل الكود المصدري (Source Code) واكتشاف الثغرات الأمنية.
- **CodeQL:** [codeql.github.com](https://codeql.github.com/) | [GitHub](https://github.com/github/codeql)
  - الاستخدام: تحليل متقدم للكود المصدري (SAST) لاكتشاف المشاكل الأمنية.
- **SonarQube Community:** [sonarsource.com](https://www.sonarsource.com/products/sonarqube/)
  - الاستخدام: تحليل جودة الكود والأمان (Code Quality & Security).
- **Bandit:** [GitHub](https://github.com/PyCQA/bandit)
  - الاستخدام: تحليل أمان الكود الخاص بلغة Python.
- **Brakeman:** [brakemanscanner.org](https://brakemanscanner.org/)
  - الاستخدام: تحليل أمان تطبيقات Ruby on Rails.
- **gosec:** [GitHub](https://github.com/securego/gosec)
  - الاستخدام: تحليل أمان الكود الخاص بلغة Go.

</div>

### Secrets & Dependencies

<div dir="rtl">

- **Gitleaks:** [GitHub](https://github.com/gitleaks/gitleaks)
  - الاستخدام: اكتشاف المفاتيح السرية وبيانات الدخول (Secrets & Credentials) داخل الكود.
- **Trivy:** [trivy.dev](https://trivy.dev/) | [GitHub](https://github.com/aquasecurity/trivy)
  - الاستخدام: فحص المكتبات (Dependencies) والحاويات (Containers) والمفاتيح السرية (Secrets).
- **OSV.dev / OSV-Scanner:** [osv.dev](https://osv.dev/) | [GitHub](https://github.com/google/osv-scanner)
  - الاستخدام: فحص المكتبات (Dependencies) ومقارنتها بقاعدة بيانات الثغرات.

</div>

### AI

<div dir="rtl">

- **Ollama:** [ollama.com](https://ollama.com/) | [GitHub](https://github.com/ollama/ollama)
  - الاستخدام: تشغيل نماذج الذكاء الاصطناعي محليًا (Local LLM) لتحليل نتائج الفحص والكود المصدري.
- **Cloud AI APIs:**
  - الاستخدام: استخدام نموذج ذكاء اصطناعي جاهز لتحليل نتائج الفحص، وشرح الثغرات، واقتراح طرق الإصلاح. التفاصيل في قسم [Free AI Models](#free-ai-models).
- **LangGraph:** [GitHub](https://github.com/langchain-ai/langgraph)
  - الاستخدام: بناء Agents بخطوات وقرارات (زي Validation وRe-scan).

</div>

### AI Security References

<div dir="rtl">

- **PentestGPT:** [GitHub](https://github.com/GreyDGL/PentestGPT)
  - الاستخدام: دراسة طريقة استخدام نماذج اللغة (LLM) للمساعدة في عمليات اختبار الاختراق.
- **Strix:** [GitHub](https://github.com/usestrix/strix)
  - الاستخدام: دراسة دمج وكلاء الذكاء الاصطناعي (AI Agents) مع أدوات الـ Security والتحقق من الثغرات.
- **CAI:** [GitHub](https://github.com/aliasrobotics/cai)
  - الاستخدام: دراسة استخدام وكلاء الذكاء الاصطناعي (AI Agents) في مهام الأمن السيبراني.
- **PentAGI:** [GitHub](https://github.com/vxcontrol/pentagi)
  - الاستخدام: دراسة استخدام عدة وكلاء ذكاء اصطناعي (Multi-Agent) في عمليات اختبار الأمان.

</div>

---

## Free AI Models

<div dir="rtl">

> حدود الاستخدام المجاني (Free Tier) بتتغير كتير. راجع الأرقام الحالية على موقع كل خدمة قبل ما نعتمد عليها في التنفيذ.

### 1. موديلات محلية (عن طريق Ollama)

مجانية تمامًا ومبتبعتش الكود لأي حد، بس محتاجة جهاز كويس (RAM وكارت شاشة يفضل).

- **Qwen2.5-Coder:** قوي في فهم الكود.
- **DeepSeek-Coder:** موديل مخصص للكود.
- **Llama 3:** موديل عام كويس في الشرح.

### 2. APIs فيها Free Tier

- **Google Gemini API:** [ai.google.dev](https://ai.google.dev/)
- **Groq:** [groq.com](https://groq.com/)
- **OpenRouter:** [openrouter.ai](https://openrouter.ai/) (فيه موديلات مجانية)
- **GitHub Models:** [github.com/marketplace/models](https://github.com/marketplace/models)

### 3. ملحوظة على المشاريع المشابهة

بعض المشاريع اللي فوق (زي isitsecure) بتشتغل بـ APIs مدفوعة. إحنا هنعتمد على الأنواع المجانية أو المحلية، وده بيدينا ميزة التكلفة وميزة الخصوصية.

</div>

---

## Testing Environments

<div dir="rtl">

- **OWASP Juice Shop:** [owasp.org](https://owasp.org/www-project-juice-shop/) | [GitHub](https://github.com/juice-shop/juice-shop)
  - الاستخدام: بيئة قانونية لاختبار أداة الفحص الخاصة بنا.
- **DVWA:** [GitHub](https://github.com/digininja/DVWA)
  - الاستخدام: بيئة قانونية لاختبار اكتشاف الثغرات.

> **تنبيه:** الفحص بيتعمل على مواقع التجربة دي أو على مواقع بإذن صاحبها بس. اختبار موقع من غير إذن ممنوع قانونيًا.

</div>

---

## References

<div dir="rtl">

- **OWASP Vulnerability Scanning Tools:** [community.owasp.org](https://community.owasp.org/Vulnerability_Scanning_Tools)
- **Pentest-Tools Website Scanner:** [pentest-tools.com](https://pentest-tools.com/website-vulnerability-scanning/website-scanner)
- **PortSwigger — AI-Powered Scanner Vulnerabilities:** [portswigger.net](https://portswigger.net/web-security/llm-attacks/ai-powered-scanner-vulnerabilities)
  - ملحوظة: بتشرح مخاطر الـ AI Scanners نفسها، زي Prompt Injection من محتوى الموقع المفحوص. مهم نحطه في بالنا وإحنا بنصمم الـ AI.

</div>
