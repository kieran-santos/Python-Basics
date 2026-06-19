# Estudos de Python e Machine Learning

Repositório de estudos da disciplina de **Machine Learning**, reunindo notebooks de prática sobre **fundamentos de Python** e as principais bibliotecas usadas em ciência de dados: **NumPy**, **Pandas** e **Matplotlib**.

Diferente dos demais repositórios da disciplina (focados em algoritmos como regressão e KNN), este reúne os notebooks de base usados para aprender a linguagem e as ferramentas antes de aplicá-las em modelos.

## Estrutura do projeto

```
.
├── Fundamentos.ipynb       # Fundamentos de Python (estruturas de dados, condicionais, loops, funções)
├── OOP.ipynb                # Programação Orientada a Objetos em Python (teoria + exemplos)
├── ClassesPython.ipynb     # Lista de exercícios de POO em Python
├── numpy.ipynb              # Introdução à biblioteca NumPy
├── pandas.ipynb             # Introdução à biblioteca Pandas
└── matplotlib.ipynb         # Introdução à biblioteca Matplotlib
```

## Notebooks

### `Fundamentos.ipynb`

Revisão dos fundamentos da linguagem Python voltados para Machine Learning:

- Estruturas de dados: listas, tuplas e dicionários
- Condicionais (`if`/`else`) e loops (`for`), incluindo list comprehensions
- Definição de funções, parâmetros com valor padrão e funções `lambda`

### `OOP.ipynb`

Introdução teórica e prática à **Programação Orientada a Objetos (POO)** em Python:

- Classes e objetos (construtor `__init__`, atributos e métodos)
- Encapsulamento, com atributos privados (prefixo `__`)
- Herança, com `super()` para reaproveitar o construtor da classe pai
- Polimorfismo, com classes diferentes implementando o mesmo método de formas distintas

### `ClassesPython.ipynb`

Lista de **10 exercícios práticos de POO**, aplicando os conceitos vistos em `OOP.ipynb` em cenários variados:

1. Classe `Aluno` com cálculo de média e situação de aprovação
2. Classe `Conversor` com atributo privado e validação de valores
3. Classes `Livro` e `Biblioteca` (composição de objetos)
4. Herança com `Veiculo`, `Carro` e `Moto`
5. Classe base `Pagamento` com subclasses `PagamentoCartao` e `PagamentoBoleto`
6. Classe `Sensor` para um cenário de IoT, com cadastro via dicionário
7. Classe `Usuario` com validação de senha
8. Herança múltipla com `Camera`, `Telefone` e `Smartphone`
9. Classe `Funcionario` com registro de logs de horário (`datetime`)
10. Classe `Calculadora` como exemplo de namespace de funções utilitárias

> Os comentários no próprio notebook documentam dúvidas e descobertas durante a resolução dos exercícios — fazem parte do processo de aprendizado.

### `numpy.ipynb`

Introdução à biblioteca **NumPy** para criação e manipulação de arrays:

- Criação de sequências numéricas com `np.arange`
- Criação de valores igualmente espaçados com `np.linspace`
- Inspeção de arrays: `shape`, `ndim`, `size` e `dtype`

### `pandas.ipynb`

Introdução à biblioteca **Pandas** para manipulação e análise de dados tabulares:

- Diferença entre `Series` (unidimensional) e `DataFrame` (bidimensional)
- Criação de `DataFrame` a partir de dicionários
- Leitura de dados de um CSV externo (dataset público do Titanic, via URL)
- Inspeção do dataset com `head()`, `shape` e `info()`
- Seleção de colunas e filtragem de linhas por condições (ex: passageiros com mais de 60 anos, mulheres da 1ª classe que sobreviveram)

### `matplotlib.ipynb`

Introdução à biblioteca **Matplotlib** para visualização de dados:

- Gráfico de barras (`plt.bar`) comparando quantidades de produtos em estoque
- Gráfico de dispersão (`plt.scatter`) com dados gerados aleatoriamente (`numpy.random`), simulando uma relação linear entre duas variáveis

## Tecnologias utilizadas

- Python 3
- [NumPy](https://numpy.org/)
- [Pandas](https://pandas.pydata.org/)
- [Matplotlib](https://matplotlib.org/)
- Jupyter Notebook

## Como executar

1. Clone o repositório:
   ```bash
   git clone https://github.com/seu-usuario/estudos-python-machine-learning.git
   cd estudos-python-machine-learning
   ```

2. Instale as dependências:
   ```bash
   pip install numpy pandas matplotlib
   ```

3. Abra os notebooks com Jupyter:
   ```bash
   jupyter notebook
   ```

4. Execute o notebook desejado em ordem. Não há dependência entre eles — cada um pode ser executado de forma independente.

> O notebook `pandas.ipynb` lê o dataset do Titanic diretamente de uma URL pública, portanto é necessária conexão com a internet para executar essa célula.

## Observações

Este repositório tem fins **didáticos**, reunindo o material de base estudado antes da aplicação prática em modelos de Machine Learning (regressão linear, regressão logística, KNN etc., disponíveis em outros repositórios). Por se tratar de material de estudo, alguns notebooks contêm anotações pessoais, dúvidas e comentários feitos durante o aprendizado.
