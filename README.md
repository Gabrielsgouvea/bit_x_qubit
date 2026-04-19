# ⚛️ Bit vs Qubit: Simulação de Labirinto

> **Uma analogia visual interativa comparando o processamento sequencial clássico com o conceito de paralelismo massivo na computação quântica.**

## 🚀 Sobre o Projeto

Este projeto é uma simulação teórica desenvolvida em **HTML, CSS e JavaScript** que ilustra, por meio de uma analogia didática, a diferença fundamental entre a arquitetura de computadores atuais e o potencial da computação quântica.

Utilizando um problema clássico de busca em grafos (a resolução de um labirinto), a simulação demonstra como a natureza dos **Bits** e **Qubits** impacta a estratégia de exploração de soluções.

## ⚠️ Nota sobre a Precisão Científica

> **Esta simulação é uma analogia visual para fins educacionais.**
>
> Na realidade, computadores quânticos não "enviam cópias visíveis" de agentes por todos os caminhos simultaneamente. Eles utilizam fenômenos como **Superposição** e **Interferência Quântica** para manipular amplitudes de probabilidade. Os caminhos incorretos tendem a se cancelar (interferência destrutiva), enquanto o caminho correto é amplificado, permitindo que a solução seja encontrada com muito menos etapas computacionais do que em métodos clássicos sequenciais.

## 🧠 O Conceito Teórico

### 💻 Computador Clássico (Bit)
Nos computadores atuais, a unidade básica é o **Bit**, que assume valores determinísticos `0` ou `1`.
*   **Processamento Sequencial:** Para resolver o labirinto, o algoritmo clássico (DFS - *Depth First Search*) envia um único agente. Ele testa um caminho por vez.
*   **Backtracking:** Se encontra um beco sem saída, ele precisa voltar (*backtrack*) e tentar outra rota.
*   **Limitação:** Embora existam processadores multi-core, eles ainda enfrentam limitações ao lidar com problemas complexos, pois cada núcleo opera de forma sequencial e determinística.

### ⚛️ Computador Quântico (Qubit)
Na computação quântica, usamos **Qubits**. Graças ao fenômeno da **Superposição**, um qubit pode representar `0` e `1` simultaneamente.
*   **Paralelismo Quântico:** A simulação ilustra como esse estado permite explorar múltiplas probabilidades e rotas ao mesmo tempo.
*   **Eficiência:** Enquanto o clássico tenta, erra e volta, o sistema quântico (representado aqui pela expansão em largura) cobre o espaço de busca de forma exponencialmente mais rápida, colapsando na solução assim que ela é identificada.

## 🎮 Como Funciona a Simulação

Ao clicar em **"Começar"**, dois painéis lado a lado resolvem o mesmo labirinto gerado aleatoriamente:

| Característica | 🖥️ Clássico (Bit) | ⚛️ Quântico (Qubit) |
| :--- | :--- | :--- |
| **Algoritmo** | DFS (Busca em Profundidade) | BFS / Superposição (Busca em Largura) |
| **Comportamento** | Um agente azul explora, erra e volta. | Múltiplos agentes roxos expandem-se juntos. |
| **Visualização** | Mostra becos sem saída (vermelho). | Mostra a expansão simultânea de todos os caminhos válidos. |
| **Performance** | Mais lento (simula a limitação sequencial). | Extremamente rápido (simula o paralelismo quântico). |

## 🛠️ Tecnologias Utilizadas

O projeto foi construído como uma **Single Page Application (SPA)** leve, focada em performance gráfica no navegador.

*   **HTML5 Canvas:** Para renderização dinâmica do labirinto e dos agentes em alta resolução (suporte a High DPI).
*   **CSS3 Moderno:** Utilizando Flexbox, variáveis CSS e design responsivo.
*   **JavaScript (Vanilla ES6+):**
    *   Geração procedural de labirintos usando *Recursive Backtracker*.
    *   Implementação de algoritmos de busca (DFS e BFS).
    *   Loop de animação otimizado com `requestAnimationFrame`.
*   **Google Antigravity & Gemini 3.1:** Este código foi desenvolvido e refinado utilizando o ambiente experimental **Antigravity** do Google, com assistência inteligente do modelo **Gemini 3.1**.

## 📂 Estrutura do Arquivo

O projeto consiste em um único arquivo `Antigravity-Gemini-3.1.html` que contém toda a lógica, estilo e estrutura.

1.  **Geração do Labirinto:** Cria um grid 17x17 aleatório garantindo caminho solucionável.
2.  **Simulação Clássica:** O agente azul move-se passo a passo, marcando visitados e realizando backtracking quando necessário.
3.  **Simulação Quântica:** Os agentes roxos multiplicam-se a cada passo, preenchendo os caminhos válidos em paralelo, demonstrando a cobertura exponencial do espaço de busca.

## ▶️ Como Executar

1.  Baixe o arquivo `Antigravity-Gemini-3.1.html`.
2.  Abra-o em qualquer navegador moderno (Chrome, Firefox, Edge, Safari).
3.  Clique no botão **"Começar"** e observe a diferença de desempenho!

## 📄 Licença

Este projeto é open-source e está disponível para fins educacionais e de demonstração.
