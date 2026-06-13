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

## 🚀 كيفية التشغيل (Installation & Setup)

هناك طريقتان لتشغيل المشروع على جهازك: باستخدام **Docker** (الطريقة الأسهل والأسرع) أو بالطريقة التقليدية.

### الطريقة الأولى: باستخدام Docker (مُوصى بها)
تأكد من تثبيت وتشغيل [Docker Desktop](https://www.docker.com/products/docker-desktop).
```bash
git clone https://github.com/re6-25/MUSNAD-yemen.git
cd MUSNAD-yemen
docker-compose up --build -d
```
سيتم بناء البيئة بالكامل، وتشغيل قاعدة البيانات، وسيكون الموقع متاحاً على الرابط: `http://localhost:8000`

### الطريقة الثانية: التشغيل اليدوي (Local Setup)
1. إنشاء وتفعيل البيئة الوهمية:
```bash
python -m venv venv
# On Windows
venv\Scripts\activate
# On Mac/Linux
source venv/bin/activate
```
2. تثبيت الحزم المطلوبة:
```bash
pip install -r requirements.txt
```
3. إعداد قواعد البيانات والمستخدم الخارق:
```bash
python manage.py migrate
python manage.py createsuperuser
```
4. تشغيل الخادم:
```bash
python manage.py runserver
```

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

## 📸 جولة في المنصة (Screenshots)

<p align="center">
  <img src="screenshots/dashboard.png" width="48%" alt="لوحة التحكم" />
  <img src="screenshots/inscription_detail.png" width="48%" alt="تفاصيل النقش" />
</p>
<p align="center">
  <img src="screenshots/ocr_detector.png" width="48%" alt="كاشف الذكاء الاصطناعي (OCR)" />
  <img src="screenshots/label_corrector.png" width="48%" alt="أداة تصحيح البيانات" />
</p>

---

## 📜 الترخيص وحقوق الملكية (License)
هذا المشروع هو عمل هندسي متقدم ومحفوظ الحقوق. 
تطوير وهندسة: **م. ريم الوائل** © 2026.
