# Ciclo Básico 2026.2

Material das aulas do Ciclo Básico do Insper Data.

Cada pasta `Aula N/` contém o notebook da aula (`aulaN.ipynb`) e, quando houver, a atividade e os
dados de apoio. O conteúdo das pastas é a **biblioteca de material** , agora a ideia é que seja reutilizável de um
semestre para o outro. O que muda a cada semestre é o **cronograma abaixo**, junto com os campos
*Data* e *Professor(a)* no topo de cada notebook.

## Como o material está organizado

| Pasta                                     | O que é                                                                            | Para quem                               |
| ----------------------------------------- | ----------------------------------------------------------------------------------- | --------------------------------------- |
| `Aula N/aulaN.ipynb`                    | Notebook**limpo**: todo o texto da aula, com as células de código em branco | É este que vai para os alunos          |
| `Gabaritos/Aula N/aulaN_gabarito.ipynb` | O**mesmo** notebook com todo o código preenchido                             | É este que o professor projeta na aula |

A ideia é que os alunos escrevam o código ao vivo, acompanhando o gabarito projetado.

Nos notebooks limpos, só as células de **setup** (imports e carregamento da base) continuam
preenchidas, para que ninguém perca tempo de aula digitando `import pandas as pd`. As bases são
baixadas automaticamente pelo próprio notebook: não é preciso baixar nada à mão, com a única
exceção do `clientes.csv` da Aula 1, que continua vindo do Google Drive do Ciclo Básico.

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
