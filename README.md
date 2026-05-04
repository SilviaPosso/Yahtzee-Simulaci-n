# Yahtzee-Simulacion
Descripción
Este proyecto implementa una simulación del juego Yahtzee clásico con dos jugadores (Humano vs IA o IA vs IA), utilizando el método de Montecarlo para estimar probabilidades de obtener puntos en cada categoría.
La distribución de probabilidad es uniforme discreta: cada cara del dado (1–6) tiene probabilidad 1/6.

Características
Simulación de partidas completas de Yahtzee con 12 categorías de puntuación.

Hasta 3 lanzamientos de 5 dados por turno.

Estrategia de IA basada en conservar los dados más frecuentes (greedy).

Cálculo de probabilidades mediante Montecarlo con miles de simulaciones.

Resultados mostrados en porcentajes y gráficas de barras textuales.

Requisitos
Python 3.8 o superior.

No requiere librerías externas (solo random y collections de la biblioteca estándar).

Instalación
Clona el repositorio y entra en la carpeta del proyecto:

bash
git clone https://github.com/usuario/yahtzee-montecarlo.git
cd yahtzee-montecarlo
Ejecución
Ejecuta el programa desde la terminal:

bash
python yahtzee.py
Modos de juego
Modo 1: Humano vs IA (interactivo por consola).

Modo 2: IA vs IA (simulación automática).

Al finalizar la partida, se puede ejecutar el módulo de estadísticas Montecarlo para calcular probabilidades:

text
¿Ver estadísticas Montecarlo? (s/n)
Estructura del repositorio
Código
├── yahtzee.py                # Código fuente principal
├── Apellido_Nombre_Montecarlo.docx   # Documento con introducción, metodología, resultados y conclusiones
├── README.md                 # Instrucciones de uso y descripción del proyecto
Ejemplo de salida (Montecarlo, 10 000 simulaciones)
Código
ESTADÍSTICAS MONTECARLO
10,000 simulaciones de 5 dados
Probabilidad de obtener puntos en 1 solo lanzamiento
Unos                  83.3%  ████████████████████████
Escalera corta        30.0%  ████████
Escalera larga         3.1%  █
Full House             3.9%  █
Yahtzee (5 iguales)    0.08% 
Azar                 100.0%  █████████████████████████████████████
