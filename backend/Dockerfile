# استخدم صورة Node الرسمية
FROM node:18

# تحديد مجلد العمل داخل الحاوية
WORKDIR /app

# نسخ ملفات الـ package فقط علشان نثبت الـ dependencies الأول
COPY package*.json ./

# تثبيت dependencies
RUN npm install

# نسخ باقي ملفات المشروع
COPY . .

# تشغيل التطبيق
CMD ["npm", "start"]
