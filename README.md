# 📁 **تطبيق التقاط الصور الذكي باستخدام PyQt5 و MediaPipe**

---

## 🌟 **نبذة عن المشروع**
هذا المشروع هو تطبيق سطح مكتب مبتكر يتيح للمستخدمين التقاط الصور تلقائيًا بناءً على اكتشاف الابتسامات أو حركات اليد باستخدام تقنيات الذكاء الاصطناعي. يتم استخدام مكتبة **MediaPipe** لتحليل حركة اليد، ومكتبة **OpenCV** لاكتشاف الوجوه والابتسامات، بينما توفر مكتبة **PyQt5** واجهة مستخدم جذابة وسهلة الاستخدام. ✨

---

## 🛠️ **المتطلبات الأساسية**
قبل تشغيل المشروع، تأكد من توفر المتطلبات التالية:

### 1. **المكتبات المطلوبة**
- Python 3.x
- PyQt5
- OpenCV (`cv2`)
- MediaPipe
- NumPy (مطلوب تلقائيًا بواسطة OpenCV)

```bash
pip install PyQt5 opencv-python mediapipe numpy
```

### 2. **الملفات المطلوبة**
- ملف الأيقونة الرئيسي: `icon.png` (يمكنك استبداله بأي أيقونة أخرى).
- أيقونات الأزرار:
  - `switch_camera_icon.png` (لتبديل الكاميرا).
  - `camera_icon.png` (للتقاط الصور).

---

## 🚀 **كيف يعمل المشروع؟**
### 1. **واجهة المستخدم**
- تم تصميم واجهة المستخدم باستخدام **PyQt5** لتكون بسيطة وسهلة الاستخدام.
- تحتوي الواجهة على:
  - **مربع عرض الكاميرا**: لعرض الفيديو المباشر من الكاميرا.
  - **زر تبديل الكاميرا**: للتبديل بين الكاميرات الأمامية والخلفية.
  - **زر التقاط الصورة**: لالتقاط الصور يدويًا.

### 2. **اكتشاف الابتسامات**
- يتم استخدام **OpenCV** مع تصنيفات Haar Cascade لاكتشاف الوجوه والابتسامات.
- عند اكتشاف ابتسامة، يتم التقاط الصورة تلقائيًا.

### 3. **اكتشاف حركة اليد**
- يتم استخدام **MediaPipe** لاكتشاف حركة اليد.
- إذا تم اكتشاف أن جميع الأصابع الخمسة مرفوعة، يتم التقاط الصورة تلقائيًا.

### 4. **التقاط الصور**
- يتم حفظ الصور في المسار الحالي باسم `captured_image.jpg`.
- يتم إظهار رسالة نجاح تحتوي على مسار الصورة الملتقطة.

---

## 🔧 **كيفية التشغيل**
1. قم بتنزيل المشروع وتأكد من وجود جميع الملفات المطلوبة.
2. شغل البرنامج باستخدام الأمر التالي:
   ```bash
   python script_name.py
   ```
3. سيتم فتح نافذة التطبيق الرئيسية.
4. يمكنك:
   - تبديل الكاميرا باستخدام الزر العلوي.
   - التقاط الصور يدويًا باستخدام الزر السفلي.
   - التقاط الصور تلقائيًا عند اكتشاف ابتسامة أو حركة يد.

---

## 🎨 **التخصيص**
### 1. **تغيير الأيقونات**
يمكنك استبدال أيقونات الأزرار (`switch_camera_icon.png` و `camera_icon.png`) بأيقونات أخرى لتخصيص الواجهة.

### 2. **تعديل ألوان الواجهة**
يمكنك تعديل ألوان الواجهة عن طريق تغيير القيم في `setStyleSheet`. على سبيل المثال:
```python
self.setStyleSheet("background-color: #3B4252; color: #ECEFF4;")
```

### 3. **إضافة ميزات جديدة**
يمكنك إضافة ميزات مثل:
- حفظ الصور في مجلد مخصص.
- إضافة مؤقت لالتقاط الصور.

---

## 📸 **عينة من النتائج**
عند تشغيل البرنامج:
- ستظهر نافذة تعرض الفيديو المباشر من الكاميرا.
- عند اكتشاف ابتسامة أو رفع جميع الأصابع الخمسة، سيتم التقاط الصورة تلقائيًا.
- ستظهر رسالة نجاح تحتوي على مسار الصورة الملتقطة.

---

## 🙏 **شكرًا لك!**
نأمل أن تستمتع باستخدام هذا التطبيق البسيط والمفيد! إذا كان لديك أي أسئلة أو اقتراحات، فلا تتردد في التواصل معنا. ✨

--- 

🌟 **Happy Coding!** 🌟
