





*ACT 3.1:*
Problemas de búsqueda:
Se encarga de buscar una secuencia de acciones o un camino desde un estado inicial hasta un estado objetivo dentro de un espacio de estados
Espacios de estados:
Representación matemática de un sistema dinámico o un modelo de resolución de problemas mediante un conjunto de variables 
Estado inicial:
Punto de partida o la configuración desde la cual el algoritmo comienza a explorar el espacio de problemas
Acciones:
Los movimientos, operaciones o decisiones que un agente puede realizar para pasar de un estado actual a uno nuevo
Modelo de transición: 
Regla matemática o función que describe cómo se pasa de un estado a otro cuando se ejecuta una acción específica
Prueba de meta:
Verifica si un estado actual o nodo alcanzado cumple con el objetivo
Costo del camino:
Suma numérica de los pesos o valores asociados a cada paso que recorre un nodo desde el origen hasta el objetivo
Solución:
Es la secuencia de pasos, el camino  el elemento especifico que cumple con los criterios o el objetivo
Frontera:
Es el conjunto de nodos o vértices que ya han sido generados pero que no han sido explorados o expandidos
Nodo: 
Unidad básica de información que representa un punto, estado o elemento dentro de la estructura
Agente de resolución de problemas: 
Es un tipo de agente inteligente que planea y decide que hacer mediante la exploración sistemática de una secuencia de acciones para alcanzar un objetivo específico
Sistemas de búsqueda (ciega):
Son llamados métodos ciegos, porque usan estrategias de búsqueda que solo consideran la relación de precedencia entre estados
Búsqueda no informada (ciega):
Explora espacios de estados sin utilizar ninguna pista, conocimiento adicional sobre que tan cerca está el objetivo
Búsqueda en amplitud: 
Sirve para recorrer o buscar elementos en un grafo o un árbol
Búsqueda en profundidad:
Algoritmo de recorrido de grafos y árboles que explora cada rama al máximo antes de retroceder
Búsqueda de costo uniforme:
Algoritmo de búsqueda no informada que se utiliza para encontrar el camino de menor costo acumulado entre un nodo de inicio y un nodo objetivo en un grafo ponderado
Cola:
Estructura de datos lineal que organiza los elementos bajo el principal FIFO (First In, First Out)
Pila:
Estructura de datos lineal que sigue el principio LIFO(Last In, First Out o último en entrar, primero en salir)
Completitud:
Es la garantía de que el algoritmo encontrará una solución si es que esta existe
Optimalidad:
Propiedad que garantiza que el algoritmo encuentre la mejor solución posible
Complejidad en tiempo:
Mide la cantidad de operaciones que necesita realizar para encontrar un elemento, en función del tamaño tota de los datos de entrada
Complejidad en espacio:
Mide la cantidad total de memoria RAM o de almacenamiento que el algoritmo necesita para ejecutarse en relación con el tamaño de los datos de entrada

![[Captura de pantalla 2026-10-08 181232.png|409]]
Explora en una sola desde el inicio verde, es lento porque recorre casi todo el mapa para hallar el objetivo
![[Captura de pantalla 2026-10-08 181253.png|428]]
Lanza dos búsquedas al mismo tiempo. Se encuentran en el medio, reduciendo mucho el área explorada
![[Captura de pantalla 2026-10-08 181312.png|405]]
Funciona igual que BFS unidireccional, genera un enorme circulo de exploración
![[Captura de pantalla 2026-10-08 181323.png|408]]
Combina Dijkstra con búsqueda en ambas direcciones, es la opción más rápida y eficiente

Búsqueda heurística:
Método de resolución de problemas en Inteligencia Artificial y ciencias de la computación que utiliza reglas prácticas, atajos o estimaciones para encontrar una solución aceptable de forma rápida, sin revisar todas las combinaciones posibles

*ACT 3.2:*
Algoritmos (A*) y uno ciego.
¿Qué longitud tiene cada algoritmo? 23
¿Cuánto tiempo se tardo cada algoritmo? 0,2000ms

![[Captura de pantalla 2026-10-14 155538.png|445]]

¿Qué longitud tiene cada algoritmo? 18,31
¿Cuánto tiempo se tardo cada algoritmo? 1,3000 ms

![[Captura de pantalla 2026-10-14 155711.png|452]]

¿Qué diferencia observas? 
El camino es más corto (18,31 frente a 23 anterior) porque se habilitó el movimiento en diagonal, permitiendo trazar una línea más directa hacia la meta, aunque a costo de procesar muchos más nodos.

3.4:
1. ¿Cómo se benefician las Redes Neuronales de las GPUs?

Las redes neuronales, especialmente el Deep Learning (aprendizaje profundo), requieren realizar miles de millones de operaciones matemáticas simples de forma simultánea. Las GPUs están diseñadas exactamente para eso.

- *Procesamiento masivo en paralelo:* A diferencia de una CPU (que tiene pocos núcleos pero muy rápidos para tareas secuenciales), una GPU tiene *miles de núcleos más pequeños* diseñados para manejar múltiples tareas a la vez. Esto permite calcular los pesos y sesgos de millones de neuronas simultáneamente.

- *Aceleración de operaciones de álgebra lineal:* El entrenamiento de una red neuronal consiste casi en su totalidad en *multiplicaciones de matrices y sumas de vectores*. Las GPUs destacan en este tipo de matemáticas, reduciendo el tiempo de entrenamiento de meses a solo horas o días.

- *Hardware especializado (Tensor Cores):* Las GPUs modernas (como las arquitecturas Tensor de NVIDIA) incluyen núcleos dedicados exclusivamente a acelerar las operaciones de matriz utilizadas en IA, lo que multiplica la eficiencia energética y la velocidad de cómputo.

- *Ancho de banda de memoria masivo:* Mover los gigantescos conjuntos de datos (datasets) a través del procesador requiere conexiones ultrarrápidas. Las GPUs utilizan memorias de alta velocidad (como HBM o GDDR) que evitan los cuellos de botella al alimentar la red neuronal con datos.
2. ¿Cómo se benefician las GPUs de las Redes Neuronales?

El éxito de las redes neuronales transformó por completo la industria de los gráficos por computadora y redefinió el propósito de las GPUs.

- *Evolución arquitectónica y nuevos mercados:* Originalmente creadas solo para videojuegos, el éxito de la IA obligó a empresas como NVIDIA, AMD e Intel a rediseñar sus chips. Esto creó un mercado multimillonario en centros de datos e IA que hoy supera los ingresos del sector de los videojuegos.

- *Mejora de gráficos mediante IA (DLSS y FSR):* Las GPUs utilizan redes neuronales integradas para *renderizar imágenes a menor resolución y reescalarlas inteligentemente en tiempo real* (técnicas como NVIDIA DLSS o AMD FSR). Esto permite que los videojuegos corran al doble de fotogramas por segundo con un consumo de energía menor.

- *Generación de fotogramas y Ray Tracing:* Las redes neuronales dentro de la GPU ayudan a predecir e interpolar fotogramas completos (Frame Generation) y a "limpiar" el ruido visual que genera el cálculo de iluminación realista (Ray Tracing) mediante algoritmos de denoising basados en IA.

- *Optimización del propio silicio:* Los ingenieros ahora utilizan redes neuronales para *diseñar la próxima generación de GPUs*, optimizando el acomodo de los transistores en el chip para que consuman menos energía y disipen mejor el calor.
  
  Act 3.5:
- ![[Pasted image 20261021180733.png]]