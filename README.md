# GvsTModQ
Código desarrollado por Ricardo Mogollon y Rafael Porras.

El código utiliza una base de datos comp.csv con información termodinámica para más de 200 compuestos obtenida del NIST Chemistry WebBook, para la cual se puede calcular el cambio en la energía libre de una reacción, o generar una gráfica de la diferencia de la energía libre con respecto a la temperatura.
Gráficas G vs T para dos casos:
1) G vs T, G = H° - T°S
2) G vs T, G = H(T) - TS(T)

Los rangos default de la temperatura son (298-1000) y las gráficas son generadas en este mismo; sin embargo hay compuestos cuyos parámetros termodinámicos no abarquen este rango completamente, por lo que el usuario puede redefinir el límite superior de este rango de temperatura y generar nuevamente las gŕaficas.

El código es altamente dependiente de la forma en que es escriba la ecuación química inicial, como ejemplo considere la descomposión del agua:

H2O -> O2 + H2

De esta forma las constantes y rangos de temperatura irán en el orden H2O-O2-H2; si se considerara:

H2O -> H2 + O2

Los parámetros y rangos en las listas de parámetros y rangos de temperatura tendrán el orden H2O-H2-O2.
