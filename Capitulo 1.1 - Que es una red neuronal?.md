[[Curso de Redes Neuronales]] #machine-learning #tensorflow
# Que es una neurona artificial?
Esquema biologico:
![[Captura de pantalla 2025-07-23 a la(s) 7.56.38 a. m..png]]

Una red neuronal es un modelo de computo inspirado en el cerebro humano, esto permite a las maquinas aprender desde los datos que se le proporcione. Se compone por capas, cuando la red neuronal recibe las señales este pasa capa por capa, cada capa lo procesa y decide si **disparar** (sinapsis) a la siguiente capa de acuerdo al **peso** (que se mide en importancia). Esto permite a la red neuronal reconocer patrones complejos como imágenes, voces, o incluso tomar desiciones.

![[Captura de pantalla 2025-07-23 a la(s) 1.02.15 a. m..png]]

**Capas**: Las neuronas (nodos)
**Las dentritas**: Son los inputs de información a la neurona
**Axon**: Es el canal que conecta a otras neouronas u otras dentritas de otras neuronas. Se lo representa como Función de activación.
**Sinapsis**: Activación dentro de la neurona. Es la conexion entre dos neuronas donde se transmite la informacion mediante impulsos electricos. Se representa como el peso (o "weight") de la conexion entre dos neuronas artificiales (nodos) en una red neuronal.

# Salida de una neurona (axon output value)
Las salidas pueden ser:
* Valor continuo (precio)
* Valor binario (si o no)
* Categorica (Talla, color, etc)

# Que es una sinapsis en IA?
En una red neuronal:
1. Cada **sinapsis** (peso) multiplica la señal  de entrada
2. Esa señal  luego pasa por una funcion de activación 
3. Durante el entrenamiento (ej. Backpropagation), el sistema ajusta esos pesos, es decir, modifica las sinapsis para que la salida sea mas precisa.

# Arquitectura basica de una red neuronal
Se basa en 3 capas.
1. Input layer
2. Hidden layer
3. Output layer

Por ejemplo podemos usar como esquema, si una mezcla de agua es potable para el consumo humano, podemos usar caracteristicas diferentes para el analisis que ingresaran a la red neuronal. Estos valores se analizan para determinar si es potable, estos se convierten en variables N.
![[Captura de pantalla 2025-07-23 a la(s) 10.02.18 a. m..png]]

![[Captura de pantalla 2025-07-23 a la(s) 10.04.43 a. m..png]]

Podemos tener N capas ocultas con una capa de salida.