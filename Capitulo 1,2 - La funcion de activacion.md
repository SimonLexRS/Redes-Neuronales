Esta función es la que le da una salida a la neurona, sale por un axon hacia otra neurona, o es una salida de una neurona intermedia.

![[Captura de pantalla 2025-07-24 a la(s) 11.32.30 a. m..png]]
Cada capa tiene una funcion de activacion distinta.

![[Captura de pantalla 2025-07-24 a la(s) 11.36.16 a. m..png]]
En este ejemplo tenemos 3 variables, primero le damos las respuestas como entrenamiento, dependiendo de la edad, horas de estudio y horas de diversion el estudiante aprobara el examen.

Como la IA ya sabe como calcular con los registros (la tabla de arriba).

La respuesta de salida sera 1=Si y 0=No

En nuestro modelo tendremos 3 entradas y pesos
![[Captura de pantalla 2025-07-24 a la(s) 11.40.01 a. m..png]]
![[Captura de pantalla 2025-07-24 a la(s) 11.40.30 a. m..png]]

Si los pesos son mas altos la variables es mas relevante para el modelo.

LA funcion teta es la funcion de exitacion:
![[Captura de pantalla 2025-07-24 a la(s) 11.41.32 a. m..png]]

Para poder predecir reemplazamos las variables como a continuacion:

![[Captura de pantalla 2025-07-24 a la(s) 11.42.30 a. m..png]]

![[Captura de pantalla 2025-07-24 a la(s) 11.43.02 a. m..png]]
$$
n= 24*0,15+12*0,75+6*(-0,26)
$$
$$
n=3,6+9-1,56
$$
$$
n= 11,04
$$

La funcion de activacion procesa el numero que recibe con una formula matematica y decide si se activa o no (es decir, si pasa el valor a la siguiente capa de la red o no).

Piensa como un robot que evalua entre si debe disparar un rayo laser o quedarse quieto.

# Las funciones mas comunes 
1. [[ReLU]] **(Rectified Linear Unit)**
	Formula:
		$$
			f(x)= max(0,x)
		$$
		Si el numero es negativo, lo convierte en 0. Si es positivo, lo deja como esta.
		Es rapida y funciona muy bien en muchas redes.
		**Ejemplo**: si entra -3, sale 0, si entra 5, sale 5.
	
2. [[Sigmoid]]
		Formula:
			$$
			f(x) = 1 / (1 + e^{-x})
			$$
		Esta funcion aplasta cualquier numero para que este entre 0 y 1.
		Se usa cuando se quiere saber si algo es "si o no" (por ejemplo: Hay un gato o no?)
		**Ejemplo**: Si entra 0, sale 0.5; si entra un numero muy grande, se acerca a 1.

3. [[Tanh]] (Tangente Hiperbólica)
	Formula:
		$$
		f(x)=(e^x-e^{-x})/(e^x+e^{-x})
		$$
	Esta funcion convierte el numero en algo entre -1 y 1.
	Mas centrada que la Sigmoid, util en muchas redes.
	Ejemplo: si entra 0, sale 0, si entra 3, sale 0,995
