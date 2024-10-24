markdown
Copy code
# Recomendador de Autores y Libros

## Descripción

Este proyecto es una aplicación de Streamlit que recomienda textos basados en un autor y título ingresados por el usuario. Utiliza técnicas de procesamiento de lenguaje natural y algoritmos de similitud de coseno para generar recomendaciones relevantes.

## Requisitos

Antes de ejecutar la aplicación, asegúrate de tener instaladas las siguientes dependencias. Puedes instalar todas las dependencias necesarias desde el archivo `requirements.txt`.

```bash
pip install -r requirements.txt
Instalación
Crear un entorno virtual
Para crear un entorno virtual en Mac, abre tu terminal y ejecuta:

bash
Copy code
python3 -m venv nombre_del_entorno
source nombre_del_entorno/bin/activate
Para desactivar el entorno en Mac, ejecuta:

bash
Copy code
deactivate
Para crear un entorno virtual en Windows, abre tu terminal y ejecuta:

bash
Copy code
python -m venv nombre_del_entorno
.\nombre_del_entorno\Scripts\Activate
Para desactivar el entorno en Windows, ejecuta:

bash
Copy code
deactivate
Descargar el repositorio
Para descargar los datos de origen de los libros, ejecuta el siguiente comando para clonar el repositorio:

bash
Copy code
git clone --filter=blob:none --no-checkout https://github.com/karen-pal/borges.git
Esto clonará el repositorio sin descargar todos los archivos, solo los necesarios.

Luego, navega a la carpeta clonada:

bash
Copy code
cd borges
Configura sparse-checkout:

bash
Copy code
git sparse-checkout init --cone
Agrega la carpeta específica que deseas clonar:

bash
Copy code
git sparse-checkout set datasets/datasets_pkl
Finalmente, descarga la carpeta:

bash
Copy code
git checkout
Cambiar la ruta de los archivos
Ve a la línea 12 del código app.py y cambia la ruta donde está tu carpeta datasets_pkl.

Ejecución de la aplicación
Para ejecutar la aplicación de Streamlit, utiliza el siguiente comando:

bash
Copy code
streamlit run app.py
Contribuciones
Las contribuciones son bienvenidas. Si tienes sugerencias o mejoras, no dudes en abrir un issue o un pull request.

go
Copy code

Puedes copiar y pegar este bloque en tu archivo `README.md` en tu repositorio de Git