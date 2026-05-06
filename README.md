```markdown
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>🦅 SNARKO ULTIMATE EDITION - README</title>
    <style>
        @keyframes float {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-10px); }
        }
        @keyframes glow {
            0%, 100% { text-shadow: 0 0 5px #00ff00, 0 0 10px #00ff00; }
            50% { text-shadow: 0 0 20px #00ff00, 0 0 30px #00ff00; }
        }
        @keyframes borderPulse {
            0%, 100% { border-color: #ff0000; }
            33% { border-color: #00ff00; }
            66% { border-color: #0000ff; }
        }
        @keyframes bgMove {
            0% { background-position: 0% 0%; }
            100% { background-position: 100% 100%; }
        }
        @keyframes blink {
            0%, 100% { opacity: 1; }
            50% { opacity: 0.3; }
        }
        @keyframes shake {
            0%, 100% { transform: translateX(0); }
            25% { transform: translateX(-5px); }
            75% { transform: translateX(5px); }
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            background: linear-gradient(135deg, #0a0a0a 0%, #1a1a2e 50%, #0f0f23 100%);
            font-family: 'Courier New', 'Monaco', monospace;
            min-height: 100vh;
            padding: 20px;
            color: #0f0;
            animation: bgMove 20s linear infinite;
            background-size: 200% 200%;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            background: rgba(0, 0, 0, 0.85);
            border-radius: 20px;
            padding: 30px;
            box-shadow: 0 0 50px rgba(0, 255, 0, 0.2);
            border: 2px solid #0f0;
            animation: borderPulse 3s ease-in-out infinite;
        }
        
        /* ASCII Banner متحرك */
        .ascii-banner {
            text-align: center;
            font-family: monospace;
            font-weight: bold;
            line-height: 1.2;
            animation: glow 2s ease-in-out infinite, float 3s ease-in-out infinite;
            margin-bottom: 30px;
        }
        
        .ascii-banner pre {
            background: transparent;
            color: #0f0;
            text-shadow: 0 0 10px #0f0;
            font-size: 14px;
            overflow-x: auto;
        }
        
        /* Header Styles */
        h1 {
            text-align: center;
            font-size: 2.5rem;
            margin-bottom: 20px;
            background: linear-gradient(45deg, #ff0000, #ffff00, #00ff00, #00ffff, #0000ff, #ff00ff);
            background-size: 400% 400%;
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            animation: glow 2s ease-in-out infinite, bgMove 5s linear infinite;
        }
        
        h2 {
            color: #ffcc00;
            border-right: 4px solid #ffcc00;
            padding: 10px 20px;
            margin: 25px 0 15px 0;
            background: linear-gradient(90deg, rgba(255,204,0,0.2), transparent);
            animation: shake 0.5s ease-in-out;
        }
        
        h3 {
            color: #00ffaa;
            margin: 15px 0 10px 0;
            padding: 5px 10px;
            border-left: 3px solid #00ffaa;
        }
        
        /* Code Blocks */
        pre {
            background: #0a0a0f;
            border-left: 4px solid #0f0;
            padding: 15px;
            border-radius: 10px;
            overflow-x: auto;
            font-size: 13px;
            margin: 15px 0;
            box-shadow: inset 0 0 10px rgba(0,255,0,0.1);
        }
        
        code {
            color: #ffcc00;
            font-family: monospace;
        }
        
        /* Feature List */
        .feature-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 20px;
            margin: 20px 0;
        }
        
        .feature-card {
            background: linear-gradient(135deg, rgba(0,255,0,0.1), rgba(0,0,0,0.5));
            border: 1px solid #0f0;
            border-radius: 15px;
            padding: 20px;
            transition: all 0.3s ease;
            animation: float 4s ease-in-out infinite;
        }
        
        .feature-card:hover {
            transform: scale(1.02);
            box-shadow: 0 0 20px rgba(0,255,0,0.3);
            background: linear-gradient(135deg, rgba(0,255,0,0.2), rgba(0,0,0,0.6));
        }
        
        .feature-card h3 {
            color: #0f0;
            margin-top: 0;
            border-left-color: #0f0;
        }
        
        /* Telegram Contact */
        .telegram-card {
            background: linear-gradient(135deg, #0088cc20, #00000080);
            border: 2px solid #0088cc;
            border-radius: 20px;
            padding: 30px;
            text-align: center;
            margin: 30px 0;
            animation: glow 3s ease-in-out infinite;
        }
        
        .telegram-card a {
            display: inline-block;
            background: #0088cc;
            color: white;
            text-decoration: none;
            padding: 15px 40px;
            border-radius: 50px;
            font-size: 1.5rem;
            font-weight: bold;
            margin-top: 15px;
            transition: all 0.3s ease;
            animation: blink 2s ease-in-out infinite;
        }
        
        .telegram-card a:hover {
            transform: scale(1.05);
            background: #00aaff;
            box-shadow: 0 0 30px #0088cc;
            animation: none;
        }
        
        /* Table Styles */
        table {
            width: 100%;
            border-collapse: collapse;
            margin: 20px 0;
            background: rgba(0,0,0,0.5);
        }
        
        th, td {
            border: 1px solid #0f0;
            padding: 12px;
            text-align: center;
        }
        
        th {
            background: rgba(0,255,0,0.2);
            color: #0f0;
            font-weight: bold;
        }
        
        tr:hover {
            background: rgba(0,255,0,0.1);
        }
        
        /* Badge */
        .badge {
            display: inline-block;
            padding: 5px 15px;
            border-radius: 50px;
            font-size: 12px;
            font-weight: bold;
            margin: 5px;
            animation: pulse 1s ease-in-out infinite;
        }
        
        @keyframes pulse {
            0%, 100% { opacity: 0.7; }
            50% { opacity: 1; }
        }
        
        .badge-green { background: #00ff0022; border: 1px solid #0f0; color: #0f0; }
        .badge-red { background: #ff000022; border: 1px solid #f00; color: #f00; }
        .badge-blue { background: #0088cc22; border: 1px solid #0088cc; color: #0088cc; }
        
        /* Footer */
        .footer {
            text-align: center;
            margin-top: 40px;
            padding-top: 20px;
            border-top: 1px solid #0f0;
            font-size: 12px;
            color: #0a0;
        }
        
        /* Status LED */
        .led {
            display: inline-block;
            width: 12px;
            height: 12px;
            border-radius: 50%;
            background: #0f0;
            margin-right: 8px;
            animation: blink 1s step-end infinite;
            box-shadow: 0 0 5px #0f0;
        }
        
        /* Responsive */
        @media (max-width: 768px) {
            .container { padding: 15px; }
            .ascii-banner pre { font-size: 8px; }
            h1 { font-size: 1.5rem; }
            .feature-grid { grid-template-columns: 1fr; }
        }
        
        /* Scrollbar */
        ::-webkit-scrollbar {
            width: 10px;
            height: 10px;
        }
        
        ::-webkit-scrollbar-track {
            background: #0a0a0f;
        }
        
        ::-webkit-scrollbar-thumb {
            background: #0f0;
            border-radius: 5px;
        }
        
        ::-webkit-scrollbar-thumb:hover {
            background: #0a0;
        }
        
        /* Blinking cursor effect */
        .cursor-blink {
            animation: blink 1s step-end infinite;
        }
        
        /* Terminal Input */
        .terminal-line {
            font-family: monospace;
            color: #0f0;
            margin: 10px 0;
        }
        
        .terminal-line::before {
            content: "snarko@ultimate:~$ ";
            color: #ffcc00;
        }
    </style>
</head>
<body>
    <div class="container">
        
        <!-- ASCII Banner متحرك -->
        <div class="ascii-banner">
            <pre>
╔═══════════════════════════════════════════════════════════════════════════════╗
║                                                                               ║
║      🦅  ███████╗███╗   ██╗ █████╗ ██████╗ ██╗  ██╗ ██████╗  ██████╗  ██████╗ ║
║          ██╔════╝████╗  ██║██╔══██╗██╔══██╗██║ ██╔╝██╔═══██╗██╔═══██╗██╔═══██╗║
║          ███████╗██╔██╗ ██║███████║██████╔╝█████╔╝ ██║   ██║██║   ██║██║   ██║║
║          ╚════██║██║╚██╗██║██╔══██║██╔══██╗██╔═██╗ ██║   ██║██║   ██║██║   ██║║
║          ███████║██║ ╚████║██║  ██║██║  ██║██║  ██╗╚██████╔╝╚██████╔╝╚██████╔╝║
║          ╚══════╝╚═╝  ╚═══╝╚═╝  ╚═╝╚═╝  ╚═╝╚═╝  ╚═╝ ╚═════╝  ╚═════╝  ╚═════╝ ║
║                                                                               ║
║                    ██╗   ██╗██╗████████╗██╗███╗   ███╗ █████╗ ████████╗███████╗║
║                    ██║   ██║██║╚══██╔══╝██║████╗ ████║██╔══██╗╚══██╔══╝██╔════╝║
║                    ██║   ██║██║   ██║   ██║██╔████╔██║███████║   ██║   █████╗  ║
║                    ██║   ██║██║   ██║   ██║██║╚██╔╝██║██╔══██║   ██║   ██╔══╝  ║
║                    ╚██████╔╝██║   ██║   ██║██║ ╚═╝ ██║██║  ██║   ██║   ███████╗║
║                     ╚═════╝ ╚═╝   ╚═╝   ╚═╝╚═╝     ╚═╝╚═╝  ╚═╝   ╚═╝   ╚══════╝║
║                                                                               ║
║                           V E R S I O N   U L T I M A T E                      ║
║                                                                               ║
╚═══════════════════════════════════════════════════════════════════════════════╝
            </pre>
        </div>

        <h1>🦅 SNARKO ULTIMATE EDITION 🦅</h1>
        
        <div style="text-align: center; margin-bottom: 30px;">
            <span class="badge badge-green">🔴 STATUS: OPERATIONAL</span>
            <span class="badge badge-green">⚡ THREADS API ACTIVE</span>
            <span class="badge badge-blue">🛡️ NO SKIP MODE</span>
            <span class="badge badge-green">🎯 PERSISTENT ATTACK</span>
            <span class="badge badge-red">🚫 ANTI-BAN SYSTEM</span>
        </div>

        <!-- Terminal Intro -->
        <div class="terminal-line">
            <span class="led"></span> Loading Snarko Engine...
        </div>
        <div class="terminal-line">
            <span class="led"></span> Threads API Connection: <span style="color:#0f0;">██████████ 100%</span>
        </div>
        <div class="terminal-line">
            <span class="led"></span> Proxy System: <span style="color:#0f0;">ACTIVE</span>
        </div>
        <div class="terminal-line">
            <span class="led"></span> Subscription: <span style="color:#ffcc00;">WAITING FOR ACTIVATION</span>
        </div>
        
        <hr style="border-color: #0f0; margin: 25px 0;">

        <!-- Features Section -->
        <h2>⚡ المميزات الأساسية - SNARKO CORE FEATURES ⚡</h2>
        
        <div class="feature-grid">
            <div class="feature-card">
                <h3>🎯 Persistent Bombing</h3>
                <p>لا يتم تخطي أي رقم! الأداة تستمر في الهجوم حتى النجاح أو الإيقاف اليدوي.</p>
                <code>NO SKIP - NEVER STOP</code>
            </div>
            <div class="feature-card">
                <h3>🔄 Smart Proxy Rotation</h3>
                <p>عند مواجهة Rate Limit، يتم تغيير البروكسي تلقائياً مع الاستمرار في الهجوم.</p>
                <code>Auto rotate on 429</code>
            </div>
            <div class="feature-card">
                <h3>🎲 Full Randomization</h3>
                <p>كل طلب له Device ID جديد، User Agent جديد، Headers جديدة، Cookies جديدة.</p>
                <code>100% unique per request</code>
            </div>
            <div class="feature-card">
                <h3>📁 Multi-Number Support</h3>
                <p>دعم ملفات الأرقام (phones.txt) مع إمكانية تحديد عدد المحاولات لكل رقم.</p>
                <code>Batch processing</code>
            </div>
            <div class="feature-card">
                <h3>🌍 Proxy Management</h3>
                <p>Auto Proxy (جلب تلقائي + اختبار) و Manual Proxy مع دعم كامل.</p>
                <code>HTTP/HTTPS proxies</code>
            </div>
            <div class="feature-card">
                <h3>🤖 User Agent Control</h3>
                <p>Random / Specific / Rotate modes - كل طلب بجهاز مختلف.</p>
                <code>Barcelona UA + Devices</code>
            </div>
            <div class="feature-card">
                <h3>💾 Results Saving</h3>
                <p>حفظ النتائج بتنسيق JSON مع تقارير مفصلة عن كل محاولة.</p>
                <code>snarko_results/*.json</code>
            </div>
            <div class="feature-card">
                <h3>📊 Wide Mode Display</h3>
                <p>عرض النتائج في جدول منظم ومتحرك مع إحصائيات فورية.</p>
                <code>Professional UI</code>
            </div>
        </div>

        <h2>🔧 متطلبات التشغيل - REQUIREMENTS 🔧</h2>
        <pre><code>Python 3.8+
requests
json
uuid
hashlib
hmac
random
time
os
sys
datetime</code></pre>

        <h2>📥 طريقة التثبيت والتشغيل - INSTALLATION 📥</h2>
        <pre><code># 1. تثبيت المتطلبات
pip install requests

# 2. تشغيل الأداة
python3 snarko_final.py

# 3. إدخال مفتاح التفعيل (يتم شراؤه من التليجرام)
Enter SNARKO Key: [Your Key Here]</code></pre>

        <h2>⚙️ أوامر القائمة - MENU COMMANDS ⚙️</h2>
        <table>
            <tr><th>الخيار</th><th>الوصف</th></tr>
            <tr><td>1</td><td>SPAM MODE - Single Number (هجوم لا يتوقف على رقم واحد)</td></tr>
            <tr><td>2</td><td>SPAM MODE - File (هجوم على جميع الأرقام في الملف)</td></tr>
            <tr><td>3</td><td>Proxy Settings (إعدادات البروكسي - Auto/Manual)</td></tr>
            <tr><td>4</td><td>UA Settings (إعدادات User Agent)</td></tr>
            <tr><td>5</td><td>Show Stats (عرض النتائج المحفوظة - Wide Mode)</td></tr>
            <tr><td>6</td><td>Exit SNARKO</td></tr>
        </table>

        <h2>🔄 طريقة عمل الـ Proxy - PROXY SYSTEM 🔄</h2>
        <pre><code>1. Auto Mode:
   - يقوم بجلب بروكسيات جديدة من عدة مصادر
   - اختبارها والتأكد من صلاحيتها
   - التناوب بينها تلقائياً
   - عند Rate Limit: تغيير فوري للبروكسي

2. Manual Mode:
   - إدخال بروكسي يدوي (ip:port)
   - استخدامه لجميع الطلبات</code></pre>

        <h2>🎯 سلوك الهجوم - ATTACK BEHAVIOR 🎯</h2>
        <pre><code>📌 Single Number Mode:
   - الأداة تضرب نفس الرقم بشكل مستمر
   - عند Rate Limit → تغيير بروكسي + استمرار
   - عند Fail → إعادة المحاولة مباشرة
   - لا يوجد تخطي للأرقام (NO SKIP)

📌 File Mode:
   - يقرأ الأرقام من الملف
   - لكل رقم: عدد محاولات محدد (أو لا نهائي)
   - بعد انتهاء الرقم، ينتقل للتالي
   - حفظ النتائج الكاملة في ملفات JSON</code></pre>

        <!-- Telegram Activation Card -->
        <div class="telegram-card">
            <h2 style="color: #0088cc; margin: 0 0 10px 0;">📡 تفعيل الاشتراك - ACTIVATION 📡</h2>
            <p style="font-size: 18px; margin-bottom: 15px;">للحصول على مفتاح التفعيل (API Key)، يرجى التواصل مع المطور على تليجرام</p>
            <div style="font-size: 24px; margin: 15px 0;">
                🆔 Username: <strong style="color: #00aaff;">@i_ru_l</strong>
            </div>
            <a href="https://t.me/i_ru_l" target="_blank">✨ تواصل مع SNARKO على تليجرام ✨</a>
            <p style="margin-top: 20px; font-size: 14px;">
                ⚡ بعد التواصل، سيتم إرسال مفتاح التفعيل الخاص بك<br>
                🔑 Key Format: SNARKO-XXXX-XXXX-XXXX<br>
                💰 الأسعار: تواصل للسؤال
            </p>
        </div>

        <h2>📊 التقارير المحفوظة - SAVED REPORTS 📊</h2>
        <pre><code>snarko_results/
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
}</code></pre>

        <h2>🎨 واجهة المستخدم - USER INTERFACE 🎨</h2>
        <pre><code>✨ Animated Banner (Colors changing)
📍 Real-time location detection
🤖 Current UA mode display
🌐 Proxy status display
📊 Live statistics
💾 Auto-save results
🎯 Wide mode table view</code></pre>

        <h2>⚠️ تنبيهات هامة - IMPORTANT NOTES ⚠️</h2>
        <pre><code>1. هذه الأداة للأغراض التعليمية فقط
2. استخدامها بشكل غير قانوني يتحمل مسؤوليته المستخدم
3. المطور غير مسؤول عن أي سوء استخدام
4. Threads API تابعة لشركة Meta
5. الاشتراك يتم مرة واحدة ولا يحتاج تجديد شهري</code></pre>

        <!-- Tech Specs -->
        <h2>📡 التقنيات المستخدمة - TECHNOLOGIES 📡</h2>
        <table>
            <tr><th>التقنية</th><th>الوصف</th></tr>
            <tr><td>Threads API</td><td>API رسمية من Meta لإرسال الأكواد</td></tr>
            <tr><td>HMAC-SHA256</td><td>توقيع الطلبات لحماية البيانات</td></tr>
            <tr><td>Randomization Engine</td><td>توليد Device IDs و User Agents عشوائية</td></tr>
            <tr><td>Proxy Scraper</td><td>جلب بروكسيات من عدة مصادر مجانية</td></tr>
            <tr><td>Anti-RateLimit</td><td>نظام ذكي للتعامل مع الـ Rate Limit</td></tr>
        </table>

        <h2>🔄 تحديثات مستقبلية - FUTURE UPDATES 🔄</h2>
        <pre><code>✅ Threads API (تم)
✅ No Skip Mode (تم)
✅ Full Randomization (تم)
✅ Proxy System (تم)
🔜 WhatsApp API Support
🔜 Telegram Bot Integration
🔜 GUI Version</code></pre>

        <!-- Strategy Animation -->
        <div style="text-align: center; margin: 30px 0; padding: 20px; background: rgba(0,255,0,0.05); border-radius: 15px;">
            <h3 style="color: #ffcc00;">🧠 استراتيجية الهجوم الذكية - SMART ATTACK STRATEGY 🧠</h3>
            <div class="terminal-line" style="text-align: left; max-width: 500px; margin: 15px auto;">
                if RATE_LIMIT:<br>
                &nbsp;&nbsp;&nbsp;&nbsp;proxy.rotate()<br>
                &nbsp;&nbsp;&nbsp;&nbsp;continue_attack()<br>
                <br>
                if NOT_OTP_RECEIVED:<br>
                &nbsp;&nbsp;&nbsp;&nbsp;retry_with_new_device()<br>
                &nbsp;&nbsp;&nbsp;&nbsp;continue_attack()<br>
                <br>
                # NEVER SKIP 🔥<br>
                while number_exists:<br>
                &nbsp;&nbsp;&nbsp;&nbsp;attack()<br>
            </div>
        </div>

        <!-- Footer -->
        <div class="footer">
            <p>🦅 SNARKO ULTIMATE EDITION - Developed by SNARKO 🦅</p>
            <p>📞 Contact Telegram: <strong style="color: #0088cc;">@i_ru_l</strong> للتفعيل والدعم</p>
            <p>© 2025 SNARKO - All Rights Reserved</p>
            <p style="font-size: 10px;">This tool is for educational purposes only</p>
            <div class="terminal-line" style="display: inline-block;">
                <span class="led"></span> SNARKO ENGINE: <span class="cursor-blink">READY</span>
            </div>
        </div>
        
    </div>
</body>
</html>
```
