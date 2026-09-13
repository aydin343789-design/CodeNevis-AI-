# کدنویس — نسخه Android/Kotlin

این پروژه یک پوستهٔ Android با Kotlin است که فایل اصلی `CodeNevisAI.html` را به‌صورت محلی داخل WebView اجرا می‌کند.

هدف این ساختار حفظ کامل ظاهر، رنگ‌بندی Luxury، منطق چت‌بات، درس‌ها، کوییزها، پیشرفت، XP، مدال‌ها، پرمیوم، واژه‌نامه، گواهینامه و ذخیره‌سازی آفلاین فایل اصلی است؛ بنابراین منطق آموزشی موجود در HTML بازنویسی یا تغییر داده نشده است.

## اجرا

پروژه را در Android Studio باز کنید و ماژول `app` را اجرا کنید.

فایل آموزشی در این مسیر قرار دارد:

`app/src/main/assets/CodeNevisAI.html`

برنامه برای اجرای محلی فایل HTML به مجوز اینترنت نیاز ندارد.

## Offline/minimal-dependency edition

This project has been prepared for offline-friendly builds with zero AndroidX runtime dependencies. The Android shell uses only framework APIs, while the original HTML/CSS/JavaScript application remains the local asset and is not modified.

See `OFFLINE-BUILD.md` for offline build requirements and steps.
