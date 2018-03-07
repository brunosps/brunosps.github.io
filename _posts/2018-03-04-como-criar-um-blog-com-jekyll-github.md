---
layout: post
title: Como criar um blog(Jekyll + Github)
date: 2018-03-04 20:32:20 -0300
description: Como criar seu blog de forma fácil e rápida. # Add post description (optional)
img: 2018-03-04/capa.jpg # Add image post (optional)
tags: [Jekyll, Blog, Github, VS CODE]
---
Olá, tudo bem?

Como primeiro post resolvi escrever como criei esse próprio blog.

Foi tudo bem simples, primeiramente dei um 'Fork' no repositorio [Jekyll Now](https://github.com/barryclark/jekyll-now)
![Jekyll Now Github]({{site.baseurl}}/assets/img/2018-03-04/barryclark_jekyll-now.png)
Após o fork, o próprio github cria o repositório do Jekill Now e temos que configurá-lo com o nome do nosso usuário do github. Para isso basta irmos em Settings e modificar o Repository Name.
![Settings]({{site.baseurl}}/assets/img//2018-03-04/settings.png)

Com isso feito já temos nosso blog, acessando a url http://seu_usuario.github.io no meu caso [http://brunosps.github.io](http://brunosps.github.io)

Mas ainda há configurações que devemos realizar para isso resolvi clonar o repositório para trabalhar com ele local. Nessa hora precisamos de ter o git instalado e configurado pois o clone é feito por ele.
```zsh
git clone https://github.com/brunosps/brunosps.github.io.git
```

Primeiro ajuste após o clone é editar o arquivo **_config.yml**, aqui é onde definimos o nome do titulo do blog, a imagem do profile entre outras coisas.
![_config.yml]({{site.baseurl}}/assets/img//2018-03-04/config_yml.png)
Para editar os arquivos estou usando o [VS CODE](https://code.visualstudio.com/)

Com tudo ajustado vamos ao commit e enviar essas alterações para nosso respositório remoto. Para isso utilizaremos o git novamente.
```zsh
git commit -am "Meu primeiro commit local"
```

Após o commit podemos fazer o push para o repositório remoto.
```zsh
git push origin master
```

Ao acessarmos novamente nosso [blog](http://brunosps.github.io) já veremos nossas atualizações.
![Blog brunosps.me]({{site.baseurl}}/assets/img//2018-03-04/blog.png)

Tem muitas outras coisas que podemos configurar para nosso blog como temas e plugins do Jekill, conforme for me aventurando nisso volto a escrever para contar como foi.
