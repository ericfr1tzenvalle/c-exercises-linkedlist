```markdown
# 📌 c-exercises-linkedlist

Um programa em C para comparar o desempenho de duas estruturas de dados — uma **lista encadeada** e um **array estático** — armazenando inteiros em ordem crescente.

Toda a lógica está implementada em um único arquivo: `main.c`.

---

## 📋 Descrição

### 🔹 Parte 1: Testes de Desempenho

O programa utiliza:

- ✅ Uma **lista encadeada simples** para inteiros  
- ✅ Um **array estático** para inteiros  

Ambas as estruturas armazenam os números em **ordem crescente**, sendo inseridos em **ordem decrescente** (ex: de `1.000.000.000` até `1`).

As seguintes operações são medidas:

1. 🔧 Inserir valores na lista encadeada  
2. 🔧 Inserir valores no array  
3. 🔍 Percorrer (ler) todos os valores da lista encadeada  
4. 🔍 Percorrer (ler) todos os valores do array  

### ⏱ Medição de Tempo

Use `GetTickCount()` para medir o tempo de execução:

```c
int inicio, fim, decorrido;
inicio = GetTickCount();
// ... operações ...
fim = GetTickCount();
decorrido = fim - inicio;
printf("Tempo decorrido: %d ms\n", decorrido);
```

📌 **Observações importantes:**

- ❌ **Não** use `printf()` durante os laços de inserção ou remoção  
- ⏳ Se o tempo medido for muito baixo, aumente a quantidade de elementos (ex: inserir 1.000.000 em vez de 100.000)

---

### 🔹 Parte 2: Diagramas Passo a Passo

Para uma **lista encadeada ordenada** com os valores:  
`3 → 4 → 5 → 6`

Desenhe diagramas passo a passo para:

- ❌ Remover `3`  
- ❌ Remover `5`  
- ❌ Remover `6`  
- ➕ Inserir `1`  
- ➕ Inserir `5`  
- ➕ Inserir `7`  

Para uma **lista encadeada não ordenada** com os mesmos valores:

- ➕ Inserir `1`  
- ➕ Inserir `4`  
- ➕ Inserir `7`  

Esses diagramas ajudam a visualizar o comportamento dos ponteiros e a manipulação dos nós.

---

## 🛠 Compilação e Execução

Para compilar e executar o programa:

```bash
gcc main.c -o main
./main
```

> ⚠️ Em sistemas que não sejam Windows, substitua `GetTickCount()` por `gettimeofday()` ou `clock_gettime()`.

---

## 📁 Estrutura do Projeto

```
c-exercises-linkedlist/
├── main.c       # Toda a lógica do programa
└── README.md    # Documentação do projeto
```

---

## 👨‍💻 Autor

Este repositório foi criado como parte de um exercício de estruturas de dados em programação C.

---

## 📝 Licença

Este projeto é destinado apenas para **uso educacional**.
```
