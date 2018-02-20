---
id: 40
title: 'Corrigindo erro &#8220;This computer can’t connect to the remote computer because the Remote Desktop Gateway server is temporarily unavailable. Try reconnecting later or contact your network administrator for assistance.”'
date: 2015-03-04T13:44:10+00:00
author: Jonas Giehl
layout: post
guid: http://wp.jonas-giehl.com.br/jonas-giehl/?p=40
permalink: /corrigindo-erro-computer-cant-connect-remote-computer-remote-desktop-gateway-server-temporarily-unavailable-try-reconnecting-later-contact-network-adminis/
image: https://wp.jonas-giehl.com.br/jonas-giehl/wp-content/uploads/sites/3/2015/03/RDS.png
categories:
  - Remote Desktop Services
  - Windows Server
tags:
  - 2012 R2
  - Desktop
  - Gateway
  - RDS
  - Remote
  - Windows
---
Recentemente, durante a configuração de um ambiente de testes para Remote Desktop Services no Windows Server 2012 R2, recebia a seguinte mensagem tentando realizar uma conexão ao servidor a partir das máquinas da rede:

> This computer can’t connect to the remote computer because the Remote Desktop Gateway server is temporarily unavailable. Try reconnecting later or contact your network administrator for assistance.

Após inúmeros testes, conseguir resolver o problema, colocando o computador cliente no mesmo domínio do servidor, e apontando o DNS para o Ip do Servidor RDS.

Outras opções:

http://blogs.msdn.com/b/hyperyash/archive/2012/12/11/remote-desktop-services-gateway-configuration-for-rds-farm.aspx