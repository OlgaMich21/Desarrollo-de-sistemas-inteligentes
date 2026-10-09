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

![[Captura de pantalla 2026-10-08 181232.png]]
Explora en una sola desde el inicio verde, es lento porque recorre casi todo el mapa para hallar el objetivo
![[Captura de pantalla 2026-10-08 181253.png]]
Lanza dos búsquedas al mismo tiempo. Se encuentran en el medio, reduciendo mucho el área explorada
![[Captura de pantalla 2026-10-08 181312.png]]
Funciona igual que BFS unidireccional, genera un enorme circulo de exploración
![[Captura de pantalla 2026-10-08 181323.png]]
Combina Dijkstra con búsqueda en ambas direcciones, es la opción más rápida y eficiente

