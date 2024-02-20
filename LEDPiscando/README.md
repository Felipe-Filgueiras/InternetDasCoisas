# Projeto de Piscar LED com Arduino

Este é um simples projeto de Arduino que pisca um LED conectado ao pino digital 4 com um intervalo de 500 ms ligado e 500 ms desligado.

## Materiais necessários

- Arduino Uno (ou outra placa compatível)
- LED
- Resistor de 220 ohms (ou valor próximo)
- Cabos jumper

## Conexões

Conecte o LED ao Arduino da seguinte maneira:

- Conecte o catodo (perna mais curta do LED) ao pino digital 4 do Arduino.
- Conecte o anodo (perna mais longa do LED) a um resistor de 220 ohms.
- Conecte o outro lado do resistor ao pino GND (terra) do Arduino.

Certifique-se de ter o ambiente de desenvolvimento Arduino configurado e pronto para usar.

## Código

```cpp
// Define o pino digital para o LED
const int pinoLed = 4;

void setup() {
  // Define o pino do LED como saída
  pinMode(pinoLed, OUTPUT);
}

void loop() {
  // Liga o LED
  digitalWrite(pinoLed, HIGH);
  // Aguarda 500 milissegundos
  delay(500);
  // Desliga o LED
  digitalWrite(pinoLed, LOW);
  // Aguarda mais 500 milissegundos
  delay(500);
}
````

<img src="LEDPiscando/circuit.png" alt="Embedded Video Streaming Project" width="300">
