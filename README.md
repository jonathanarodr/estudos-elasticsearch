# estudos-elasticsearch

## Pré-requisitos
* JVM previamente instalada.

## Intalação do Elasticsearch
Após o download do [elasticsearch](https://www.elastic.co/downloads/elasticsearch), descompacte o arquivo em um diretório no qual seu usuário possua permissão de leitura e escrita de arquivos.

## Instalação de plugins
Para instalação de plugins no Elasticsearch, direcione a pasta de arquivos para a pasta plugins.
> O nome da pasta do plugin instalado será a **uri** de acesso no browser.

_Exemplo_:
```
127.0.0.1:9200/_plugin/{pluginName}/
```

## Comandos
O elasticsearch trabalha utilizando a estrutura `/{indice}/{tipo}/{identificator}`.

* `_id`: utilizado para identificar um documento pelo seu id.
```
/{indice}/{tipo}/{id}
```

* `_update`: utilizado para atualizar parcialmente um documento já existente.
```
/{indice}/{tipo}/{id}/_update
```

* `_search`: utilizado para listar todos os resultados encontrados em um tipo informado.
```
/{indice}/{tipo}/_search
```
> Para filtrar os resultados de busca basta informar o parâmetro `q`: `/{indice}/{tipo}/_search?q={param}`

* `_count`: verifica a quantidade de documentos existentes em um tipo dentro de um índice.
```
/{indice}/{tipo}/_count
```
