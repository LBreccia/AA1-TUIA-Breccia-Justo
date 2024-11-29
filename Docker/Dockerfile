# Usa una imagen base de Python
FROM python:3.12-slim

# Configurar el directorio de trabajo
WORKDIR /app

# Copiar los archivos necesarios
COPY inferencia.py 
COPY requirements.txt 
COPY model/ ./model/

# Instalar dependencias
RUN pip install --no-cache-dir -r requirements.txt

# Especificar el comando por defecto
CMD ["python", "./inferencia.py"]


