# Security Policy

## Scope
This organization hosts Abrak platform development and operations. Public repositories carry documentation and org standards only; product source stays private.

> **فارسی:** این سازمان میزبان توسعه و عملیات پلتفرم ابرک است. مخازن عمومی منحصراً حاوی مستندات و استانداردهای سازمانی بوده و سورس‌کد محصولات به صورت خصوصی نگهداری می‌شود.  
> **العربية:** تستضيف هذه المنظمة تطوير وتشغيل منصة أبرك. تحتوي المستودعات العامة حصرياً على التوثيق والمعايير المؤسسية، بينما تظل الشيفرات المصدرية للمنتجات خاصة ومحمية.  
> **Türkçe:** Bu organizasyon, Abrak platformunun geliştirme ve operasyonel süreçlerine ev sahipliği yapar. Herkese açık depolar yalnızca dokümantasyon ve kurumsal standartları içerir; ürün kaynak kodları özel olarak korunur.

---

## Reporting
Report sensitive findings privately to organization owners. Do not open public issues for secrets, credentials, or production-impact vulnerabilities.

> **فارسی:** گزارش یافته‌ها و آسیب‌پذیری‌های حساس را به صورت کاملاً محرمانه به مالکان سازمان ارسال نمایید. اکیداً از ثبت گزارش عمومی (Issue) برای کلیدها، دسترسی‌ها یا آسیب‌پذیری‌های موثر بر محیط پروداکشن خودداری فرمایید.  
> **العربية:** يُرجى إرسال أي ملاحظات أو ثغرات أمنية حساسة بشكل خاص وسري إلى مسؤولي المنظمة. يُمنع منعاً باتاً فتح بلاغات عامة (Issues) تخص المفاتيح المشفرة، بيانات الاعتماد، أو الثغرات المؤثرة على بيئة الإنتاج.  
> **Türkçe:** Hassas güvenlik bulgularını lütfen gizli bir şekilde organizasyon sahiplerine iletiniz. Gizli anahtarlar, kimlik bilgileri veya canlı sistemleri etkileyebilecek güvenlik açıkları için herkese açık bildirimler (Issue) açmayınız.

---

## Red Lines
No direct operational changes on:

- `abrak.org` — production SaaS and tenant databases
- `mx1.abrak.org` — production mail gateway

> **فارسی (خطوط قرمز):** هرگونه تغییر مستقیم عملیاتی بر روی دامنه‌ها و سرویس‌های زیر اکیداً ممنوع است:
> - `abrak.org` — محیط عملیاتی پروداکشن SaaS و پایگاه‌های دادهٔ مستاجران
> - `mx1.abrak.org` — درگاه و سرویس ایمیل پروداکشن
>
> **العربية (الخطوط الحمراء):** يُحظر حظراً قاطعاً إجراء أي تعديلات تشغيلية مباشرة على:
> - `abrak.org` — بيئة الإنتاج السحابية وقواعد بيانات المستأجرين
> - `mx1.abrak.org` — بوابة البريد الإلكتروني للإنتاج
>
> **Türkçe (Kırmızı Çizgiler):** Aşağıdaki bileşenler üzerinde doğrudan operasyonel değişiklik yapılması kesinlikle yasaktır:
> - `abrak.org` — Canlı üretim SaaS ortamı ve kiracı veri tabanları
> - `mx1.abrak.org` — Canlı üretim e-posta sunucusu ve ağ geçidi
