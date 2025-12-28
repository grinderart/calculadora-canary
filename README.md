# 💨 Canary Vape Shop - Calculadora de Mezclas & Herramientas

![Status](https://img.shields.io/badge/estado-producción-green)
![Tech](https://img.shields.io/badge/stack-HTML5%20|%20CSS3%20|%20JS-blue)
![Version](https://img.shields.io/badge/version-1.2.0-orange)

Aplicación Web Progresiva (PWA) de uso interno diseñada para **estandarizar la alquimia y optimizar la venta** en el mostrador. Herramienta "Todo en Uno" para el cálculo de e-liquids, consulta de resistencias y generación de guías físicas.

## 🚀 Funcionalidades Clave

### 🧠 1. Algoritmo Inteligente de Hardware
El sistema elimina el error humano calculando la mezcla ideal basándose en el dispositivo del cliente:
* **PODS (0.8Ω - 1.2Ω):** Prioriza Sales de Nicotina y ratios 50/50.
* **AIO / RDL (0.6Ω - 0.4Ω):** Balancea entre Sales y Base Libre automáticamente.
* **Sub-Ohm (0.3Ω - 0.2Ω):** Fuerza Base Libre y Max VG (70/30).

### 🧪 2. Química de Precisión
Calcula el equilibrio exacto de **Sales VG vs Sales PG**.
* *Ejemplo:* Si la receta requiere 2 nicokits para un Pod, la app puede sugerir **1 VG + 1 PG** para mantener la densidad correcta y evitar fugas.

### 💰 3. Lógica de Venta (Upselling)
El motor de cálculo aplica un **redondeo estratégico al alza** en los nicokits.
* *Objetivo:* Evitar botes abiertos en stock y maximizar el ticket medio vendiendo unidades completas.

### ⚡ 4. Centro de Recursos
* **Calculadora:** Núcleo principal de mezclas.
* **Guía de Resistencias (`coils.html`):** Catálogo interactivo visual para explicar al cliente los tipos de calada (MTL, RDL, DTL) y potencias recomendadas.
* **Cheat Sheet PDF (`imprimir.html`):** Generador de tablas de referencia optimizadas para impresión (Ink-saver) para uso físico en tienda.

---

## 📂 Estructura del Proyecto

```text
/
├── index.html       # 🏠 Calculadora Principal (SPA)
├── coils.html       # ⚡ Guía Interactiva de Resistencias y Potencias
├── imprimir.html    # 🖨️ Hoja Maestra para imprimir (PDF)
├── logo.svg         # 🎨 Logotipo vectorial (Adaptable)
└── README.md        # 📄 Documentación
