WORLD IN CONTEXT — ADMIN / EXPORT SETUP

1. Firebase Console → Authentication → Get started.
2. Sign-in method / Sign-in providers → Google → Enable → Save.
3. Replace feedback/test.html with the included corrected file.
4. Create an admin folder in GitHub and upload admin/index.html inside it.
5. Firestore Database → Rules → replace existing rules with firestore.rules → Publish.
6. Open: https://zopidouanastasia.github.io/world-in-context/admin/
7. Sign in with: zopidou@gmail.com

Notes:
- Existing responses will not have age, because the old form did not save it.
- New responses will store the optional value inside answers.age.
- The dashboard can view responses, show basic stats, and export CSV.
- The admin URL does not provide security by itself; Firestore Rules enforce access.
