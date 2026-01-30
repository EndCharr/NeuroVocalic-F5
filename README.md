# 🚀 **NeuroVocalic-F5**
### **Sistema de Síntesis de Voz en Español de Nueva Generación**
#### *Desarrollado por [EndCharr](https://github.com/EndCharr) | [Academia EndCharr](https://github.com/EndCharr)*

---

![Futuristic Banner](https://img.shields.io/badge/UI-Futuristic-cyan?style=for-the-badge)
![Optimization](https://img.shields.io/badge/Optimizado-Castellano-blue?style=for-the-badge)
![Colab](https://img.shields.io/badge/Colab-Ready-orange?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

## 🌌 **Acerca de NeuroVocalic-F5**

**NeuroVocalic-F5** es un ecosistema avanzado de síntesis de voz (**Text-to-Speech**) basado en la arquitectura *F5-TTS (Diffusion Transformer with Flow Matching)*. Esta versión ha sido profundamente personalizada y optimizada por **EndCharr** y **Academia EndCharr** para ofrecer una experiencia premium en castellano.

Hemos rediseñado la interfaz visual con una estética **futurista y minimalista**, optimizado las dependencias para evitar errores en entornos como Google Colab y mejorado el procesamiento lingüístico para el español.

---

## ✨ **Características Principales**

- 🇪🇸 **ADN Castellano**: Modelo de alta fidelidad entrenado específicamente para la prosodia y fonética del español.
- 🎨 **Interfaz Futurista**: Nueva interfaz Gradio estilo *Glassmorphism* con acentos de neón y modo oscuro.
- 🎭 **Expresividad Multi-Estilo**: Capacidad para generar emociones (sorpresa, tristeza, susurro, gritos) de forma fluida.
- 💬 **Voz Interactiva**: Chat de voz potenciado por Qwen2.5 para conversaciones naturales.
- ⚙️ **Estabilidad Colab**: Dependencias optimizadas (libres de `torchcodec`) para evitar crasheos y reinicios.
- 🔢 **Procesamiento Inteligente**: Conversión automática de números y símbolos a texto hablado.

---

## 🚀 **Acceso Rápido (Google Colab)**

La forma más eficiente de probar la potencia de **NeuroVocalic-F5** sin configurar nada localmente:

[![Abrir en Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/EndCharr/NeuroVocalic-F5/blob/main/NeuroVocalic-F5.ipynb)

---

## 🛠️ **Instalación Local**

### 1. Preparar el Entorno
Se recomienda usar Python 3.10 y un entorno virtual:

```bash
conda create -n neurovocalic-f5 python=3.10
conda activate neurovocalic-f5

# Instalar PyTorch (ajusta según tu versión de CUDA)
pip install torch==2.3.0+cu118 torchaudio==2.3.0+cu118 --extra-index-url https://download.pytorch.org/whl/cu118
```

### 2. Instalar NeuroVocalic-F5
Puedes instalarlo como un paquete o de forma editable para desarrollo:

#### **Como paquete (Inferencias rápidas)**
```bash
pip install git+https://github.com/EndCharr/NeuroVocalic-F5.git
```

#### **Modo Desarrollador (Entrenamiento y Modificación)**
```bash
git clone https://github.com/EndCharr/NeuroVocalic-F5.git
cd NeuroVocalic-F5
pip install -e .
```

---

## 🖥️ **Uso de la Interfaz Web (Gradio)**

Lanza la aplicación con la nueva interfaz futurista:

```bash
# Iniciar App de Inferencia
f5-tts_infer-gradio

# Para compartir un enlace público
f5-tts_infer-gradio --share
```

---

## 🧠 **Entrenamiento (Finetuning)**

Si deseas entrenar el modelo con tu propia voz, usa la interfaz optimizada:

```bash
f5-tts_finetune-gradio
```
*Consulta la carpeta `src/f5_tts/train` para guías detalladas sobre la preparación del dataset.*

---

## 🤝 **Agradecimientos y Créditos**

- **EndCharr** & **Academia EndCharr**: Rebranding, optimización de dependencias y rediseño de UI futurista.
- [jpgallegoar](https://github.com/jpgallegoar): Por la adaptación original al español y el modelo base.
- [E2-TTS](https://arxiv.org/abs/2406.18009) & [F5-TTS](https://arxiv.org/abs/2410.06885): Investigación original y arquitectura base.
- [Lucidrains](https://github.com/lucidrains): Por la estructura CFM inicial.

---

## 📜 **Licencia**

Este proyecto se distribuye bajo la licencia **MIT**. Los modelos pre-entrenados pueden tener restricciones adicionales basadas en los datasets de origen (CC-BY-NC).

---
<p align="center">
  Hecho con ❤️ por <b>Academia EndCharr</b>
</p>
