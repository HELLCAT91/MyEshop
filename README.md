# MyEshop

**MyEshop** یک پروژه‌ی فروشگاه اینترنتی (E-commerce) است که با استفاده از **ASP.NET Core** توسعه داده شده است. این پروژه به عنوان یک نمونه‌ی کاربردی از توسعه‌ی وب‌اپلیکیشن‌های مدرن با استفاده از تکنولوژی‌های مایکروسافت طراحی شده است.

---

## امکانات پروژه

- **احراز هویت و مدیریت دسترسی کاربران:**
  - امکان ثبت‌نام و ورود کاربران.
  - کنترل دسترسی بر اساس نقش‌ها (مانند ادمین و مشتری).

- **مدیریت محصولات:**
  - امکان افزودن، ویرایش و حذف محصولات توسط ادمین.
  - دسته‌بندی و برچسب‌گذاری محصولات برای سازمان‌دهی بهتر.

- **سبد خرید:**
  - امکان افزودن و حذف محصولات از سبد خرید.
  - به‌روزرسانی سبد خرید به صورت بلادرنگ.

- **مدیریت سفارشات:**
  - امکان ثبت سفارش و مشاهده‌ی تاریخچه‌ی سفارشات توسط کاربران.
  - امکان مدیریت سفارشات توسط ادمین (مانند تغییر وضعیت سفارش).

- **طراحی واکنش‌گرا:**
  - طراحی مناسب برای نمایش در دستگاه‌های مختلف (دسکتاپ و موبایل).

- **پایگاه‌داده:**
  - استفاده از **SQL Server** برای ذخیره‌سازی داده‌ها.
  - استفاده از **Entity Framework Core** برای مدیریت عملیات پایگاه‌داده.

---

## تکنولوژی‌های استفاده شده

- **فرانت‌اند:**
  - HTML, CSS, JavaScript
  - Bootstrap برای طراحی رابط کاربری
  - Razor Pages برای ایجاد صفحات داینامیک

- **بک‌اند:**
  - ASP.NET Core
  - Entity Framework Core (روش Code-First)

- **پایگاه‌داده:**
  - SQL Server

- **سایر ابزارها:**
  - Visual Studio (به عنوان IDE)
  - Git (برای کنترل نسخه)

---

## راه‌اندازی پروژه

برای راه‌اندازی پروژه روی سیستم محلی خود، مراحل زیر را دنبال کنید.

### پیش‌نیازها

- [.NET 6 SDK](https://dotnet.microsoft.com/download/dotnet/6.0)
- [Visual Studio 2022](https://visualstudio.microsoft.com/vs/) (یا هر IDE سازگار دیگر)
- [SQL Server](https://www.microsoft.com/en-us/sql-server/sql-server-downloads)

### نصب و راه‌اندازی

1. **کلون کردن ریپازیتوری:**
   ```bash
   git clone https://github.com/HELLCAT91/MyEshop.git
   cd MyEshop
   ```

2. **تنظیم پایگاه‌داده:**
   - در فایل `appsettings.json`، رشته‌ی اتصال به پایگاه‌داده را به SQL Server خود تغییر دهید.
   - سپس دستورات زیر را برای اعمال migrations و ایجاد پایگاه‌داده اجرا کنید:
     ```bash
     dotnet ef database update
     ```

3. **اجرای پروژه:**
   - پروژه را در Visual Studio باز کنید.
   - با فشردن دکمه‌ی `F5`، پروژه را Build و Run کنید.

4. **دسترسی به پروژه:**
   - مرورگر خود را باز کرده و به آدرس `https://localhost:5001` بروید.

---

## ساختار پروژه

```
MyEshop/
├── Controllers/          # کنترلرهای ASP.NET Core
├── Data/                 # پایگاه‌داده و migrations
├── Models/               # مدل‌های Entity
├── Views/                # صفحات Razor
├── wwwroot/              # فایل‌های استاتیک (CSS, JS, تصاویر)
├── appsettings.json      # فایل تنظیمات
└── Program.cs            # نقطه‌ی شروع اجرای برنامه
```

---
