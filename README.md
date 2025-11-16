📁 Organizador Automático de Archivos por Extensión

Este proyecto es una herramienta en Python que automatiza la organización de archivos dentro de una carpeta.
El programa analiza una ruta proporcionada por el usuario y clasifica los archivos según su extensión, creando subcarpetas para cada tipo (pdf, txt, py, etc.) y moviendo los archivos a su carpeta correspondiente.

Además, recorre todas las subcarpetas de forma recursiva para organizar todo el contenido del árbol de directorios.


🚀 Características

Clasifica archivos según su extensión.

Crea automáticamente carpetas para cada tipo de archivo.

Evita reprocesar las carpetas de extensión generadas por el propio programa.

Recorre todas las subcarpetas (recursivo).

Automatiza una tarea común de organización de archivos.

Funciona en Windows, Linux y macOS.



🛠️ Tecnologías utilizadas

Python 3

os — manejo de rutas y sistema de archivos

shutil — mover archivos

Recursividad — para recorrer subdirectorios

📦 Instalación

Clona el repositorio o descarga el archivo:

git clone https://github.com/tuusuario/organizador-carpetas.git


Entra en la carpeta del proyecto:

cd organizador-carpetas


Asegúrate de tener Python instalado:

python --version



▶️ Uso

Ejecuta el programa desde la terminal:

python organizador.py


Cuando lo pida, introduce la ruta que deseas organizar:

Introduzca la ruta que desea organizar:


Ejemplo:

C:\Users\MiUsuario\Documentos


o en Linux:

/home/miusuario/Descargas


El programa:

Listará todos los archivos

Creará carpetas por extensión

Moverá cada archivo a su carpeta

Repetirá el proceso en cada subcarpeta



📂 Ejemplo de organización

Entrada:

/Documentos
    foto.png
    trabajo.pdf
    /Subcarpeta
        script.py
        notas.txt


Salida:

/Documentos
    /pdf
        trabajo.pdf
    /png
        foto.png
    /Subcarpeta
        /py
            script.py
        /txt
            notas.txt



🧩 Estructura del código

listar_contenido() → Obtiene todos los elementos de una carpeta

es_carpeta_o_archivo() → Separa archivos de carpetas

clasificar_archivo() → Mueve los archivos según extensión

crear_carpeta() → Crea una carpeta nueva si no existe

procesar_carpeta() → Función recursiva que organiza todo el árbol

main() → Entrada del programa



🔒 Posibles mejoras futuras

Añadir interfaz gráfica (GUI) con Tkinter o Qt

Añadir opción para deshacer cambios

Integrarlo como servicio automático del sistema
