# Dockerfile
# Utiliza una imagen base de Python
FROM python:3.8-slim

# Establece el directorio de trabajo
WORKDIR /app

# Copia los archivos locales al contenedor
COPY app.py .
COPY requirements.txt .
COPY templates templates

# Instala las dependencias
RUN pip install -r requirements.txt

# Expone el puerto en el que se usa la aplicación Flask
EXPOSE 5000

# Ejecuta la aplicación al iniciar el contenedor
CMD ["python", "app.py", "--host", "0.0.0.0"]
