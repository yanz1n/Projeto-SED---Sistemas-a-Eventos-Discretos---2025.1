# Projeto-SED---Sistemas-a-Eventos-Discretos---2025.1
Esse repositório apresenta uma solução de modo a realizar a síntese de um Supervisor para o problema do Gato e do Rato Usando Supremica.

# Objetivos

- Construir um modelo de autômato e supervisor que represente o sistema e suas especificacações utilizando o software Supremica;
- Reforçar e utilizar da teoria de controle supervisório de autômatos determinísticos vista na disciplina.

# Descrição do Sistema

Imagine uma torre com 5 salas conectadas em um ciclo (Sala 1 → Sala 2 → Sala 3 → Sala 4 → Sala 5 → Sala 1). Há um gato e um rato que se movem livremente entre as salas. Sem controle:

- O gato pode entrar em qualquer sala adjacente:
  - Eventos: gato_move_esquerda, gato_move_direita

- O rato idem:
  - Eventos: rato_move_esquerda, rato_move_direita

# Especificações

- O gato não pode entrar na sala onde o rato está. Caso isso ocorra, o gato irá comer o rato (estado perigoso).
- O sistema deve ser não bloqueante e garantir o máximo de liberdade para o gato e o rato.

  # Eventos

  - Controláveis: Movimentos do gato (podem ser desabilitados pelo supervisor).
  - Não controláveis: Movimentos do rato (não podem ser desabilitados pelo supervisor).

 # Comando
 Construir um autômato e o supervisor utilizando o software Supremica.

 # Implementação
Foi realizado a modelagem de 5 autômatos correspondentes a cada uma das 5 salas, onde cada sala possui 4 estados:

- Vazia;
- Apenas o gato na sala;
- Apenas o rato na sala;
- Gato e Rato na sala.

Este último estado é o estado indesejado para cada um desses autômatos, portanto, foram marcados como proibidos (forbidden). Os eventos de movimento do rato foram considerados controláveis quando este se move entre salas conectadas por portas e incontroláveis quando se locomovem entre salas sem portas.

 # Autor

 [Yan Abrantes](https://github.com/yanz1n)

 # Arquivo da Solução do Supremica

 [Arquivo](https://github.com/yanz1n/Projeto-SED---Sistemas-a-Eventos-Discretos---2025.1/blob/main/ProjetoSED_Salas.wmod)

 # Slides

 [Slides utilizado no vídeo descrevendo o sistema](https://github.com/yanz1n/Projeto-SED---Sistemas-a-Eventos-Discretos---2025.1/blob/main/Apresentacao_ProjetoSED.pdf)

 # Esquema Utilizado
![Esquema do Sistema](https://github.com/yanz1n/Projeto-SED---Sistemas-a-Eventos-Discretos---2025.1/blob/main/Esquema_remodelado.png)

 # Vídeo Demonstrativo
 
[Vídeo demonstrativo](https://drive.google.com/file/d/1mEHa9MMcA8azv8ORKV6Zb5ost1DCAewS/view?usp=sharing)
 
