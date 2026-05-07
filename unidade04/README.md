# Análise Exploratória Bivariada (E Multivariada)
## De Univariada para Bivariada
A análise univariada descreve uma variável por vez — sua distribuição, média, mediana. A análise bivariada expande esse olhar para investigar a relação entre duas variáveis: elas variam juntas? Uma influencia a outra? A resposta depende inteiramente do tipo de cada variável.

## A Matriz de Técnicas Bivariadas
A escolha da técnica correta depende da combinação dos tipos das duas variáveis sendo analisadas:

<img width="814" height="265" alt="image" src="https://github.com/user-attachments/assets/075d2a60-6742-42fd-9a39-5457b3ec8c93" /><br>

## Diagrama de Dispersão (Scatter Plot)
- O ponto de partida para analisar duas variáveis numéricas é sempre o **Diagrama de Dispersão**
- Cada ponto representa uma observação, posicionada no plano cartesiano conforme os valores de X e Y.
- **O que observar no gráfico?**
  - A nuvem sobe da esquerda para a direita? → Correlação positiva
  - A nuvem desce da esquerda para a direita? → Correlação negativa
  - Sem padrão definido? → Correlação nula
  - Pontos isolados? → Possíveis outliers
 
~~~python
import seaborn as sns
import pandas as pd

# Exemplo: notas de alunos
sns.scatterplot(
  data=df,
  x='nota_lingua_portuguesa',
  y='nota_matematica'
)
plt.title('Correlação: Port. vs Mat.')
plt.show()
~~~

> Exemplo: Diagrama de Dispersão

> Este diagrama de dispersão mostra a relação entre as Horas de Estudo (eixo X) e a Nota Final (eixo Y) de um grupo de alunos. Cada ponto representa um aluno. Podemos observar uma tendência clara: à medida que as horas de estudo aumentam, a nota final também tende a aumentar. Isso indica uma correlação positiva forte entre essas duas variáveis. Quanto mais dedicados os alunos são ao estudo, melhores são seus resultados. A dispersão dos pontos em torno de uma linha imaginária ascendente sugere que, embora a tendência seja clara, há variações individuais. Alguns alunos podem obter notas altas com menos horas, e vice-versa, devido a outros fatores não representados no gráfico.

<img width="482" height="277" alt="image" src="https://github.com/user-attachments/assets/bdee67e9-1eb1-4036-99d6-d0e857e2d792" />
 
