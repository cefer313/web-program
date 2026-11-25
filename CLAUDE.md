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

## Mövcud layihələr

- **`baxisini-deyis/`** — "Baxışını dəyiş" motivasiya saytı (AZ/RU/EN, PWA), Capacitor ilə Android/iOS tətbiqi,
  `www/game.html` — "Fikir Tutan" oyunu, `www/serieet/` — "Şəriət məsələləri" kitab oxuyucusu.
  - **Vacib:** kitab mətni nəşriyyatın icazəsi ilə, nəşriyyatın adı qeyd edilmək şərti ilə dərc olunur — `serieet/` səhifəsində və ana səhifədəki kitab bölməsində bu qeyd **silinməməlidir**. Kitab mətni dəyişdirilmir (PDF-dən avtomatik çıxarılır, `tools/verify.py` ilə yoxlanır).
  - Workflow-lar: `.github/workflows/baxisini-deyis-android.yml`, `-ios.yml`, `-pages.yml` (Pages əl ilə işə salınır).

## Yeni qaydalar

İstifadəçi yeni qayda və ya üstünlük deyəndə (məs. "bundan sonra belə et"):
1. Onu bu fayla, uyğun bölməyə əlavə et (uyğun bölmə yoxdursa, aşağıdakı siyahıya).
2. Dəyişikliyi dərhal `main`-ə göndər.
3. İstifadəçiyə qısaca hansı qaydanı yadda saxladığını de.

### Əlavə olunmuş qaydalar (tarixlə)

- 2026-11-25 — Bu fayl yaradıldı.
- 2026-11-25 — "Baxışını dəyiş" saytı/tətbiqi, "Fikir Tutan" oyunu və "Şəriət məsələləri" oxuyucusu `iphone`-dan köçürüldü və birləşdirildi.
