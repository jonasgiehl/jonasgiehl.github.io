---
id: 26
title: Validando regras do Varnish
date: 2011-12-22T02:23:42+00:00
author: Jonas Giehl
layout: post
guid: http://wp.jonas-giehl.com.br/jonas-giehl/?p=26
permalink: /validando-regras-varnish/
image: https://wp.jonas-giehl.com.br/jonas-giehl/wp-content/uploads/sites/3/2011/12/varnish.png
categories:
  - Linux
  - Software Livre
  - Varnish
tags:
  - Cache
  - linux
  - Varnish
---
O Varnish, da mesma maneira que o Apache, permite que o usuário teste a sintaxe da sua nova configuração.

O comando é:

<pre>varnishd -C -f /caminho/ate/arquivo.vcl</pre>

A saída, em caso de erro será algo como:

<pre><span style="color: #993300;">&gt; Message from VCC-compiler: &gt; Expected an action, 'if', '{' or '}' &gt; ('input' Line 82 Pos 6) &gt; vcl_hash(req.http.Cookie);</span></pre>

<pre><span style="color: #993300;">&gt; -----########------------------ &gt; &gt; Running VCC-compiler failed, exit 1</span></pre>

Como você pode ver é muito simples e ajuda na hora de alterar a sua configuração.