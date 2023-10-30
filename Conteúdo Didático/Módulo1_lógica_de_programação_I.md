# Modulo 1 - Lógica da Programação I (PY) 

### ⚡️ Variáveis

Frequentemente, em nossos programas, precisamos armazenar **temporariamente** dados. Esses dados podem ser adquiridos de várias maneiras, como entrada do teclado, leitura de um arquivo, ou cálculos feitos pelo programa com base em outros dados. Por exemplo, para calcular a média de um aluno com base em suas notas, precisamos que o aluno insira suas notas, e o programa calculará a média. Usamos variáveis para armazenar temporariamente esses dados.

Variáveis são **"pequenas áreas de memória"** onde guardamos informações. Sempre que referenciamos o nome de uma variável, acessamos a área de memória associada a ela e recuperamos os dados nela armazenados.

**Para criar variáveis**, damos a elas um nome e usamos o operador de atribuição (o sinal de igual: =) para atribuir um valor inicial.

Exemplo:

```python
x = 10
```
No exemplo acima, uma variável chamada `"x"` foi criada para armazenar o valor `10`. Em outras palavras, reservamos uma área de memória e armazenamos o número 10 nela.

É importante escolher nomes descritivos para suas variáveis. O nome da variável deve refletir o que ela armazena. Nomes como `'x', 'y', 'z', 'a', 'b', 'c', 'a1', 'a2', 'a3'`, etc., podem se tornar confusos em programas grandes. Quanto mais descritivo for o nome, melhor.

Os nomes das variáveis podem conter letras, números e o símbolo "_", mas não podem começar com um número.

Dica: Existem vários padrões de nomenclatura que podem ser usados para nomear variáveis. Em Python, é recomendado o uso do "snake case," onde palavras em nomes de variáveis com múltiplas palavras são separadas pelo símbolo "_". Exemplos: `nome_completo, nota_da_prova, etc.`

### Tipos de Variáveis

Variáveis podem ter diferentes tipos. Alguns tipos são considerados tipos primitivos, ou seja, são tipos de dados fundamentais que podem ser usados para criar tipos mais complexos. Em Python, os tipos primitivos são conhecidos como:

- `int`: números inteiros, ou seja, números sem parte decimal, como 0, 5, -1, 1000.

- `float`: números reais, ou seja, números com parte decimal, como 1.0, -2.7, 3.14.

- `str`: cadeias de caracteres (strings), ou seja, dados textuais, como 'Olá Mundo!' ou "eu tenho 18 anos".

- `bool`: valores lógicos (booleanos), ou seja, podem ser apenas True ou False.
  
Exemplos:

```python
nome = 'Sarah'  # uma variável do tipo string - observe as aspas
email = "Sarah@gmail.com"  # outra string
idade = 28  # uma variável inteira
salário = 5999.85  # uma variável float - usamos ponto, não vírgula
receber_newsletter = True  # uma variável bool
```
Python é uma linguagem de tipagem dinâmica, o que significa que não é necessário especificar o tipo de uma variável explicitamente; a linguagem tenta determinar o tipo com base nos dados atribuídos à variável.

### Comentários

Observamos que nos exemplos anteriores utilizamos o símbolo "#" para incluir comentários no código. Comentários são usados para explicar partes do código, tornando-o mais compreensível para os desenvolvedores e facilitando modificações e correções no futuro. Também é possível criar comentários de várias linhas utilizando aspas triplas, que servem para abrir e fechar blocos de comentários.

Exemplo:

```python
'''
Este é um comentário de várias linhas.
Tudo que vem depois do primeiro conjunto de aspas tripas e antes do segundo
será ignorado pelo Python.
'''
```
Na verdade, esse tipo de comentário não é exatamente um comentário, mas uma string com várias linhas. O Python ignora essa "string" porque ela não está atribuída a nenhuma variável e a trata como um comentário.

Na maioria das IDEs, você pode usar atalhos de teclado para transformar um bloco inteiro de código em comentário temporariamente, o que é útil ao testar soluções alternativas ou corrigir erros.

### Saídas
As saídas de um programa são os dados gerados pelo programa e apresentados ao usuário. No Python, usamos a função print para exibir dados na tela. Os dados que desejamos mostrar são colocados entre parênteses após o print.

Exemplo:

```python
print('Olá, mundo!')  # exibe a frase 'Olá, mundo' na tela
```

Os dados exibidos não precisam ser valores constantes, como a frase fixa no exemplo acima. Eles podem ser variáveis:

Exemplo:

```python
idade = 20
print(idade)
```
Observe que quando usamos aspas, o Python trata o valor como uma string, ou seja, como texto literal. Quando não usamos aspas, o Python considera que é o nome de uma variável e busca o valor associado a ela.

Podemos exibir vários dados em uma única instrução print, separando-os por vírgulas. Eles aparecerão na tela na mesma ordem em que foram especificados no código:

Exemplo:

```python
nome = 'Mario'
linguagem = 'Python'
print('Oi, eu sou o', nome, 'e eu programo em', linguagem)
```

Resultado na tela:

```python
Oi, eu sou o Mario e eu programo em Python
```
Observe que os dados aparecem separados por espaços automaticamente. Duas instruções print consecutivas também incluem uma quebra de linha entre elas. Se desejar, você pode passar opções como sep e end para personalizar o comportamento.

Exemplo:


```python
nome = 'Mario'
linguagem = 'Python'
print('Oi, eu sou o', nome, sep='@', end='***')
print('Eu programo em', linguagem, sep='@')

```

Resultado na tela:


```python
Oi, eu sou o@Mario***Eu programo em@Python
```

Dica: Se a separação de dados por vírgulas parecer confusa, você pode optar pelo uso de f-strings, que são uma alternativa mais legível. No entanto, não entraremos em detalhes aqui. A ideia


