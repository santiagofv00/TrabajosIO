## TALLER DE FORMULACION DE PROBLEMAS DE PROGRAMACION LINEAL


1.	Un carpintero fabrica dos productos: sillas y marcos.  Su producción está limitada por las disponibilidades en listones de madera (36 semanales), por las horas de mano de obra contratada (48 semanales) y por las horas de trabajo disponibles en la máquina cepilladora automática (70 semanales).  Cada silla requiere 4 listones de madera, 3 horas de mano de obra y 10 horas de cepilladora.  Cada marco requiere 4 listones, 6 horas hombre y 5 horas de cepilladora.  El carpintero obtiene $300 y $200 de utilidades por cada silla y marco respectivamente. Formule el problema tal que se halle el programa de fabricación que haga máximas las utilidades.
Buscamos encontrar el número **óptimo** de sillas y marcos a realizar para **máximizar** las ganancias.
#### Variables decisorias:
 Considere:
 $X$ = Número de sillas a realizar
 $Y$ = Número de marcos a realizar
 #### Función Objetivo:
 $Max Z= 300x +200y$
#### Observaciones:
* Se disponen de 36 listones de madera semanales.
* Se disponen de 48 horas de mano de obras semanales.
* Se disponen de 70 horas semanales en la máquina cepilladora.
*  Cada marco requiere 4 listones, 6 horas hombre y 5 horas de cepilladora.
* Cada silla requiere de 6 horas hombre y 5 horas de cepilladora.
#### Restricciones:
$4x + 4y <= 36$  [listones] (Se disponen de 36 listones) 
$3x +  6y <= 48$ [Horas hombre] (Se disponen de 48 horas de mano de obra semanales)
$10x+5y  <= 70$ [Horas cepilladora] (Se disponen de 70 horas semanales en la máquina cepilladora)

Observe que las restricciones pueden ser vistas como la primer columna correspondiente a lo necesario para realizar las sillas, mientras que la segunda columna corresponde a la cantidad de recursos necesarios para realizar los marcos.

 
2.	La cervecería Bloomington produce cerveza común y la de tipo ale.  La cerveza se vende a 5 dólares el barril, y el de ale a 2 dólares el barril.  La producción de un barril de cerveza requiere de 5 libras de cebada y 2 libras de lúpulo. La producción de un barril de ale requiere de 2 libras de cebada y 1 libra de lúpulo.  Se dispone de 60 libras de cebada y de 25 libras de lúpulo.  Formule el problema para maximizar los ingresos.
Buscamos encontrar el número óptimo de cervezas de cierto tipo para vender para máximizar las ganancias.
#### Variables decisorias:
$X$ = Unidades producidas de cerveza común \\
$Y$ = Unidades producidas de cerveza tipo ale 
#### Función Objetivo
$Max Z = 5X+ 2Y$
#### Observaciones
* La producción de un barril de cerveza requiere de 5 libras de cebada y 2 libras de lúpulo.
* La producción de un barril de ale requiere de 2 libras de cebada y 1 libra de lúpulo.
* Se dispone de 60 libras de cebada y de 25 libras de lúpulo.
#### Restricciones
$5x + 2y \leqslant60$ [Libras de cebada]
$2x + y\leqslant25$    [Libras de lúpulo]
3.	Un agricultor tiene 200 acres y dispone de 18000 horas-hombre.  El desea determinar el área (en acres) que asignará a los siguientes productos: maíz, trigo, quimbombó, tomate y ejotes.  El agricultor debe producir al menos 250 toneladas de maíz para alimentar a sus puercos y ganado, y debe producir al menos 80 toneladas de trigo, debido a un contrato que firmó previamente.  A continuación se resumen el tonelaje y la mano de obra en horas-hombre por acre para diferentes productos:

|	   | Maíz | Trigo | Quimbombó | Tomate | Ejote |
|------|-------|----------------|----------|--------|-------|
|Ton/acre |	10  |	4	| 4 |	8 |	6 |
|Horas-hombre/acre |120	|150|100|80|120|

El maíz, trigo, quimbombó, tomate y ejote se venden, respectivamente, en $120, $150, $50, $80 y $55 por tonelada.  Formular el problema para maximizar los ingresos.
#### Variables decisorias:
$X_{i=1,2,3,4,5}$= Cantidad de acres a asignar para el producto $i=$ 1(Maíz), 2(Trigo), 3(Quimbombó), 4(Tomate), 5(Ejote)
#### Función Objetivo
$Max Z = 120(X_1-250)+ 150(X_2 -80) + 50X_3+80X_4 +55X_5$
#### Observaciones
* Se tienen 200 acres.
* Se disponen de 18000 horas-hombre.
* Se deben de producir al menos 250 toneladas de maíz.
* Se deben de producir al menos 80 toneladas de trigo.
#### Restricciones
* X1+ X2+ X3 + X4 + X5 = 200 [Acres] (Dispone de 200 acres)
* 10X1 >= 250 [Toneladas de maíz] 
* 4X2 >= 80 [Toneladas de trigo]
* $X_{i=1,2,3,4,5}$ (No negatividad)

