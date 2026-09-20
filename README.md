<div align="right" dir="rtl">

## پنل مدیریت VPN

### 🚀 راهنمای نصب و دیپلوی

────────

### ⚡ نصب مستقیم روی VPS

```bash
curl -fsSL https://raw.githubusercontent.com/gAhkejdkdf/SpiderPanel/main/start.sh | bash
```

> 💡 **دستور بالا را کپی کرده و در ترمینال VPS اجرا کنید.**

### 🔒 فعال‌سازی TLS روی VPS (برای کار کردن کانفیگ‌ها)

کانفیگ‌های TLS به HTTPS روی پورت 443 نیاز دارند. یک دامنه را به IP سرور وصل کنید، بعد:

```bash
spiderpanel tls vpn.example.com
```

این دستور Caddy را نصب می‌کند و خودش سرتیفیکیت می‌گیرد و تمدید می‌کند. بدون دامنه، TLS کار نمی‌کند.

────────

### 🚄 دیپلوی روی Railway

۱. پروژه را Fork کنید و آن را روی اکانت GitHub خود ذخیره نمایید.

۲. وارد Railway شوید و با استفاده از حساب GitHub خود Login کنید.

۳. پروژه Fork‌شده را انتخاب کرده و مراحل Deploy را آغاز کنید.

۴. پس از اتمام کامل Deploy:

• وارد بخش Settings شوید.
• روی Generate Domain کلیک کنید.
• پورت را روی 8080 تنظیم کنید.

۵. پس از ساخت Domain، عبارت زیر را به انتهای آدرس اضافه کنید:

```text
/spider
```

مثال:

```text
https://your-domain.up.railway.app/spider
```

────────

### 📌 اطلاعات پروژه

پورت پیش‌فرض:

```text
8080
```

مسیر ورود به پنل:

```text
/spider
```

نام کاربری پیش‌فرض: `admin` — رمز پیش‌فرض: `admin`
(با متغیر محیطی `ADMIN_PASSWORD` قابل تغییر است.)

</div>
