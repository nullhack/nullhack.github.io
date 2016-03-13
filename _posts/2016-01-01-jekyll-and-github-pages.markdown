---
layout: post
title:  "Jekyll+github pages: Criando blogs estáticos e simples de configurar"
date:   2016-01-01 02:13:12 -0200
categories: [jekyll, github]
audience: bloggers, programmers, githubers
tags: [tutorial, jekyll, github-pages]
last_updated: March 8, 2016
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


<div class="summary">Jekyll+github pages: Criando blogs estáticos e simples de configurar</div>



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

<div id='resumo'/> 

## Resumo


<div id='jekyll'></div> 
## Jekyll


<div id='github'></div>
## Github

<div id='github-pages'></div> 
## Github Pages

## Criando, configurando e mantendo seu próprio blog

<div id='criando'></div>
### Instalando programas e criando um blog

<div id='configurando'></div> 
### Configurando informações pessoais

<div id='editando'></div>
### Editando postagens

<div id='melhorando'></div>
### Melhorando a experiência do usuário utilizando CSS 


<div class="info">Info message</div>

<div class="success">Successful operation message</div>

<div class="warning">Warning message</div>

<div class="error">Error message</div>



<div class="bash">Bash</div>
{% highlight bash %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
{% endhighlight %}


<div class="cpp">CPP</div>
{% highlight bash %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
{% endhighlight %}


<div class="python">Python</div>
{% highlight python linenos=table %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
{% endhighlight %}

{% include icon-flickr.svg %}

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

references: 

* https://milanaryal.com/2015/writing-on-github-pages-and-jekyll-using-markdown/

* https://keybase.io/

* http://www.jankoatwarpspeed.com/css-message-boxes-for-different-message-types/

* http://itweek.deviantart.com/art/Knob-Buttons-Toolbar-icons-73463960
 


[jekyll-docs]: http://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
