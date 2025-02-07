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

<img src="https://github.com/agodoi/m05-semana02/blob/main/imgs/circuito-01.png" width="500">

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

## (1.6) Quando vale o VR1, VR2 e VR3? 


## Comprovando matematicamente os valores observados usando LKC



