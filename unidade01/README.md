# Conceitos Iniciais

- A **união** entre **grandes volumes de dados** que são gerados constantemente na internet (*Big Data*) e a utilização de **algoritmos de aprendizagem de máquina** (*Machine Learning*) permite a montagem de **modelos estatísticos** para geração de **resultados de complexas análises de dados**;
- Tais modelos podem ser **preditivos (tentam adivinhar um comportamente futuro)** ou de **agrupamento (encontrando semelhanças entre usuários)**
- Ambos são baseados em **estatística**;

> Exemplo 01: Sistemas de recomendação de streaming ou música

> Exemplo 02: Detecção de fraudes em transações financeiras - modelos analisam o padrão de compra de um usuário em tempo real e, ao identificar uma compra fora do padrão, bloqueiam preventivamente   

- Algoritmos aprendem com os dados que lhes são fornecidos, aumentando o nível de responsabilidade em sistemas para internet

## Hierarquia DIKW (Data, Information, Knowledge, Wisdom)
- **Data:** É um registro bruto, sem contexto. Por exemplo, "10" ou "vermelho";
- **Information:** É o dado contextualizado. "10" se torna "10 alunos faltaram" (contexto educacional);
- **Knowledge:** Conexão de várias informações, permitindo compreensão de padrões e a capacidade de "tentar adivinhar" ou tomar decisões

## Tipos de dados
| Tipos |
| ----- |
| Estruturados - Tabelas |
| Semi-estruturados - JSON, XML |
| Não estruturados - Imagens, textos |

## Esquema básico de um projeto de Ciência de Dados (Pipeline de KDD)
```
                ( Definição do problema )
                          |
                          v
              +------------------------+
              | Coleta e análise       |
              | de dados               |
              +------------------------+
                          |
                          v
 --------------------------------------------------------------
 |                                                            |
 |   +-------------------+     <-->     +-------------------+ |
 |   | Pré-processamento |  <---------> | Modelagem e       | |
 |   |                   |              | Inferência        | |
 |   +-------------------+     <-->     +-------------------+ |
 |                                             <-->           |
 |                                      +-------------------+ |
 |                                      | Pós-processamento | |
 |                                      +-------------------+ |
 |                                                            |
 --------------------------------------------------------------
                          |
                          v
              +------------------------+
              | Apresentação de        |
              | resultados             |
              +------------------------+
                          |
                          v
        +--------------------------------------------+
        | Implantação do modelo e geração de valor   |
        +--------------------------------------------+
```
- **Definição do problema:** Entender o que precisa ser resolvido
- **Coleta de dados:** Identificar e obter acesso aos dados necessários de diversas fontes
- **Pré-processamento (Data Wrangling):** Limpeza e formatação/conserto de dados, adaptação para um contexto formal, já que os dados do mundo são "sujos"
