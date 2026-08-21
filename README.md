<div align="center">

# Introdução ao Python para Análise de Dados

Coleção de notebooks Jupyter com três listas de exercícios de fundamentos de Python aplicados à análise de dados, além de um projeto prático de Data Science que consolida os conceitos estudados.

![Python](https://img.shields.io/badge/Python_3-3776AB?style=flat-square&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter_Notebook-F37626?style=flat-square&logo=jupyter&logoColor=white)

</div>

## Visão geral

O repositório organiza a progressão dos estudos em duas frentes: as listas de exercícios, que percorrem desde operações básicas até problemas interpretativos mais desafiadores, e o notebook de projeto, que aplica os fundamentos em um fluxo de análise de dados. Cada exercício acompanha enunciado, explicação e solução passo a passo em Markdown.

## Conteúdo

| Notebook | Conteúdo |
| --- | --- |
| Lista de Exercícios — Parte 1 | Operações básicas (adição, subtração, multiplicação, divisão) com interpretação de problemas |
| Lista de Exercícios — Parte 2 | Operações combinadas e problemas de maior complexidade |
| Lista de Exercícios — Parte 3 | Consolidação dos fundamentos com novos desafios |
| Projeto Python Data Science | Projeto prático aplicando os conceitos em análise de dados |

## Decisões de projeto

Algumas escolhas que não são óbvias pelo código:

**O caderno do curso e as listas resolvidas ficam separados.** `Notebook/` guarda o material acompanhado em aula, com as células na ordem da explicação; `Notebook - Exercícios/` guarda as três listas resolvidas por conta própria. Misturar os dois num arquivo só apagaria a distinção entre o que foi copiado e o que foi produzido — que é justamente o que um repositório de estudo precisa deixar claro.

**O teste de primo usa `for`/`else`, não variável de controle.** O `else` de um laço em Python roda apenas quando ele termina sem `break`. Isso dispensa o `eh_primo = True` que a maioria das soluções cria e depois precisa lembrar de atualizar dentro do laço — o próprio fluxo carrega a resposta.

**A leitura por sentinela é feita antes e dentro do laço.** No exercício da média de temperaturas, o valor é lido uma vez antes do `while` e novamente ao final de cada volta. É o que impede o encerrador (`-273`) de entrar na soma e no contador, erro clássico de quem lê só dentro do laço.

## Tecnologias

| Tecnologia | Aplicação no projeto |
| --- | --- |
| Python 3 | Resolução dos exercícios e do projeto |
| Jupyter Notebook | Execução interativa e documentação das soluções |
| Markdown | Enunciados e explicações passo a passo |

## Como executar

Pré-requisitos: Python 3 e Jupyter instalados (ou uma IDE com suporte a notebooks, como o VS Code).

```bash
git clone https://github.com/OTAVIO-2507/Introducao_Python_Analise_de_Dados.git
cd Introducao_Python_Analise_de_Dados
jupyter notebook
```

Abra os notebooks da pasta `Notebook - Exercícios` para as listas ou `Notebook` para o projeto de Data Science. Alternativamente, os arquivos `.ipynb` podem ser visualizados diretamente aqui no GitHub.

## Estrutura do projeto

```
Introducao_Python_Analise_de_Dados/
├── Notebook/
│   └── Projeto_Python_Data_Science.ipynb
├── Notebook - Exercícios/
│   ├── Lista de Exercícios - Parte1.ipynb
│   ├── Lista de Exercícios - Parte2.ipynb
│   └── Lista de Exercícios - Parte3.ipynb
└── README.md
```

