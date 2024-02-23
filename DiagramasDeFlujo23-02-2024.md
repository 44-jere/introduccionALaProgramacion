
# Problema #1:

> * Realizar la carga de dos números enteros por teclado e imprimir su suma y su producto.

```mermaid
graph TB
fin((fin))
inicio((Inicio)) 
variables[/número1,número2/]

inicio--> 
variables --> 
verificarInput{Son los numeros 1 y 2 enteros?}--no-->
inicio
verificarInput--si-->
operacion{La operacion a realizar es una suma?}

operacion--si-->
sumar[resutlado de la suma = número 1+número 2]-->
resultadoSuma[\resutlado de la suma \] --> fin

operacion--no-->
multiplicar[resutlado de la multiplicaicón= número 1*número 2] -->
resultadoMultiplicacion[/resutlado de la multiplicación/] --> fin

```

# Problema #2:

> * Realizar la carga del precio de un producto y la cantidad a llevar. 
> * Mostrar cuanto se debe pagar 
> * (se ingresa un valor entero en el precio del producto).
```mermaid
graph TB
fin((fin))
inicio((Inicio)) 
variables[/Cantidad a llevar,Precio del producto/]
validarCantidadLlevada{Es la cantidad a llevar y el precio del producto un número entero mayor a 0? <br> y <br> Es la cantidad a llevar es un número positivo?}

inicio --> variables
variables --> 
validarCantidadLlevada--no--> 
inicio

validarCantidadLlevada --si-->
cobrar[Total a pagar = <br> Precio del producto * Cantidad a Llevar] -->
total[/Total a pagar/]--> 
fin
```
# Problema #3:

> * Realizar la carga del lado de un cuadrado, mostrar por pantalla el perímetro del 
mismo (El perímetro de un cuadrado se calcula multiplicando el valor del lado por cuatro)
```mermaid
graph TB
fin((fin))
inicio((Inicio)) 
variables[/Lado/]
esEntero{Es el Lado un número positivo mayor a 0?}

inicio-->
variables -->
esEntero --no-->inicio

esEntero--si-->
operar[Perímetro = lado * 4 ]-->
perimetro[/Perímetro/]-->
fin

```
