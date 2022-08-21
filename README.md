# DMC-w2-pandas-project

![Shark](https://emtstatic.com/2014/07/tiburon.jpg)

## Introduction

Se ha empezado a trabajar en las herramientas explicadas durante la semana para limpiarla y preparla para ser analizada. Se han centrado los esfuerzos en las columnas que más información analizable contenía intentando categorizarla en el menor número posible de valores diferentes.

La base de datos trata de un registro guardado en un archivo "excel" en el que manualmente se han ido anotando todos los ataques de tiburones desde que hay registros hasta 2018. La base de datos se caracteriza por su falta de rigor a la hora de ordenar varias de las columnas, ya que aunque son explicativos, falta enfocarlos hacia el posible análisis de datos. 


El resultado es una base de datos con 25723 filas iniciales y que se han eliminado 22811, dejando únicamente las que contenían información valiosa para un futuro análisis. Como se puede ver en el gráfico siguiente, muchas de la información estaba vacía (Las parte en amarillo son datos vacíos): 
 
 insertar imagen##comment

 ### Filas

 Las filas donde se han estandarizado el dato para facilitar el análisis son:
 Case_number: Se han numero de más antoguo a más moderno. 
 date: se ha incluido en la lista las filas que contenían día, mes y año. Se ha dejado en formato fecha.
 Year: se ha puesto el mismo año que en la fecha, dejandolo en formato int. 
 type: se ha simplificado en 7 posibilidades
 Country: Se ha comparado cada país de la lista con el nombre oficial de cada pais y se han arregla los que contenían discrepancias. 
 activity: Se ha categorizado las diferentes actividades que se realizaban mientras se ha sufrido un ataque de tiburones y se ha filtrado según este criterio. 
 Name: Se ha simplificado el nombre del atacado a 1 persona.
 Age: En los casos que había una edad específica se ha dejado, en el resto de casos se ha eliminado. 
 Injury: Se ha simplificado las heridas recibidas a una serie de 17 tipos diferentes. En los casos en los que el ataque fue  mortal según la columna "fatal" y no había información según esta categoría, se ha actualizado. 
 Fatal: Se ha eliminado los errores y se ha dejado en SI/NO. 
 Time: En caso de que estuviese la hora y min del ataque, se ha dejado. En caso contrario se ha eliminado de la lista. 
 Species: Se ha filtrado la información contrastandola con una lista de nombres de tiburones no extistos para ver cuantas de estas filas contenían a esos tiburones. 
 Resto de filas: Se han eliminado los datos vacíos dandole consistencia con restecto al tipo de datos que alberga cada columna.  


## Resultado

Se ha generado una archivo denominado "sharks_clean.csv" que está en la carpeta "code" con la base de datos filtrada. 

 ### Archivos generados

 Se han generado 5 carpetas: 
 Code: Contiene el notebook con el código y el resultado
 Images: Imágenes con las gráficas de NaN y otras imágenes
 Presentation: Presentación del trabajo realizado
 raw_data: Data inicial utilizada
 Support_files: Incluye la lista de tiburones. 







