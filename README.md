# Automatizacion-Katalon
Este proyecto tiene como objetivo automatizar la interacción con un formulario web utilizando Selenium WebDriver. En este caso, se utiliza una página de demostración disponible en https://katalon-demo-cura.herokuapp.com/.

## Requisitos
Antes de ejecutar el script de automatización, asegúrate de tener instalado lo siguiente:

- Python 3.11.0
- Selenium WebDriver
- Chromedriver (o el controlador adecuado para tu navegador)
- Python Dotenv

Puedes instalar las dependencias necesarias utilizando pip:

Copy code
pip install selenium python-dotenv


Uso
Clona este repositorio en tu máquina local:

git clone https://github.com/tu-usuario/nombre-repositorio.git

Ve al directorio del proyecto:

cd nombre-repositorio

Crea un archivo .env en el directorio raíz del proyecto y configurar las variables de entorno USER_LOGIN y PASSWORD_LOGIN con las credenciales proporcionadas en la página de inicio de sesión de [Katalon](https://katalon-demo-cura.herokuapp.com/profile.php#login)
USER_LOGIN = _usuario obtenido en la página_
PASSWORD_LOGIN = _Contraseña obtenida en página_

## Ejecuta el script de automatización:

python .\Login_Katalon.py

El script abrirá un navegador, iniciará sesión en la página de demostración de [Katalon](https://katalon-demo-cura.herokuapp.com/) y verificará si la redirección después del inicio de sesión es la esperada.


## Notas

+ Asegúrate de que el controlador del navegador esté instalado y configurado correctamente en tu sistema.
+ Es posible que necesites ajustar las esperas (time.sleep()) según la velocidad de carga de la página y la latencia de la red.
