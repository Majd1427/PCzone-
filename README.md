# PCzone Store
متجر إلكترونيات وGaming مع تسجيل دخول وطلبات ولوحة تحكم وقاعدة بيانات Supabase.

## الإعداد
1. أنشئ مشروع Supabase وشغّل schema.sql في SQL Editor.
2. ضع Project URL وanon/publishable key في config.js.
3. أنشئ حسابك من الموقع ثم نفّذ: update public.profiles set role='admin' where email='Majd.shaar15@gmail.com';
4. انشر دالة البريد الموجودة في supabase/functions/send-order-email وضع RESEND_API_KEY وSUPABASE_SERVICE_ROLE_KEY كـ secrets في Supabase.
5. في GitHub Settings > Pages اختر GitHub Actions. workflow جاهز للنشر بعد كل push إلى main.

GitHub Pages يستضيف الواجهة فقط؛ Supabase يستضيف قاعدة البيانات والمصادقة والدالة الخلفية.