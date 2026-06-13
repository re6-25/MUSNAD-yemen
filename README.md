<div align="center">
  <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/c/cb/Musnad_Alef.svg/120px-Musnad_Alef.svg.png" alt="Musnad Logo" width="100" />
  <h1>🏛️ منصة مُسند للتراث اليمني | Musnad Platform</h1>
  
  <p><b>أرشيف رقمي ذكي لإحياء التراث اليمني العريق بقوة الذكاء الاصطناعي وهندسة البرمجيات الحديثة.</b></p>

  <!-- Badges -->
  <p>
    <img src="https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=green" alt="Django" />
    <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
    <img src="https://img.shields.io/badge/AI_OCR-Ultralytics-FF9900?style=for-the-badge&logo=opencv&logoColor=white" alt="AI OCR" />
    <img src="https://img.shields.io/badge/Docker-2CA5E0?style=for-the-badge&logo=docker&logoColor=white" alt="Docker" />
    <img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL" />
  </p>
</div>

<br>

## 🌟 عن المشروع (About The Project)

**منصة خط المسند** ليست مجرد موقع إلكتروني، بل هي **جسر تقني يربط بين حضارات اليمن القديمة وتكنولوجيا المستقبل**. 
تم بناء هذا النظام المعقد من الصفر ليكون المرجع الأول للباحثين والمهتمين بالنقوش اليمنية والممالك القديمة (سبأ، حمير، أوسان، قتبان، حضرموت، ومعين). 

يجمع المشروع بين **تطوير الويب المتقدم (Django)**، **الذكاء الاصطناعي (Computer Vision)**، و**البيئات السحابية (Docker)** لتقديم تجربة مستخدم لا مثيل لها، تتيح للزوار ترجمة النقوش والمساهمة في حفظ التاريخ.

---

## ✨ الخصائص التقنية والمميزات (Core Features)

### 🧠 1. الذكاء الاصطناعي وكاشف المسند (AI OCR Detection)
- نظام مدمج يعتمد على تقنيات الذكاء الاصطناعي للتعرف البصري على حروف المسند من الصور المرفوعة مباشرة.
- تحويل الصور إلى نصوص رقمية لتسهيل الترجمة والبحث.

### 👥 2. مجتمع المعرفة والترجمة التشاركية (Crowdsourced Translations)
- منصة تفاعلية تتيح للمستخدمين إضافة ترجماتهم للنقوش.
- نظام **تصويت (Voting)** و**مراجعة (Reviewing)** يعتمد على المجتمع لاختيار الترجمات الأدق.

### 🏆 3. نظام السمعة والمكافآت (Reputation System)
- نظام تحفيزي ذكي يمنح المستخدمين نقاطاً وشارات (Badges) عند الموافقة على مساهماتهم (نقوش أو ترجمات).
- لوحة تحكم (Dashboard) تبرز إنجازات الباحث وتصنيفه.

### 🎨 4. تجربة مستخدم مذهلة (UI/UX & HTMX)
- واجهات متجاوبة كلياً مبنية بلمسة تراثية أصيلة.
- تصفح ديناميكي بدون إعادة تحميل الصفحة بفضل تقنية **HTMX**.
- معرض صور (Masonry Grid) يستعرض تفاصيل النقوش بدقة عالية.

### 🐳 5. بيئة عمل معيارية (Dockerized Environment)
- المشروع مغلف بالكامل باستخدام Docker و Docker Compose لضمان استقرار الخوادم وسهولة التشغيل في بيئة الإنتاج أو التطوير بضغطة زر.

---

## 🛠️ التقنيات المستخدمة (Tech Stack)

| المجال | التقنيات |
| :--- | :--- |
| **الواجهة الخلفية (Backend)** | Django 5, Python 3.11, Django REST Framework |
| **الواجهة الأمامية (Frontend)** | HTML5, CSS3, Vanilla JS, Bootstrap 5 RTL, HTMX |
| **الذكاء الاصطناعي (AI/ML)** | PyTorch, Ultralytics YOLO, OpenCV |
| **قواعد البيانات (Database)** | PostgreSQL (Production), SQLite (Dev) |
| **النشر والتشغيل (DevOps)** | Docker, Docker Compose |



---

## 📂 هيكلية التطبيقات (Django Apps Architecture)

