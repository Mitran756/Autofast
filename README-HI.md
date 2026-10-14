# Ride Fare Filter — शुरुआती Android प्रोजेक्ट

यह Kotlin आधारित Android demo है। यह न्यूनतम/अधिकतम किराया सेट करने और नकली टेस्ट किराये को MATCH या SKIP दिखाने देता है।

## अभी क्या करता है?
- न्यूनतम किराया, डिफ़ॉल्ट ₹100
- अधिकतम किराया, डिफ़ॉल्ट ₹500
- नकली टेस्ट राइड का किराया डालकर फ़िल्टर जाँच
- कोई नेटवर्क, लॉगिन, OTP या दूसरी ऐप की स्क्रीन एक्सेस नहीं
- कोई वास्तविक राइड स्वीकार नहीं करता

## मोबाइल से APK बनाना (GitHub Actions)
1. GitHub पर नया खाली repository बनाएँ।
2. इस ZIP को extract करें और इसके अंदर की सभी फ़ाइलें repository में upload करें। `.github/workflows/build-apk.yml` भी शामिल होनी चाहिए।
3. GitHub repository में **Actions** टैब खोलें।
4. `Build Android APK` workflow चुनें और **Run workflow** दबाएँ (या `main` पर फ़ाइलें push करें)।
5. Build पूरा होने पर workflow run के नीचे **Artifacts** में `RideFilterStarter-debug-apk` डाउनलोड करें।
6. ZIP को extract करें; `app-debug.apk` आपके Vivo Y56 में इंस्टॉल किया जा सकता है। केवल अपने बनाए हुए APK को इंस्टॉल करें।

## महत्वपूर्ण
- यह production-ready ऐप नहीं है।
- Rapido, Ola या Uber से राइड डेटा नहीं लेता और auto-accept नहीं करता।
- वास्तविक इंटीग्रेशन से पहले संबंधित प्लेटफ़ॉर्म की अनुमति/आधिकारिक API और ऐप की शर्तें जाँचें।
- Google Play पर Accessibility API का इस्तेमाल करने के लिए नीति और खुलासा/सहमति की शर्तें लागू हो सकती हैं।
