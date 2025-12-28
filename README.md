# 💨 Calculadora de Mezclas - Canary Vape Shop

![Version](https://img.shields.io/badge/version-1.0.0-blue.svg) ![Status](https://img.shields.io/badge/status-production-green.svg) ![Stack](https://img.shields.io/badge/tech-HTML%20%7C%20CSS%20%7C%20JS-yellow.svg)

Web App de uso interno diseñada para optimizar y estandarizar el proceso de venta y mezcla de eliquids en mostrador. Automatiza los cálculos de alquimia basándose en la resistencia del dispositivo del cliente y el formato del bote.

## 🚀 Propósito del Proyecto

El objetivo principal es **eliminar el error humano** en la tienda y **normalizar las mezclas**. La aplicación asegura que, independientemente de quién atienda, el cliente siempre reciba el líquido con la proporción VG/PG y nicotina exacta para su dispositivo.

## ✨ Funcionalidades Clave

### 🧠 1. Lógica Inteligente de Hardware
El sistema no solo calcula ml, sino que sugiere la mezcla según la resistencia:
* **PODS (0.8Ω - 1.2Ω):** Prioriza Sales de Nicotina y ratios 50/50 o 60/40.
* **AIO / RDL (0.6Ω - 0.4Ω):** Balancea entre Sales y Base Libre según potencia.
* **Sub-Ohm / Cloud (0.3Ω - 0.2Ω):** Prioriza Base Libre y Max VG (70/30).

### 🧪 2. Algoritmo de Equilibrio Químico
Para conseguir el ratio objetivo (ej. 60VG/40PG) usando nicokits de Sales (que vienen en 100% VG o 100% PG), la app calcula combinaciones exactas:
* *Ejemplo:* Si se necesitan 2 nicokits, la app puede sugerir **1 Naranja (VG)** y **1 Rosa (PG)** para equilibrar la mezcla automáticamente.

### 💰 3. Estrategia de Venta (Upselling)
El algoritmo de cálculo de nicotina aplica un **redondeo al alza** en el número de nicokits necesarios.
* *Beneficio:* Asegura la venta del nicokit completo y evita acumular restos de botes abiertos en la tienda.

### 🎨 4. Sistema Visual de Iconos (CSS Puro)
Para facilitar la rapidez en mostrador, se utilizan códigos de color visuales sin necesidad de imágenes pesadas:
* 🔵 **Azul:** Aroma
* 🟠 **Naranja:** Sales VG
* 💗 **Rosa:** Sales PG
* 🟣 **Morado:** Base Libre
* 🟡 **Amarillo:** Base de Relleno

### 📄 5. Módulo de Impresión (Cheat Sheet)
Incluye un enlace directo a una **Guía Maestra de Mezclas** (`imprimir.html`) optimizada para impresora (fondo blanco, alto contraste) para tener una referencia física plastificada en tienda.

---

## 📂 Estructura del Proyecto

```text
/
├── index.html       # La Aplicación Web (Calculadora)
├── imprimir.html    # La Guía Maestra para imprimir (PDF)
├── logo.svg         # Logotipo vectorial (se invierte auto según fondo)
└── README.md        # Documentación
