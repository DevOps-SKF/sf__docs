# SF-4 sf__docs
https://devops-skf.github.io/sf__docs/ - original url
http://sfdocs.arlab.pw/ - custom domain ()


    python -m pip install "pelican[markdown]"
    create directory for the project (site)
    cd sf__wordpress

    # Дважды проверьте, что вы работаете в хранилище исходного Git с помощью:
    git remote -v 

    #Вы должны видеть, что вы используете репозиторий username.github.io-src. Затем клонировать репозиторий в качестве выходного субмодуля git (заменить имя пользователя GitHub):
    git submodule add git@github.com:username/username.github.io.git output

    pelican-quickstart


`python -m http.server` из ./output/ и запустить `http://localhost:8000` 