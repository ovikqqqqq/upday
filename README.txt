UPDAY — сборка с Firebase

Перед запуском:
1. В index.html найди объект firebaseConfig и замени все PASTE_* значениями из Firebase Console → Project settings → Your apps → Config.
2. В Authentication → Settings → Authorized domains добавь домен сайта.
3. Размести файлы на HTTPS-хостинге (например, Firebase Hosting). Не открывай index.html как file://.
4. Открой сайт и нажми «Ещё» → «Войти через Google».

Путь документа Firestore: users/{uid}/app/state.
Правила Firestore должны разрешать доступ только владельцу uid. Используй правила, которые настроили в Firebase Console.

Если вход не работает, проверь Google provider, Authorized domains и firebaseConfig.
Не публикуй пароль Google, OAuth client secret или приватные ключи. Firebase Web config используется в клиентском приложении; безопасность данных обеспечивают правила Firestore.

Ограничения: Apple Health, каталог продуктов и push-уведомления пока не подключены. Для Apple Health понадобится нативная iOS-обёртка с HealthKit.
Установка на iPhone: открой сайт по HTTPS в Safari → Поделиться → На экран Домой.
