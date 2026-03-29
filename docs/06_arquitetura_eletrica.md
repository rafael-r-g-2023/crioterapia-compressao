# ARQUITETURA ELÉTRICA

## Visão geral

Este documento define a estrutura elétrica do sistema V1.

---

## Alimentação

- Fonte principal: 12V DC
- Distribuição direta para cargas

---

## Conversão de tensão

- Regulador para alimentação do ESP32
- Conversão de 12V para 5V ou 3.3V

---

## Controle

- ESP32 como unidade central
- Controle de cargas via MOSFET

---

## Cargas

- Bomba de água
- Compressor de ar
- Válvula solenóide

---

## Sensores

### Temperatura
- Sensor digital (DS18B20)

### Pressão
- Sensor analógico

---

## Interface

- Botões conectados ao ESP32

---

## Estrutura elétrica

- Sistema com GND comum
- Linhas separadas para potência e controle

---

## Proteções

- Diodos de flyback nas cargas indutivas
- Proteção básica na entrada de alimentação

---

## Observações

- Arquitetura focada em simplicidade
- Projeto adequado para prototipagem inicial
- Base para desenvolvimento futuro de PCB
