## Análisis de Resultados

### Árbol de Decisión

La incorporación de la variable de cluster en el Árbol de Decisión produce una mejora consistente en el rendimiento del modelo. El modelo optimizado alcanza una accuracy del 87.80% y un F1-score macro de 0.8742, ligeramente superiores al modelo base.

El análisis de la matriz de confusión muestra una mejor separación entre las clases extremas (`Low` y `High`), reduciendo confusiones con la clase intermedia. Esto sugiere que el árbol se beneficia de la información agregada que aporta el cluster, permitiéndole capturar patrones de comportamiento más complejos y no lineales.

En este caso, la variable de cluster actúa como una característica de alto nivel que refuerza la capacidad del modelo para discriminar entre perfiles de engagement.

---

### Regresión Logística

En la Regresión Logística, la inclusión de la variable de cluster no genera una mejora significativa. El modelo con cluster obtiene una accuracy del 81.86% y un F1-score macro de 0.8110, ligeramente inferiores al modelo sin cluster, que alcanza un F1-score macro de 0.8133.

Las matrices de confusión son muy similares en ambos casos, lo que indica que el modelo lineal no aprovecha de forma efectiva la información adicional introducida por el clustering. Esto es coherente con la naturaleza de la regresión logística, que presenta limitaciones para modelar relaciones no lineales y dependencias complejas entre variables.

---

## Conclusión

Los resultados muestran que el impacto de añadir una variable de cluster depende del tipo de modelo utilizado. En modelos no lineales como los Árboles de Decisión, la variable de cluster aporta información relevante y mejora ligeramente el rendimiento, al capturar patrones globales de comportamiento del jugador.

En cambio, en modelos lineales como la Regresión Logística, esta variable no ofrece una ventaja clara, lo que sugiere que su utilidad está estrechamente ligada a la capacidad del modelo para explotar relaciones complejas entre variables.

En conjunto, el clustering se presenta como una técnica complementaria útil, especialmente cuando se combina con modelos capaces de aprovechar estructuras no lineales en los datos.
