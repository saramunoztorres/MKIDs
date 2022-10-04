A continuación se detalla el contenido de este repositorio, referido al trabajo realizado durante la Beca de Verano en Desarrollo Tecnológico 2022, en el Departamento de Electrónica del IAC.

## Breve descripción 📖

El proyecto llevado ha cabo a consistido en:

- Estudiar el comportamiento del criostato HPD Rainier 103, en cuanto a tiempos y estabilidad.
- Caracterizar unos detectores de microondas basados en inductancia cinética, los MKIDs.

Para más detalle mirar los respectivos informes.

## Requisitos para ejecutar los códigos ⚙️

Los paquetes de terceros de Python que deben tener instalados para la ejecución de los códigos son:

- [numpy](https://numpy.org/)
- [matplotlib](https://matplotlib.org/)
- [pandas](https://pandas.pydata.org/)
- [scipy](https://scipy.org/)
- [seaborn](https://seaborn.pydata.org/)
- [imageio](https://pypi.org/project/imageio/)


## Estructura del repositorio 📋  

Se va a detallar brevemente el contenido de cada archivo de código por orden de pruebas, teniendo en cuenta que en total han sido cuatro: 

1. Prueba inicial del criostato (anterior a la beca)
2. Prueba del criostato con el montaje interno de fábrica
3. Prueba del criostato con el montaje de los MKIDs
4. Prueba de caracterización de los MKIDs.

Además, en la carpeta `\Datos\` se tienen todos los archivos necesarios para la ejecución de los códigos, que igualmente se va a especificar a qué código pertenece cada uno.

#### Prueba del criostato con el montaje interno predeterminado

1. `Test_Cryo_1file&graph` -  `\Datos\PruebaCryo-1\` y `\Datos\Test_1_Cryo.csv`
2. `Test_Cryo_1_stability.ipynb` - `\Datos\Test_1_Cryo.csv`

El primer archivo contiene el código para armar el csv y graficar las distintas magnitudes de estudio del criostato. 
El segundo archivo calculas las estabilidades de las distintas etapas en cada control.

#### Pruebas del criostato con el montaje de los MKIDs

1. `Test_Cryo+MKIDs_graph.ipynb` - `\Datos\PruebaCryo-MKID-1\s21051_SAT_MGB_2022_08_16_10;01.csv`

Se muestran las gráficas de las magnitudes del criostato de la primera prueba con los MKIDs en el interior del criostato.

#### Pruebas de caracterización de los MKIDs

1. `MKIDs_csvFiles_convert&graph.ipynb` - `\Datos\MKID\`
2. `Test_MKIDs_1.ipynb` - `\Datos\MKID\`

El primer código adecúa los archivos csv descargados del VNA para su correcta lectura.
El segundo archivo contiene todo el análisis de caracterización realizado sobre los MKIDs.

#### Prueba inicial y comparativas entre pruebas

1. `Test_Cryo_Initial.ipynb` - `\Datos\Test_Initial_Cryo.csv`
2. `Test_Cryo&Cryo+MKIDs_compare.ipynb` - `\Datos\PruebaCryo-MKID-1\s21051_SAT_MGB_2022_08_16_10;01.csv` y `\Datos\Test_1_Cryo.csv`
3. `Comparation_Tests_0&2.ipynb` - `\Datos\PruebaCryo-MKID-1\s21051_SAT_MGB_2022_08_16_10;01.csv` y `\Datos\Test_Initial_Cryo.csv`

El primer código arregla el archivo de la prueba del criostato realizada anteriormente a mi estancia, y determina estabilidades del mismo.
El segundo compara la prueba realizada del criostato sin y con el montaje interno de los MKIDs.
El tercero compara la prueba inicial y la prueba con el montaje interno de los MKIDs.

Por último, el archivo `Graficas presentación.ipynb`contiene los códigos para la creación de las gráficas empleadas en la presentación final.
