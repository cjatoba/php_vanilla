# php_vanilla
Projeto desenvolvido para agrupar conteúdos relacionados ao uso do PHP puro

## Ferramentas utilizadas

- [XAMPP 7.4.22 / PHP 7.4.22](https://www.apachefriends.org/download.html)
- [Instalação global do Composer](https://getcomposer.org/doc/00-intro.md#globally)

## Configurações iniciais

### Configuração do Composer

- Iniciar o composer no projeto:
```
composer init
```
- Serão solicitadas algumas informações para configuração do projeto e após será gerado um arqivo 'composer.json', que listará todas as dependências do projeto.

### Autoloader

- Criar um diretório onde ficarão as classes do projeto, utilizaremos neste projeto o diretório app:
```
mkdir app
```
- Abrir o arquivo composer.json e configurar o autoloader:
```json
...
"require": {},
"autoload": {
      "psr-4": {
          "App\\": "app"
      }
  }
...
```

