<div align="center">
  <h1> 🛡️ Valunix 🛡️ </h1>
  <p><b>AI-Powered Web Security & Penetration Testing Platform</b></p>
</div>

## Table of Contents

* [Project Overview](#project-overview)
* [Similar Projects](#similar-projects)
* [Free Tools](#free-tools)



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

منصة مفتوحة المصدر لفحص أمان تطبيقات الويب، بتجمع بين SAST وDAST وLLM Code Review في عملية فحص واحدة. بتحلل الـSource Code، وتفحص الـWeb App الشغال، وتستخدم نتائج تحليل الكود لتوجيه اختبارات على التطبيق، ثم تستخدم الـAI لتحليل النتائج وتوليد حلول للإصلاح.

### 2. Shannon

**GitHub:** https://github.com/KeygraphHQ/shannon
**Website:** https://keygraph.io/

أداة AI Pentester مستقلة لتطبيقات الويب والـAPIs. بتحلل الـSource Code لاكتشاف مسارات الهجوم، وبعدها تستخدم Browser Automation وأدوات اختبار فعلية لمحاولة استغلال الثغرات. الـFinding لا يظهر في التقرير إلا بعد وجود Proof of Concept قابل للتنفيذ، بهدف تقليل النتائج الوهمية.

### 3. Strix

**GitHub:** https://github.com/usestrix/strix
**Website:** https://strix.ai/

منصة مفتوحة المصدر تعتمد على AI Agents لتنفيذ Penetration Testing بشكل مستقل. بتشغل التطبيق، وتعمل Reconnaissance واختبارات واستغلال، ثم تتحقق من الثغرات من خلال Proof-of-Concepts حقيقية، وتقدم نتائج قابلة للتنفيذ والإصلاح، مع إمكانية استخدامها داخل CI/CD.

### 4. WebPatcher

**GitHub:** https://github.com/OmarHassan-99/WebPatcher
**Website:** Local / GitHub Project

منصة بتركز على الربط بين اكتشاف ثغرات الويب وإصلاحها. بتستخدم DAST لاكتشاف المشاكل، وبعدها LLMs عبر LangChain لتوليد Security Patches مناسبة للـFramework والـCode، ثم تعمل Validation للـPatch للتأكد إنه عالج المشكلة من غير ما يكسر سلوك التطبيق.

### 5. Diana

**GitHub:** https://github.com/SageSalmon/Diana-Web-Scanner
**Website:** Local / GitHub Project

المشروع عبارة عن أداة لفحص ثغرات تطبيقات الويب، وبيجمع بين تقنيات فحص الويب التقليدية وتقنيات LLM-driven Security Testing.

الـAI بيستخدم لفهم الـEndpoints والـResponses، وتوليد Payloads مناسبة للسياق، واكتشاف Attack Chains، بالإضافة إلى التحقق من النتائج بهدف تقليل الـFalse Positives.

### 6. Argus

**GitHub:** https://github.com/Kentunji/argus
**Website:** Local / GitHub Project

المشروع عبارة عن Web Application Vulnerability Scanner بيعمل Crawling وفحص للـWeb App بحثًا عن ثغرات زي XSS وSQL Injection ومشاكل الـSecurity Headers.

بعد كده بيستخدم LLM لتحليل النتائج، وإعطاء Confidence Rating، وشرح مبسط للثغرات، واقتراح حلول مناسبة للـTechnology Stack، مع إمكانية إنشاء تقارير بصيغ HTML وJSON.

### 7. VulnIQ

**GitHub:** https://github.com/namanadep/vuln-iq
**Website:** Local / GitHub Project

المشروع عبارة عن منصة Security Assessment بتجمع نتائج عدة أدوات Security في Dashboard واحدة، منها CodeQL وTrivy وGitleaks وOWASP ZAP لفحص الـSource Code والـContainers والـSecrets والـWeb Applications.

المنصة بتستخدم GPT-4 لتحليل النتائج، وعمل Risk Scoring، وترتيب الـVulnerabilities حسب الخطورة، وإنشاء تقارير بصيغة PDF.

### 8. AutoSecScan

**GitHub:** https://github.com/jhammant/AutoSecScan
**Website:** Local / GitHub Project

المشروع عبارة عن Security Scanner مفتوح المصدر وموجه للـContinuous Automated Pentesting.

بيجمع نتائج أدوات مختلفة لفحص الـNetwork والـHosts والـCode والـDependencies والـSecrets، وبعدها يستخدم LLM لعمل Triage للنتائج، واكتشاف False Positives، وإعادة ترتيب الخطورة، وشرح المشاكل واقتراح حلول في تقرير موحد.

## Free Tools

### Web Scanning — DAST

* **OWASP ZAP**
  https://www.zaproxy.org/
  **الاستخدام:** المحرك الأساسي للـDAST في المشروع، يفحص الـWeb App ويطلع الـFindings.

* **Nuclei**
  https://nuclei.projectdiscovery.io/
  **الاستخدام:** فحص إضافي بالـTemplates لاكتشاف Vulnerabilities معروفة.

* **Wapiti**
  https://wapiti-scanner.github.io/
  **الاستخدام:** Web Vulnerability Scanner إضافي للمقارنة والتحقق.

* **Nikto**
  https://cirt.net/Nikto2
  **الاستخدام:** فحص الـWeb Server والـConfiguration.

* **OpenVAS / Greenbone**
  https://www.greenbone.net/en/community-edition/
  **الاستخدام:** فحص الـSystems والـNetworks، كخيار للتوسع مستقبلًا.

### Source Code — SAST

* **Semgrep CE**
  https://semgrep.dev/
  **الاستخدام:** فحص الـSource Code واكتشاف Vulnerabilities.

* **CodeQL**
  https://codeql.github.com/
  **الاستخدام:** SAST متقدم لتحليل الـSource Code.

* **SonarQube Community**
  https://www.sonarsource.com/products/sonarqube/
  **الاستخدام:** Code Quality + Security Analysis.

* **Bandit**
  https://github.com/PyCQA/bandit
  **الاستخدام:** Security Analysis للـPython.

* **Brakeman**
  https://brakemanscanner.org/
  **الاستخدام:** Security Analysis لـRuby on Rails.

* **gosec**
  https://github.com/securego/gosec
  **الاستخدام:** Security Analysis للـGo.

### Secrets & Dependencies

* **Gitleaks**
  https://github.com/gitleaks/gitleaks
  **الاستخدام:** اكتشاف Secrets وCredentials داخل الـCode.

* **Trivy**
  https://trivy.dev/
  **الاستخدام:** فحص Dependencies وContainers وSecrets.

* **OSV.dev / OSV-Scanner**
  https://osv.dev/
  https://github.com/google/osv-scanner
  **الاستخدام:** فحص الـDependencies ومقارنتها بقاعدة Vulnerabilities.

### AI

* **Ollama**
  https://ollama.com/
  **الاستخدام:** تشغيل Local LLM لتحليل الـFindings والـSource Code.

* **Cloud AI APIs**
  **الاستخدام:** استخدام LLM جاهز لتحليل الـFindings، شرح الـVulnerabilities، واقتراح الـRemediation.

### AI Security References

* **PentestGPT**
  https://github.com/GreyDGL/PentestGPT
  **الاستخدام:** دراسة طريقة استخدام LLM في عمليات الـPentesting.

* **Strix**
  https://github.com/usestrix/strix
  **الاستخدام:** دراسة دمج AI Agents مع أدوات الـSecurity والـVulnerability Validation.

* **CAI**
  https://github.com/aliasrobotics/cai
  **الاستخدام:** دراسة استخدام AI Agents في Cybersecurity.

* **PentAGI**
  https://github.com/vxcontrol/pentagi
  **الاستخدام:** دراسة الـMulti-Agent Security Testing.

### Testing Environments

* **OWASP Juice Shop**
  https://owasp.org/www-project-juice-shop/
  **الاستخدام:** بيئة قانونية لاختبار الـScanner.

* **DVWA**
  https://github.com/digininja/DVWA
  **الاستخدام:** بيئة قانونية لاختبار Vulnerability Detection.

### References

* **OWASP Vulnerability Scanning Tools**
  https://community.owasp.org/Vulnerability_Scanning_Tools

* **Pentest-Tools Website Scanner**
  https://pentest-tools.com/website-vulnerability-scanning/website-scanner

* **PortSwigger — AI-Powered Scanner Vulnerabilities**
  https://portswigger.net/web-security/llm-attacks/ai-powered-scanner-vulnerabilities



