# Estimacion
No estimamos las tareas
Partimos simepre de los requerimeintos del proyecto 

#### Variables de estimacion 
- Tamaño
- Tiempo
- Costo
- Recursos

#### Preguntas que nos hacemos al estimar:
1. **Cual va a ser el tamaño del proyecto** es lo unico que se estima, las demas preguntas salen por conclucion de haber estimado el tamaño del proyecto. *(complejidad)*
2. Cuanto esfuerzo vamos a necesitar
3. Cual va a ser el costo final del proyecto
4. Cual va a ser la furacion final de proyecto en horas.
Cuanto tiempo vamos a tardar?
Cuantos hs/persona vamos a necesitar?
Cuanto va a costar ?

#### Porque fallan las estimaciones:
- Optimismo
- Estimaciones Informales *(a ojo)*
- No hay historia
- Mala definicion de alcance
- Falta de experiencia
- ...

*La estimacion puede ser buena pero la unica forma de ver si la estimacion fue correcta es al final del proyecto*

#### Nivel de incertidumbre
La certesa la tenemos al finalizar el proyecto, ya que ahi es donde podemos ver los resultados de nuestra estimacion.

**Cono de la insertidumbre**: Se deve forzar a que el cono se vaya achicando, forzando la certidumbre para ir descartando variables para llegar a una estimacion muy proxima al resultado real del proyecto. 
![[Pasted image 20220502201517.png]]


*Cuanto mas refinada la definicion y el objetivo, mas exacta sera la estimacion*



#### Tips Para estimar:
Hay constraints, osea restricciones que tenemos que tener en cuenta a la hora de estimar

- Recordar que hay cosas que se van deribando de otras, como el costo que se deriva de el esfuerzo, o el tiempo
- Asociar a las estimaciones un % de confiabilidad a la estimacion
- Diferenciar entre estimaciones objetos y compromisos
- Siempre presentar juento con la estimacion, los supuestos que se tuvieron en cuenta para llegar a la misma.
- 

#### Ciclo de estimacion 
- Estimar: *estimar el tamaño para deriovar el esfuerzo y el costo*
- Medir: *mientras va evolucionando el proyecto seguir mirando como evolucionan los valores estimados*
- Registrar: *Dejar clara las mediciones tomadas*
- Analizar: *supuestos que quizas variaron*
- Calibrar: *Ajustar parametros que intervienen en el proceso de estimacion*
- Volver a estimar: *El mismo proyecto pero ahora con mas informacion que al comienzo del mismo*

### Metodos de estimacion
- **Metodos rudimentarios** (horas) (estomago)
	- Jucio experto: Donde alguien estima por el tamaño o el sefuerzo del proyecto, donde no necesitamos mucha info para poder realizarla y nos sale muy varata de realizar.
	- Clarck: Donde hay mas de una persona y estimas con un juicio experto el esfuerzo requerido, y luego se pondera el resultado de estas personas 
	- Wideband Delphi:  
	- Planning Poker: generan una estimacion de forma independiente y se consensua segun todas las estimaciones cual fue la mas acertada, pero se hacen estiomaciones de forma indibidual, ademas de ir estimando requerimiento segun tiempo y hora que puede tardar alguien.
	
- **Metodos Parametricos** (tamaño)
	- Function Points: Evalua la funcionslidad del sistema, en donde aplica una serie de reglas, obtiene una unidad de tamanio que se llama function points. *(generalmente son 5 parametros y es complejo detectarlos y realizar los calculos por eso se recomienda realizarlo si hay expertos)*
	- Use Case Points: Vasado en Function Points, el objetivo era desarrollar un metodo mas sencilo, en donde la idea es la idea es poder contabilizar el numero de trasnacciones de cada caso de uos -> **transaccion** es un evento que ocurre entre un actor y un sistema.  
	- Story Points: Lo quie mide es la dificultad o el tamaño de una user story donde vos capturas el tamaño y determian el tamaño (nos enfocamos mas en el requerimiento )
	- Objects Points: El primer paso es entender como el sistema esta construido y con ese analisis lo descompongo en objetos

	Como deribar el tamaño a tiempo necesario de esfuerzo -> generalmente tienen un historial o trabajos ya realizados antes en donde se almaceno informacion estadistica de la duracion de otros proyectos, entonces esto lo usan para unir lo que realmente paso y la unidad de medida utiliada calculoamos en horas de esfuerzo necesarias