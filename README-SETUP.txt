GB KITCHEN PWA — FREE DEPLOYMENT
1) Firebase Console > Authentication > Sign-in method: enable Email/Password.
2) Firestore Database: create in Production mode; publish firestore.rules from this folder.
3) Firebase Authentication > Users: Add user nikchit@gmail.com (your owner login) and employees.
   Owner email is automatically treated as owner by the rules. For each employee, copy their UID.
4) Firestore > Start collection users > document ID = employee UID; add field active (boolean) = true.
   (Owner doesn't need a users document.)
5) Host these files on GitHub Pages: index.html, firebase-config.js, manifest.json, sw.js, icon.svg.
   GitHub repo Settings > Pages > Deploy from branch (main/root). Open the generated HTTPS URL.
6) On Android Chrome: menu > Install app. On iPhone Safari: Share > Add to Home Screen.
Never share passwords or Firebase service-account keys. Firebase web config is public by design; database rules protect data.
