Stock Inventory Android build project

এই ZIP-টি Android Studio-তে খুলে APK বানানোর জন্য প্রস্তুত করা সোর্স প্রজেক্ট। এটি নিজে থেকে APK ফাইল নয়।

APK বানানোর ধাপ:
1. কম্পিউটারে Android Studio ইনস্টল করুন।
2. ZIP ফাইল Extract করুন।
3. Android Studio > Open > StockInventory ফোল্ডার নির্বাচন করুন।
4. Gradle Sync শেষ হওয়া পর্যন্ত অপেক্ষা করুন। SDK 35 ও Android Gradle Plugin ডাউনলোড চাইতে পারে।
5. Build > Build Bundle(s) / APK(s) > Build APK(s) নির্বাচন করুন।
6. সফল হলে app/build/outputs/apk/debug/app-debug.apk ফাইল পাওয়া যাবে।
7. APK ফোনে পাঠিয়ে ইনস্টল করতে পারবেন। ইনস্টল করার সময় Android অনুমতি চাইতে পারে।

অ্যাপের বৈশিষ্ট্য:
- পণ্য যোগ/সম্পাদনা/মুছে ফেলা
- স্টক ও বিক্রয়মূল্য (SAR)
- পণ্য খোঁজা ও কম স্টকের সারাংশ
- JSON ব্যাকআপ/ইমপোর্ট
- ব্রাউজার/WebView সমর্থন করলে বারকোড স্ক্যান

গুরুত্বপূর্ণ:
- ডেটা এই ফোনের অ্যাপের ভিতরে স্থানীয়ভাবে সংরক্ষিত; অনলাইনে অন্য ফোনের সঙ্গে অটো-সিঙ্ক হয় না।
- ফোন বদলানোর আগে অ্যাপের Export/Backup ব্যবহার করুন।
- এই প্রজেক্টে এখনো তৈরি করা/সাইন করা release APK নেই। Android Studio দিয়ে build করতে হবে।


মোবাইল দিয়েই ক্লাউডে APK বানানোর বিকল্প (GitHub Actions):
1. ZIP Extract করে সব ফাইল GitHub-এ নতুন repository-তে upload করুন। Hidden .github ফোল্ডারটিও upload হতে হবে।
2. Repository-তে Actions ট্যাব খুলুন।
3. "Build Stock Inventory APK" workflow নির্বাচন করে "Run workflow" চাপুন।
4. Build সফল হলে workflow run-এর পেজের নিচে Artifacts থেকে "StockInventory-debug-APK" ZIP ডাউনলোড করুন।
5. ZIP Extract করলে app-debug.apk পাবেন।
নোট: GitHub অ্যাকাউন্ট ও ইন্টারনেট প্রয়োজন। GitHub-এর ওয়েব UI-তে ফোল্ডার/ফাইল upload করা কিছুটা কঠিন হতে পারে।
