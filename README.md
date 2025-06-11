# Meu-CPU-8-Bits-no-Logisim-My-CPU-8-BITS-in-Logisim-
 Minha CPU de 8 Bits criado no Logisim / My 8-Bit CPU created in Logisim
Processador de 8 bits com Foco em Aprendizado de Máquina
Visão Geral do Projeto
Este repositório contém o código e a implementação de um
processador de 8 bits modificado para aplicações educacionais,
com foco em operações de aprendizado de máquina (ML). O processador
simula a execução de modelos simples de ML, como redes neurais básicas
e regressão linear, em um ambiente controlado.
Estrutura do Processador:
1. ALU (Unidade Lógica e Aritmética): A ULA foi dividida em duas unidades:
 - Unidade Aritmética: Realiza operações como soma, subtração e overflow.
 - Unidade Lógica: Executa operações lógicas como AND, OR, XOR.
2. Datapath: O Datapath inclui registradores de propósito geral, barramentos de dados
e a integração com a ULA.
3. Memória: Armazena dados de treinamento e pesos do modelo. Permite a leitura e
atualização durante o processo de aprendizado.
4. Unidade de Controle: Controla o fluxo das operações dentro do processador.
Modificado para coordenar tarefas de ML como multiplicação de dados, cálculo de erro e ajuste de
pesos.
5. Cálculos de Aprendizado de Máquina: O processador foi adaptado para executar
operações de multiplicação (dados x pesos) e soma acumulada (MAC), essenciais em modelos de
ML simples.
Arquitetura
O Diagrama abaixo mostra a estrutura principal do processador após as modificações.
Ele inclui:
- Unidade Aritmética (Arithmetic Unit): Responsável por realizar as operações de soma, subtração,
cálculo de overflow e carry.
- Unidade Lógica (Logic Unit): Executa operações lógicas como AND, OR, XOR.
- Memória: Armazena dados de entrada e pesos do modelo.
- Registradores: Armazenam temporariamente dados de entrada, saída e pesos durante a
execução do modelo.
Fluxo de Dados:
1. Entrada de Dados: O processador recebe dados de entrada e pesos armazenados na memória.
2. Multiplicação de Dados e Pesos: A ULA realiza multiplicações (dados x pesos) e acumula os
resultados.
3. Cálculo de Erro: Após a execução, o erro é calculado comparando a saída prevista e a saída
real.
4. Atualização de Pesos: Os pesos são ajustados com base no erro calculado, utilizando uma regra
de aprendizado simples (ex: Delta Rule).
5. Display: A saída pode ser visualizada diretamente ou usada para decisões no controle do
processador.
Instruções de Uso
Requisitos:
- Logisim Evolution: Para simular o processador.
- Python 2.7.x: Se você desejar gerar instruções em Assembly para testes e simulações.
Passos para Simulação:
1. Clone este repositório:
$ git clone https://github.com/SeuUsuario/Processador-8-Bits-ML.git
$ cd Processador-8-Bits-ML
2. Abra o arquivo `Processor8bits.circ` no Logisim.
3. Configuração de Entrada: Dados de entrada e pesos podem ser definidos manualmente ou por
arquivos de dados.
4. Execute a Simulação: No Logisim, inicie a simulação e observe a execução do modelo de ML. A
saída será exibida no display.
5. Modificar o Modelo de ML: Você pode alterar os pesos ou os dados de entrada diretamente no
Logisim para testar diferentes modelos.
Arquitetura do Projeto
1. Processor8bits.circ: Arquivo principal de circuito, contém toda a configuração do processador de
8 bits e suas unidades (ULA, controle, Datapath).
2. README.md: Este arquivo! Explica a estrutura e como utilizar o projeto.
3. /Assembly/: Contém exemplos de código Assembly para testar a CPU com operações aritméticas
e lógicas.
4. /Test/: Arquivos gerados a partir do Assembly convertido para formato hexadecimal. Esses
arquivos podem ser carregados diretamente no Logisim.
5. /Docs/: Contém materiais de apoio e apresentações sobre a arquitetura do processador e as
modificações.
Como Contribuir
Se você deseja contribuir com melhorias, sugestões ou novos modelos de aprendizado de
máquina, fique à vontade para fazer um Fork do repositório, adicionar suas mudanças e submeter
uma pull request.
Referências
1. Tanenbaum, A. S. Organização e Estrutura de Computadores. Pearson Prentice Hall.
2. Goodfellow, I., et al. Deep Learning. MIT Press.
3. Schuurman, D. C. (2013). Step-by-step design and simulation of a simple CPU architecture.
4. 
