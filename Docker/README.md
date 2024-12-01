# Modelo en Docker para Inferencia

Este proyecto contiene un modelo entrenado de Machine Learning 
y un script de inferencia para realizar predicciones con el modelo cargado. 

## Instrucciones para construir la imagen Docker

 - Clonar este repositorio:
	git clone https://github.com/LBreccia/AA1-TUIA-Breccia-Justo.git
	cd AA1-TUIA-Breccia-Justo/docker

 - Construir la imagen Docker:
	docker build -t inferencia .

 - Ejecutar el contenedor Docker:
   Se debe pasar un archivo input.csv como argumento de entrada y 
   se obtiene el archivo output.csv con las predicciones.

	docker run --rm -v $(pwd)/input_data:/app/input_data -v $(pwd)/output:/app/output inferencia
