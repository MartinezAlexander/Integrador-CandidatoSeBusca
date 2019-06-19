# Candidato se busca

## Ejercicio integrador

_**La aplicación que en estos días desean todas las fuerzas políticas para armar su fórmula presidencial.**_

### Planteo del problema
Conocemos cierta información de los dirigentes políticos, tales como su nombre, su imagen positiva, sus habilidades, su cargo actual y el partido politico al que pertenece.

~~~
data Dirigente = UnDirigente { …
dirigentes = [ … ]
~~~
Los partidos politicos arman alianzas electorales con otros partidos, y juntos determinan su cantidato a presidente y vice. 

*Ejemplos de alianzas electorales:*
~~~
cambiemos = ["pro","ucr","cc"]
frenteDeIzquierda = ["po","pcr"]
~~~

Hay diferentes modos de construccion política, por ejemplo:
* El dirigente con mayor cargo actual como presidente (determinar de alguna manera la jerarquía de cargos actuales, por ejemplo, que el cargo de presidente es más que el de gobernador y que el de gobernador es más que el de concejal) y cualquiera que tenga más de 20 puntos de imagen positiva como vice.
* El dirigente de mayor imagen positiva como presidente y cualquier gobernador que entre sus habilidades tenga "honestidad" como vice.
* El dirigente de mayor imagen positiva como vice y el que tiene más habilidades como presidente.

### Consignas
1. Hacer la función que permita, a partir de una alianza electoral, un modo de construcción política y una lista con dirigentes de cualquier partido, obtener cómo queda conformada la fórmula, eligiendo los candidatos entre los dirigentes que pertenzcan a los diferentes partidos que conforman dicha alianza electoral.

2. Definir los modos de construcción politica descriptos e inventar uno nuevo a elección, aprovechando funciones ya definidas.

3. Completar datos de ejemplo y mostrar algunas consulta posibles, donde la misma alianza con diferentes modos de construcción obtiene diferentes fórmulas.

4. Justificar si fue útil el concepto de aplicacíon parcial y composición.

5. Explicar qué sucede si la lista de dirigentes es infinita: Si es posible, encontrar al menos una función de las desarrolladas que permita obtener respuesta y otra que no. Justificar.

*Notas:*
- Puede suceder que una misma persona quede como candidata a presidente y a vice, no se requiere validarlo. 
- Puede suceder que la alianza política no encuentre ningún dirigente para alguno de los lugares de la fórmula y se produzca un error.
- Si hay más de un dirigente que cumple con los requisitos buscados (tener el mejor cargo, ser goberandor honesto, tener mayor imagen positiva, etc.) cualquiera de ellos puede ser el elegido para ocupar su lugar en la fórmula.




