# Lógica de Programação com Python

## Imprimindo na tela

```python

print(123)
print('Olá Python')

```


## Operações Básicas

```python

print(1 + 1)
print(1 - 1)
print(2 * 3)
print(2 ** 3)
print(4 / 2)
print(7 % 3)

```


## Operações com Texto

```python

print('Olá novamente' + ' Python')
print('Olá novamente' in ' Python')
print('Olá' in 'Olá novamente')

```



## Declaração de Variáveis

Diferentemente da linguagem C++, as variáveis em Python não são declaradas explicitamente

```python

qtde_vendas = 1000
nome = 'Python'

print(qtde_vendas)
print(nome)

```


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

## Format e f-string

```python

# com format 
print("O faturamento foi de {} e o lucro de {}" .format(faturamento, lucro))

# com f-string
print(f"O faturamento foi de {faturamento} e o lucro de {lucro}")

```


