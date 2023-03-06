---
layout: post
title:  "Configurar Mac para trabajar con Python"
date:   2023-03-06
categories: coding
tags: guía
author: Ramón Molina
---

Changelog

| Fecha  |   |
|---|---|
| 03/06/2023 | versión inicial |


## Instalación de Homebrew
http://brew.sh

```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

```
brew update
```

## Instalación de ohmyzsh
Instalacióln de iterm2
```
brew install iterm2
```
Desde iterm instalamos zsh para que quede accesible para iterm
```
brew install zsh
```

Para cambiar el tema a agnoster modificar la siguiente línea
```
ZSH_THEME="robbyrussel"
ZSH_THEME="agnoster"
```
Instalar las fuentes necesarias
```
git clone https://github.com/powerline/fonts
cd fonts && ./install.sh
```

![image](https://user-images.githubusercontent.com/796634/223115878-5174957d-ef46-4b42-bc5f-ddc1b6650b9a.png)


## Instalando python con pyenv
https://github.com/pyenv/pyenv

Nos permitirá tener varias versiones de python instaladas y cambiar a cada una de ellas según la necesidad.

```
brew install pyenv
pyenv install --list
pyenv install 3.11.2
pyenv global 3.11.2
```
Para que siempre tengamos la versión correcta activa en nuestra terminal
```
vim ˜/.zshrc
```
```
#evaluate pyenv python version
eval "$(pyenv init --path)"
```

## Instalando VSCode
https://code.visualstudio.com/docs/setup/mac


