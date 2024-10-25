# Lógica de Programação com Python

## Imprimindo na tela

```python

print(123)
print('Olá Python')

```
<br>


## Operações Básicas

```python

print(1 + 1)
print(1 - 1)
print(2 * 3)
print(2 ** 3)
print(4 / 2)
print(7 % 3)

```
<br>


## Operações com Texto

```python

print('Olá novamente' + ' Python')
print('Olá novamente' in ' Python')
print('Olá' in 'Olá novamente')

```
<br>



## Declaração de Variáveis

Diferentemente da linguagem C++, as variáveis em Python não são declaradas explicitamente

```python

qtde_vendas = 1000
nome = 'Python'

print(qtde_vendas)
print(nome)

```
<br>


## Tipos de Variáveis

```python

faturamento = 1000
print(type(faturamento))

faturamento = 1000.00
print(type(faturamento))

faturamento = '1000.00'
print(type(faturamento))

faturamento = True
print(type(faturamento))

```
<br>


## Input - Pegando informações do Usuários

Fazendo a leitura de uma string(str)

```python

nome = input("Qual é o seu primeiro nome? ")
sobrenome = input("Qual é o seu sobrenome? ")
print(nome + ' ' + sobrenome)

```


Convertendo o input do tipo str para tipo float

```python

faturamento = float(input("Insira o faturamento: "))
custo = float(input("Insira o custo: "))

lucro = faturamento - custo 
print(lucro)

```
<br>

## Format e f-string

```python

# com format 
print("O faturamento foi de {} e o lucro de {}" .format(faturamento, lucro))

# com f-string
print(f"O faturamento foi de {faturamento} e o lucro de {lucro}")

```
<br>

## Estrutura if - Condições no Python

### Exemplo 01
Estrutura if simples

```python

meta = 50000

qtde_vendidas = int(input('Entre com a quantidade vendida: '))

if qtde_vendidas >= meta:
    print(f'Batemos a meta, vedemos {qtde_vendidas} unidades')
else: 
    print(f'Não batemos a meta, vedemos apenas {qtde_vendidas} unidade')

``` 
<br>

### Exemplo 02

Estrutura composta por uma estrutura if dentro de outra estrutura if

```python

meta = 0.05
taxa = 0
redimento = 0.21

if redimento > meta:
    if redimento > 0.20 :
        taxa = 0.04
        print(f'A taxa foi de {taxa}')
    else:
        taxa = 0.02
        print(f'A taxa foi de {taxa}')
else: 
    taxa = 0
    print(f'A taxa foi de {taxa}')

```
<br>

### Estrutura elif

```python

meta = 20000
bonus = 0

valor_vendas = float(input('Entre com total de vendas realizado pelo vendedor: '))


if valor_vendas > meta * 2:
    bonus = 0.07 * valor_vendas
elif valor_vendas > meta :
    bonus = 0.03 * valor_vendas
else: 
    bonus = 0 * valor_vendas

print(f"O total de vendas foi {valor_vendas}, a meta era {meta}, portanto o bonus foi de {bonus}") 

```
<br>

### Comparadores 

Se em alguma condição não quiser fazer nada, você simplesmente escre `pass`

Comparador | Descrição
---|---
`==` | igual
`!=` | diferente
`>` | maior que 
`<` | menor que 
`in` | Verifica se um texto existe dentro de outro texto
`not` | Verifica o contrario da comparação

<br>

### Casos com várias condições/comparações: `or` e `end`

### Exemplo 1

```python

meta_funcionario = 10000
meta_loja = 250000
vendas_funcionario = 15000
vendas_loja = 280000

if vendas_funcionario > meta_funcionario and vendas_loja > meta_loja:
    bonus = 0.03 * vendas_funcionario
else: 
    bonus = 0


print(f'O bonus do funcionário foi de {bonus}')

```

### Exemplo 2

```python

meta_funcionario = 10000
meta_loja = 250000
vendas_funcionario = 8000
vendas_loja = 200000

nota_funcionario = 9
meta_nota = 9 

if nota_funcionario >= meta_nota or (vendas_funcionario > meta_funcionario and vendas_loja > meta_loja):
    bonus = 0.03 * vendas_funcionario
    print(f'Bonus do funcionário foi de {bonus}')
else:
    print('O funcionário não recebeu bonus')

```

<br>