14.	Una corporación ha decidido producir tres productos nuevos.  En este momento, cinco de sus plantas tienen capacidad de producción en exceso.  El costo unitario de fabricación del primer producto sería de $90, $82, $92, $84 y $86, en las plantas 1, 2, 3, 4 y 5, respectivamente.  El costo unitario de fabricación del segundo producto sería $62, $58, $64, $56 y $58, en las plantas 1, 2, 3, 4 y 5, respectivamente. El costo unitario de fabricación del tercer producto sería $76, $70, $80, en las plantas 1, 2, y 3, respectivamente, mientras que las plantas 4 y 5 no tienen la capacidad para elaborar este producto.  Los pronósticos de ventas indican que deben producirse al día 5000, 3000 y 4000 unidades de los productos 1, 2 y 3, respectivamente.  Las plantas 1, 2, 3, 4 y 5 tienen capacidad para producir 2000, 3000, 2000, 3000 y 5000 unidades cada día, respectivamente, sin importar el producto o la combinación de productos de que se trate.  Supóngase que cualquier planta que tenga los elementos y la capacidad necesarias puede producir cualquier combinación de los productos en cualquier cantidad.
#### Observaciones
Se disponen de **3 productos** y de **5 plantas**, el producto 3 no se puede elaborar en las plantas 4 y 5; hay un pronóstico de ventas y una capacidad de producción en cada fábrica. 
Unas posibles variables decisorias serían los pares de productos y fábricas, teniendo en cuenta la restricción en las plantas 4 y 5 para la planta 3.
#### Variables decisorias:
$X_{ij}$: Cantidad del producto i elaborado en la planta j.  
$i=1,2,3,4,5 \\ j=1,2,3$
#### Función Objetivo:
$$Min Z = \begin{bmatrix}  
					90 X_{11}& 62X_{12} & 76X_{13} \\ 
					82X_{11} & 58X_{22}& 70X_{23} \\
					92X_{11} &64 X_{32}& 80X_{33} \\
					84X_{11} & 56X_{42} & 0 \\
					86X_{11} & 58X_{52} & 0
					\end{bmatrix}
					\begin{bmatrix}
		           1 \\
		           1 \\
		           1
		         \end{bmatrix}
$$ 
#### Restricciones:
* Producción diaria:
$$ \begin{bmatrix}  
					90 X_{11}& 62X_{12} & 76X_{13} \\ 
					82X_{11} & 58X_{22}& 70X_{23} \\
					92X_{11} &64 X_{32}& 80X_{33} \\
					84X_{11} & 56X_{42} & 0 \\
					86X_{11} & 58X_{52} & 0
					\end{bmatrix}
					\begin{bmatrix}
		           1 \\
		           0 \\
		           0
			     \end{bmatrix} = 5000\\ 
			      $$
			       $$\begin{bmatrix}  
					90 X_{11}& 62X_{12} & 76X_{13} \\ 
					82X_{11} & 58X_{22}& 70X_{23} \\
					92X_{11} &64 X_{32}& 80X_{33} \\
					84X_{11} & 56X_{42} & 0 \\
					86X_{11} & 58X_{52} & 0
					\end{bmatrix}
					\begin{bmatrix}
		           0 \\
		           1 \\
		           0
			     \end{bmatrix} =3000$$
			      $$\begin{bmatrix}  
					90 X_{11}& 62X_{12} & 76X_{13} \\ 
					82X_{11} & 58X_{22}& 70X_{23} \\
					92X_{11} &64 X_{32}& 80X_{33} \\
					84X_{11} & 56X_{42} & 0 \\
					86X_{11} & 58X_{52} & 0
					\end{bmatrix}
					\begin{bmatrix}
		           0 \\
		           0 \\
		           1
			     \end{bmatrix} =4000$$
* Producción de las plantas:
 $$\begin{bmatrix}  
					90 X_{11}& 62X_{12} & 76X_{13} \\ 
					82X_{11} & 58X_{22}& 70X_{23} \\
					92X_{11} &64 X_{32}& 80X_{33} \\
					84X_{11} & 56X_{42} & 0 \\
					86X_{11} & 58X_{52} & 0
					\end{bmatrix}^\mathsf{T}
					\begin{bmatrix}
		             1 \\
		           0 \\
		           0 \\
		           0\\
		           0\\
			     \end{bmatrix} = 2000$$
