---
layout: post
title: Instalando e configurando Postgresql para Rails
date: 2018-12-25 19:00:00 -0300
description:  # Add post description (optional)
img: 2018-12-26/capa.png # Add image post (optional)
imgpost: 2018-12-26/capa.png # Add image post (optional)
tags: [Ubuntu, Mint, VsCode]
---

Instalar Postgresql
```zsh
sudo apt-get install postgresql postgresql-contrib libpq-dev
```

Instalar GEM
```zsh
gem install pg
```

Criar role para aplicação
```zsh
su - postgres
psql
create role rails_app with createdb login password 'rails_app';
```


