# Componentes Eletrônicos para o balão estratosférico do Projeto Sapiens-1 - LaSE - UnB

Este documento lista os principais componentes utilizados para o balão estratosférico do Projeto Sapiens-1, organizados por subsistemas.

## OBDH (On-Board Data Handling)

### Raspberry Pi Zero 2W
- **Função**: Computador de bordo principal
- **Descrição**: Microcomputador responsável pelo processamento de dados, controle dos subsistemas e execução dos experimentos
- **Especificações principais**:
  - Processador: Quad-core ARM Cortex-A53 64-bit @ 1GHz
  - RAM: 512MB LPDDR2
  - Conectividade: Wi-Fi 2.4GHz, Bluetooth 4.2/BLE
  - GPIO: 40 pinos
- **Datasheet**: [Link para o datasheet](https://datasheets.raspberrypi.com/rpizero2/raspberry-pi-zero-2-w-product-brief.pdf)

### INA266
- **Função**: Monitor de corrente e tensão
- **Descrição**: Sensor de corrente bidirecional e monitor de tensão para monitoramento do sistema de energia
- **Especificações principais**:
  - Tensão de alimentação: 2.7V a 5.5V
  - Corrente máxima: ±81.92A
  - Resolução: 16-bit
  - Interface: I²C
- **Datasheet**: [Link para o datasheet](https://www.alldatasheet.com/datasheet-pdf/pdf/419932/TI1/INA226.html)

### TPL5010
- **Função**: Watchdog Timer
- **Descrição**: Timer de watchdog de baixo consumo para reinicialização automática do sistema em caso de travamento
- **Especificações principais**:
  - Tensão de operação: 1.8V a 5.5V
  - Corrente de operação: 35nA (típico)
  - Intervalo de tempo: 100ms a 7200s
  - Interface: Pulso de reset
  - Temperatura de operação: -40°C a +125°C
- **Datasheet**: [Link para o datasheet](https://www.alldatasheet.com/datasheet-pdf/pdf/683850/TI1/TPL5010.html)

### BME280
- **Função**: Sensor ambiental
- **Descrição**: Sensor combinado de pressão barométrica, temperatura e umidade relativa
- **Especificações principais**:
  - Pressão: 300-1100 hPa (±1 hPa)
  - Temperatura: -40 a +85°C (±1°C)
  - Umidade: 0-100% RH (±3% RH)
  - Interface: I²C/SPI
  - Tensão de operação: 1.71V a 3.6V
- **Datasheet**: [Link para o datasheet](https://www.alldatasheet.com/datasheet-pdf/pdf/2163285/BOSCH/BME280.html)

---

## EPS (Electrical Power System)

### Energizer Ultimate Lithium (L91)
- **Função**: Bateria primária
- **Descrição**: Bateria de lítio AA de alta performance para aplicações extremas
- **Especificações principais**:
  - Tensão nominal: 1.5V
  - Capacidade: 3000-3500 mAh
  - Temperatura de operação: -40°C a +60°C
  - Química: Lítio-Ferro Dissulfeto (LiFeS2)
  - Vida útil: 20+ anos
  - Peso: ~15g
- **Datasheet**: [Link para o datasheet](https://data.energizer.com/pdfs/l91.pdf)

### DS18B20 (Sonda de Temperatura)
- **Função**: Monitor de temperatura das baterias
- **Descrição**: Sensor de temperatura digital de precisão em formato de sonda para monitoramento térmico das baterias
- **Especificações principais**:
  - Faixa de temperatura: -55°C a +125°C
  - Precisão: ±0.5°C (-10°C a +85°C)
  - Resolução: 9 a 12 bits configurável
  - Interface: 1-Wire
  - Tensão de operação: 3.0V a 5.5V
  - Tempo de conversão: 750ms (12-bit)
- **Datasheet**: [Link para o datasheet](https://www.alldatasheet.com/datasheet-pdf/pdf/58557/DALLAS/DS18B20.html)

---

## TT&C (Telemetry, Tracking and Command) (Verificar se a antena é ideal)**

### Heltec WiFi LoRa 32
- **Função**: Módulo de comunicação principal
- **Descrição**: Placa de desenvolvimento com ESP32, Wi-Fi, Bluetooth e transceptor LoRa integrados
- **Especificações principais**:
  - Processador: ESP32 dual-core 240MHz
  - Wi-Fi: 802.11 b/g/n
  - Bluetooth: v4.2 BR/EDR e BLE
  - LoRa: SX1276 (868/915 MHz)
  - Flash: 8MB
  - RAM: 520KB
  - Display: OLED 0.96" integrado
  - GPIO: 18 pinos disponíveis
- **Datasheet**: [Link para o datasheet](https://heltec.org/project/wifi-lora-32-v3/)

### Antena Omnidirecional 915 MHz
- **Função**: Antena para comunicação LoRa
- **Descrição**: Antena omnidirecional otimizada para frequência de 915 MHz (banda ISM)

---

## Sensores e Instrumentação

---

**Última atualização**: 12 de julho de 2025  
**Responsável**: Equipe de Eletrônica do projeto Sapiens-1 do Laboratório de Sistemas Espaciais - UnB
