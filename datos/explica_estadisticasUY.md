Columna   | Descripción
----------|---------------------------------------------------
fecha	  |día calendario en que se informaron estos datos
dia	    | día correlativo desde el 13 de marzo, cuando se anunció el primer caso
cantPersonasConInfeccionEnCurso |	cantidad de personas que actualmente cursan la infección
cantCasosNuevos| **cantidad de casos nuevos** <sup>3</sup> identificados ese día 
acumCasos| **cantidad de casos acumulados**<sup>2</sup> hasta el momento 
cantFallecidos |	cantidad de fallecidos reportados ese día
acumFallecidos |acumulado de la cantidad de fallecidos hasta ese día
cantCTI  |	cantidad de pacientes reportados en CTI ese día
cantCI  |	cantidad de pacientes reportados en CI ese día
cantRecuperados	| cantidad de pacientes recuperados reportados ese día
acumRecuperados |acumulado de la cantidad de recuperados hasta ese día
cantTest  |	**cantidad de tests**<sup>1</sup> realizados ese día
acumTest	|acumulado de la cantidad de tests realizados hasta ese día
cantTestPositivos |	cantidad de tests positivos de ese día
acumTestPositivos	  |acumulado de la cantidad de tests positivos hasta ese día





## Fuente

Datos extraídos de los [informes de situación publicados por el MSP](https://www.gub.uy/sistema-nacional-emergencias/comunicacion/noticias/informacion-interes-actualizada-sobre-coronavirus-covid-19-uruguay).
El valor `N/A` se utiliza para indicar valores no disponibles o faltantes en los reportes.

<sup>1</sup> Nótese que siempre se hace referencia a cantidad de tests y no cantidad de personas. Sobre algunas personas se realizan tests más de una vez por lo que la cantidad de infectados es menor o igual a la cantidad de tests positivos.

<sup>2</sup> A partir del 9/4 este valor se obtiene como (cantPersonasConInfeccionEnCurso + acumRecuperados + cantFallecidos). Antes del 8/4, el valor de cantPersonasConInfeccionEnCurso no se conoce y por lo tanto este valor se estima. Esta estimación se hace distribuyendo la diferencia entre número de test positivos y número de personas positivas al 9/4 (22, o sea 22 tests dobles) en los 11 días anteriores, a 2 extra por día.

<sup>3</sup> La cantidad de casos nuevos se computa como cantPersonasConInfeccionEnCurso(hoy)-cantPersonasConInfeccionEnCurso(ayer)+cantRecuperados(hoy)+cantFallecidos(hoy)
