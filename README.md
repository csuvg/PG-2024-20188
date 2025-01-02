# Gestión de Residuos y Reducción de Huella de Carbono con Inteligencia Artificial

Este proyecto tiene como objetivo optimizar la gestión de residuos en la Ciudad de Guatemala mediante el uso de inteligencia artificial. Integra dos componentes principales:

1. **Modelo de clasificación de residuos:** Utiliza redes neuronales convolucionales (CNN) basadas en la arquitectura Xception para clasificar residuos en seis categorías. Este modelo fue desarrollado en Google Colab usando el notebook `WasteNet_Xception_Final.ipynb`, ubicado en la carpeta `/src/`.
2. **Chatbot inteligente:** Implementado con FastAPI y la API de OpenAI, este sistema asiste a los usuarios en temas de reciclaje conforme a normativas locales.

---

## Instrucciones de Instalación

### Requisitos previos
- Python 3.8 o superior
- TensorFlow (para el modelo de clasificación)
- FastAPI y OpenAI API (para el chatbot inteligente)

### Instalación del modelo de clasificación de residuos

1. Acceder al notebook en Google Colab:
   - El archivo `WasteNet_Xception_Final.ipynb` está disponible en la carpeta `/src/` del repositorio.
   - Subir el archivo a Google Colab.
2. Instalar las dependencias necesarias en el entorno de Colab:
   ```python
   !pip install tensorflow
   ```
3. Ejecutar cada celda del notebook para entrenar o utilizar el modelo de clasificación.

### Instalación del chatbot inteligente

1. Clonar el repositorio:
   ```bash
   git https://github.com/unclepete-20/chatbot-test.git
   cd chatbot-test
   ```
2. Crear un entorno virtual y activarlo:
   ```bash
   python -m venv env
   source env/bin/activate # En Windows: env\Scripts\activate
   ```
3. Instalar dependencias:
   ```bash
   pip install -r requirements.txt
   ```
4. Configurar la variable de entorno para la API de OpenAI:
   ```bash
   export OPENAI_API_KEY="<tu-api-key-aqui>" # En Windows: set OPENAI_API_KEY=<tu-api-key-aqui>
   ```
5. Ejecutar el servidor:
   ```bash
   uvicorn chatbot:app --host 0.0.0.0 --port 8000
   ```

---

## Demo
Incluye un video en la carpeta `/demo/` que muestra el modelo y el chatbot en funcionamiento.

---

## Informe Final
El informe completo del proyecto se encuentra en la carpeta `/docs/` bajo el nombre `informe_final.pdf`.
