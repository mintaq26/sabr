# سَبْر — خطوات النشر على GitHub

## ١. أنشئي مشروع Firebase (مرة واحدة، نحو عشر دقائق)
1. ادخلي إلى https://console.firebase.google.com بحساب Google، واضغطي **Add project**، وسمّيه `sabr`. (يمكنكِ إيقاف Google Analytics.)
2. من القائمة الجانبية: **Build ← Authentication ← Get started**، ثم في تبويب **Sign-in method** فعّلي **Email/Password**.
3. من القائمة: **Build ← Firestore Database ← Create database**، واختاري أقرب منطقة، ثم **Start in production mode**.
4. في Firestore افتحي تبويب **Rules**، وامسحي ما فيه، والصقي محتوى الملف `firestore.rules`، ثم **Publish**.
5. من أيقونة الترس: **Project settings**، ثم في أسفل الصفحة اضغطي أيقونة الويب `</>`، وسجّلي التطبيق باسم `sabr`.
6. انسخي القيم التي تظهر داخل `firebaseConfig` وضعيها في الملف `config.js` مكان النصوص الفارغة.

## ٢. ارفعي الملفات إلى GitHub
1. أنشئي مستودعًا جديدًا (مثلًا `sabr`).
2. ارفعي **كل الملفات** في هذا المجلد كما هي: `index.html` و`config.js` و`manifest.webmanifest` و`sw.js` والأيقونات.
3. من **Settings ← Pages**: اختاري `Deploy from a branch`، والفرع `main`، والمجلد `/ (root)`، ثم **Save**.
4. بعد دقيقة يظهر الرابط، مثل: `https://اسمك.github.io/sabr/`

## ٣. اسمحي لرابطكِ في Firebase
في Firebase: **Authentication ← Settings ← Authorized domains ← Add domain**، وأضيفي `اسمك.github.io`.

## ٤. أول دخول
- افتحي الرابط، واكتبي أسماء العضوات، ثم اختاري اسمكِ ورمزكِ.
- أرسلي الرابط للعضوات؛ تختار كل واحدة اسمها وتضع رمزها من أربعة أرقام أول مرة، ثم تدخل به من أي جهاز.
- لإضافة سبر إلى الشاشة الرئيسية: Safari ← زر المشاركة ← «إضافة إلى الشاشة الرئيسية».

## إذا نسيت عضوة رمزها
احذفي حسابها من **Authentication ← Users**، ثم من الإعدادات في سبر اضغطي «أعيدي التعيين» بجانب اسمها.
