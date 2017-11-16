mpdg.govbr.biblioteca: Biblioteca
====================================
[![Coverage Status](https://coveralls.io/repos/github/Samuelbsb/mpdg.govbr.biblioteca/badge.svg?branch=master)](https://coveralls.io/github/Samuelbsb/mpdg.govbr.biblioteca?branch=master) [![Build Status](https://travis-ci.org/Samuelbsb/mpdg.govbr.biblioteca.svg?branch=master)](https://travis-ci.org/Samuelbsb/mpdg.govbr.biblioteca)

Introdução
-----------

Este pacote provê um conjunto de funcionalidades para gerenciar mensagens do Fale Conosco do portal. Dentre as principais:

- Confirmação da mensagem através de token enviado por email;
- Painel administrativo para gerenciamento das mensagens;
- Busca simples e avançada;
- Possibilidade de encaminhar a mensagem para usuários responsáveis por outros setores;
- Categorização e arquivamento de mensagens;
- Estatísticas de mensagens respondidas, em aberto, em atraso e alerta;
- Mensagens de notificação de email customizadas;

Compatibilidade
---------------

O pacote foi testado em versões do Plone 4.x

Instalação
------------

Para habilitar a instalação deste produto em um ambiente que utilize o
buildout:

1. Editar o arquivo buildout.cfg (ou outro arquivo de configuração) e
   adicionar o pacote `mpdg.govbr.biblioteca` à lista de eggs da instalação:

        [buildout]
        ...
        eggs =
            mpdg.govbr.biblioteca

2. Após alterar o arquivo de configuração é necessário executar
   ''bin/buildout'', que atualizará sua instalação.

3. Reinicie o Plone

4. Acesse o painel de controle e instale o produto
**mpdg.govbr.biblioteca: Arquivo Biblioteca**.

Estado deste pacote
---------------------

O **mpdg.govbr.biblioteca** está em constante atualização e está em sua primeira versão estável aberta. O pacote ainda não possui testes automatizados mas estamos trabalhando para aumentar sua cobertura de testes e assim fornecer uma experiência ainda melhor. Você está convidado a ajudar!

Uso
---

Após instalação, será criado na raiz do Plone site uma pasta chamada "Documentos da Biblioteca" (/documentos-e-arquivos) essa pasta é o local onde serão salvas os arquivos enviados. Também e criado um link chamado "Biblioteca" (/acesso-a-informacao/biblioteca) este link será chamado quando o usuário clicar em Biblioteca na barra de conteudo.

No link estará disponível para que o usuário possa criar uma capa utilizando os Tiles, implementado em Layout encontrado na barra de editação.

Na instalação do produto é criados "Tiles" que fornecem funcionalidades de navegação como arquivos mais acessados, buscas, os recentes adicionados e todos os arquivos adicionados.

Com o produto já instalado o usuário pode criar um portlet de navegação com link para o painel de "Adicionar Arquivo".

No painel Adicionar Arquivo tem a funcionalidade de adicionar arquivos. 

Inicie colocando o titulo, a descrição, referencia o produto (Deverar se ignorado a referencia BoaPratica a menos que o usuário refere-se a um arquivo BoaPratica) e logo depois selecione um arquivo ou escolhe um tipo de arquivo.

Após o preenchimento o usuário deverá clicar no link de salvar ou no link de cancelar, caso o usuário desejar.

O Painel de Adicionar Arquivo é acessível apenas para os usuários que tiverem permissão de editar.

Ao acessar a parta "documentos-e-arquivos", será mostrado todos os arquivos.
