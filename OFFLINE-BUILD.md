# ساخت آفلاین CodeNevis

این نسخه برای کمترین وابستگی Android آماده شده است:

- هیچ کتابخانه AndroidX/Jetpack در `app` استفاده نمی‌شود.
- `MainActivity` فقط از Android Framework API استفاده می‌کند.
- تم فقط از `Theme.Material.NoActionBar` سیستم استفاده می‌کند.
- فایل `CodeNevisAI.html` بدون تغییر در `app/src/main/assets/` باقی مانده است.
- مجوز `INTERNET` وجود ندارد؛ برنامه محتوای خود را از asset محلی باز می‌کند.

## نکته مهم درباره Offline

برای Build کاملاً آفلاین، **خود Gradle + Android Gradle Plugin + Android SDK Platform 35 + Build Tools** باید قبلاً روی سیستم نصب/کش شده باشند. این موارد بخشی از پروژه نیستند.

در Android Studio:

1. پروژه `CodeNevisKotlin` را باز کنید.
2. Gradle را روی Offline Mode قرار دهید: `Settings > Build Tools > Gradle > Offline work`.
3. مطمئن شوید SDK Platform 35 و Build Tools متناظر روی سیستم موجود است.
4. از منوی `Build > Build APK(s)` استفاده کنید.

اگر Android Studio/Gradle اعلام کرد Plugin یا Gradle distribution در cache نیست، یک بار همان نسخه‌ها را در حالت آنلاین دریافت کنید؛ بعد Buildهای بعدی می‌توانند کاملاً آفلاین انجام شوند.

## خروجی APK

پس از Build معمولاً APK در این مسیر قرار می‌گیرد:

`app/build/outputs/apk/debug/app-debug.apk`

برای انتشار، از `Build > Generate Signed Bundle / APK` استفاده کنید.
