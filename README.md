<h3 align="center">yarn global add heroku || npm install --global heroku</h3>
<p align="center">- Baixar heroku CLI</p>

<h3 align="center">heroku login</h3>
<p align="center">- Autentica sua conta heroku onde irá fazer o deploy</p>

<h3 align="center">heroku create NOME_PROJETO_UNICO --buildpack mars/create-react-app</h3>
<p align="center">- Acesse o link do heroku buildpack para mais informações</p>

<h3 align="center">https://github.com/mars/create-react-app-buildpack
ctrl+F: Quick start</h3>
<p align="center">- Crie um arquivo chamado static.json na raiz do projeto e adicione as seguintes configurações:

    {
        "root": "build/",
        "routes": {
            "/**": "index.html"
        }
    }

</p>

<p align="center">- "root" = Informa ao heroku que a build será executada sempre que iniciar o projeto</p>

<h3 align="center">git remote</h3>
<p align="center">- demonstra todas as branchs do projeto</p>

<h3 align="center">- Agora basta fazer o primeiro commit da aplicação:</h3>
<p align="center">
# git add --all
<br/>
# git commit -m "deploy projeto"
<br/>
# git push heroku master</p>

<h3 align="center">heroku config:set NODE_MODULES_CACHE=false</h3>
<p align="center">Para desabilitar caches das dependencias e evitar erros.</p>
    
<h3 align="center">heroku open</h3>
<p align="center">- Irá abrir seu projeto no navegador</p>
