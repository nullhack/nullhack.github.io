---
layout: post
title:  "Jekyll+github pages: Criando blogs estáticos e simples de configurar"
date:   2016-01-01 02:13:12 -0200
categories: [jekyll, github]
audience: bloggers, programmers, githubers
tags: [tutorial, jekyll, github-pages]
last_updated: March 14, 2016
keywords: jekyll, github, tutorial
summary: "A simple tutorial about using jekyll and github pages"
---

<div class="objectives">Direto ao ponto</div>

Este tutorial é destinado a usuários GNU/Linux com pouca experiência, que querem criar seu próprio blog.
Estou assumindo que você já tenha baixado e instalado [Ruby](https://www.ruby-lang.org/pt/documentation/installation/), [Rubygems](https://rubygems.org/pages/download), que você tenha uma conta no [github](https://github.com/) com nome de usuário '**GITHUBUSER**' além do programa [git](https://git-scm.com/book/pt-br/v1/Primeiros-passos-Instalando-Git) instalado, assim é possível seguir passos que descreverei a seguir para criar um blog particular e customizável, sem precisar ser um expert em programação.
O guia completo sobre jekyll também pode ser encontrado [aqui](https://jekyllrb.com/docs/installation/). 

Comece no terminal digitando o seguinte comando:

```bash
gem install jekyll
```

Após a instalação, crie um [repositório](https://help.github.com/articles/create-a-repo/) no github, com o nome exatamente igual a **GITHUBUSER.github.io** (sendo GITHUBUSER seu nome de usuário). Então:

```bash
git clone https://github.com/GITHUBUSER/GITHUBUSER.github.io
cd GITHUBUSER.github.io
jekyll new
git add *
git commit -m "First commit"
git push
```

Basta digitar seu usuário e senha do github e quando o processo terminar, seu blog estará disponível no endereço `http://GITHUBUSER.github.io`

Parabéns, seu primeiro blog está criado =D

Para mais informações, leia a postagem completa!


<div class="summary">Jekyll+github pages: criando blogs estáticos e simples de configurar</div>



## Conteúdo 

* [Resumo](#resumo)
* [O que é Jekyll](#jekyll)
* [O que é o github](#github)
* [Github Pages](#github-pages)
* Criando, configurando e mantendo seu próprio blog
	* [Instalando programas e criando um blog](#criando)
	* [Configurando informações pessoais](#configurando)
	* [Editando postagens](#editando)
	* [Melhorando a experiência do usuário utilizando CSS](#melhorando)

---

<div id='resumo'></div> 
## Resumo

Este tutorial visa reproduzir o processo de criação deste blog, possibilitando qualquer usuário criar seu próprio blog gratuito, utilizando a plataforma Github.

Para isso, um leque de aplicativos e serviços WEB são necessários, dentre eles Ruby, Jekyll, Git e usuário na plataforma Github.


<div id='jekyll'></div> 
## Jekyll


[Jekyll](https://jekyllrb.com/docs/home/) é um gerador de sites estáticos simples. Para criação, utiliza padrões pré estabelecidos de páginas e os preenche com conteúdo convertido a partir da linguagem Markdown, criando páginas HTML prontas para serem publicadas. Também é a engine por trás do Github Pages, tornando o processo de publicação neste serviço simples e transparente para o usuário.


<div id='github'></div>
## Github

Github é uma plataforma para hospedagem e publicação e compartilhamento para projetos que utilizam o [GIT](https://git-scm.com/) como software controlador de versão. Possuindo planos gratuitos para projetos que sejam disponibilizados de forma pública e planos comerciais para projetos privados e fechados ao público.

Também possui funcionalidades de rede social (feeds, followers, wiki, etc.), além de ferramentas de produtividade e disponibilização de trechos de código com a ferramenta [Gist](https://gist.github.com/).


<div id='github-pages'></div> 
## Github Pages

Segundo o próprio [github](https://help.github.com/articles/what-are-github-pages/), este serviço provê páginas WEB hospedadas e publicadas através do github.

Com ele, é possível criar e publicar páginas online usando um gerador automático de páginas, além da possibilidade de trabalhar localmente utilizando o controlador de versão GIT, utilizando a linha de comando.

As páginas são disponibilizadas por HTTP, não HTTPS, desta forma não é aconselhável para páginas com conteúdo cujas transações necessitam de segurança (senhas e cartões de crédito por exemplo).

<div class='warning'>Sites disponibilizados desta forma são públicos, mesmo que seu repositório seja privado, cuidado ao disponibilizar dados sensíveis.</div>


## Criando, configurando e mantendo seu próprio blog

<div id='criando'></div>
### Instalando programas e criando um blog

Para conseguir criar um blog utilizando jekyll, é necessário a instalação de alguns programas: [Ruby](https://www.ruby-lang.org/pt/documentation/installation/), [Rubygems](https://rubygems.org/pages/download), [git](https://git-scm.com/book/pt-br/v1/Primeiros-passos-Instalando-Git).

Também é necessário uma conta no github [github](https://github.com/) com nome de usuário '**GITHUBUSER**'.
 
Comece no terminal digitando o seguinte comando:

<div class='bash'>Instalando o Jekyll</div>
```bash
gem install jekyll
```

Em seguida, crie um [repositório](https://help.github.com/articles/create-a-repo/) no github, com o nome exatamente igual a **GITHUBUSER.github.io** (sendo GITHUBUSER seu nome de usuário). 

<div class='warning'>O nome do repositório tem de ser exatamente o citado, caso contrário o github não reconhecerá a página como uma página acessável pela URL: http://GITHUBUSER.github.io</div>

Então:

<div class='bash'>Criando uma nova página</div>
```bash
git clone https://github.com/GITHUBUSER/GITHUBUSER.github.io
cd GITHUBUSER.github.io
jekyll new
git add *
git commit -m "First commit"
git push
```

Basta digitar seu usuário e senha do github e quando o processo terminar, seu blog estará disponível no endereço `http://GITHUBUSER.github.io`


<div id='configurando'></div> 
### Configurando informações pessoais

O arquivo `GITHUBUSER.github.io/_config.yml` contém configurações para o nome do autor, e-mail e conta do github, além de outras informações configuráveis

```
# Welcome to Jekyll!
#
# This config file is meant for settings that affect your whole blog, values
# which you are expected to set up once and rarely need to edit after that.
# For technical reasons, this file is *NOT* reloaded automatically when you use
# 'jekyll serve'. If you change this file, please restart the server process.

# Site settings
title: BLOG-TITLE
#email: your-email@domain.com
description: > # this means to ignore newlines until "baseurl:"
  Just a blog to talk about things I like. If you want to read good tutorials,
  thoughts, tips and tricks about computers, free software or photography. this is your place \0.
baseurl: "" # the subpath of your site, e.g. /blog
url: "http://YOURSITE.com
twitter_username: TWITTERUSER
github_username: GITHUBUSER

# Build settings
markdown: redcarpet
```

Basta alterar as configurações de acordo com suas necessidades pessoais e seu blog estará pronto e configurado.

<div id='editando'></div>
### Editando postagens

Criar e editar postagens é simples, basta criar um novo arquivo na pasta `GITHUBUSER.github.io/_posts`, este arquivo deve ter tags indicando algumas características do documento, além de ser possível criar outras que sejam úteis para manutenção do documento, neste blog, utilizo o seguinte arquivo padrão:

```html
--- 
layout: post
title:  "Jekyll+github pages: Criando blogs estáticos e simples de configurar"
date:   2016-01-01 02:13:12 -0200
categories: [jekyll, github]
audience: bloggers, programmers, githubers
tags: [tutorial, jekyll, github-pages]
last_updated: Jan 3, 2016
keywords: jekyll, github, tutorial
summary: "A simple tutorial about using jekyll and github pages"
---

CORPO DA POSTAGEM
```

Para inserção de títulos, links, imagens e outros marcadores de texto, utiliza-se a linguagem [Markdown][github-pages-markdown]. Os comandos básicos para edição de postagens são:

#### - Cabeçalhos

```
## Cabeçalho de tamanho 2
### Cabeçalho de tamanho 3
...
###### Cabeçalho de tamanho 6
```

> ## Cabeçalho de tamanho 2
> ### Cabeçalho de tamanho 3
> ...
> ###### Cabeçalho de tamanho 6

#### - Ênfase

```
*Itálico* ou _Itálico_
**Negrito** ou __Negrito__
**_Misto_**
```
*Itálico*

**Negrito**

**_Misto_**

#### - Listas

```
1. lista numérica
2. lista numérica
  3. lista numérica

* lista simples
* lista simples
  * lista simples
```

1. lista numérica
2. lista numérica
  3. lista numérica

* lista simples
* lista simples
  * lista simples

#### - Links e Imagens

```
[link]({{ site.url }}/jekyll/github/2016/01/01/jekyll-and-github-pages.html)
![Imagem]({{ site.url }}/css/success.png)
```
[link]({{ site.url }}/jekyll/github/2016/01/01/jekyll-and-github-pages.html)

![Imagem]({{ site.url }}/css/success.png)

#### - Miscelânea

```
> Citações
--- Linha separatória
```

> Citações

---


<div id='melhorando'></div>
### Melhorando a experiência do usuário utilizando CSS 

Para criar tags personalizadas, podemos alterar o arquivo `GITHUBUSER.github.io/css/main.scss`. Abaixo estão alguns exemplos de folha de estilos para criação de algumas tags personalizadas utilizadas nesta página:


```css

//message styles
.info {
	border: 1px solid;
	border-radius: 10px;
	margin: 10px 0px;
	padding:15px 10px 15px 50px;
	background-repeat: no-repeat;
	background-position: 10px center;
	color: #00529B;
	background-color: #BDE5F8;
	background-image: url('info.png');
}


//programming styles
.bash {
	border: 1px solid;
	font-weight: bold;
	border-radius: 20px 0px 0px 0px;
	padding:15px 10px 15px 50px;
	background-repeat: no-repeat;
	background-position: 0px center;
	background-size: 50px 50px;
	color: #FFFFFF;
	background-color: #000000;
	background-image: url('bash.png');
}

//title styles
.summary {
	border: 1px solid;
	border-radius: 10px 0px 10px 10px;
	margin: 10px 0px;
	padding:15px 10px 15px 50px;
	background-repeat: no-repeat;
	background-position: 0px center;
	background-size: 70px 70px;
	font-weight: bold;
	text-align: center;
	color: #FFFFFF;
	background-color: #666666;
	background-image: url('summary.png');
}
```

Utilizando a tag `<div class="info">Info message</div>`
<div class="info">O resultado é esta barra informativa!</div>

Utilizando a tag `<div class="bash">Bash</div>`
<div class="bash">Bash</div>

```bash
Criamos uma barra informativa que pode ser útil para identificar linhas de código
```

A tag `<div class="summary">Mensagem</div>` pode ser útil para criar cabeçalhos personalizados como abaixo:
<div class="summary"> Insira um título criativo aqui!  =D</div>

Os ícones utilizados podem ser obtidos [aqui][icons-knob] ou aqui: ![INFO]({{ site.url }}/css/info.png) ![SUCCESS]({{ site.url }}/css/success.png) ![WARNING]({{ site.url }}/css/warning.png) ![ERROR]({{ site.url }}/css/error.png)

---

## references: 

* [https://milanaryal.com/2015/writing-on-github-pages-and-jekyll-using-markdown/][github-pages-markdown]
* [http://www.jankoatwarpspeed.com/css-message-boxes-for-different-message-types/][css-messages]
* [http://itweek.deviantart.com/art/Knob-Buttons-Toolbar-icons-73463960][icons-knob]
 
---

[github-pages-markdown]: https://milanaryal.com/2015/writing-on-github-pages-and-jekyll-using-markdown/
[css-messages]: http://www.jankoatwarpspeed.com/css-message-boxes-for-different-message-types/
[icons-knob]:http://itweek.deviantart.com/art/Knob-Buttons-Toolbar-icons-73463960
