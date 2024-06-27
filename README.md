# Cam-HackBSZ
El Python que utiliza la biblioteca requests para interactuar con la API del sitio web insecam.org y obtener información sobre cámaras de seguridad accesibles públicamente en diferentes países.
![image](https://github.com/AvastrOficial/Cam-HackBSZ/assets/91764815/35da9edf-4f11-44e9-ada6-0139eb55bf47)

### Resumen
El script realiza los siguientes pasos:
<br></br>
Envía una solicitud a insecam.org para obtener una lista de países y la cantidad de cámaras disponibles en cada uno.
<br></br>
Imprime la lista de países junto con un banner ASCII en la terminal.
<br></br>
Solicita al usuario que ingrese el código de un país.
<br></br>
Busca y extrae direcciones IP de cámaras en el país seleccionado.
<br></br>
Guarda las direcciones IP en un archivo de texto.

### Funcionamiento
Importaciones y Configuración Inicial:
<br></br>
Se importan las bibliotecas necesarias (requests, re, colorama, random) y se inicializa colorama para el color en la terminal.
Se define la URL y los encabezados para la solicitud HTTP.
Solicitud de Datos de Países:
<br></br>
Se realiza una solicitud GET a la URL para obtener datos en formato JSON sobre los países.
Se extrae la lista de países y se imprime en la terminal junto con un banner ASCII.
Interacción con el Usuario:
<br></br>
Se solicita al usuario que ingrese el código de un país.
Se realiza una solicitud GET a la página del país seleccionado para obtener el número de páginas disponibles.
Extracción de Direcciones IP:
<br></br>
Para cada página, se realiza una solicitud GET y se buscan direcciones IP en el contenido de la página usando expresiones regulares.
Las direcciones IP encontradas se guardan en un archivo de texto nombrado con el código del país.
Manejo de Excepciones y Finalización:
<br></br>
Se maneja cualquier excepción que pueda ocurrir durante la ejecución.
Se imprime un mensaje final indicando que el archivo se ha guardado y se cierra el programa.

### requerimientos :
pkg install git
<br></br>
git clone https://github.com/AvastrOficial/Cam-HackBSZ
<br></br>
cd Cam-HackBSZ
<br></br>
pip install -r requirements.txt
<br></br>
python cam_hackbsz.py

### Referencias de uso :
https://github.com/AngelSecurityTeam/Cam-Hackers

## Quieres correrlo en una pagina web ?
link : https://replit.com/@StrAva1/Cam-Hack-Bsz