تم تقسيم المشروع إلى تطبيقات (Apps) مصغرة لضمان سهولة الصيانة وقابلية التوسع (Scalability):
- `core/`: الإعدادات الأساسية، والصلاحيات، والـ Middleware.
- `accounts/`: نظام المصادقة المخصص وإدارة الملفات الشخصية.
- `inscriptions/`: الأرشيف الأساسي للنقوش، الممالك، والمقاطعات.
- `translations/`: محرك الترجمة، التقييم، والتصويت.
- `community/`: إدارة التفاعل والمناقشات حول النقوش.
- `reputation/`: محرك النقاط والمكافآت للمستخدمين النشطين.
- `frontend/`: إدارة واجهات العرض (Views) والقوالب (Templates).

---

## 📸 جولة تفصيلية داخل المنصة (Platform Showcase)

تتميز المنصة بتصميم نهاري/ليلي متجاوب يعكس الأصالة اليمنية. إليك نظرة مفصلة على أبرز أقسام المنصة:

### 1️⃣ الواجهة الرئيسية والممالك القديمة (Home & Kingdoms)
بوابة الدخول للتاريخ اليمني، حيث تستعرض الواجهة الرئيسية إحصائيات النظام الحية (أكثر من 5800 نقش موثق). كما يتيح لك قسم الممالك القديمة استكشاف (سبأ، حمير، قتبان...) عبر بطاقات معلومات تفصيلية مبهرة.
<p align="center">
  <img src="screenshots/01_home.png" width="48%" alt="الواجهة الرئيسية" />
  <img src="screenshots/02_kingdoms.png" width="48%" alt="الممالك القديمة" />
</p>

### 2️⃣ مكتبة النقوش والمعرض التراثي (Inscriptions & Gallery)
أرشيف رقمي ضخم يسمح بالبحث المتقدم في النقوش، واستعراض تفاصيلها التاريخية مع إظهار النص الأصلي المحفور بخط المسند الذهبي، بالإضافة لمعرض صور شبكي انسيابي.
<p align="center">
  <img src="screenshots/03_inscriptions.png" width="48%" alt="مكتبة النقوش" />
  <img src="screenshots/04_gallery.png" width="48%" alt="المعرض التراثي" />
</p>

### 3️⃣ الذكاء الاصطناعي ورفع النقوش (AI OCR & Upload)
أداة متطورة تسمح للباحثين برفع صور لأي حجر أثري، ليقوم نظام الذكاء الاصطناعي بالتعرف البصري على الحروف المسندية وتحديد أماكنها بدقة (Bounding Boxes)، مع إمكانية مساهمة الباحث برفع وتوثيق نقوش جديدة.
<p align="center">
  <img src="screenshots/06_ocr.png" width="48%" alt="كاشف المسند (OCR)" />
  <img src="screenshots/05_upload.png" width="48%" alt="رفع نقش جديد" />
</p>

### 4️⃣ لوحة التحكم والملف الشخصي (Dashboard & Profile)
مساحة مخصصة لكل مستخدم وباحث تعرض إحصائياته الخاصة، مستواه، والنقوش التي ساهم في ترجمتها، مما يعزز نظام التفاعل الأكاديمي والسمعة داخل المنصة.
<p align="center">
  <img src="screenshots/07_dashboard.png" width="48%" alt="لوحة تحكم المستخدم" />
  <img src="screenshots/08_profile.png" width="48%" alt="الملف الشخصي" />
</p>

### 5️⃣ المفضلة وإعدادات الحساب (Favorites & Settings)
نظام مرن لحفظ النقوش للرجوع إليها سريعاً أثناء البحث العلمي، مع واجهة إعدادات شاملة تتيح للمستخدم تخصيص تجربته، إدارة الخصوصية، وتحديث بياناته.
<p align="center">
  <img src="screenshots/09_favorites.png" width="48%" alt="المفضلة والمحفوظات" />
  <img src="screenshots/10_settings.png" width="48%" alt="إعدادات الحساب" />
</p>

---

## 🤝 فريق العمل (The Team)
تم تصميم وتطوير المنصة كجهد أكاديمي هندسي مشترك:
- **تطوير وهندسة:** 
  - [ م. ريم الوعيل](https://github.com/re6-25)
  - [م. الزهراء الصباحي](https://github.com/zahraa-khalid2)
- **إشراف:** د. أكرم الصباري
- **مساعد مشرف:** [م. قسورة المحمدي](https://github.com/KASSWRH)

© 2026 جميع الحقوق محفوظة لـ منصة خط المسند.
