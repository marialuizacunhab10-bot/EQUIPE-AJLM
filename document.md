# Manual de montagem do robô definitivo

**Discentes:** Amanda Lemos, Júlia Nunes, Luana Bastos e Maria Luiza Cunha
**Docente:** Robson Marinho
**Disciplina:** Computação Aplicada à Engenharia


------------


Este manual foi montado com o objetivo de descrever a montagem mecânica e eletrônica do Otto Ninja, incluindo rodas com O-rings e retroescavadeira simples.
## 1. Visão geral do robô

O Otto Ninja é um robô educacional com:

- Controle via ESP8266 (Otto Ninja PCB ou Wemos + Servo Shield)

- Locomoção por rodas com O-rings (não é bípedo)

- Sensor ultrassônico frontal

- Interface sonora e visual (buzzer, botão, LED matrix ou OLED – opcionais)

- Retroescavadeira frontal fixa com pá móvel

## 2. Lista de componentes

**2.1 Eletrônica**

- Otto Ninja PCB ESP8266 (ou Wemos + Servo Shield)

- Cabo Micro USB (dados)

- Bateria 9V 6F22 recarregável (650mAh)

- Toggle switch + UBEC 5V / 3A + conector XH 2P + clip 9V

- Sensor ultrassônico HC-SR04

- Módulo botão com headers

- Módulo buzzer com headers

- 1 × Cabo Dupont 4 pinos

- 2 × Cabos Dupont 3 pinos

*Opcionais*

- Matriz LED 16×8 HT16K33

- Display OLED 1.3"/6g

**2.2 Atuadores**

- 2 × Servo 180° metal gear (posicionais)

- 2 × Servo 360° metal gear (rotação contínua)

**2.3 Fixação e ferramentas**

- 4 × Parafusos metálicos autoatarraxantes M2×5 (ferromagnéticos)

- Chave Phillips 2.5×40mm (ponta magnética)

**2.4 Peças impressas em 3D**

- Base – preta

- Inner Bottom – preto

- Starter Lid – preto

- Plate Matrix Lid – preto

- Plate Ultrasonic Lid – rosa

- Band – vermelha

- Legs – preto

- Ankle Left – preto

- Ankle Right – preto

- 2 × Foot – preto

- Retroescavadeira

- Pá frontal (integrada, sem braços adicionais)

**2.5 Rodas**

- 2 × O-rings (68 mm OD / 60 mm ID / 4 mm)

##3. Preparação dos servos (etapa crítica)

Antes de montar:

- Conecte cada servo à placa

- Alimente com 5V do UBEC

- Posicione os servos 180° em posição central (90°)

- Servos 360° devem estar parados (neutro)

Nunca force o eixo do servo manualmente.

##4. Montagem da base

1. Posicione o Inner Bottom dentro da Base

2. Fixe utilizando os parafusos M2×5

3. Garanta que as aberturas laterais fiquem livres

##5. Montagem do sistema de locomoção (rodas)
**5.1 Servos de tração**

1. Instale os 2 servos 360° nas laterais da Base

2. O eixo deve ficar voltado para fora

3. Parafuse firmemente

**5.2 Rodas com O-ring**

1. Encaixe cada Foot no eixo do servo

2. Coloque o O-ring ao redor do Foot

3. O O-ring funciona como pneu de tração

##6. Montagem da estrutura superior

1. Fixe a peça Legs sobre a Base

2. Instale o Ankle Left e Ankle Right conforme o lado correto

3. Verifique alinhamento vertical

##7. Montagem da retroescavadeira

A retroescavadeira deste modelo possui apenas a pá, sem braços adicionais.

1. Posicione a pá frontal no encaixe da Base

2. Fixe com parafuso M2×5

3. Instale 1 servo 180° responsável pelo movimento da pá

4. Centralize o servo antes da fixação

##8. Instalação da eletrônica
**8.1 Placa principal**

1. Fixe a Otto Ninja PCB ESP8266 na Base

2. Caso use Wemos, conecte ao Servo Shield

**8.2 Alimentação**

1. Conecte a bateria 9V ao UBEC

2. Saída do UBEC (5V) → placa e servos

3. Instale o toggle switch entre bateria e UBEC

**8.3 Conexões**

- Servos 360° → canais de tração

- Servo 180° (pá) → canal dedicado

- Sensor HC-SR04 → cabo Dupont 4 pinos

- Botão → cabo Dupont 3 pinos

- Buzzer → cabo Dupont 3 pinos

##9. Sensor ultrassônico

1. Fixe o HC-SR04 na Plate Ultrasonic Lid (rosa)

2. Encaixe a tampa na parte frontal

3. Atenção aos pinos: VCC / TRIG / ECHO / GND

##10. Módulos opcionais
**10.1 Matriz LED 16×8**

1. Fixe na Plate Matrix Lid

2. Conecte via I2C

**10.2 Display OLED**

3.  Fixe na tampa correspondente

4.  Conecte via I2C

##11. Fechamento do robô

1. Organize os cabos internamente

2.  Coloque o Starter Lid

3.  Finalize com a Band vermelha

##12. Testes finais

- Teste rotação das rodas

- Teste subida/descida da pá

- Teste sensor ultrassônico

- Teste botão e buzzer

Se algum movimento estiver errado, revise a centralização dos servos.

##13. Conclusão

O Otto Ninja está completamente montado, incluindo:

- Locomoção por rodas com O-ring

- Retroescavadeira frontal simples

- Eletrônica baseada em ESP8266

- Agora ele está pronto para programação e testes.
