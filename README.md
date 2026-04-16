# 🌱 Sistema de Irrigação Inteligente - FarmTech Solutions

## 📌 Descrição do Projeto

Este projeto simula um sistema de irrigação inteligente aplicado à agricultura digital, utilizando o microcontrolador ESP32 na plataforma Wokwi.

O sistema monitora as condições do solo em tempo real e automatiza a irrigação, garantindo uso eficiente da água.

---

## 🎯 Objetivo

Desenvolver um sistema capaz de:

* Monitorar a umidade do solo
* Simular o pH do solo
* Verificar os níveis de nutrientes (NPK)
* Automatizar a irrigação

---

## ⚙️ Componentes Utilizados

* ESP32
* Sensor DHT22 (umidade do solo - simulado)
* Sensor LDR (simulação de pH)
* 3 Botões (N, P e K)
* Módulo Relé (bomba de água)
* Jumpers (fios de conexão)

---

## 🔌 Funcionamento do Sistema

O sistema realiza leituras contínuas dos sensores e exibe os dados no monitor serial.

### 💧 Umidade (DHT22)

O sensor DHT22 mede a umidade do solo (simulada) e é o principal fator para decisão da irrigação.

---

### 🌡️ pH do Solo (LDR)

O sensor LDR simula o pH do solo através de valores analógicos.

Faixa adotada:

* 1500 a 2500 → pH ideal
* Fora dessa faixa → pH inadequado

---

### 🌱 Nutrientes (NPK)

Os botões representam:

* Nitrogênio (N)
* Fósforo (P)
* Potássio (K)

Botão pressionado → nutriente presente
Botão não pressionado → nutriente ausente

Os nutrientes influenciam o pH do solo e são utilizados para monitoramento.

---

## 🚿 Lógica de Irrigação

A irrigação é baseada na umidade do solo:

* Umidade < 60% → Irrigação LIGADA
* Umidade ≥ 60% → Irrigação DESLIGADA

Os valores de pH e NPK são utilizados apenas para análise e não interferem diretamente na irrigação.

---

## 🧠 Lógica do Sistema

O sistema executa:

1. Leitura da umidade (DHT22)
2. Leitura do LDR (pH)
3. Leitura dos botões (NPK)
4. Exibição dos dados no Serial Monitor
5. Decisão de ligar ou desligar a irrigação

---

## 📊 Monitoramento

O sistema exibe:

* Umidade (%)
* Valor do LDR
* Status dos nutrientes
* Estado da irrigação

---

## 🖼️ Imagens do Circuito


![Circuito](./imagens/circuito.png)


---

## 🚀 Possíveis Melhorias

* Integração com API de clima (Python)
* Previsão de chuva
* Análise de dados com R
* Uso de sensores reais

---

## 📚 Conclusão

O projeto demonstra como a tecnologia pode ser aplicada na agricultura para otimizar recursos, principalmente a água.

A automação permite decisões mais eficientes, contribuindo para o desenvolvimento de uma fazenda inteligente.
