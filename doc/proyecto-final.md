# Proyecto Final  “Farmacia ABC”
* Programación Avanzada Backend
* Diplomado Java

## Objetivos
* Fomentar la investigación y autoaprendizaje del alumno.
* Aplicar los conocimientos de Programación Orientada a Objetos, utilizando interfaces, clases, clases abstractas.
* Resolver problemas aplicando estructuras de datos dinamicas y recursividad.
* Implementar métodos de ordenamiento implicitos (arboles) o explicitos (quicksort) sobre estructuras de datos.
* Utilizar los conocimientos adquiridos de uso de estructuras, listas y árboles dinámicos

## Descripción

La empresa “Tu salud en mis manos” es una distribuidora de fármacos a nivel nacional, actualmente cuenta con un inventario de fármacos los cuales son dis-tribuidos únicamente vía telefónica, para ello le han requerido que construya una aplicación  la cual permita administrar el inventario existente y poder crear los pedidos desde esta.

La aplicación debe de permitir la carga del inventario inicial desde un archivo,  dado que los inventarios pueden crecer demasiado no podrá cargar todo el ar-chivo a memoria, por lo que deberá de crear un indice utilizando la estructura de árbol binario almacenando el numero de linea y el nombre del fármaco dentro del nodo.

Una vez cargado el archivo el sistema debe de permitir la creación de pedidos, para los cuales se necesita ingresar la siguiente información: nombre del cliente, dirección, nit, el listado de fármacos a despachar y el total a cancelar.

La aplicación deberá estar optimizada para la búsqueda de los fármacos por nombre, y debe permitir la búsqueda de los mismos para poder agregarlos a un pedido.

Dado que se cuenta con una cantidad finita de elementos de un fármaco cuando la cantidad disponible del fármaco sea 0 este elemento se deberá de eliminar del árbol.

Deberá de contar con la interfaz necesaria para poder re abastecer los fármacos que no tengan existencia en un momento dado, el re abastecimiento de los fárma-cos será a travez de una simulación generando inventario de forma aleatoria en-tre 1 y 15. Esto hará que el sistema deba de genera nuevamente el indice y poder así incluir a los fármacos con existencia.

En todo momento se podrá evaluar el estado del indice a travez de los recorridos  vistos en clase para los arboles binarios, así como poder exportar el mismo a travez de un archivo.
