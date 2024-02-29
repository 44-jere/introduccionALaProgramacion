# Hoja de Trabajo 3
## Problema #1:
* Realizar un programa que solicite la carga por teclado de dos números, si el primero es mayor al segundo informar su suma y diferencia, en caso contrario informar el producto y la división del primero respecto al segundo.Problema 
```mermaid

graph TB

inicio((inicio))
fin((fin))
validarTamaño{es número 1 mayor a numero 2?} 
validarIgualdad{son número 1 y 2 iguales?}
validaTipoDeDato{son número 1 y 2 de tipo number?}
variables[/Ingrese número 1 y número 2/]
alert[ingrese numeros que sean diferentes]
devolverSumaYDiferencia[/Devolver <br> número 1 + número 2 <br> número 1 - número 2/]
devolverDivisionYProducto[/Devolver <br> número 1 / número 2 <br> número 1 * número 2/]

inicio -->

variables --> 
validaTipoDeDato --si-->
validarIgualdad --no-->

validarTamaño --si-->
devolverSumaYDiferencia -->
fin

validarTamaño --no-->
devolverDivisionYProducto -->
fin

validaTipoDeDato --no-->inicio
validarIgualdad --si-->alert-->inicio


classDef estilo fill:#f9f,stroke:#333stroke-width:2px
class inicio estilo
```

# Diagrama 2
> * Se ingresan tres notas de un alumno, si el promedio es mayor o igual a siete mostrar un mensaje "Promocionado".Problema 

```mermaid
graph TB
inicio((inicio))
fin((fin))
variables[/Lista de notas/]
retornoPositivo[/promocionado/]
retornoNegativo[/no promocionado/]
validarArray{es nuestra lista de notas un array? }
ValidarValoresArray{son todos los valores del array dato de tipo number}
operar[cantidadNotas = tamaño del array tomando el cuenta el 0 <br> sumaTotal = todos los valores del array sumados]
obtenerPromedio[promeidio = sumaTotal/cantidadNotas]
estaAprovado{es el promedio mayor o igual a 7?}

inicio --> variables -->

validarArray--no-->
    inicio

validarArray--si--> 
    iterar[iterar cada valor] -->

        ValidarValoresArray--no-->
            inicio

        ValidarValoresArray --si-->
            operar -->
            obtenerPromedio -->
                estaAprovado --si--> 
                    retornoPositivo --> fin
                estaAprovado --no--> 
                    retornoNegativo --> fin
                    
classDef estilo fill:#f9f,stroke:#333stroke-width:2px
class inicio estilo
```

# Diagrama 3:
> * Se ingresa por teclado un número positivo de uno o dos dígitos (1..99) mostrar un mensaje indicando si el número tiene uno o dos dígitos.(Tener en cuenta que condición debe cumplirse para tener dos dígitos un número entero)

```mermaid
graph TB
inicio((inicio))
fin((fin))
variables[/números/]
validarNumero{es número de tipo number? <br>y<br>es menor a 100 y mayor a igual a 0?}
validarDigito{es mayor igual a 10?}
RespuestaNumeroDosDigitos[/el Número tiene 2 digitos/]
RespuestaNumeroUnDigito[/el Número tiene 1 digito/]

inicio -->
variables-->

validarNumero --no-->inicio

validarNumero --si-->
validarDigito--no-->RespuestaNumeroUnDigito-->fin

validarDigito--si-->RespuestaNumeroDosDigitos-->fin

classDef estilo fill:#f9f,stroke:#333stroke-width:2px
class inicio estilo

```
