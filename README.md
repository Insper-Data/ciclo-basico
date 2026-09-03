# Ciclo Básico 2026.2

Material das aulas do Ciclo Básico do Insper Data.

Cada pasta `Aula N/` contém o notebook da aula (`aulaN.ipynb`), a atividade quando houver, e a base
de dados. O conteúdo das pastas é a **biblioteca de material** , agora a ideia é que seja
reutilizável de um semestre para o outro. O que muda a cada semestre é o **cronograma abaixo**,
junto com os campos *Data* e *Professor(a)* no topo de cada notebook.

## Como o material está organizado

| Pasta                                     | O que é                                                                            | Para quem                               |
| ----------------------------------------- | ----------------------------------------------------------------------------------- | --------------------------------------- |
| `Aula N/aulaN.ipynb`                    | Notebook**limpo**: todo o texto da aula, com as células de código em branco | É este que vai para os alunos          |
| `Gabaritos/Aula N/aulaN_gabarito.ipynb` | O**mesmo** notebook com todo o código preenchido                             | É este que o professor projeta na aula |

A ideia é que os alunos escrevam o código ao vivo, acompanhando o gabarito projetado.

Nos notebooks limpos, só as células de **setup** (imports e carregamento da base) continuam
preenchidas, para que ninguém perca tempo de aula digitando `import pandas as pd`.

## Como o material chega nos alunos

**Cada pasta `Aula N/` é autossuficiente.** Zipe a pasta, mande no grupo do WhatsApp, e o aluno
extrai em qualquer lugar do computador dele e já sai codando — não precisa clonar o repositório,
nem instalar nada além das bibliotecas, nem ajustar caminho nenhum. Os notebooks não importam nada
de fora da própria pasta.

Se você rodar a célula de setup **uma vez antes de zipar**, a base vai junto no zip e a aula
funciona mesmo sem internet — útil quando o wi-fi da sala resolve não colaborar. A pasta `data/`
não precisa ir no zip: o notebook recria sozinho.

## As bases de dados

Dentro da pasta de cada aula ficam duas pastas, criadas na primeira vez que a célula de setup roda:

| Pasta       | O que é                                                                    |
| ----------- | --------------------------------------------------------------------------- |
| `data_raw/` | A base **original**, do jeito que veio da fonte. É a referência: não mexa. |
| `data/`     | A **cópia de trabalho** — é essa que os notebooks leem                     |

A separação existe porque durante as aulas os alunos limpam, filtram e alteram a base. Tudo isso
acontece em `data/`; o original em `data_raw/` continua lá para comparação. **Se alguém bagunçar a
base, é só apagar o arquivo em `data/` e rodar a célula de setup de novo** — ele é recriado a partir
do original, sem precisar baixar nada.

A célula de setup faz tudo isso em ~10 linhas, escritas dentro do próprio notebook. É de propósito:
qualquer arquivo auxiliar fora da pasta quebraria o envio por zip.

Só duas bases **não** são baixadas automaticamente, porque vêm do Google Drive do Ciclo Básico:
`clientes.csv` (Aula 1) e `vendas.csv` (atividade da Aula 1). Essas ficam versionadas aqui, em
`Aula 1/data_raw/`, justamente para a pasta já sair zipada com a base dentro.

Nas atividades da Aula 2 e na Aula 3, cada aluno recebe uma amostra própria de 800 linhas do
Titanic, sorteada a partir do nome digitado. Como a semente vem do nome, o aluno recebe exatamente
a mesma amostra nas duas aulas, mesmo sendo dois zips separados.

## Cronograma

| Aula | Título                               | Data        | Professor(a) |
| ---- | ------------------------------------- | ----------- | ------------ |
| 1    | Limpeza e Tratamento dos Dados        | (preencher) | (preencher)  |
| 2    | Análise Exploratória — Parte 1     | (preencher) | (preencher)  |
| 3    | Visualização Gráfica               | (preencher) | (preencher)  |
| 4    | Regressão Linear                     | (preencher) | (preencher)  |
| 5    | Machine Learning                      | (preencher) | (preencher)  |
| 6    | Classificação                       | (preencher) | (preencher)  |
| 7    | Validação e Otimização de Modelos | (preencher) | (preencher)  |
| 8    | Proposta de Projeto                   | (preencher) | (preencher)  |
| 9    | Apresentações dos Projetos          | (preencher) | (preencher)  |
| 10   | Aula Final — Encerramento do Ciclo   | (preencher) | (preencher)  |

> As aulas 1 a 7 têm notebook próprio nas pastas `Aula 1/` a `Aula 7/`.
> Os encontros 8 a 10 não têm notebook são a proposta de projeto, as apresentações e o
> encerramento.

## Ambiente

As dependências estão em `requirements.txt` / `pyproject.toml`.
