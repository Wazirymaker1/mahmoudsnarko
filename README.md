<div align="center">

<!-- Animated Banner (Neon/RGB) -->
<img src="https://gifs.alphacoders.com/gifs/download/10066292/8BitBoy-Neon-Hacker-in-the-Pixel-Matrix.gif" width="100%" alt="Neon Hacker Matrix Banner">

# 🦅 SNARKO ULTIMATE EDITION 🦅

<img src="https://img.shields.io/badge/STATUS-OPERATIONAL-success?style=for-the-badge&logo=github&logoColor=white" />
<img src="https://img.shields.io/badge/NO_SKIP_MODE-ACTIVE-blue?style=for-the-badge&logo=shield&logoColor=white" />
<img src="https://img.shields.io/badge/PERSISTENT_ATTACK-ENABLED-red?style=for-the-badge&logo=target&logoColor=white" />
<img src="https://img.shields.io/badge/ANTI_BAN_SYSTEM-ONLINE-blueviolet?style=for-the-badge&logo=security&logoColor=white" />

<br>

```text
╔═══════════════════════════════════════════════════════════════════════════════╗
║                                                                               ║
║      🦅  ███████╗███╗   ██╗ █████╗ ██████╗ ██╗  ██╗ ██████╗  ██████╗  ██████╗ ║
║          ██╔════╝████╗  ██║██╔══██╗██╔══██╗██║ ██╔╝██╔═══██╗██╔═══██╗██╔═══██╗║
║          ███████╗██╔██╗ ██║███████║██████╔╝█████╔╝ ██║   ██║██║   ██║██║   ██║║
║          ╚════██║██║╚██╗██║██╔══██║██╔══██╗██╔═██╗ ██║   ██║██║   ██║██║   ██║║
║          ███████║██║ ╚████║██║  ██║██║  ██║██║  ██╗╚██████╔╝╚██████╔╝╚██████╔╝║
║          ╚══════╝╚═╝  ╚═══╝╚═╝  ╚═╝╚═╝  ╚═╝╚═╝  ╚═╝ ╚═════╝  ╚═════╝  ╚═════╝ ║
║                                                                               ║
║                           V E R S I O N   U L T I M A T E                     ║
║                                                                               ║
╚═══════════════════════════════════════════════════════════════════════════════╝
```

</div>

---

## ⚡ المميزات الأساسية - SNARKO CORE FEATURES ⚡

<div align="right">

- **🎯 Persistent Bombing**: لا يتم تخطي أي رقم! الأداة تستمر في الهجوم حتى النجاح أو الإيقاف اليدوي. (`NO SKIP - NEVER STOP`)
- **🔄 Smart Proxy Rotation**: عند مواجهة Rate Limit، يتم تغيير البروكسي تلقائياً مع الاستمرار في الهجوم. (`Auto rotate on 429`)
- **🎲 Full Randomization**: كل طلب له Device ID جديد، User Agent جديد، Headers جديدة، Cookies جديدة. (`100% unique per request`)
- **📁 Multi-Number Support**: دعم ملفات الأرقام (phones.txt) مع إمكانية تحديد عدد المحاولات لكل رقم. (`Batch processing`)
- **🌍 Proxy Management**: Auto Proxy (جلب تلقائي + اختبار) و Manual Proxy مع دعم كامل. (`HTTP/HTTPS proxies`)
- **🤖 User Agent Control**: Random / Specific / Rotate modes - كل طلب بجهاز مختلف. (`Barcelona UA + Devices`)
- **💾 Results Saving**: حفظ النتائج بتنسيق JSON مع تقارير مفصلة عن كل محاولة. (`snarko_results/*.json`)
- **📊 Wide Mode Display**: عرض النتائج في جدول منظم ومتحرك مع إحصائيات فورية. (`Professional UI`)

</div>

---

## 🔧 متطلبات التشغيل - REQUIREMENTS 🔧

```python
Python 3.8+
requests
json
uuid
hashlib
hmac
random
time
os
sys
datetime
```

---

## 📥 طريقة التثبيت والتشغيل - INSTALLATION 📥

```bash
# 1. تثبيت المتطلبات
pip install requests

# 2. تشغيل الأداة
python3 snarko.py

# 3. إدخال مفتاح التفعيل (يتم شراؤه من التليجرام)
Enter SNARKO Key: [Your Key Here]
```

---

