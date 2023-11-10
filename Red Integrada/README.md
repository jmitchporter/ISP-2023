Acá se encuentra la programmación de la integración inicial de la red trófica de Marina, et al, (en revisión)
y la provisión de servicios ecosistémicos anotado en la sección anterior. Todos los archivos necesarios para
ejecutar el código incluido acá también se puede encontrar en el archivo.

Algunas calculaciones se hacen con la información de la red original y de los SEs, pero sin integrarlos en una
sola red. Estas inlcuyen algunos diagramas de caja que caracterizan las especies que proveen cada SE según su
nivel trófico y su nivel de conectividad dentro de la red. El archivo "ESProvidersList.csv" se usa para estos 
gráficos ya que se restringe a solo los proveedores SE.

Los archivos "ESInteractionList_Burdwood.csv" y "ESBurdwoodSpeciesList.csv" se usan para la creación de las redes
tróficas integradas. Todos los gráficos se hacen por alteraciones de la función "plot_trophic_level" en el paquete 
"multiweb". Hay uno que mapea todos los servicios implicado en la red y seis más que destacan un SE en particular. 



Notas para uso de datos:

Representaciones númericos para cada SE se usan:
1. Pesca
2. Materia prima
3. Biodiversidad
4. Biopurificación
5. Ciclo de carbono
6. Identidad y geopolítica
7. Educación y investigación

A partir de estas representaciones, para las funciones de igraph cada especie con una combinación única de asociaciones 
con una combinación de SEs (i.e., con SE 1, SE 5, SE 6, etc.) ha recibido un código único para denotar esta combinación 
bajo la columna "vertextype". Estos códigos se usan para que cada proveedor de un SE pueda recibir el color correcto sin 
que se tengan que replicar los nodos cuando una especie tenga más de una conexión.
