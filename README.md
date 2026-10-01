<div align="center">
  <h1> 🛡️ Valunix 🛡️ </h1>
  <p><b>AI-Powered Web Security & Penetration Testing Platform</b></p>
</div>

## Table of Contents

- [Project Overview](#project-overview)
- [Similar Projects](#similar-projects)
- [Free Tools](#free-tools)
- [Research Papers](#research-papers)
- [Tutorials](#tutorials)


## Project Overview

### 💡 ملخص الفكرة
المشروع عبارة عن منصة ذكية بتفحص أمان مواقع الويب وبتستخدم الذكاء الاصطناعي في اكتشاف الثغرات وتحليلها ومساعدة المطور يسدها. المنصة بتفحص الموقع من بره من غير ما تحتاج الكود، وبتعمل هجمات وهمية عشان تشوف فيه ثغرات ولا لأ. وكمان تقدر ترفع الـ Repository أو السورس كود بتاعك فتعدي على الملفات كلها وتفحصها بنفس الطريقة. بعد الفحص، المنصة بتقولك على كل ثغرة نوعها وخطورتها وبترتبهم من الأخطر للأقل خطورة، عشان تعرف تبدأ تسد منين. وفي المنصة شات AI تسأله فيشرحلك الثغرة دي خطورتها إيه، وتسدها إزاي، وتتفاداها بعد كده إزاي، ويديك كمان اقتراحات كود للحل من غير ما يعدل على الكود بتاعك.

### 🎯 الفيتشرز الأساسية (MVP)
* **فحص الموقع من بره (Web Pentest):** المنصة تفحص الموقع الشغّال من غير ما تحتاج الكود، وتعمل هجمات وهمية عشان تكتشف الثغرات.
* **فحص الكود المصدري:** المستخدم يرفع الـ Repository أو السورس كود، والمنصة تعدي على الملفات كلها وتحلل الثغرات بنفس الطريقة.
* **تصنيف الثغرات:** كل ثغرة يتحدد نوعها وخطورتها، وتتعرض مرتبة من الأخطر للأقل خطورة، عشان المطور يعرف يبدأ يسد منين.
* **شات AI للشرح والإرشاد:** المستخدم يسأل، والشات يشرحله الثغرة دي خطورتها إيه، وتتسد إزاي، وتتفادى بعد كده إزاي.
* **اقتراحات كود للإصلاح:** المنصة تديك كود مقترح لسد الثغرة، من غير ما تعدل على الكود بتاعك.

### 🚀 الفيتشرز المستقبلية
* **الإصلاح التلقائي:** المنصة تسد الثغرة بنفسها بعد ما تحلل الكود كله وتفهمه.
* **محرر أكواد مدمج بـ AI:** محرر جوه المنصة يراجع الكود وانت بتكتب وينبهك للثغرات في نفس اللحظة.
* **Validation قبل العرض:** تأكيد الثغرة قبل ما تظهر للمستخدم، وده يقلل الـ False Positives وهو أكبر شكوى في الأدوات دي.
* **Re-scan بعد الإصلاح:** يتأكد إن الثغرة اتسدت فعلاً.
* **ترتيب ذكي:** مش CVSS بس، ضيفوا EPSS وقائمة CISA KEV (الثغرات المستغلة فعلاً)، وسياق الموقع نفسه.
* **شرح بالعربي:** الأدوات دي كلها بالإنجليزي. شات يشرح بالعربي المصري ويناسب المبتدئين ميزة حقيقية.
* **تقرير PDF:** يتقدم للدكتور أو العميل.
* **GitHub Action / CI:** فحص تلقائي مع كل Pull Request.
* **Fix كـ Pull Request:** مش تعديل مباشر، والمستخدم يراجع ويوافق (ده أأمن وأحسن أكاديمياً).
* **Dashboard:** بتطور الأمان مع الوقت.
* **وضع تعليمي:** يشرح للطالب إزاي الهجوم بيتم على موقع تجريبي، وتوصيات OWASP Top 10.
* **LLM محلي (Ollama):** للي مش عايز يبعت الكود لأي API خارجي.

## Similar Projects

### 1. isitsecure

**GitHub:** https://github.com/jaurakunal/isitsecure  
**Website:** https://isitsecure.ai/

منصة مفتوحة المصدر لفحص أمان تطبيقات الويب، بتجمع بين `SAST` و`DAST` و`LLM Code Review` في عملية فحص واحدة. بتحلل الـ`Source Code`، وتفحص الـ`Web App` الشغال، وتستخدم نتائج تحليل الكود لتوجيه اختبارات على التطبيق، ثم تستخدم الـ`AI` لتحليل النتائج وتوليد حلول للإصلاح.

---

### 2. Shannon

**GitHub:** https://github.com/KeygraphHQ/shannon  
**Website:** https://keygraph.io/

أداة `AI Pentester` مستقلة لتطبيقات الويب والـ`APIs`. بتحلل الـ`Source Code` لاكتشاف مسارات الهجوم، وبعدها تستخدم `Browser Automation` وأدوات اختبار فعلية لمحاولة استغلال الثغرات. الـ`Finding` لا يظهر في التقرير إلا بعد وجود `Proof of Concept` قابل للتنفيذ، بهدف تقليل النتائج الوهمية.

---

### 3. Strix

**GitHub:** https://github.com/usestrix/strix  
**Website:** https://strix.ai/

منصة مفتوحة المصدر تعتمد على `AI Agents` لتنفيذ `Penetration Testing` بشكل مستقل. بتشغل التطبيق، وتعمل `Reconnaissance` واختبارات واستغلال، ثم تتحقق من الثغرات من خلال `Proof-of-Concepts` حقيقية، وتقدم نتائج قابلة للتنفيذ والإصلاح، مع إمكانية استخدامها داخل `CI/CD`.

---

### 4. WebPatcher

**GitHub:** https://github.com/OmarHassan-99/WebPatcher  
**Website:** Local / GitHub Project

منصة بتركز على الربط بين اكتشاف ثغرات الويب وإصلاحها. بتستخدم `DAST` لاكتشاف المشاكل، وبعدها `LLMs` عبر `LangChain` لتوليد `Security Patches` مناسبة للـ`Framework` والـ`Code`، ثم تعمل `Validation` للـ`Patch` للتأكد إنه عالج المشكلة من غير ما يكسر سلوك التطبيق.

---

### 5. Diana

**GitHub:** https://github.com/SageSalmon/Diana-Web-Scanner  
**Website:** Local / GitHub Project

`AI-powered Web Vulnerability Scanner` بيجمع تقنيات الـ`Web Scanning` التقليدية مع `LLM-driven Security Testing`. الـ`AI` بيستخدم لفهم الـ`Endpoints` والـ`Responses`، وتوليد `Payloads` مناسبة للسياق، واكتشاف `Attack Chains` والتحقق من النتائج بهدف تقليل الـ`False Positives`.

---

### 6. Argus

**GitHub:** https://github.com/Kentunji/argus  
**Website:** Local / GitHub Project

`Web Application Vulnerability Scanner` بيعمل `Crawling` وفحص للـ`Web App` بحثًا عن ثغرات زي `XSS` و`SQL Injection` ومشاكل الـ`Security Headers`. بعد كده بيستخدم `LLM` لتحليل النتائج وإعطاء `Confidence Rating` وشرح مبسط وحلول مناسبة للـ`Technology Stack`، مع تقارير `HTML` و`JSON`.

---

### 7. VulnIQ

**GitHub:** https://github.com/namanadep/vuln-iq  
**Website:** Local / GitHub Project

منصة `Security Assessment` بتجمع نتائج عدة أدوات Security في `Dashboard` واحدة، منها `CodeQL` و`Trivy` و`Gitleaks` و`OWASP ZAP` لفحص الـ`Source Code` والـ`Containers` والـ`Secrets` والـ`Web Applications`. وبتستخدم `GPT-4` لتحليل النتائج وعمل `Risk Scoring` وترتيب الـ`Vulnerabilities` وإنشاء تقارير `PDF`.

---

### 8. AutoSecScan

**GitHub:** https://github.com/jhammant/AutoSecScan  
**Website:** Local / GitHub Project

`Security Scanner` مفتوح المصدر وموجه للـ`Continuous Automated Pentesting`. بيجمع نتائج أدوات مختلفة لفحص الـ`Network` والـ`Hosts` والـ`Code` والـ`Dependencies` والـ`Secrets`، وبعدها يستخدم `LLM` لعمل `Triage` للنتائج، واكتشاف `False Positives`، وإعادة ترتيب الخطورة، وشرح المشاكل واقتراح حلول في تقرير موحد.

## Free Tools
List of free tools goes here...

## Research Papers
List of research papers goes here...

## Tutorials
List of tutorials goes here...
## Free Tools

List of free tools goes here...

## Research Papers

List of research papers goes here...

## Tutorials

List of tutorials goes here...
