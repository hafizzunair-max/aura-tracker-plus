AURA TRACKER PLUS — PWA / ANDROID SETUP (Roman Urdu)

Is version mein installable PWA aur offline cache add kiya gaya hai.

PART 1 — Laptop par test
1. ZIP ko Extract All karein.
2. VS Code mein File > Open Folder par click karein.
3. AuraTracker-Plus folder select karein.
4. VS Code Extensions mein "Live Server" install karein (agar pehle se nahi hai).
5. index.html par right-click > Open with Live Server.
6. Chrome/Edge mein app khul jayegi. Browser DevTools > Application mein Manifest aur Service Worker check kar sakte hain.
7. Pehli dafa app ko internet/local server par load hone dein. Phir browser ko offline karke reload test karein.

PART 2 — Android phone par install
Installable PWA ke liye app ko HTTPS website par host karna zaroori hai. Sirf index.html ko WhatsApp se bhejna ya file manager se kholna install/offline service worker enable nahi karega.

Asaan free tareeqa (GitHub Pages):
1. GitHub par sign in karein aur naya public repository banayein, misaal: aura-tracker-plus.
2. Is folder ke andar ki tamam files/folders repository mein upload karein — index.html, manifest.webmanifest, sw.js, icons folder.
3. Repository > Settings > Pages par jayein.
4. Build and deployment mein Deploy from a branch choose karein.
5. Branch: main aur folder: /(root) select karke Save karein.
6. GitHub jo HTTPS website link de, usay Android Chrome mein open karein.
7. Chrome menu (three dots) > Install app ya Add to Home screen choose karein. Menu ka lafz phone/browser ke mutabiq mukhtalif ho sakta hai.
8. Install ke baad app icon se khol kar check karein.

DATA / IMPORTANT:
- Habits abhi isi browser/device ke LocalStorage mein save hoti hain; cloud sync nahi hai.
- Browser data clear karne ya app ko doosre browser/device par kholne se data automatically transfer nahi hota. Preferences & Data mein JSON export/backup ka option use karein.
- Offline caching pehli successful online load ke baad kaam karti hai. Update ke baad naya version load hone ke liye app ko band karke dobara kholna par sakta hai.
- PWA browser notifications aur reliable scheduled alarms is build mein shamil nahi; is liye isay reminder/alarm feature samajh kar rely na karein.
- GitHub Pages par repository public ho sakti hai, lekin app ka habit data GitHub par upload nahi hota; woh browser ke local storage mein rehta hai.

Troubleshooting:
- Service worker sirf HTTPS ya localhost par kaam karta hai; file:// se nahi.
- Agar install option na aaye, website ko Chrome mein open karein, page reload karein aur kuch seconds wait karein.
