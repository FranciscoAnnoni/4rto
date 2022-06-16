# TESTING
### Definicion de calidad - rapida*
Aquel que *cumpla con los requisitos* y que *no presente fallas*

###### Aseguramiento de calidad y Control de la calidad
**Aseguramiento de la Calidad**
Cumplimientos de los requisitos del proceso.
Todas las acciones que yo hago para asegurar y darle validez a lo que estamos construyendo y que eso que constriuimos cumpla con los requermientos establecidos.(y si no se encuentra un requerimiento avisara que falta x cosa)

**Control de la Calidad**
 Es sobre algo que ya esta hecho, chequeamos que eso que esta hechi cumpla con lo que esperaba que se hiciera.
Lo que yo esperaba que se haga el producto y lo que verdaderamente se hizo.
Apunta directamente a un componente hecho.

--
Una vez definidos los requermientos de calidad tengo que tener en cuenta:
 * La calidad no puede inyectarse al final.
 * la calidad del producto depende de las tareas realizadas durante el proceso.
 * Detectar errores de forma temprana ahorra esfuerzos, tuiempo y recursos.
 

### Que persigue testing
>**Encontrar fallas en el producto. (cumple su objetivo cuando las encuentra)**

Hacerlo lo mas **Eficiente** posible:  
**- Rapido y varato** 

Haciendo lo mas **Eficazmente** posible:
    - Encontrar la mayor cantidad de fallas
	- No detectar fayas que no son *(gastas recursos probando algo que al final no se probava asi)*
	**- encontrar las mas importantes**

*si no se encuentran errores, vasicamente fallo el testing y habria que cambiar al equipo*

### Prueba de SW
Actividad en donde un componente o sistema es ejecutado bajo condiciones determinadas, y sus resultados son analizados para poder hacer una evaluacion de dicho sistema o componente. (recordar que a distintas condiciones iniciales distintos resultados)

> Una prueba es exitosa si encuentra fallas


No podemos probar si no hay reglas de negocios, con lo cual la documentacion es necesaria, para poder tener las reglas de negocios para realizar las pruebas, sabiendo que es lo que hay que probar y como probarlo, y cuales son los resultados esperados. (No tiene sentido probar lo que ya esta en el codigo un if, un for van a andar igual)

>Las pruebas siempre se realizan contra un resultado esperado

**Falla:**
Resultado de ejecucion incorrecto. 
Diferencia entre el resultado esperado y el obtenido

**Defecto**
Es el originador de la falla, es lo que causo la falla.

**Equivoacion**
	Accion humana que produce un resultado incorrecto.
	Accion humana que origino el defecto.
	
##### Conceptos Relacionados
- Una equivolcacion lleva a uno o mas defectos que estan presentes en el codigo
- Un defecto puede ocacionar cero, una o varias fallas (ya que tranquilamente puede haber defectos que todavia no hayan fallado, pero que a futuro lo hagan)
- La falla es la manifestacion del defecto
- Una falla tiene que ver con uno o mas defectos	

	
#### INCIDENTE
**Toda ocurrencia de un evento que sucede durante la ejecucion de una prueba de software que requiere investigacion**

Recordar que ante cada incidente devemos recorrer: *** - Falla - Defecto - Equivocacion ***
Ya que con esto podemos allar la solucion principal del problema y evitar futuras fallas ocultas.

**Recordar:** no toda incidencia es una falla 
*Siempre que hacemos tesnting encontramos incidentes, los cuales pueden ser:*
>1- Una falla
>2- Pueden ser falsos positivos (que teine una error pero en realidad no lo tiene)

(uno reporta incidentes, donde son evaluados y se determina si todos los incidentes reportados son fallas o son falsos positivos)

#### Codiciones  y casos de Prueba
**Condiciones de Prueba**
Son incidentes de situaciones que queiren probarse para saber cual es la respuesta del sistema *(crear condiciones, proceso creativo)*
> El exito esta en construir buenas condiciones de prueba

**Casos de Prueba**
Son las acciones necesarias para que se de una determinada condicion de prueba *(Proceso laboreoso)*
	
	
*Criterio de Seleccion*
Es una condicion para seleccionar un conjunto de casos de prueba
	- La idea es tener la mayor cantidad de condiciones de prueba para asi poder probarlas en la mayor cantidad de casos posibles. 
*Si elegimos pocas o malas condiciones, mas al pedo van a estar los casos de prueba*




## Prueba de Caja Negra  
A una determinada entrada, vemos la salida que genera y comparamos con el resultado esperado  
- Criterio de acpetacion: Escenario que quiero probar  
- Casos de Prueba: datos que voy a usar para evaluar el escenario  
- Tecnicas: Con las tecnicas elegimos los casos de prueba (modelos, etc)  
  
## Prueba de Caja Blanca  
Analizamos el codigo y los procesos internos que se hacen para obtener ante una entrada determinada salida.  
  
###### Tipos de coberturas  
**Cobertura de Sentencia:**  
    - Vamos a buscar coberturas de prueba y datos que nos ayuden a pasar por la mayor cantidad de codigo posible. (> % de cogio usado)  
  
**Cobertura de Desicion:**  
    - Que cubra todas las salidas (en un if, seria el verdadero o falso)  
  
**Cobertura de Condicion:**  
    - Busca evaluar todas las condiciones (en un if, serian todos los valores posibles de las comparaciones, *if(A>B|| B<C||C<D))*  
  
## Prueba de camino basico  
**Complejidad Ciclomatica**(METRICA)  
Cantidad de caminos independientes que tiene nuestro sistema  
  
Se trata de dividir nuestro sistema armando un grafo, donde hay un inicio y un fin, y se calcula desde el inicio hasta el fin cuantos camios independientes tubo que pasar. (no se si el dato o ke ) #TODO

## Tipos de Pruebas
#### Funcionales
1. Prueba de Sistema: valida que cumpla con los requisitos funcionales
2. Prueba de aceptacion de Usuario: Se ejecuta en el ambiente del ususario
3. Prueba de Homologacion: Cumpla con las caracteristicas para el entorno en el que fue concebido

#### NO Funcionales
1) Volumen: Validar los requerimientos, que cumpla para lo que fue diseñado
2) Stress: Se exede el volumen inicial
3) Resistencia: Se exede el sistema hasta que falle y se evalua como reacciona ante eso
4) Seguridad
5) Usdabilidad
6) ..... ISO 2500

## Otros Tipos de Pruebas
#### Regresion
####
####
####