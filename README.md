# Mahakal Mobile Hub - Android App

Professional e-commerce Android app for mobile shop (Indore based).

## Features

- Clean modern UI inspired by Amazon / Ovantica
- Categories: New Smartphones, Refurbished, Accessories, Repair Services
- Product detail pages with specs, pricing, warranty
- Cart + Checkout
- **WhatsApp integration** for orders & inquiries (no AI)
- **Indore**: 2-hour delivery + COD
- **All India**: Shipping available, COD disabled (prepaid only)
- **Admin Panel**: Add / Edit / Delete products, update price & stock in real-time
- Custom Request form (customer can ask for unlisted models)

---

## Sabse Aasaan Tarika - GitHub se APK Banaye (Step by Step)

### Step 1: GitHub Account Banao
1. Browser mein jao → https://github.com
2. Sign up / Sign in karo (free)

### Step 2: Naya Repository Banao
1. GitHub pe **+** button pe click → **New repository**
2. Repository name likho: `MahakalMobileHub`
3. Public select karo
4. **Create repository** pe click karo

### Step 3: Code Upload Karo
**Asaan tarika (Browser se):**
1. Naye repository page pe **uploading an existing file** link pe click
2. Ya "Add file" → "Upload files"
3. Apne computer se **saari files** (folder ke andar ki files) select karke drag & drop karo
   - `lib` folder, `android` folder, `pubspec.yaml`, `.github` folder, README.md sab upload karo
4. Niche **Commit changes** pe click

**Ya ZIP se:**
- Is project ka zip extract karo
- Saari files (folders ke sath) GitHub pe upload karo

### Step 4: APK Automatically Banega
1. Repository mein **Actions** tab pe jao (upar)
2. Pehli baar **I understand my workflows...** pe click karke enable karo
3. Left side mein **Build APK** workflow dikhega
4. **Run workflow** button pe click karo (ya wait karo jab push hua ho)
5. 5-8 minute wait karo (green tick aane tak)
6. Green tick aane ke baad us job pe click karo
7. Niche **Artifacts** section mein **Mahakal-Mobile-Hub-APK** dikhega
8. Uspe click karke **download** kar lo
9. Download hone ke baad unzip karo → andar `app-release.apk` milega

### Step 5: Phone pe Install Karo
1. APK ko phone mein transfer karo
2. Phone settings → Unknown sources / Install unknown apps allow karo
3. APK pe tap karke install karo

---

## WhatsApp Number Change Karna (Zaroori)

File kholo: `lib/utils/constants.dart`

Yeh line dhoondo aur apna number daalo (91 ke sath):

```dart
static const String whatsappNumber = '919876543210'; // yahan apna WhatsApp number
```

Phir GitHub pe phir se upload / commit karo aur naya APK banao.

## Admin Password

Default: `mahakal@123`

Change karna ho to `lib/services/product_service.dart` file mein `mahakal@123` dhoondh ke change karo.

---

## Local Computer pe Banane ka Tarika (Agar Flutter aata ho)

```bash
flutter pub get
flutter build apk --release
```

APK yahan milega: `build/app/outputs/flutter-apk/app-release.apk`

---

Made for Mahakal Mobile Hub, Indore.
