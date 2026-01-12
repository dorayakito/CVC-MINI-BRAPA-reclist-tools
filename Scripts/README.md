# Scripts de Compatibilidade (Phonemizer BRAPA)

Este diretório contém scripts desenvolvidos para garantir a compatibilidade de listas de fonemas com o Phonemizer BRAPA no [OpenUtau](https://github.com/stakira/OpenUtau).

## Pré-requisitos

Para a execução dos scripts, é necessário ter o Python instalado (versão 3.10 ou superior).

* [Download do Python](https://www.python.org/downloads/)

## Instruções de Uso

Após a conclusão da configuração do arquivo `oto.ini`, os scripts devem ser executados rigorosamente na ordem descrita abaixo:

### 1. Separador_BRAPA

Este script realiza a análise dos fonemas, identificando apenas aqueles que necessitam de alteração de *alias*.

* **Resultado:** Geração do arquivo `edit.txt`.

### 2. Aliaser_BRAPA

Este script processa as informações e gera os fonemas ausentes na base original.

* **Resultado:** Geração do arquivo `modified.txt`.

### 3. Integração Final

1. Abra o arquivo `modified.txt`.
2. Copie todo o conteúdo gerado.
3. Cole as linhas ao final do arquivo `oto.ini` do seu banco de voz.

## Informações Técnicas

Os scripts são disponibilizados em dois formatos:

* **.py:** Código-fonte original em Python.
* **.pyc:** Versão compilada do script para execução em ambiente Python.

Ambas as versões possuem a mesma funcionalidade, sendo a versão `.pyc` otimizada para execução.
