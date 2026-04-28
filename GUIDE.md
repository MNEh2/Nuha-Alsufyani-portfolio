# 🛠️ دليل التعديل البرمجي — Portfolio Nuha

## 📁 هيكل الملفات
```
📁 portfolio/
  ├── nuha-portfolio.html   ← الملف الرئيسي
  ├── fameet-logo.png
  ├── lasen-cover.png
  ├── cpoint-ui.png         ← صورة Filming
  ├── cpoint-video.mp4      ← فيديو Filming
  └── GUIDE.md              ← هذا الملف
```

---

## 🔍 كيف تبحثين عن أي شي في VS Code
```
Ctrl + F         ← بحث في الملف
Ctrl + H         ← بحث واستبدال
Ctrl + S         ← حفظ
Alt + Z          ← تفعيل Word Wrap (عشان تشوفين النص كامل)
```

---

## ✏️ تعديل النصوص الأساسية

### الاسم والعنوان
ابحثي عن:
```
Nuha Alsufyani
```

### الوصف الشخصي (Hero)
ابحثي عن:
```
IT graduate who bridges
```

### الإيميل
ابحثي عن:
```
nuhaalsufyani@gmail.com
```

### رقم الجوال
ابحثي عن:
```
(+966) 50 078 1805
```

### LinkedIn
ابحثي عن:
```
linkedin.com/in/nuhaalsufyani
```

---

## 🖼️ إضافة صورة لمشروع

### في البطاقة الرئيسية (الكارد)
ابحثي عن اسم المشروع مثلاً `project-img-placeholder` بجانب `🏥` لـ Bayan:
```html
<!-- قبل -->
<div class="project-img-placeholder">🏥</div>

<!-- بعد -->
<img src="bayan.png" class="project-img" style="object-fit:cover;">
```

### في الـ Popup
ابحثي عن:
```html
<div class="modal-img-slot empty">
```
واستبدليها بـ:
```html
<div class="modal-img-slot">
  <img src="اسم-الصورة.png" onclick="openLightbox(this.src)">
</div>
```

---

## 📝 تعديل وصف المشاريع في الـ Popup

### Lasen
ابحثي عن: `modal-lasen`
- **About:** ابحثي عن النص بعد `About the Project` داخل `modal-lasen`
- **My Role:** ابحثي عن النص بعد `My Role` داخل `modal-lasen`

### Bayan
ابحثي عن: `modal-bayan`

### FaMeet
ابحثي عن: `modal-fameet`

### Filming
ابحثي عن: `modal-filming`

### Device
ابحثي عن: `modal-device`

---

## 🏷️ إضافة أو تعديل التقنيات (Tags)

داخل أي modal ابحثي عن `modal-tech` وأضيفي:
```html
<span>اسم التقنية</span>
```

---

## 🏆 تعديل الجوائز

ابحثي عن قسم الجوائز:
```
Recognition
```
كل جائزة شكلها:
```html
<div class="ac">
  <div class="ae">🥇</div>
  <div class="at">1st Place</div>
  <div class="ad">اسم المسابقة · السنة</div>
</div>
```

---

## 🎨 تغيير الألوان

في بداية الملف داخل `:root` تقدرين تغيرين:
```css
--accent: #7B6EF6;    ← اللون البنفسجي الرئيسي
--accent2: #A78BFA;   ← البنفسجي الفاتح
--teal: #2DD4BF;      ← التيل
--green: #4ADE80;     ← الأخضر
--bg: #0D0D0F;        ← خلفية الصفحة
--text: #F0EEF8;      ← لون النص
```

---

## 🔗 إضافة رابط GitHub لمشروع

داخل الـ modal المطلوب، أضيفي:
```html
<div class="modal-section">
  <div class="modal-section-label">GitHub</div>
  <a href="https://github.com/رابطك" target="_blank" 
     style="color:var(--accent2);font-size:0.9rem;">
    github.com/رابطك →
  </a>
</div>
```

---

## 🎬 تغيير الفيديو

ابحثي عن:
```
cpoint-video.mp4
```
واستبدليها باسم ملف الفيديو الجديد، وتأكدي إنه في نفس المجلد.

---

## 🌐 رفع الموقع على Netlify

1. روحي على: https://app.netlify.com/drop
2. اسحبي المجلد كامل (كل الملفات مع بعض)
3. يعطيكِ رابط فوراً ✅
4. تقدرين تغيرين اسم الرابط من Site Settings

---

## 💡 نصائح سريعة

- **دايماً** احفظي `Ctrl + S` بعد أي تعديل
- افتحي الملف في المتصفح تشوفين التغيير مباشرة
- لو خربتِ شي، `Ctrl + Z` للتراجع
- الصور لازم تكون **في نفس المجلد** مع الـ HTML
