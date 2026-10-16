# Dark Glass Water Theme — Cloud APK Build (মোবাইল থেকে)

এই ZIP-এ Android Studio project এবং GitHub Actions workflow আছে। GitHub Actions-এর মাধ্যমে cloud runner-এ APK build করার জন্য তৈরি। **এই প্রজেক্টের build এখনো এই প্যাকেজ তৈরির পরিবেশে চালিয়ে যাচাই করা হয়নি**, তাই প্রথম run সফল হবে—এ নিশ্চয়তা নয়।

## Termux নিয়ে
আপনার আগের Termux ইনস্টলেশন/Java 17 রেখে দিন। APK বানানোর জন্য এখন আর Termux-এ Android SDK ডাউনলোড বা extract করবেন না। এই cloud পদ্ধতিতে Termux build toolchain দরকার নেই।

## মোবাইল থেকে ধাপ
1. ZIP extract করুন। Extract করা ফোল্ডারের সব project file GitHub repository-তে upload করতে হবে; `.github/workflows/build.yml`-ও অবশ্যই থাকতে হবে।
2. GitHub-এ repository-এর **Actions** tab খুলুন।
3. **Build Dark Glass Water APK** workflow নির্বাচন করে **Run workflow** চাপুন।
4. Build সফল হলে workflow run-এর নিচে **Artifacts** থেকে `DarkGlassWaterTheme-debug-apk` ডাউনলোড করুন।
5. ZIP artifact extract করে `app-debug.apk` ইনস্টল করুন।

## সীমাবদ্ধতা
- এটি standalone demo app; XOS-এর actual home screen, lock screen বা system Control Center বদলায় না।
- app-এর ভেতরের liquid panels accelerometer tilt-এ নড়ে।
- প্রথম build-এ error এলে Actions-এর error log দেখে ঠিক করতে হবে; সফল build আগে থেকে নিশ্চিত নয়।
