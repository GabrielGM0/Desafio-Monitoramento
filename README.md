#### Gabriel Oliveira Moreira Brazão
#### Algoritmos e Pensamento Computacional
#### Profa. Karla Sartin;

# 🌡️ Monitoramento de Temperatura

## 📌 Descrição

Este projeto consiste em um programa desenvolvido em **linguagem C** para realizar o monitoramento de temperaturas informadas pelo usuário.

O programa permite definir um limite de temperatura e, posteriormente, registrar várias temperaturas. Durante o monitoramento, são calculadas algumas estatísticas e verificadas situações em que a temperatura ultrapassa o limite estabelecido.

O monitoramento é encerrado automaticamente quando são registradas **3 temperaturas consecutivas acima do limite** ou quando o usuário informa o valor `-999`.

---

## 🎯 Objetivo

O objetivo do programa é **monitorar temperaturas e identificar situações em que elas ultrapassam um determinado limite**, fornecendo ao final um relatório com informações estatísticas.

O programa apresenta:

* Quantidade de temperaturas registradas;
* Média das temperaturas;
* Maior temperatura;
* Menor temperatura;
* Quantidade de temperaturas acima do limite;
* Percentual de temperaturas acima do limite;
* Alerta quando existem 3 temperaturas consecutivas acima do limite.

---

## ⚙️ Funcionamento do Programa

### 1. Definição do limite

Primeiramente, o programa solicita ao usuário um limite de temperatura.

O valor deve estar entre:

```text
-50 °C e 100 °C
```

Caso seja informado um valor fora desse intervalo, o programa apresenta uma mensagem de erro e solicita um novo valor.

A validação é realizada utilizando a estrutura `do...while`.

---

### 2. Entrada das temperaturas

Depois de definir o limite, o programa começa a solicitar temperaturas.

Cada temperatura deve estar entre:

```text
-50 °C e 100 °C
```

O usuário também pode digitar:

```text
-999
```

para encerrar manualmente o monitoramento.

---

### 3. Validação dos valores

Quando uma temperatura é digitada, o programa verifica se ela está dentro do intervalo permitido.

Se o valor for inválido:

```text
Temperatura inválida!
```

o programa não contabiliza essa temperatura e continua solicitando novos valores.

---

### 4. Temperaturas acima do limite

Depois de validar uma temperatura, o programa verifica se ela é maior que o limite definido pelo usuário.

Por exemplo, considerando:

```text
Limite = 30 °C
```

Uma temperatura de:

```text
35 °C
```

será considerada **acima do limite**.

Nesse caso, o programa:

* Incrementa a quantidade de temperaturas acima do limite;
* Incrementa o contador de temperaturas consecutivas;
* Exibe uma mensagem informando que a temperatura está acima do limite.

---

### 5. Temperaturas consecutivas

O programa utiliza a variável `consecutivas` para contar quantas temperaturas acima do limite foram registradas em sequência.

Exemplo:

```text
Limite: 30
```
