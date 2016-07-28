---
layout: post
title:  ""
date:   2016-07-28 18:13:12 -0200
categories: [vim]
audience: programmers
tags: [tutorial, vim]
last_updated: June 27, 2016
keywords: vim
summary: "Using vim as hexeditor for binary files"
---

<div class="summary">Ideias</div>

O vim não tem suporte por padrão à codificação hexadecimal derivada de arquivos binários, para obter este resultado temos que fazer uma pequena gambiarra, tranformamos o conteúdo em HEX e em seguida desviamos o fluxo para o arquivo corrente, como exemplificado abaixo:


<div class="bash">Vim</div>
{% highlight bash %}
:%!xxd
{% endhighlight %}

Após as alterações, podemos fazer o processo inverso transformando o conteúdo hexadecimal em fluxo binário e reescrevendo o arquivo corrente antes de salvá-lo e concluir as alterações.

<div class="bash">Vim</div>
{% highlight bash %}
:%!xxd -r
{% endhighlight %}


