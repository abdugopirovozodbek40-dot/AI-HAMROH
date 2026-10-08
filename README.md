# Hamroh — Android APK

## Yangi versiya (v3): milliy va zamonaviy ilova

- Milliy uslub: lapis, firuza va oltin ranglar, arka shaklidagi bosh karta, girih naqshi, "Xayrli tong / kun / kech" salomlari, Navro'z banneri.
- Asosiy ekranlar: Bosh (nazorat halqasi, dori qabuli, milliy maslahat), Tahlil (grafik, tendensiya, tarix), Maslahat (o'zbek taomlari bo'yicha tavsiyalar), Profil (ma'lumotlar va shifokorga hisobot).
- "+" tugmasi: qand yoki qon bosimini kiritish, vaqt holatini tanlash, xavfda 103 va shifokor tugmalari.
- Shifokorga hisobot: matnni SMS orqali yuborish (sms: havolasi telefonning xabar ilovasini ochadi).
- Tungi rejim: telefon sozlamasiga qarab avtomatik.

Bu papka Hamroh ilovasining Android versiyasi. Ilova telefonda ishlaydi, ma'lumotlar telefonning o'zida saqlanadi (internet shart emas, faqat Google Fonts shriftlari uchun).

Ilovaning asosiy fayli: `app/src/main/assets/index.html`. Uni brauzerda ham ochish mumkin.

## 1-usul: APK ni GitHub orqali olish (eng oson, kompyuterda dastur kerak emas)

1. github.com da bepul hisob oching va yangi repo yarating (masalan: `hamroh`).
2. Ushbu papkadagi barcha fayllarni repo ga yuklang.
3. Yuklangandan keyin "Actions" bo'limida "Build APK" avtomatik ishga tushadi. 5–10 daqiqa kuting.
4. "Releases" bo'limida yangi versiya chiqadi. Unda `app-debug.apk` fayli bor.
5. Faylni telefonga yuklab oling va o'rnating. Telefon "noma'lum manba" deb ogohlantirsa, Sozlamalar → Ilovalar → Noma'lum ilovalarni o'rnatish bo'limida ruxsat bering.

Repo Private bo'lsa, telefonda GitHub hisobiga kirish kerak bo'ladi.

## 2-usul: Android Studio (kompyuterda)

1. Android Studio ni o'rnating (developer.android.com).
2. File → Open → shu papkani tanlang.
3. Build → Build App Bundle(s) / APK(s) → Build APK(s).
4. Tayyor fayl: `app/build/outputs/apk/debug/app-debug.apk`.

## Muhim

- Bu debug APK. Sinov va ko'rsatish uchun mos. Google Play'ga chiqarish uchun imzolangan release (AAB) va Google Play hisobi (bir martalik taxminan $25) kerak bo'ladi.
- Ma'lumotlar faqat shu telefonda saqlanadi. Bir nechta bemor va shifokor o'rtasida sinxronlash uchun server kerak (`hamroh-mvp` loyihasidagi backend).
- AI tahlil (Claude) hozircha faqat claude.ai dagi demo versiyada ishlaydi. APK ichida qoidaga asoslangan tavsiyalar ishlaydi.
- "103 — Tez yordam" va "Shifokorga qo'ng'iroq" tugmalari telefon qo'ng'iroq oynasini ochadi.
- Tibbiy chegaralar (qand 3.9 / 10 / 13.9 mmol/L, bosim 140/90 / 180/120) namunaviy. Ishlatishdan oldin shifokor tasdiqlashi shart.