$$\begin{bmatrix}  
					90 X_{11}& 62X_{12} & 76X_{13} \\ 
					82X_{11} & 58X_{22}& 70X_{23} \\
					92X_{11} &64 X_{32}& 80X_{33} \\
					84X_{11} & 56X_{42} & 0 \\
					86X_{11} & 58X_{52} & 0
					\end{bmatrix}^\mathsf{T}
					\begin{bmatrix}
		             0 \\
		           1 \\
		           0 \\
		           0\\
		           0\\
			     \end{bmatrix} = 3000$$
$$\begin{bmatrix}  
					90 X_{11}& 62X_{12} & 76X_{13} \\ 
					82X_{11} & 58X_{22}& 70X_{23} \\
					92X_{11} &64 X_{32}& 80X_{33} \\
					84X_{11} & 56X_{42} & 0 \\
					86X_{11} & 58X_{52} & 0
					\end{bmatrix}^\mathsf{T}
					\begin{bmatrix}
		             0 \\
		           0 \\
		           1 \\
		           0\\
		           0\\
			     \end{bmatrix} = 2000$$
$$\begin{bmatrix}  
					90 X_{11}& 62X_{12} & 76X_{13} \\ 
					82X_{11} & 58X_{22}& 70X_{23} \\
					92X_{11} &64 X_{32}& 80X_{33} \\
					84X_{11} & 56X_{42} & 0 \\
					86X_{11} & 58X_{52} & 0
					\end{bmatrix}^\mathsf{T}
					\begin{bmatrix}
		             0 \\
		           0 \\
		           0 \\
		           1\\
		           0\\
			     \end{bmatrix} = 3000$$
$$\begin{bmatrix}  
					90 X_{11}& 62X_{12} & 76X_{13} \\ 
					82X_{11} & 58X_{22}& 70X_{23} \\
					92X_{11} &64 X_{32}& 80X_{33} \\
					84X_{11} & 56X_{42} & 0 \\
					86X_{11} & 58X_{52} & 0
					\end{bmatrix}^\mathsf{T}
					\begin{bmatrix}
		           0 \\
		           0 \\
		           0 \\
		           0\\
		           1\\
			     \end{bmatrix} = 5000$$ 
			     11.	Supóngase que Inglaterra, Francia y España producen todo el trigo, la cebada y la avena del mundo.  La demanda mundial de trigo requiere que se dediquen 125 millones de acres de tierra a la producción de este cereal.  Análogamente, se requieren 60 millones de acres de tierra para cebada y 75 millones de acres para avena.  La cantidad total de tierra para este fin en Inglaterra, Francia y España es de 70 millones de acres, 110 millones de acres y 80 millones de acres, respectivamente.  El número de horas de trabajo necesarias en Inglaterra, Francia y España para producir un acre de trigo es de 18 horas, 13 horas y 16 horas, respectivamente. El número de horas de trabajo necesarias en Inglaterra, Francia y España para producir un acre de cebada es de 15 horas, 12 horas y 12 horas, respectivamente.  El número de horas de trabajo necesarias en Inglaterra, Francia y España para producir un acre de avena es de 12 horas, 10 horas y 16 horas, respectivamente.  El costo de la mano de obra por hora para producir trigo es de $3.00, $2.40 y $3.30 en Inglaterra, Francia y España, respectivamente. El costo de la mano de obra por hora para producir cebada es de $2.70, $3.00 y $2.80 en Inglaterra, Francia y España, respectivamente. El costo de la mano de obra por hora para producir avena es de $2.30, $2.50 y $2.10 en Inglaterra, Francia y España, respectivamente.  El problema es asignar el uso de la tierra en cada país de manera que se satisfagan los requerimientos de alimentos y se minimice el costo total de la mano de obra.
#### Observaciones:
Se busca encontrar la cantidad adecuada de acres de recursos para producir en cada país.
La cantidad total de tierra para este fin en Inglaterra, Francia y España es de 70 millones de acres, 110 millones de acres y 80 millones de acres, respectivamente.
#### Variables decisorias:
$X_{ij}$: Millones de Acres del producto i producidos en el país j.
#### Función objetivo:
$Min Z = \begin{bmatrix}  
					90 X_{11}& 62X_{12} & 76X_{13} \\ 
					82X_{11} & 58X_{22}& 70X_{23} \\
					92X_{11} &64 X_{32}& 80X_{33}
					\end{bmatrix}
					\begin{bmatrix}  
					1 \\ 
					1\\
					1 
					\end{bmatrix}$
#### Restricciones:

<!--stackedit_data:
eyJoaXN0b3J5IjpbMTIyODg4NjEzNF19
-->