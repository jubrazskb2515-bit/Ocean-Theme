# Dark Glass Water Theme — Android Studio project

এটি Infinix Hot 50 Pro / Android 15-এর জন্য একটি বিজ্ঞাপনবিহীন **ইন্টারঅ্যাকটিভ কনসেপ্ট অ্যাপ**। গ্লাস প্যানেলের ভেতরের তরল-ঢেউ অ্যাক্সিলেরোমিটার সেন্সরের সঙ্গে নড়ে।

## গুরুত্বপূর্ণ সীমাবদ্ধতা
- এটি এখন একটি standalone demo app; ফোনের আসল launcher, lock screen, notification shade বা system Control Center-কে প্রতিস্থাপন করে না।
- এই পরিবেশে Android SDK/Gradle ইনস্টল না থাকায় APK compile ও device-test করা যায়নি। তাই এটিকে তৈরি APK বলে দাবি করা হচ্ছে না।
- পুরো হোম স্ক্রিনে চলমান live wallpaper করতে হলে পরবর্তী ধাপে Android `WallpaperService` যোগ করতে হবে। XOS-এর সিস্টেম UI বদলানো সাধারণ APK দিয়ে নিশ্চিত নয়।

## APK বানানোর ধাপ
1. কম্পিউটারে Android Studio ইনস্টল করুন।
2. `DarkGlassWaterTheme` ফোল্ডারটি Android Studio-তে **Open** করুন।
3. Android SDK Platform 35 এবং Gradle sync সম্পন্ন করুন।
4. ফোনে Developer options → USB debugging চালু করে USB-তে যুক্ত করুন।
5. **Run** চাপুন। APK ফাইলের জন্য Build → Build APK(s) ব্যবহার করুন।

## কী আছে
- Dark glass cards, neon typography, simulated waterline and bubbles
- Accelerometer-based tilt response
- No ads, analytics, subscription, or network permission
