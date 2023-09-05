# MejoraExtraccionDatosWeb
Extracción de datos desde la pagina web de earthquare.usgs.gov de varios años por mes del año 1970 a 2023, mes por mes, se mejora el tiempo de extracción

luego de cuantificar los tiempos con la codificación original, se realiza un proceso de mejora en eficiencia del código, con los siguientes cambios:
Se utiliza list comprehensions: En lugar de utilizar bucles for para iterar sobre años y meses, se puede utilizar list comprehensions para generar las fechas de inicio y fin de forma más eficiente.

Se Usa un solo bucle para las solicitudes HTTP: En lugar de realizar solicitudes HTTP por mes, se puede realizar una sola solicitud HTTP para cada año y luego filtrar los resultados en función de los meses. Esto reducirá la sobrecarga de las solicitudes HTTP.

Usamos Parallelización: podemos utilizar la biblioteca concurrent.futures para realizar solicitudes HTTP en paralelo, lo que acelerará la descarga de datos.

Se procede a ejecutar y el resultado da de 2m 1.9s
