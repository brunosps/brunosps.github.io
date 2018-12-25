---
layout: post
title: Instalando VsCode Linux Mint(18.03)
date: 2018-12-25 19:00:00 -0300
description:  # Add post description (optional)
img: 2018-12-25/capa.png # Add image post (optional)
imgpost: 2018-12-25/capa.png # Add image post (optional)
tags: [Ubuntu, Mint, VsCode]
---

Adicionar o repositório do VsCode
```zsh
curl https://packages.microsoft.com/keys/microsoft.asc | gpg --dearmor > microsoft.gpg
sudo install -o root -g root -m 644 microsoft.gpg /etc/apt/trusted.gpg.d/
sudo sh -c 'echo "deb [arch=amd64] https://packages.microsoft.com/repos/vscode stable main" > /etc/apt/sources.list.d/vscode.list'
```

Instalando VsCode
```zsh
sudo apt-get update
sudo apt-get install code
```
