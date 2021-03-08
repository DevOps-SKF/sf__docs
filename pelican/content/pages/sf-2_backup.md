Title: sf-2_experimental_backup
Date: 2021-03-08

# [Бэкап на Яндекс.Диск](https://github.com/DevOps-SKF/sf__wordpress_experimental)

В предыдущий репозиторий [sf__wordpress_experimental](https://github.com/DevOps-SKF/sf__wordpress_experimental) добавлен скрипт `btoya.sh` (backup to Yandex).

Для работы через WebDAV регистрирую не API (https://oauth.yandex.ru/), а пароль приложения (https://passport.yandex.ru/profile/)

Из соображений безопасности в скрипт учетные данные передаются как переменные окружения. Например, можно прописать в .bashrc:

    export YA_user=username # имя аккаунта в Яндексе
    export YA_webdavkey=app-secretkey # ключ, показанный при создании пароля приложения

Впрочем, похоже, что  функциональность хранения бэкапов на бесплатном Яндекс Диск урезали (https://qna.habr.com/q/677787)

P.S.  
При желании видеть прогресс загрузки curl (`--progress-bar`) обязатально добавить также `> /dev/null`

[https://github.com/DevOps-SKF/sf__wordpress_experimental](https://github.com/DevOps-SKF/sf__wordpress_experimental)
