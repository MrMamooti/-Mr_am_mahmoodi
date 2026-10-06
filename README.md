<div align="center">

<img src="banner.svg" width="100%" alt="Mamooti Panel">

<a href="https://t.me/ParsPing_ir"><img src="https://readme-typing-svg.demolab.com?font=Inter&weight=800&size=22&duration=2600&pause=700&color=6C7BFF&center=true&vCenter=true&width=620&lines=One-click+Reseller+Panel+on+Railway;PasarGuard+%2B+Xray+in+a+single+service;5+configs+%C2%B7+2+groups+%C2%B7+self-healing;Free+forever+%C2%B7+X4G+%C3%97+Mamooti" alt="Mamooti"></a>

<h1>Mamooti</h1>

<p><b>پنل نمایندگی حرفه‌ای، رایگان و متن‌باز بر پایه‌ی PasarGuard</b><br>
یک Fork تا یک سرویس کامل: پنل، هسته‌ی Xray و 5 کانفیگ آماده، همه روی Railway</p>

<a href="https://t.me/ParsPing_ir"><img src="https://img.shields.io/badge/Telegram-Mamooti-26A5E4?style=for-the-badge&logo=telegram&logoColor=white" alt="Mamooti"></a>

</div>

---

## ✨ درباره پروژه

Mamooti یک پنل نمایندگی کامل و رایگان است که پنل، هسته‌ی Xray، کانفیگ‌های آماده و سیستم مدیریت اشتراک را در یک سرویس ارائه می‌دهد.

### امکانات

| قابلیت | توضیحات |
|---|---|
| 🚀 نصب سریع | نصب کامل روی Railway |
| ⚡ 5 کانفیگ | Pro، Flash، Fire، Diamond، Night |
| 👥 2 گروه | مدیریت کاربران و نمایندگان |
| 🧾 قالب فروش | چند قالب آماده برای فروش |
| 📱 پشتیبانی اپ‌ها | V2Box، v2rayNG، Hiddify و... |
| 🔄 Self-Healing | بازیابی خودکار سرویس |
| 🆓 رایگان | بدون نیاز به سرور اختصاصی |

---

## 📸 Preview

صفحه‌ی اشتراک با طراحی MAMOOTI PASS، نمایش حجم مصرفی، تاریخ انقضا، وضعیت سرور، QR Code و کانفیگ‌ها.

---

## 🏗️ معماری

`mermaid
flowchart TD
    A["Railway"] --> B["Mamooti Bootstrap<br/>auto setup + self-heal"]
    B --> C["PasarGuard"]
    B --> D["Xray Core"]
    C --> E["Reseller Panel"]
    D --> F["VLESS / VMess / Trojan"]
    E --> G["Subscription Page"]
HTML
🚀 نصب
1. ساخت پروژه در Railway
Repository را در Railway Deploy کنید.
2. Volume
برای نگهداری اطلاعات پنل Volume زیر را اضافه کنید:
/var/lib/pasarguard
3. Domain
از قسمت Networking یک Domain برای سرویس ایجاد کنید.
پورت:
8080
4. Region
پیشنهاد:
EU West - Amsterdam
پس از اجرای موفق باید چیزی مشابه زیر در Log مشاهده شود:
[bootstrap] DONE -> https://YOUR-DOMAIN/dashboard/
هر نصب دارای مسیرهای امنیتی اختصاصی و Secret تصادفی است.
🔐 ورود اولیه
اطلاعات ورود اولیه:
Username: admin
Password: admin
بعد از اولین ورود حتماً رمز عبور را تغییر دهید.
👤 Owner Key
پس از ورود به پنل، Owner Key را در محل مناسب تنظیم کنید و از قرار دادن آن در اختیار افراد دیگر خودداری کنید.
💰 ساخت کاربر و فروش
نمونه:
30GB - 30 روز
Group: Mamooti
Config: Pro
یا:
Pro 30GB - 30 روز
Group: مموتی پرو
Config: Pro
📱 اپلیکیشن‌های پیشنهادی
برنامه
سیستم‌عامل
V2Box
iOS / Android
v2rayNG
Android
Hiddify
Android / iOS / Windows
Streisand
iOS
Happ
Android / iOS
NekoBox
Android
Clash Meta
Android / Windows
sing-box
چندسکویی
🔑 Subscription Link
فرمت لینک اشتراک:
https://YOUR-DOMAIN/sub/<token>
این لینک را می‌توان داخل QR Code، ربات فروش و صفحه‌ی اشتراک استفاده کرد.
⚙️ کانفیگ‌ها
گروه
نام کانفیگ
Protocol
Transport
مناسب برای
توضیحات
مموتی پرو
𝗣𝗿𝗼
VLESS
WebSocket + Early Data
Chrome
تک‌کانفیگ با کمترین پینگ
Mamooti
⚡ 𝗙𝗹𝗮𝘀𝗵
VLESS
WebSocket
Firefox
سریع و سبک

🔥 𝗙𝗶𝗿𝗲
Trojan
WebSocket
Safari
مناسب iOS

💎 𝗗𝗶𝗮𝗺𝗼𝗻𝗱
VMess
WebSocket
Edge
سازگاری با اپ‌های قدیمی

🌙 𝗡𝗶𝗴𝗵𝘁
VLESS
HTTPUpgrade
iOS
پایدار در شبکه‌های سخت
نام کانفیگ‌ها
𝗣𝗿𝗼
⚡ 𝗙𝗹𝗮𝘀𝗵
🔥 𝗙𝗶𝗿𝗲
💎 𝗗𝗶𝗮𝗺𝗼𝗻𝗱
🌙 𝗡𝗶𝗴𝗵𝘁
👥 گروه‌های نمایندگی
گروه
حجم‌ها
Mamooti
10GB، 30GB، 50GB، 100GB، 200GB، نامحدود
مموتی
Pro 30GB، Pro 50GB، Pro 100GB، Pro Unlimited
🪪 MAMOOTI PASS
صفحه‌ی اشتراک شامل:
طراحی هولوگرامی MAMOOTI
نمایش فارسی و انگلیسی
تاریخ شمسی
نمایش میزان مصرف
نمایش حجم باقی‌مانده
نمایش تاریخ انقضا
وضعیت و Ping سرور
لینک اشتراک
QR Code
دکمه‌ی اتصال سریع
لیست کانفیگ‌ها
پشتیبانی از اپلیکیشن‌های مختلف
🔄 Self-Healing
سیستم Mamooti دارای مکانیزم بررسی و بازیابی خودکار سرویس است.
Railway
   ↓
Mamooti Bootstrap
   ↓
