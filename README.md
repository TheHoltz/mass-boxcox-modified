# mass-boxcox-modified

It's a small modification of the function boxcox of the R package MASS, to return the best lambda at the method.
The motivation for this occurred because the people at my work usually searches manually by using zoom on the graph, wasting so much time.

Use example:
```
modelo <- lm(iris$Sepal.Length~iris$Sepal.Width+iris$Petal.Length+iris$Petal.Width)

ajuste <- boxcox(modelo)

ajuste$bestLambda

```
