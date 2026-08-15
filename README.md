# Effi Money — публичный сайт

Статический сайт для App Store: лендинг, политика конфиденциальности и
поддержка. Публикация через GitHub Pages, без сервера.

## Публичные адреса (после включения Pages)

Подставьте свой GitHub-логин вместо `USERNAME` и имя репозитория
`effi-money-site`:

- https://USERNAME.github.io/effi-money-site/
- https://USERNAME.github.io/effi-money-site/privacy/
- https://USERNAME.github.io/effi-money-site/support/

В приложении URL политики задаётся в
`lib/core/legal/legal_config.dart` (`kPrivacyPolicyUrl`).

## Как опубликовать

1. Создайте **публичный** репозиторий `effi-money-site` на GitHub.
2. Из этой папки:

```bash
git init
git add .
git commit -m "Add public site: landing, privacy, support"
git branch -M main
git remote add origin git@github.com:USERNAME/effi-money-site.git
git push -u origin main
```

3. На GitHub: **Settings → Pages → Build and deployment**
   - Source: **Deploy from a branch**
   - Branch: **main**, folder: **/ (root)**
   - Save
4. Через 1–2 минуты откройте `/privacy/` в браузере без авторизации.

Файл `.nojekyll` нужен, чтобы GitHub Pages отдавал файлы как есть.
