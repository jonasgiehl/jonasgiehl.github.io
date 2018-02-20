---
id: 60
title: 'SQL Server &#8211; Identificar índices pouco ou não utilizados'
date: 2016-09-30T17:17:29+00:00
author: Jonas Giehl
layout: post
guid: http://wp.jonas-giehl.com.br/jonas-giehl/?p=60
permalink: /sql-server-identificar-indices-pouco-ou-nao-utilizados/
image: https://wp.jonas-giehl.com.br/jonas-giehl/wp-content/uploads/sites/3/2016/09/sql-spaceused-001.png
categories:
  - Banco de Dados
  - SQL SERVER
tags:
  - GIST
  - SQL SERVER
---
Em nossas bases de dados de produção, com o passar do tempo de vida da aplicação  e da evolução do software, alguns índices criados para aumentar a performance passam a não faz mais sentido. Em algum momento os mesmos passam a atrapalhar mais do que ajudar, uma vez que os mesmos são afetados por operações de insert/update/delete.

Baseado no artigo http://imasters.com.br/desenvolvimento/indices-e-o-excesso-de-coisa-boa-parte-02-objetos-sem-uso/ elaborei o gist abaixo para identificar os índices menos utilizados. No meu caso, optei por remover índices do ixratio menor que 1.

<div class="oembed-gist">
  <noscript>
    View the code on <a href="https://gist.github.com/jonasgiehl/0377e7d0776454f87ab6b11476a3f545">Gist</a>.
  </noscript>
</div>