# ⚡ Árvore Binária de Busca em Java

Este projeto implementa uma **árvore binária de busca (BST - Binary Search Tree)** em Java, permitindo inserção, remoção, busca de elementos e percursos na árvore.

## ✨ Funcionalidades

- Inserção de elementos na árvore.
- Remoção de elementos mantendo as regras da BST.
- Busca de elementos na árvore.
- Percursos:
  - **Pré-ordem** (Root - Left - Right)
  - **Em ordem** (Left - Root - Right)
  - **Pós-ordem** (Left - Right - Root)
- Gera arquivos **.dot** para visualização da árvore.

## 💪 Tecnologias Utilizadas

- **Java** (linguagem principal)
- **Graphviz** (para gerar visualização da árvore em DOT)

## ✅ Como Executar o Projeto

1. **Clone o repositório**

   ```sh
   git clone https://github.com/seu-usuario/arvore-binaria-java.git
   cd arvore-binaria-java
   ```

2. **Compile o código**

   ```sh
   javac ArvoreBinariaBusca.java
   ```

3. **Execute o programa**

   ```sh
   java ArvoreBinariaBusca
   ```

4. **Visualize os arquivos DOT** (Opcional)

   - Gere a imagem da árvore usando o Graphviz:
     ```sh
     dot -Tpng arvore1.dot -o arvore1.png
     ```
   - Abra o arquivo `arvore1.png` gerado.

## 📝 Exemplo de Uso

```java
ArvoreBinariaBusca arvore = new ArvoreBinariaBusca();
arvore.inserir(50);
arvore.inserir(30);
arvore.inserir(70);
arvore.inserir(20);
arvore.inserir(40);
arvore.inserir(60);
arvore.inserir(80);

System.out.print("Em ordem: ");
arvore.emOrdem();
```

Saída esperada:

```
Em ordem: 20 30 40 50 60 70 80
```

## 🎨 Visualização da Árvore

Se você deseja visualizar a estrutura da árvore graficamente, utilize o arquivo **.dot** gerado pelo método `gerarArquivoDot()` e utilize o **Graphviz** para convertê-lo em uma imagem.

Exemplo de conteúdo gerado:

```
digraph BST {
  50 -> 30;
  50 -> 70;
  30 -> 20;
  30 -> 40;
  70 -> 60;
  70 -> 80;
}
```

## 🛠️ Possíveis Melhorias Futuras

- Implementação de uma interface gráfica.
- Melhor tratamento de erros.
- Implementação de balanceamento (AVL ou Red-Black Tree).

---

Desenvolvido por [Pedro Thomas](www.linkedin.com/in/pedro-gustavo-thomas-5935392b7).

