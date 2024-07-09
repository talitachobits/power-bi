# Desafio Modelagem Dimensional - Universidade

O desafio consiste em transformar o modelo transacional abaixo em um modelo dimensional star schema para análise de dados com base no professor.

<p align="center" alt="Diagrama Entidade Relacionamento Universidade">
<img 
    src="https://github.com/talitachobits/power-bi/blob/main/Modelagem%20Dimensional/der_universidade.png"
    width="800"  
/>
</p>

## Criação da modelagem dimensional

Para criação da modelagem foi utilizada a ferramenta [sqldbm](https://sqldbm.com/Home/) 

Como o foco da análise são os dados do professor, ela é a nossa tabela fato e as dimensões são:

- Disciplina
- Curso
- Departamento

São das tabelas dimensões que recuperaremos os dados para responder questões como departamento que o professor faz parte, aulas que ministra etc.

Também foi criada a tabela dimensão tempo para que possamos ter uma análise temporal dos dados a serem analisados. Foi considerado que a universidade divide o ano letivo em semestres.

Abaixo a modelagem dimensional originada para análise analítica dos dados:

<p align="center" alt="Diagrama Entidade Relacionamento Universidade">
<img 
    src="https://github.com/talitachobits/power-bi/blob/main/Modelagem%20Dimensional/Modelagem%20Dimensional.png"
    width="800"  
/>
</p>




  

  
