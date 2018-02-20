---
id: 24
title: Instalando Google Chrome com Yum no Fedora, Centos e Red Hat
date: 2011-10-29T17:11:19+00:00
author: Jonas Giehl
layout: post
guid: http://wp.jonas-giehl.com.br/jonas-giehl/?p=24
permalink: /instalando-google-chrome-com-yum-fedora-centos-e-red-hat/
image: https://wp.jonas-giehl.com.br/jonas-giehl/wp-content/uploads/sites/3/2011/10/chrome.png
categories:
  - Fedora
  - Linux
  - Software Livre
tags:
  - centos
  - chrome
  - fedora
  - linux
  - rpm
---
Este post é uma adaptação <a title="dete" href="http://www.if-not-true-then-false.com/2010/install-google-chrome-with-yum-on-fedora-red-hat-rhel/" target="_blank">deste aqui</a>.

O procedimento abaixo funciona para Fedora 12 ou superior, Centos 6 e Red Hat 6.

Primeiramente, você precisa adicionar o repositório do google que contém os pacotes do chrome. Crie o arquivo  _/etc/yum.repos.d/google.repo_ (caso não existir) e adicione as linhas abaixo:

Se seu sistema operacional for 32 bits

[google-chrome]
  
name=google-chrome &#8211; 32-bit
  
baseurl=http://dl.google.com/linux/chrome/rpm/stable/i386
  
enabled=1
  
gpgcheck=1
  
gpgkey=https://dl-ssl.google.com/linux/linux\_signing\_key.pub
  
Caso seu sistema seja 64 bits:

[google-chrome]
  
name=google-chrome &#8211; 64-bit
  
baseurl=http://dl.google.com/linux/chrome/rpm/stable/x86_64
  
enabled=1
  
gpgcheck=1
  
gpgkey=https://dl-ssl.google.com/linux/linux\_signing\_key.pub

Agora é só instalar:
  
yum install google-chrome-stable

Simples não?