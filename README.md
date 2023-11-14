# Algoritmos_curso_Ada
Nesse documento apresento meus aprendizados no módulo de Algorítmos da trilha digital da Ada Tech.

## Índice
1. [Conceito de algorítmos](#conceito)
2. [Fluxos simples e sequêncial](#fluxos)
3. [Tipos de dados](#tipos)
4. [Estruturas de decisão](#decisão)
5. [Estruturas de repetição](#repetição)
6. [Listas, listas de listas, dicionários, tuplas](#listas)
7. [Funções](#funções)
8. [Desempenho de algorítmos](#desempenho)
8. [Como melhorar a construir um algorítmo](#dicas)<div id='conceito'/>

## Conceito de Algorítmos
Algoritmos são conjuntos de instruções ou passos precisos e bem definidos que descrevem como resolver um problema ou realizar uma tarefa. Em termos simples, são como receitas, especificando uma sequência de ações para alcançar um resultado desejado.

Por exemplo, um algoritmo para fazer um sanduíche pode ser:

1. Pegue duas fatias de pão.
2. Espalhe maionese em uma fatia de pão.
3. Adicione alface, tomate e queijo na fatia com maionese.
4. Coloque a outra fatia de pão por cima para fazer o sanduíche.

A diferença fundamental entre a maneira como os computadores processam algoritmos e como os humanos o fazem está na capacidade de um computador seguir precisamente e sem erros as instruções fornecidas. Os computadores executam algoritmos de forma extremamente rápida e consistente, seguindo cada passo exatamente conforme instruído.

Enquanto os seres humanos podem interpretar e ajustar algoritmos com base na intuição, experiência ou nuances do problema, os computadores processam algoritmos de maneira estrita e literal. Um erro de sintaxe ou lógica pode fazer com que um computador interprete de forma diferente ou falhe ao executar um algoritmo, algo que os seres humanos podem corrigir mais facilmente.

Os algoritmos são a base da computação e estão presentes em quase todas as atividades que envolvem processamento de informações. Desde pesquisas na internet até cálculos complexos, os algoritmos são a essência do funcionamento de muitos sistemas e softwares que usamos diariamente.
<div id='fluxos'/>

## Fluxos simples e sequêncial

O fluxo de um algoritmo descreve a sequência de passos ou a lógica de execução que o algoritmo segue para resolver um problema ou realizar uma tarefa específica. Vou explicar de forma simplificada como funciona o fluxo de um algoritmo:

1. **Início:** O algoritmo começa com uma etapa inicial, onde são definidos os parâmetros iniciais e variáveis necessárias para resolver o problema.

2. **Sequência de Instruções:** O corpo do algoritmo contém a sequência de instruções, cada uma descrevendo uma ação específica a ser executada. Essas instruções podem ser operações matemáticas, lógicas, atribuições de valores, chamadas de funções, estruturas de controle (como loops e condicionais), entre outras.

3. **Tomada de Decisão:** Em certos pontos, o algoritmo pode precisar tomar decisões com base em condições específicas. Por exemplo, um algoritmo para verificar se um número é par ou ímpar precisa verificar se o resto da divisão por 2 é igual a zero (condição de paridade).

4. **Laços (Loops):** Em muitos algoritmos, é necessário repetir certas operações várias vezes. Os loops (como o loop "for" ou "while") são usados para essa finalidade, permitindo que um bloco de código seja executado várias vezes até que uma condição seja atendida.

5. **Fim:** O algoritmo termina quando todas as instruções foram executadas ou quando uma condição específica é atendida.

Exemplo:
|       Comando                         |   Saída na tela     |   Armazenamento          |
|:-------------------------------------:|:-------------------:|:------------------------:|
| MOSTRAR digite seu nome               | 'Digite seu nome'   |         -                |
| ESPERAR DIGITAÇÃO + nome              |                     |    Nome-Julia            |
| JUNTAR TEXTO Bom dia nome saudacao    |                     |    Nome-Julia            |
|                                       |                     |Saudacao = "Bom dia Julla"|
| MOSTRAR saudacao                      |    Bom dia Julla    |    Nome-Julia            |
|                                       |                     |Saudacao = "Bom dia Julla"|

o fluxo de um algoritmo pode ser visualizado graficamente usando diagramas de fluxo, fluxogramas ou pseudocódigo para representar a sequência de passos e as decisões tomadas durante a execução. Isso ajuda a visualizar e compreender melhor o funcionamento do algoritmo.

Em suma, o fluxo de um algoritmo descreve a ordem lógica e sequencial das etapas necessárias para resolver um problema, e a precisão e clareza dessa sequência são fundamentais para a correta execução do algoritmo. <div id='tipos'/>

## Tipos de dados

Os tipos de dados representam os diferentes tipos de informações que podem ser armazenados e manipulados em um programa de computador. Aqui estão alguns tipos comuns de dados:

1. **Números Inteiros (Integer):** Representam números inteiros sem parte fracionária. Ex: `-3`, `0`, `42`.

2. **Números de Ponto Flutuante (Float):** Representam números com parte fracionária. Ex: `3.14`, `2.71828`.

3. **Texto (String):** Sequências de caracteres. Ex: `'Olá, mundo!'`, `'123'`.

4. **Booleano (Boolean):** Representa valores lógicos verdadeiro (`True`) ou falso (`False`).

5. **Lista (List):** Coleção ordenada de itens. Ex: `[1, 2, 3]`, `['maçã', 'banana', 'laranja']`.

6. **Tupla (Tuple):** Semelhante a uma lista, mas imutável (não pode ser alterada após a criação). Ex: `(1, 2, 3)`.

7. **Dicionário (Dictionary):** Coleção de pares chave-valor. Ex: `{'nome': 'João', 'idade': 25}`.

8. **Conjunto (Set):** Coleção não ordenada de itens únicos. Ex: `{1, 2, 3}`.

9. **Bytes e ByteArray:** Usados para representar dados binários em formatos específicos.

10. **Null (None):** Representa a ausência de valor.

11. **Objetos Personalizados (Classes):** Em linguagens orientadas a objetos, é possível criar tipos de dados personalizados com suas próprias propriedades e métodos.

Cada linguagem de programação pode ter sua própria variedade de tipos de dados com diferentes capacidades e características. Compreender os tipos de dados disponíveis é fundamental para manipular informações de maneira adequada em um programa.


|      Tipo de Dado                 |            Exemplo               |
|:---------------------------------:|:--------------------------------:|
|          Número Inteiro           |        `-3`, `0`, `42`           |
|    Número de Ponto Flutuante      |      `3.14`, `2.71828`           |
|          Texto (String)           | `'Olá, mundo!'`, `'123'`         |
|             Booleano              |        `True`, `False`           |
|              Lista                | `[1, 2, 3]`, `['maçã', 'banana', 'laranja']` |
|              Tupla                |       `(1, 2, 3)`                |
|           Dicionário              |   `{'nome': 'João', 'idade': 25}` |
|             Conjunto              |       `{1, 2, 3}`                |
|            Null (None)            |             `None`               |
| Objeto Personalizado (Classes)    | Personalizado com propriedades e métodos | 
<div id='decisão'/>

## Estrutura de Decisão

As estruturas de decisão são parte fundamental na programação, permitindo que um programa tome decisões com base em condições específicas. Aqui estão algumas das estruturas de decisão mais comuns:

1. **IF (Se):** O IF verifica uma condição e executa um bloco de código se essa condição for verdadeira. Se a condição não for verdadeira, o bloco de código dentro do IF pode ser ignorado ou um bloco ELSE (senão) pode ser executado.

   Exemplo em Python:
   ```python
   idade = 20
   if idade >= 18:
       print("Você é maior de idade.")
   else:
       print("Você é menor de idade.")
   ```

2. **ELSE (Senão):** O ELSE é usado em conjunto com o IF para fornecer um bloco de código alternativo a ser executado caso a condição do IF não seja verdadeira.

3. **ELSE IF (ELIF, Senão Se):** O ELIF é utilizado para verificar condições adicionais quando a condição do IF não é atendida.

   Exemplo em Python:
   ```python
   nota = 75
   if nota >= 90:
       print("Nota A")
   elif nota >= 80:
       print("Nota B")
   elif nota >= 70:
       print("Nota C")
   else:
       print("Nota D")
   ```

4. **Switch-Case (Seleção de Caso):** Presente em algumas linguagens, como C++, Java e JavaScript, permite selecionar um bloco de código a ser executado com base no valor de uma variável.

   Exemplo em Java:
   ```java
   int opcao = 2;
   switch (opcao) {
       case 1:
           System.out.println("Opção 1 selecionada");
           break;
       case 2:
           System.out.println("Opção 2 selecionada");
           break;
       default:
           System.out.println("Opção inválida");
           break;
   }
   ```

Essas estruturas permitem que um programa tome diferentes caminhos com base em condições específicas, tornando possível criar lógicas mais complexas e dinâmicas. <div id='repetição'/>

## Estruturas de Repetição

As estruturas de repetição, também conhecidas como loops, são usadas para executar um bloco de código repetidamente enquanto uma condição é verdadeira, ou por um número específico de vezes. Aqui estão algumas das estruturas de repetição mais comuns:

1. **For:** O loop for é usado quando se sabe quantas vezes o código precisa ser repetido. Geralmente é usado com uma variável de iteração que é atualizada a cada iteração do loop.

   Exemplo em Python:
   ```python
   for i in range(5):  # Repetirá 5 vezes (0, 1, 2, 3, 4)
       print(i)
   ```

2. **While:** O loop while é usado quando a condição para a repetição não é baseada em um número específico de iterações, mas sim em uma condição booleana. O código é executado enquanto a condição for verdadeira.

   Exemplo em Python:
   ```python
   contador = 0
   while contador < 5:
       print(contador)
       contador += 1
   ```

3. **Do-While:** Presente em algumas linguagens (por exemplo, C, C++), é semelhante ao while, mas garante que o bloco de código seja executado pelo menos uma vez antes de verificar a condição.

   Exemplo em C:
   ```c
   int contador = 0;
   do {
       printf("%d\n", contador);
       contador++;
   } while (contador < 5);
   ```

Essas estruturas de repetição permitem a automação de tarefas repetitivas, o processamento de grandes volumes de dados e a execução de ações baseadas em condições específicas, tornando a programação mais eficiente e dinâmica. <div id='listas'/>

## Listas, Listas de Listas, Tuplas e Dicionário


Claro, vou explicar brevemente sobre listas, listas de listas, dicionários e tuplas em Python:

1. **Listas:** São coleções ordenadas e mutáveis de itens. Permitem armazenar diversos tipos de dados em uma única estrutura e são definidas por colchetes `[]`.

   Exemplo:
   ```python
   lista_frutas = ['maçã', 'banana', 'laranja']
   ```

2. **Listas de Listas:** São listas que contêm outras listas como elementos. Podem ser utilizadas para representar estruturas de dados mais complexas ou matrizes. 

   Exemplo:
   ```python
   matriz = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
   ```

3. **Dicionários:** São estruturas de dados que armazenam pares chave-valor, permitindo acesso aos valores por meio das chaves associadas. São definidos por chaves `{}` e são úteis para representar informações relacionadas.

   Exemplo:
   ```python
   dados_pessoa = {'nome': 'João', 'idade': 30, 'cidade': 'Exemplo'}
   ```

4. **Tuplas:** São coleções ordenadas e imutáveis de itens, geralmente utilizadas para armazenar dados relacionados de forma que não possam ser modificados. São definidas por parênteses `()`.

   Exemplo:
   ```python
   coordenadas = (10, 20)
   ```

Essas estruturas de dados são fundamentais em Python e oferecem maneiras diferentes de organizar e manipular conjuntos de informações. As listas e dicionários são mutáveis (podem ser alterados), enquanto as tuplas são imutáveis. O uso de cada uma depende das necessidades específicas de um determinado problema ou contexto.

### Como acessar os dados nessas variáveis

Claro, vou explicar como acessar os dados em cada uma das estruturas:

1. **Listas:**

   Para acessar os dados em uma lista, você pode usar seu índice (posição na lista). Os índices em Python começam em 0.

   Exemplo:
   ```python
   lista_frutas = ['maçã', 'banana', 'laranja']
   
   print(lista_frutas[0])  # Saída: 'maçã'
   print(lista_frutas[1])  # Saída: 'banana'
   print(lista_frutas[2])  # Saída: 'laranja'
   ```

2. **Listas de Listas:**

   Para acessar os dados em listas de listas, é necessário usar índices aninhados para acessar elementos específicos.

   Exemplo:
   ```python
   matriz = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
   
   print(matriz[0][0])  # Saída: 1
   print(matriz[1][2])  # Saída: 6
   ```

3. **Dicionários:**

   Para acessar os dados em um dicionário, você usa a chave correspondente ao valor desejado.

   Exemplo:
   ```python
   dados_pessoa = {'nome': 'João', 'idade': 30, 'cidade': 'Exemplo'}
   
   print(dados_pessoa['nome'])    # Saída: 'João'
   print(dados_pessoa['idade'])   # Saída: 30
   ```

4. **Tuplas:**

   O acesso aos dados em uma tupla é semelhante ao acesso em listas, usando índices.

   Exemplo:
   ```python
   coordenadas = (10, 20)
   
   print(coordenadas[0])  # Saída: 10
   print(coordenadas[1])  # Saída: 20
   ```

Essas são maneiras básicas de acessar os dados em diferentes tipos de estruturas em Python. É importante lembrar que algumas estruturas, como tuplas e dicionários, têm comportamentos específicos devido à imutabilidade ou ao uso de chaves para acessar valores. <div id='funções'/>

## Funções

As funções são blocos de código reutilizáveis que executam uma tarefa específica quando são chamadas. Elas são fundamentais na programação para modularizar o código, tornando-o mais legível, organizado e fácil de manter. Aqui está uma visão geral das funções em Python:

1. **Definindo uma Função:**
   
   Para definir uma função em Python, você usa a palavra-chave `def`, seguida pelo nome da função e, opcionalmente, parâmetros entre parênteses. O bloco de código da função é indentado.

   Exemplo:
   ```python
   def saudacao(nome):
       return f"Olá, {nome}!"
   ```

2. **Chamando uma Função:**

   Para chamar uma função, você simplesmente usa o nome da função seguido por parênteses, possivelmente passando argumentos se a função esperar parâmetros.

   Exemplo:
   ```python
   mensagem = saudacao('Maria')
   print(mensagem)  # Saída: Olá, Maria!
   ```

3. **Parâmetros e Argumentos:**

   As funções podem receber parâmetros (valores) que são passados quando a função é chamada. Esses parâmetros são usados dentro da função para realizar operações.

   Exemplo:
   ```python
   def soma(a, b):
       return a + b

   resultado = soma(3, 5)
   print(resultado)  # Saída: 8
   ```

4. **Retorno de Valores:**

   As funções podem retornar valores usando a palavra-chave `return`. Isso permite que o resultado da função seja usado em outras partes do código.

5. **Escopo de Variáveis:**

   Variáveis declaradas dentro de uma função têm um escopo local, o que significa que elas só existem dentro da função.

   Exemplo:
   ```python
   def minha_funcao():
       variavel_local = 10
       print(variavel_local)

   minha_funcao()  # Saída: 10
   print(variavel_local)  # Erro: NameError - variavel_local não está definida globalmente
   ```

As funções ajudam a organizar o código, evitando a repetição de blocos de código idênticos e facilitando a manutenção do programa. Elas são componentes essenciais em muitos aspectos da programação, permitindo modularidade, reusabilidade e legibilidade do código. <div id='desempenho'/>

## Desempenho de algorítmos

O desempenho de algoritmos é uma consideração crucial na programação, especialmente ao lidar com grandes conjuntos de dados ou sistemas que precisam ser eficientes. Aqui estão alguns pontos-chave relacionados ao desempenho dos algoritmos:

1. **Complexidade de Tempo e Espaço:**

   - **Complexidade de Tempo:** Refere-se à quantidade de tempo que um algoritmo leva para executar, geralmente expressa em termos de "O grande". Isso indica como o tempo de execução aumenta à medida que o tamanho da entrada aumenta.
   
   - **Complexidade de Espaço:** Refere-se à quantidade de memória usada por um algoritmo para resolver um problema, também expressa em termos de "O grande".

2. **Melhores, Piores e Casos Médios:**

   - **Melhor Caso:** O tempo mais rápido ou a menor quantidade de memória que um algoritmo pode levar para resolver um problema.
   
   - **Pior Caso:** O tempo mais lento ou a maior quantidade de memória que um algoritmo pode levar para resolver um problema.
   
   - **Caso Médio:** Tempo ou espaço médio esperado para resolver um problema, considerando diferentes entradas.

3. **Tipos de Complexidade:**

   - **Linear (O(n)):** Aumenta linearmente com o tamanho da entrada.
   
   - **Logarítmica (O(log n)):** Aumenta de forma logarítmica, com um crescimento muito mais lento que o linear.
   
   - **Quadrática (O(n^2)):** Aumenta com o quadrado do tamanho da entrada, sendo menos eficiente com entradas maiores.

4. **Fatores de Influência:**

   - **Tamanho da Entrada:** O desempenho do algoritmo pode variar drasticamente com diferentes tamanhos de entrada.
   
   - **Uso de Recursos:** Algoritmos que consomem mais recursos (CPU, memória) podem ser menos eficientes.

5. **Otimização de Algoritmos:**

   - **Técnicas de Otimização:** Reescrever algoritmos para reduzir a complexidade ou melhorar a eficiência.
   
   - **Escolha do Algoritmo:** Selecionar o algoritmo mais apropriado para um problema específico pode influenciar significativamente o desempenho.

6. **Análise Empírica e Teórica:**

   - **Análise Empírica:** Testar algoritmos com conjuntos de dados reais para medir o desempenho real.
   
   - **Análise Teórica:** Analisar a complexidade do algoritmo sem executá-lo.

7. **Trade-offs:**

   - Algoritmos mais eficientes em termos de tempo podem consumir mais memória e vice-versa. Otimizações em uma área podem resultar em perdas em outra.

O entendimento e a consideração do desempenho dos algoritmos são essenciais para a seleção adequada de técnicas de programação, especialmente em situações onde a eficiência é crítica, como sistemas de tempo real, processamento de grande volume de dados ou em ambientes com recursos limitados.

**Lembre-se que não é preciso inventar a roda, já existem muitos algorítmos prontos que reduzem a complexidade e aprimoram o desempenho.** <div id='dicas'/>

## Como melhorar a construir um algorítmo

Maneiras de melhorar algoritmos com dicas gerais:

### 1. Entenda a complexidade do algoritmo:
- Conheça a complexidade de tempo e espaço do seu algoritmo. Isso ajuda a entender como ele cresce com entradas maiores e a identificar oportunidades para melhorias.

### 2. Escolha a estrutura de dados certa:
- Utilize estruturas de dados eficientes para o problema em questão. Por exemplo, para busca rápida, use dicionários em vez de listas.

### 3. Escolha o algoritmo certo:
- Para problemas específicos, existem algoritmos otimizados. Por exemplo, para ordenação, existem diferentes algoritmos (Bubble Sort, Quick Sort, Merge Sort) com diferentes eficiências.

### 4. Refatore seu código:
- Simplifique o código, remova duplicações e torne-o mais legível. Às vezes, pequenas mudanças podem melhorar significativamente a eficiência.

### 5. Faça uso de técnicas avançadas:
- Explore técnicas como divisão e conquista, programação dinâmica, algoritmos greedy, entre outros, que são eficazes para resolver problemas específicos.

### 6. Otimização de laços:
- Evite laços aninhados sempre que possível, pois eles podem aumentar a complexidade do algoritmo. Procure oportunidades para otimizar ou parar iterações antecipadamente.

### 7. Teste e otimize:
- Teste seu código com diferentes conjuntos de dados para identificar gargalos de desempenho. Em seguida, otimize as partes do código que são mais lentas.

### 8. Use ferramentas e bibliotecas eficientes:
- Em muitos casos, bibliotecas já otimizadas oferecem implementações mais rápidas para operações comuns. Utilize-as sempre que possível.

### 9. Aprenda com outros códigos:
- Estude algoritmos bem otimizados e códigos eficientes. A análise de códigos de outras pessoas pode ajudar a aprender novas técnicas.

### 10. Mantenha-se atualizado:
- Esteja atento a novas descobertas, algoritmos e técnicas de otimização que possam surgir na área em que você trabalha.

Melhorar algoritmos é um processo contínuo. Às vezes, pequenas mudanças podem ter um grande impacto no desempenho do seu código!






