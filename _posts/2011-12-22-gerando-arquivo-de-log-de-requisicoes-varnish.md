---
id: 28
title: Gerando arquivo de log de requisições no Varnish
date: 2011-12-22T02:25:36+00:00
author: Jonas Giehl
layout: post
guid: http://wp.jonas-giehl.com.br/jonas-giehl/?p=28
permalink: /gerando-arquivo-de-log-de-requisicoes-varnish/
image: https://wp.jonas-giehl.com.br/jonas-giehl/wp-content/uploads/sites/3/2011/12/varnish.png
categories:
  - Linux
  - Software Livre
  - Varnish
tags:
  - Cache
  - linux
  - Log
  - Varnish
---
Você pode gerar um arquivo de log com todas as informações das requisições que o Varnish atendeu em dado momento. O comando é:

<pre>varnishlog -w /caminho/ate/arquivo.log</pre>

Referência: <https://www.varnish-cache.org/docs/2.1/reference/varnishlog.html>