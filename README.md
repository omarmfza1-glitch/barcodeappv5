# 📚 نظام إدارة الدورات (Barcode App)

نظام لإدارة الدورات التدريبية مع توليد باركود QR للتسجيل عبر الجوال.

## 🛠️ التقنيات

- **Next.js 16** - إطار العمل
- **TypeScript** - لغة البرمجة
- **Prisma 6** - ORM قاعدة البيانات
- **PostgreSQL (Neon)** - قاعدة البيانات السحابية
- **NextAuth.js** - نظام المصادقة
- **Vercel** - الاستضافة

## 🚀 التشغيل المحلي

```bash
# تثبيت المكتبات
npm install

# إعداد قاعدة البيانات
npx prisma db push

# إضافة مستخدم Admin
npx prisma db seed

# تشغيل السيرفر
npm run dev
```

## 🔐 بيانات الدخول الافتراضية

- **اسم المستخدم:** `admin`
- **كلمة المرور:** `admin123`

## 🌐 متغيرات البيئة

أنشئ ملف `.env` بالمحتوى التالي:

```env
DATABASE_URL="postgresql://user:pass@host/db?sslmode=require"
NEXTAUTH_SECRET="your-secret-key"
NEXTAUTH_URL="http://localhost:3000"
```

## 📱 الميزات

- ✅ إدارة الدورات (إضافة/تعديل/حذف)
- ✅ توليد باركود QR للتسجيل
- ✅ تسجيل الحضور عبر الجوال
- ✅ التحكم بعدد التسجيلات من كل جهاز
- ✅ تصدير بيانات الحضور
- ✅ لوحة تحكم إحصائية

## 📋 الأوامر المفيدة

```bash
npm run dev          # تشغيل محلياً
npm run build        # بناء للإنتاج
npx prisma studio    # عرض قاعدة البيانات
npx prisma db push   # مزامنة الجداول
```

## 🔗 الروابط

- **الموقع:** https://barcodeappv4.vercel.app
- **GitHub:** https://github.com/omarmfza1-glitch/barcodeappv4
