Goutte
================================

[![Build Status](https://travis-ci.org/MasterkeyInformatica/goutte.svg?branch=master)](https://travis-ci.org/MasterkeyInformatica/goutte)

Goutte é uma biblioteca de captura e leitura de tela escrita em PHP. Esta ferramenta porvê uam API rica
para realizar leitura de respostas HTML/XML.

Requirements
------------

Goutte depende de PHP 5.5+ e Guzzle 6+.

Instalação
----------

Adicione ``masterkey/goutte`` como dependência em seu arquivo ``composer.json``:


    composer require masterkey/goutte

Uso
---

Cria uma instância da classe Client (que extende ``Symfony\Component\BrowserKit\Client``):


    use Goutte\Client;

    $client = new Client();

Realiza requests com o método ``request()``:

    // Vai ao site Symfony.com
    $crawler = $client->request('GET', 'http://www.symfony.com/blog/');

O método retorna um objeto ``Crawler`` (``Symfony\Component\DomCrawler\Crawler``).

Mais Informações
----------------

Este pacote foi Baseado no pacote [Goutte](https://github.com/FriendsOfPHP/Goutte).
