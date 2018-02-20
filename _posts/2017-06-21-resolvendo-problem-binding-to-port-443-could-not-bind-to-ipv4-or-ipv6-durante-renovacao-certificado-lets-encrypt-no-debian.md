---
id: 121
title: 'Resolvendo &#8220;Problem binding to port 443: Could not bind to IPv4 or IPv6&#8221; durante renovação certificado Let&#8217;s Encrypt no Debian'
date: 2017-06-21T20:00:54+00:00
author: Jonas Giehl
layout: post
permalink: /resolvendo-problem-binding-to-port-443-could-not-bind-to-ipv4-or-ipv6-durante-renovacao-certificado-lets-encrypt-no-debian/
categories:
  - Sem categoria
---
Hoje, ao realizar a renovação dos certificados Let's Encrypt, estava recebendo a mensagem descrita no título deste post.

No meu caso era exibido porque a porta 443 ocupada pelo apache em execução. Criei o GIST abaixo para manter o procedimento de atualização dos certificados que utilizo atualmente.

{% gist 14e62ed7f969cb693adbcb3e1d00c52b %}