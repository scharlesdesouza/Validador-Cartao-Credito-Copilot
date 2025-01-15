# Validador de Cartão de Crédito e Identificador de Bandeira

Este repositório contém uma função em Python para validar números de cartões de crédito e identificar suas bandeiras. A função utiliza expressões regulares para verificar o formato do número e determinar a bandeira correspondente com base nos prefixos dos cartões.

## Bandeiras Suportadas

- **Visa**
- **MasterCard**
- **American Express**
- **Diners Club**
- **Discover**
- **EnRoute**
- **JCB**
- **Voyager**
- **Hipercard**
- **Aura**

## Funcionalidade

A função `validar_cartao_credito` valida um número de cartão de crédito e retorna a bandeira correspondente. Ela verifica o formato do número de cartão e faz a correspondência com as bandeiras listadas usando expressões regulares.

### Como Funciona:

1. O número do cartão é passado como string para a função.
2. A função remove quaisquer espaços em branco e valida o formato e a quantidade de dígitos.
3. Com base no prefixo e no comprimento do número, a função retorna a bandeira correspondente ou uma mensagem de erro caso o número seja inválido ou não corresponda a nenhuma das bandeiras acima.

### Exemplo de Uso:

```python
# Exemplo de uso para validar o cartão e identificar a bandeira
cartao = "86996 7655 69531"  # Exemplo para Voyager
print(validar_cartao_credito(cartao))  # Esperado: Voyager
