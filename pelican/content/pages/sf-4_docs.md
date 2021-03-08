Title: sf-4_docs
Date: 2021-03-08

# [sf__wordpress_staging](https://github.com/DevOps-SKF/sf__docs)

[https://devops-skf.github.io/sf__docs/](https://devops-skf.github.io/sf__docs/) - original url  
[https://sfdocs.arlab.pw/](https://sfdocs.arlab.pw/) - custom domain

Установка:

    python -m pip install "pelican[markdown]"

Создать директорию, перейти в нее, и запустить

    pelican-quickstart

Важные директории:

- /pelican/content - файлы .md и прочие
- /pelican/themes - темы оформелния
- /pelican/output - формируется при запуске `pelican content`
- /docs - содержимое этой диреткории показывается на статическом сайте github.io.
В реальности /pelican/output - линк на /docs.

[https://devops-skf.github.io/sf__docs/](https://devops-skf.github.io/sf__docs/) - "стандартное" обращение к статическим страницам.  
[https://sfdocs.arlab.pw/](https://sfdocs.arlab.pw/) - пользовательский домен.  
Описан как CNAME на devops-skf.github.io  
Также добавлена CAA запись для получения сертификата LetsEncrypt.  

Для тестирования можно запускать `python -m http.server` из /pelican/output/ или /docs/  
Сайт доступен на `http://localhost:8000`

[https://github.com/DevOps-SKF/sf__docs](https://github.com/DevOps-SKF/sf__docs)
