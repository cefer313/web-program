# Web / Program — Claude üçün təlimat

Bu repozitoriya istifadəçinin saytları, veb-tətbiqləri, mobil tətbiqləri və oyunları üçündür.
Dil dərslikləri burada deyil (`ingilis_dili`, `fars-dili`, `-r-b-dili`), videolar `iphone` repozitoriyasındadır.
Bu fayldakı qaydalara hər söhbətdə əməl et.

## Ünsiyyət

- Həmişə **Azərbaycan dilində** cavab ver. İstifadəçi proqramçı deyil: sadə dillə izah et, texniki terminləri lazım olanda qısaca aç.
- Bilmədiyin və ya yoxlaya bilmədiyin şeyi açıq de. Uydurma.
- Bir neçə yol varsa, birini tövsiyə et və qısa səbəbini de; uzun siyahı vermə.

## Git qaydaları

- Bu repozitoriyada dəyişiklikləri **birbaşa `main` budağına** yaz və göndər.
- Hər yeni layihə əlavə olunanda kök `README.md`-dəki layihələr cədvəlini yenilə (ad, nədir, necə açılır/link).
- `node_modules/`, build qovluqları və böyük yaradılmış fayllar repoya əlavə olunmur (`.gitignore`).

## Qovluq quruluşu

- Hər layihə öz qovluğunda: `<layihe-adi>/` (kiçik hərf, tire ilə, latın hərfləri: məs. `baxisini-deyis/`, `fikir-tutan/`).
- Hər layihədə qısa `README.md`: nədir, necə açılır/işə salınır, harada yayımlanıb.
- GitHub Actions faylları kökdə, `.github/workflows/` qovluğunda olur; hər workflow yalnız öz layihəsinin qovluğu dəyişəndə işləsin (`paths:` filtri).

## Saytlar və veb-tətbiqlər

- Mətnlər **Azərbaycan dilində**; istifadəçi istəsə, AZ / RU / EN dil seçimi (mətnlər ayrıca tərcümə faylında).
- Şrift Azərbaycan hərflərini, xüsusilə böyük **Ə**-ni dəstəkləməlidir: **Inter**, **Montserrat** uyğundur (Manrope böyük Ə-ni dəstəkləmir).
- Telefon üçün də işləməlidir (responsive): telefonda üfüqi sürüşmə olmasın.
- Sadə layihələr üçün çərçivəsiz HTML/CSS/JS üstündür; lazım olanda kitabxana işlət.
- **Uydurma məlumat yazma**: əlaqə məlumatı, rəylər, statistika, qiymət verilməyibsə — nümunə olduğunu açıq qeyd et və istifadəçidən əsl məlumatı istə.
- Təhvil verməzdən əvvəl Playwright ilə kompüter və telefon ölçüsündə ekran şəkli çıxarıb bax, brauzer xətalarını yoxla.
- İstifadəçi baxmaq üçün link istəyəndə: Artifact önizləməsi (yalnız istifadəçiyə açıq) və ya GitHub Pages (hamıya açıq).

## Mobil tətbiqlər

- Saytdan tətbiq: **Capacitor** (Android + iOS) və/və ya **PWA** (ana ekrana əlavə et, offline).
- Android APK GitHub Actions-da yığılır (bulud mühitində Android SDK yükləmək bloklanır). APK yükləmə yerini istifadəçiyə izah et.
- iOS tətbiqi yığmaq üçün Mac + Xcode lazımdır; App Store üçün Apple Developer hesabı ($99/il). Bunu açıq de.

## Oyunlar

- Sadə brauzer oyunları: tək HTML faylında və ya kiçik layihə kimi; həm siçan, həm toxunuşla idarə olunsun.
- Məlum oyunların surətini (adı, personajları, dizaynı) yaratma; orijinal oyun hazırla.

## Mövcud layihələr (hələ `iphone` repozitoriyasında)

Bunları istifadəçi istəsə bu repozitoriyaya köçür:
- **"Baxışını dəyiş"** saytı və tətbiqi — `iphone` repozitoriyasının əsas budağında: `www/`, `android/`, `ios/`, `capacitor.config.json`, `.github/workflows/android.yml`, `pages.yml`.
- **"Fikir Tutan"** oyunu — `iphone`, budaq `claude/focused-thompson-ma5y47`.
- **"Şəriət məsələləri"** kitab oxuyucusu (+ iOS workflow) — `iphone`, budaq `claude/friendly-keller-lza1y9`.

## Yeni qaydalar

İstifadəçi yeni qayda və ya üstünlük deyəndə (məs. "bundan sonra belə et"):
1. Onu bu fayla, uyğun bölməyə əlavə et (uyğun bölmə yoxdursa, aşağıdakı siyahıya).
2. Dəyişikliyi dərhal `main`-ə göndər.
3. İstifadəçiyə qısaca hansı qaydanı yadda saxladığını de.

### Əlavə olunmuş qaydalar (tarixlə)

- 2026-11-25 — Bu fayl yaradıldı.
