# Atendimento do Professor

## Terças e quintas. Professor de horário parcial. Nesses 2 dias, podem contar comigo!

# Semama 02 - Introdução à Eletrônica Analógica

## Impactos no seu Projeto

* Montagem de circuitos auxiliares:
  * ao braço robótico
  * ao leitor de QRCode
  * ao motor de passo
* Diagnóstico de falhas de fontes
* Filtragem de ruído


# Isso é uma bomba!

![Fonte](https://github.com/agodoi/m05-semana02/blob/main/imgs/fonte12V1A.jpg)

## Princpiais problemas

* Regulador de tensão com defeito
* Diodos em curto
* Capacitores abertos
* Resistores superaquecidos com valores alterados

### Bora Aprender Eletrônica e Diagnosticar com Instrumentação de Bancada!

# 1ª Lei - Ohm

<img src="https://github.com/agodoi/m05-semana02/blob/main/imgs/pessoa_vendo.jpg" width="250"> <img src="https://github.com/agodoi/m05-semana02/blob/main/imgs/pessoa_sorrindo.jpg" width="250">

## Fórmula

$$
V = R \cdot I
$$


<img src="https://github.com/agodoi/m05-semana02/blob/main/imgs/leideohm.jpg" width="500">



# 2ª Lei - Kirchhoff para Tensões (LKT)

<img src="https://github.com/agodoi/m05-semana02/blob/main/imgs/montanha_russa.png" width="500">


* Imagine uma montanha-russa onde o carrinho sobe uma colina e depois desce em várias partes da pista.
* A energia total que o carrinho ganha no início (tensão fornecida pela bateria) deve ser totalmente dissipada ao longo do percurso (quedas de tensão nos resistores).
* Isso representa a soma algébrica das tensões em um circuito fechado, que deve ser zero.

## Fórmula

$$
V_1 + V_2 + V_3 + ... + V_n = 0
$$

$$
R_1.I_1 + R_2.I_2 + R_3.I_3 + ... + R_n.I_n = 0
$$



# 3ª Lei - Kirchhoff para Corrente (LKC)

<img src="https://github.com/agodoi/m05-semana02/blob/main/imgs/rotatoria.jpg" width="500">


* Imagine um cruzamento de ruas onde carros entram e saem.
* A soma dos carros que entram em um cruzamento deve ser igual à soma dos carros que saem.
* Assim como em um nó de um circuito, a soma das correntes que entram deve ser igual à soma das que saem.

## Fórmula

$$
\sum I_{entrada} = \sum I_{saida}
$$

# Onde usar cada Lei?

### Lei de Ohm, em todos os diagnósticos e conferências de circuitos

### Lei de Kirchhoff, quando for projetar ou resolver problemas com o esquema elétrico em mãos.

# Simulador TinkerCad

Usaremos esse simulador para aprender a Lei de Ohm por meio da instrumentação de bancada.

* Usaremos multímetro na escala de tensão
* Multímetro na escala de corrente
* Gerador de Sinais
* Fonte de bancada


# Hands On

## (1) Monte o circuito abaixo no TinkerCad e realize as medições solicitadas

<img src="https://github.com/agodoi/m05-semana02/blob/main/imgs/circuito-serie.png" width="500">

R1 (esquerda) e R2 (centro) = 100 ohms
R3 (direita) = 330 ohms


### (1.1) Medição da tensão

Medir a tensão (voltagem) é uma das funções mais comuns de um multímetro digital ou analógico. A tensão é medida em **volts (V)** e pode ser classificada como tensão contínua (DC) ou alternada (AC).

### (1.2) Coloque o seletor na escala de tensão apropriada

   - **DCV (Tensão Contínua)** para medir baterias, fontes de alimentação CC, etc.
   - **ACV (Tensão Alternada)** para medir tomadas, circuitos AC, etc.
   - Certifique-se de selecionar uma escala maior do que a tensão esperada, caso o multímetro não seja automático.

### (1.3) Conecte os cabos
   - **Cabo preto (COM):** Insira no conector marcado como "COM".
   - **Cabo vermelho:** Insira no conector marcado como "V" ou "Volt".

### (1.4) Conectando ao Circuito
   - **Ligue o multímetro** e coloque as pontas de prova nos pontos onde deseja medir a tensão:
   - **Ponta preta:** Conecte ao ponto de referência ou terra (GND).
   - **Ponta vermelha:** Conecte ao ponto onde deseja medir a tensão.

### (1.3) Observação sobre polaridade
   - Para tensão DC, observe a polaridade:
   - Se a ponta vermelha estiver no positivo e a preta no negativo, a leitura será positiva.
   - Caso contrário, a leitura será negativa.
   - Para tensão AC, a polaridade não importa.

## (1.4) Leitura da Medida
   - **Observe o valor no display do multímetro**:
   - O valor exibido será a tensão entre os dois pontos medidos.
   - Certifique-se de que a unidade (V, mV) esteja correta.

## (1.5) Dicas Importantes
   - **Segurança:** Sempre tenha cuidado ao medir tensões em tomadas ou circuitos vivos. Use proteção adequada.
   - **Não exceda a escala:** Se não souber a tensão esperada, comece na escala mais alta e vá reduzindo.
   - **Calibração:** Certifique-se de que o multímetro esteja calibrado para medidas precisas.

## (1.6) Meça o quanto vale o VR1, VR2 e VR3.

## (1.7) Comprove matematicamente, pela Lei de Ohm, o valor que você mediu

---
### (2.1) Medição da Corrente

Medir a corrente elétrica é também uma das funções mais importantes de um multímetro digital ou analógico. A corrente é medida em **ampères (A)** e pode ser classificada como corrente contínua (DC) ou alternada (AC).

### (2.2) Coloque o seletor na escala de corrente apropriada

   - **DCA (Corrente Contínua)** para medir circuitos alimentados por fontes CC.
   - **ACA (Corrente Alternada)** para medir circuitos alimentados por fontes AC.
   - Certifique-se de selecionar a escala adequada para a corrente esperada, geralmente especificada no circuito. Use a escala mais alta se não souber o valor aproximado.

### (2.3) Conecte os cabos
   - **Cabo preto (COM):** Insira no conector marcado como "COM".
   - **Cabo vermelho:**
     - Insira no conector marcado como "A" ou "10A" para correntes altas.
     - Insira no conector marcado como "mA" para correntes menores (se disponível).

### (2.4) Conectando ao Circuito
   - **Interrompa o circuito** no ponto onde deseja medir a corrente, removendo o respectivo jumper.
   - Conecte o multímetro **em série** com o circuito:
     - **Ponta vermelha:** Conecte ao lado do circuito que está mais próximo do positivo ou da fonte.
     - **Ponta preta:** Conecte ao lado do circuito que está mais próximo do negativo ou GND.

### (2.5) Observação sobre polaridade
   - Para corrente DC, observe a polaridade:
     - Se a corrente fluir no sentido convencional (ponta vermelha no lado positivo), a leitura será positiva.
     - Caso contrário, a leitura será negativa.
   - Para corrente AC, a polaridade não importa.

## (2.6) Leitura da Medida
   - O valor exibido será a corrente que flui pelo ponto medido.
   - Certifique-se de que a unidade (A, mA, µA) esteja correta para a faixa selecionada.

## (2.7) Dicas Importantes
- **Segurança:** Sempre tenha cuidado ao medir correntes altas. Use proteção adequada e certifique-se de que o multímetro suporta o valor esperado.
- **Evite danos:** Nunca tente medir corrente em um circuito sem interrompê-lo. Nunca conectar o multímetro em paralelo usando a escala de corrente.
- **Calibração:** Certifique-se de que o multímetro esteja calibrado para garantir medidas precisas.

## (2.8) Meça a corrente nos resistores IR1, IR2 e IR3.

## (2.9) Comprove matematicamente, pela Lei de Ohm, o valor que você mediu.


## (3) Meça Tensão e Corrente no circuito Paralelo abaixo e comprove matematicamente seu valor.

<img src="https://github.com/agodoi/m05-semana02/blob/main/imgs/circuito-paralelo.png" width="500">

## (4) Meça Tensão e Corrente no circuito Misto abaixo e comprove matematicamente seus valores.

<img src="https://github.com/agodoi/m05-semana02/blob/main/imgs/circuito-misto.png" width="500">

## (5) Aplicando LKT

<img src="https://github.com/agodoi/m05-semana02/blob/main/imgs/circuito-misto-lkt.png" width="500">

[circuito](https://www.tinkercad.com/things/2xXIkL78lpx-eletricidade-simulacao-corrente/editel?returnTo=https%3A%2F%2Fwww.tinkercad.com%2Fdashboard%2Fdesigns%2Fcircuits%3Fpage%3D1&sharecode=LYk_PSfHtcqp-YjCDKfLuxgOQWMHT0V35CXY6Yg4WA8)

### Dados do circuito:

* Fonte CC da esquerda = 45V
* Fonte CC da direita = 10V
* Resistor superior horizontal esquerdo (R1) = 2 ohms
* Resistor superior horizontal direito (R2) = 9 ohms
* Resistor vertical central (R3) = 12 ohms
* Resitor inferior horizontal esquerdo (R5) = 4 ohms
* Resistor inferior horizontal direito (R4) = 3 ohms

## Ponderada do Dia

Cada aluno deve comprovar matematicamente o valor da corrente I1 (malha 1) e I2 (malha 2) usando o LKT e a Lei de Ohm.
Montar o circuito em seu TinkerCad, ligar as fontes CC, os resistores, e o amperímetro para medir o Itotal saindo da fonte de 45V, outro para medir o Itotal saindo da fonte de 10V e terceiro amperímetro para medir a corrente no ramo do R3. Além dos amperímetros, precisa ligar um voltímetro em cada resistor do circuito.

### Barema

Trabalho individual. O que precisa ser entregue?

Relatório em PDF contendo:

 (a) Print do Tinkercad com os instrumentos mostrando os valores medidos (tensão e corrente);
 (b) Link do seu Tinkercad da sua montagem e simulação. Cuidado ao pegar essa URL. Pegue pelo botão **ENVIAR PARA** que fica no canto direito superior;
 (c) Explicar porque a corrente I1 e I2 deram sinal positivo ou negativo;
 (d) Apresentar as equações das respectivas malhas 1 e 2 (isto é, o sistema linear matemático);
 (e) Apresentar os resultados de I1 e de I2 calculados, que precisam bater com os valores simulados;
 (f) Suponha que seu multímetro tenha 12 ohms de impedância interna na escala de tensão. O que aconteceria com o valor da tensão medido no R3? Justifique.

