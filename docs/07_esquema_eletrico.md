# ESQUEMA ELÉTRICO

## Visão geral

[Fonte 12V]
     ↓
[Distribuição]
     ↓
+-----------+-----------+-----------+
|           |           |           |
Bomba     Compressor   Válvula   Regulador
                                ↓
                              ESP32

Este documento define as conexões elétricas do sistema.

---

## Alimentação

+12V  → linha positiva
GND   → linha negativa

- Fonte 12V DC
- Linha principal distribuída para cargas

---

## Regulador

- Conversão de 12V para 5V/3.3V
- Alimentação do ESP32

---

## Controle de cargas

+12V -----------+
                |
             [BOMBA]
                |
                +-------> Dreno (MOSFET)
                          |
                       MOSFET
                          |
GND ----------------------+

GPIO → Resistor → Gate do MOSFET

- MOSFET para cada carga:
  - Bomba
  - Compressor
  - Válvula

---

## Proteção

   +12V
     |
   [Carga]
     |
     +------ MOSFET
     |
    | |
    | | Diodo (flyback)
    |_|
     |
    +12V

- Diodo flyback em cada carga indutiva

---

## Sensores

### Temperatura

VCC → 3.3V
GND → GND
DATA → GPIO

+ resistor 4.7k entre VCC e DATA
  
- DS18B20
- Comunicação digital

### Pressão

VCC → 5V ou 3.3V
GND → GND
OUT → GPIO analógico

- Sensor analógico

---

## Interface

GPIO → botão → GND

- Botões conectados aos GPIOs

---

## Estrutura

- GND comum
- Separação entre potência e controle

---
DIAGRAMA GERAL (SIMPLIFICADO)

ESP32
│
├── MOSFET → Bomba
├── MOSFET → Compressor
├── MOSFET → Válvula
│
├── Sensor temperatura
├── Sensor pressão
└── Botões

## Observações

- Projeto voltado para prototipagem
- Base para futura criação de PCB
