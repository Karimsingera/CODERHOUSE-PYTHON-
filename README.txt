Nombre del Proyecto:

Revisão histórica de dados meteorológicos de 3 cidades do Brasil. 
Uruçuca, Rio de Janeiro, Brasília (1950-2023)


Descripción:

Neste projeto trabalhamos com o banco de dados de 'Open-Meteo', uma API
gratuita para consultas de diversos dados meteorológicos.

Instalación:

Certifique-se de ter o Python 3 instalado. Você pode baixá-lo em https//:www.python.org/).

2. Crie e ative seu ambiente virtual.

Como Configurar Seu Ambiente Virtual

Antes de começar a codificar, você precisará garantir que tenha todas as
ferramentas e bibliotecas necessárias instaladas. Para garantir que você tenha
um ambiente limpo e isolado, você criará um ambiente virtual usando o venv.
Crie um diretório de projeto e navegue até ele no terminal:

	mkdir weather-forecast
	cd weather-forecast

Crea un entorno virtual llamado env con el siguiente comando:

	python -m venv env

Python ahora incluye la biblioteca venv preinstalada para crear entornos
virtuales.



Activa el entorno virtual de la siguiente manera:

	source env/bin/activate

Deberías ver (env) en tu indicador de terminal, lo que indica que el entorno
virtual ha sido activado.

3. Instale as bibliotecas necessárias executando o seguinte comando:

   pip install -r requirements.txt


Uso:

Una vez descargadas e instalas todas las bibliotecas necesarias, podemos
proceder a consultar la API de “Open Meteo” (https://open-meteo.com/)

En esta ocasión, solicitamos información histórica del clima para 3 ciudades de
Brasil (Rio de Janeiro, Brasilia, Uruçuca), entre los años 1950-2023.

La información solicitada es:

Temperaturas máximas y mínimas (a 2 metros de distancia del suelo).
Sensación térmica máxima y mínima.
Suma total de precipitaciones.

Cuando la información está descargada. Procedemos a revisar si está correcta,
comprobando presencia de datos nulos y/o duplicados, en caso de existir, los
eliminamos para dejar las base de datos listas para posteriores consultas.

Los datos son almacenados en archivos .csv con el respectivo nombre de. La ciudad:

rio_de_janeiro.csv
brasilia.csv
uruçuca.csv 

Las 3 tablas son posteriormente agrupadas en una base de datos relacional (SQL) para consultas, bajo el nombre de:

historico_clima.db

Para comprobar que la base de datos está correctamente cargada se realizan consultas como el promedio de lluvia anual en cada ciudad y luego se presentan en una visualización de datos a través de un gráfico que muestra los promedios de las 3 ciudades desde el año 1950 al 2023.






Créditos:

Para crear este código usé material de Coderhouse, Open-Meteo y chatGPT.


Licencia:

Este trabajo fue realizado como proyecto final en una formació de python en la
Plataforma Coderhouse.

El código puede ser usado libremente para fines de estudio y aprendizaje. No
requiere consultar al autor.

Contacto:

Karim Singer.
karim.singer@gmail.com


