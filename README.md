# BOT_DISCORD_DETECCION_IMAGEN
Discord AI Image Classification Bot es un bot de Discord desarrollado en Python que utiliza un modelo de Inteligencia Artificial entrenado con TensorFlow/Keras para clasificar imágenes enviadas por los usuarios en tiempo real.

Este proyecto integra un bot de Discord con un modelo de clasificación de imágenes entrenado mediante TensorFlow/Keras.

Cuando un usuario envía una imagen en formato JPG o PNG, el bot:

1. Descarga la imagen del mensaje.
2. La preprocesa (redimensionado y normalización).
3. Ejecuta inferencia usando el modelo entrenado (`keras_model.h5`).
4. Obtiene la clase predicha desde `labels.txt`.
5. Devuelve al usuario el resultado junto con el porcentaje de confianza.

El sistema incluye:
- Validación de formatos de imagen.
- Manejo de errores.
- Control de predicciones con baja confianza.
- Respuestas claras y formateadas.

---

## Tecnologías utilizadas

- Python
- discord.py
- TensorFlow / Keras
- NumPy
- Pillow

---

## Estructura del proyecto
├── bot.py
├── model.py
├── keras_model.h5
├── labels.txt
├── README.md
└── LICENSE


---

## ⚙️ Cómo usar el bot

1. Clonar el repositorio:

git clone https://github.com/TU_USUARIO/TU_REPOSITORIO.git


2. Instalar dependencias:

pip install -r requirements.txt


3. Configurar el token del bot como variable de entorno.

4. Ejecutar:

python bot.py


----------------------------------------------------------------------

##  Ejemplo de uso

Usuario envía una imagen.

El bot responde:


La imagen que mandaste es un/una Perro con una confianza de 99.92%


---

## 📜 Licencia

Este proyecto está bajo la licencia MIT. Consulta el archivo LICENSE para más información.
