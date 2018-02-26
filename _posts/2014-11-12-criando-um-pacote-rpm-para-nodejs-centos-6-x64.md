---
id: 30
title: Criando um pacote .RPM para NodeJS no Centos 6 x64
date: 2014-11-12T12:25:13+00:00
author: Jonas Giehl
layout: post
permalink: /criando-um-pacote-rpm-para-nodejs-centos-6-x64/
categories:
  - Desenvolvimento Web
  - Linux
  - Software Livre
tags:
  - linux
  - Node JS
  - rpm
---
Afim de facilitar a instalação do NodeJs no Centos (principalmente quando você necessita de uma versão específica e por algum motivo não for interessante utilizar o **yum**), criei um script de compilação/geração de pacote rpm. O processo é bem simples:

Acesse <a href="https://github.com/jonasgiehl/centos6-nodejs-rpm" target="_blank">https://github.com/jonasgiehl/centos6-nodejs-rpm</a> e faça download/clone dos arquivos.

Em seguida, abra o arquivo defines.mk e altere a diretiva **ver=0.8.14** para a versão desejada. Pelo terminal execute o comando **make rpm**. Este procedimento irá fazer o download da versão escolhida do node, preparar e compilar o pacote rpm. Atenção: para o correto funcionamento, é necessário ter:

  * make
  * wget
  * rpmbuild
  * g++ (for NodeJS compile)

Quando o processo estiver concluído, o pacote estará em ~/rpmbuild/RPMS/_<SuaArquitetura>_

Referências:

<a href="https://github.com/jonasgiehl/centos6-nodejs-rpm" target="_blank">https://github.com/jonasgiehl/centos6-nodejs-rpm</a>

<http://vibol.hou.cc/installing-node-js-on-centos-6-3>
