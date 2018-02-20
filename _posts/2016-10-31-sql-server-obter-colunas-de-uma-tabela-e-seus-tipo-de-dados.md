---
id: 66
title: 'SQL SERVER &#8211; Obter colunas de uma tabela e seus tipo de dados'
date: 2016-10-31T14:02:13+00:00
author: Jonas Giehl
layout: post
guid: http://jonas-giehl.com.br/?p=66
permalink: /sql-server-obter-colunas-de-uma-tabela-e-seus-tipo-de-dados/
image: https://wp.jonas-giehl.com.br/jonas-giehl/wp-content/uploads/sites/3/2016/10/sql-server-express1.png
categories:
  - Banco de Dados
  - SQL SERVER
tags:
  - SQL SERVER
---
Em alguns casos, precisamos obter informações sobre os campos de uma tabela em tempo de execução da aplicação. No SQL Server a consulta abaixo pode ser útil.

{% gist bf89a128a1bddef0241b7b0163512fee %}

Quando necessário recuperar essas mesmas informações de várias tabelas, o comando abaixo poderá ajudar.

{% gist 16fe66b1774e7cad8125e5b24056cfc0 %}
