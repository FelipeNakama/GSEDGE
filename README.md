Integrantes do Grupo:

Felipe Megumi Nakama RM:552821

Micael Azarias RM:552699

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Sistema de Monitoramento de Temperatura para Amostras de Exame de Sangue

## Descrição do Projeto
Este projeto utiliza um Arduino UNO R3 em conjunto com sensores e componentes eletrônicos para monitorar a temperatura de amostras de exame de sangue em centros de coleta. O objetivo é garantir que as amostras sejam armazenadas corretamente, reduzindo problemas como a inviabilidade de amostras devido a condições inadequadas de armazenamento.

## Componentes Necessários
- Arduino UNO R3
- Protoboard
- Tela LCD clássica
- Potenciômetro
- 3 LEDs (azul, verde e vermelho)
- Sensor de temperatura TMP36
- 4 Resistores de 220 ohms
- Fios de conexão

## Montagem do Circuito
- Conecte o Sensor de Temperatura TMP36 à protoboard.
- Conecte os LEDs (azul, verde e vermelho) à protoboard, utilizando resistores de 220 ohms para limitar a corrente.
- Conecte o potenciômetro à protoboard para ajuste do contraste da tela LCD.
- Conecte a tela LCD à protoboard.
- Conecte os fios de conexão conforme indicado no código fornecido.
  
## Configuração do Software Arduíno IDE

Instale o Arduino IDE:
- Faça o download da última versão do Arduino IDE em Arduino Software.
- Siga as instruções de instalação para o seu sistema operacional.
- Instale a Biblioteca LiquidCrystal:

Abra o Arduino IDE.
- Vá para "Sketch" -> "Include Library" -> "Manage Libraries...".
- Na janela que se abre, digite "LiquidCrystal" na barra de pesquisa.
- Localize a biblioteca "LiquidCrystal" por Francisco Malpartida e clique no botão "Install".

Abra o Código do Projeto:
- Copie o código fornecido para um novo arquivo no Arduino IDE ou abra diretamente o arquivo fornecido.

Selecione a Porta USB:
- Conecte o cabo USB ao Arduíno UNO R3 e ao computador
- Vá para "Tools" -> "Port" e selecione a porta USB à qual o Arduino está conectado.
  
Compile e Carregue o Código no Arduino:
- Clique no botão de "Verificação" (ícone de visto) para compilar o código e garantir que não há erros.
- Clique no botão de "Carregar" (ícone de seta para a direita) para enviar o código para o Arduino.

Ajuste do Potenciômetro:
- Se o contraste da tela LCD não estiver adequado, ajuste o potenciômetro conectado à protoboard.

Observe a Saída:
- Abra a "Serial Monitor" no Arduino IDE para visualizar as leituras de temperatura e informações adicionais.

## Funcionamento
O sistema lê a temperatura da amostra de sangue por meio do sensor TMP36. Essa leitura é exibida em uma tela LCD, juntamente com mensagens indicativas da faixa de temperatura em que a amostra se encontra. Além disso, três LEDs indicam visualmente se a temperatura está baixa, adequada ou alta.

## Limites de Temperatura
Os limites de temperatura podem ser ajustados no código conforme necessário, atualmente estão configurados entre 2°C e 6°C, que é range ideal de temperatura para o armazenamento de amostras de sangue coletadas

## Simulação do Projeto:
https://www.tinkercad.com/things/eoummDj0RCY-gs-medidor-de-temperatura-amostra-de-sangue
