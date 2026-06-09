# 📖 قاعدة بيانات التفاسير القرآنية (Quran Tafseer API & JSON Assets)

<p align="center">
  <img src="https://img.shields.io/badge/Maintained%3F-yes-green.svg" alt="Maintained">
  <img src="https://img.shields.io/badge/License-MIT-blue.svg" alt="License MIT">
  <img src="https://img.shields.io/badge/Auth-No%20Token%20Required%20(For%20Read)-brightgreen" alt="No Auth Required">
  <img src="https://img.shields.io/badge/Security-HTTPS%20Secure-brightgreen" alt="HTTPS Secure">
</p>

مستودع مفتوح المصدر ومطور خصيصاً لتوفير بيانات التفاسير القرآنية المتعددة وتغذية تطبيقات **المصحف الإلكتروني** بشكل مستقل وآمن 100% عبر روابط خوادم GitHub CDN المباشرة. 

يحل هذا المشروع مشكلة حظر المحتوى غير المشفر (`Mixed Content HTTP/HTTPS`) تماماً، حيث يقدم البيانات عبر بروتوكول `HTTPS` آمن وبأعلى كفاءة وسرعة تحميل ممكنة.

---

## ⚡ هيكلية النظام والأداء (Performance & Structure)

بدلاً من طلب البيانات آية بآية من السيرفرات الخارجية (مما يسبب بطء الاستجابة)، تم تقسيم التفاسير بصيغة الـ `JSON` إلى **114 ملفاً فقط لكل كتاب تفسير** (ملف مستقل لكل سورة كاملة). 

هذه الهيكلية الذكية تتيح لتطبيقك تحميل السورة كاملة بطلب (`fetch`) واحد فقط، وتخزينها في ذاكرة المتصفح (Cache)، لتصفح فوري وتنقّل فائق السرعة بين تفاسير الآيات وبدون أي انتظار.

---

## 📚 كتب التفاسير المتاحة ومعرفاتها (Available Tafseers)

يمكنك استدعاء أي كتاب تفسير باستخدام رقم المعرّف (`ID`) الخاص به كالتالي:

| ID | اسم كتاب التفسير |
| :---: | :--- |
| **1** | التفسير الميسر |
| **3** | تفسير السعدي |
| **4** | تفسير ابن كثير |
| **5** | تفسير الوسيط لطنطاوي |
| **6** | تفسير البغوي |
| **7** | تفسير القرطبي |
| **8** | تفسير الطبري |

---

## 🛠️ طريقة الاستدعاء البرمجي عبر الروابط المباشرة (API Usage)

```text
[https://raw.githubusercontent.com/em350709-svg/tafseer/main/tafseer/](https://raw.githubusercontent.com/em350709-svg/tafseer/main/tafseer/){tafseerId}/{surahNumber}.json
```
## 📜 رخصة المشروع (License)
هذا المشروع متاح مجاناً تحت رخصة MIT - يمكنك استخدامه وتضمينه وتطويره بحرية تامة في موقعك أو تطبيقاتك البرمجية والمصاحف الإلكترونية.

صدقة جارية • نسأل الله أن يتقبل هذا العمل ويجعله خالصاً لوجهه الكريم ولخدمة كتاب الله العزيز وعباده المسلمين.
