# 🧠 Modelo Dimensional – Análise de Professores

Este repositório apresenta a construção de um **modelo dimensional (Star Schema)** a partir de um **modelo relacional transacional** previamente existente.

O objetivo foi transformar o modelo operacional original em uma estrutura voltada à **análise de informações sobre professores**, permitindo consultas analíticas relacionadas a cursos, disciplinas, departamentos e períodos de oferta.


## 🎯 Objetivo do Projeto

O foco do modelo é o **professor** como entidade central de análise.
A partir das tabelas do modelo transacional, foi desenvolvida uma **tabela fato** que consolida os principais indicadores e dimensões relacionadas, proporcionando uma base para análises de desempenho e alocação docente.


## 🧩 Estrutura do Modelo

O modelo final segue o formato **Star Schema**, composto por:

* **FatoProfessor** — tabela fato central, relacionando professores, cursos, disciplinas, departamentos e datas de oferta.
* **Dimensões**:

  * `DimensãoProfessor` — dados descritivos do docente (nome, titulação, tempo de casa, e-mail).
  * `DimensãoDepartamento` — informações sobre o departamento (nome, campus, coordenador).
  * `DimensãoCurso` — nome e nível do curso.
  * `DimensãoDisciplina` — carga horária, número de pré-requisitos e cursos associados.
  * `DimensãoDataOferta` — data, semestre, mês, trimestre e turno da oferta.

Essa modelagem possibilita análises por tempo, curso, disciplina ou departamento, sempre com o **professor** como ponto central.

## 🧭 Observações

* O modelo foi construído com base nas diretrizes do projeto original, que pedia a criação de um **esquema em estrela** centrado no professor.
* Não foram incluídos dados sobre alunos, visto que não são o foco do esquema.
* A tabela de **datas** foi adicionada para enriquecer a granularidade temporal das análises.


## 💡 O que foi utilizado?

* Modelagem de dados relacional e dimensional
* Diagramas ER (Entity-Relationship)
* Star Schema Design


## 📸 Imagens

1. Modelo Transacional - Inicial
<img width="1356" height="744" alt="image" src="https://github.com/user-attachments/assets/fc94e4da-554a-402d-8237-ece25de77a3a" />

  
2. Modelo Dimensional (Star Schema) - Final

<img width="1063" height="675" alt="MapeandoStarSchema" src="https://github.com/user-attachments/assets/58fa3098-0194-496e-b865-35e88d5e8345" />