## ⚙️ أوامر القائمة - MENU COMMANDS ⚙️

| الخيار | الوصف |
| :---: | :--- |
| **1** | SPAM MODE - Single Number (هجوم لا يتوقف على رقم واحد) |
| **2** | SPAM MODE - File (هجوم على جميع الأرقام في الملف) |
| **3** | Proxy Settings (إعدادات البروكسي - Auto/Manual) |
| **4** | UA Settings (إعدادات User Agent) |
| **5** | Show Stats (عرض النتائج المحفوظة - Wide Mode) |
| **6** | Exit SNARKO |

---

## 🔄 طريقة عمل الـ Proxy - PROXY SYSTEM 🔄

```text
1. Auto Mode:
   - يقوم بجلب بروكسيات جديدة من عدة مصادر
   - اختبارها والتأكد من صلاحيتها
   - التناوب بينها تلقائياً
   - عند Rate Limit: تغيير فوري للبروكسي

2. Manual Mode:
   - إدخال بروكسي يدوي (ip:port)
   - استخدامه لجميع الطلبات
```

---

## 🎯 سلوك الهجوم - ATTACK BEHAVIOR 🎯

```text
📌 Single Number Mode:
   - الأداة تضرب نفس الرقم بشكل مستمر
   - عند Rate Limit → تغيير بروكسي + استمرار
   - عند Fail → إعادة المحاولة مباشرة
   - لا يوجد تخطي للأرقام (NO SKIP)

📌 File Mode:
   - يقرأ الأرقام من الملف
   - لكل رقم: عدد محاولات محدد (أو لا نهائي)
   - بعد انتهاء الرقم، ينتقل للتالي
   - حفظ النتائج الكاملة في ملفات JSON
```

---

## 📡 تفعيل الاشتراك - ACTIVATION 📡

<div align="center">
  <br>
  <a href="https://t.me/i_ru_l" target="_blank">
    <img src="https://img.shields.io/badge/Telegram-Contact_Me-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white" alt="Telegram Contact" />
  </a>
  <br><br>
  <b>🆔 Username:</b> <code>@i_ru_l</code>
  <br>
</div>

---

## 📊 التقارير المحفوظة - SAVED REPORTS 📊

```json
snarko_results/
├── snarko_report_20250101_120000.json
├── snarko_report_20250101_130000.json
└── ...

محتوى التقرير:
{
    "total_ok": 50,
    "total_att": 100,
    "results": [
        {"phone": "201234567890", "success": 10, "attempts": 15},
        ...
    ]
}
```

---

## 🎨 واجهة المستخدم - USER INTERFACE 🎨

```text
✨ Animated Banner (Colors changing)
📍 Real-time location detection
🤖 Current UA mode display
🌐 Proxy status display
📊 Live statistics
💾 Auto-save results
🎯 Wide mode table view
```

---

## ⚠️ تنبيهات هامة - IMPORTANT NOTES ⚠️

```text
1. هذه الأداة للأغراض التعليمية فقط
2. استخدامها بشكل غير قانوني يتحمل مسؤوليته المستخدم
3. المطور غير مسؤول عن أي سوء استخدام
4. الاشتراك يتم مرة واحدة ولا يحتاج تجديد شهري
```

---

## 📡 التقنيات المستخدمة - TECHNOLOGIES 📡

| التقنية | الوصف |
| :---: | :--- |
| **HMAC-SHA256** | توقيع الطلبات لحماية البيانات |
| **Randomization Engine** | توليد Device IDs و User Agents عشوائية |
| **Proxy Scraper** | جلب بروكسيات من عدة مصادر مجانية |
| **Anti-RateLimit** | نظام ذكي للتعامل مع الـ Rate Limit |

---

## 🔄 تحديثات مستقبلية - FUTURE UPDATES 🔄

```text
✅ No Skip Mode (تم)
✅ Full Randomization (تم)
✅ Proxy System (تم)
🔜 WhatsApp API Support
🔜 Telegram Bot Integration
🔜 GUI Version
```

<br>

<div align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=20&pause=1000&color=00FF00&center=true&vCenter=true&width=435&lines=SNARKO+ULTIMATE+EDITION;Developed+by+SNARKO;Contact+Telegram:+@i_ru_l" alt="Typing SVG" />
  <br>
  <p><i>© 2025 SNARKO - All Rights Reserved</i></p>
  <p><i>This tool is for educational purposes only</i></p>
</div>
