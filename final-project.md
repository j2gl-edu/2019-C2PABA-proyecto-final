# Proyecto Final - Programación Avanzada Backend 

![Logo Academik](./doc/logo_Academik.png)

## Farmacia ABC
* **Código** 2019-C2PABA
* **Ciclo** 1-2019
* **Sección** A
* **Fecha de Entrega** 3 de Junio 2019

## Objetivos
* Fomentar la investigación y autoaprendizaje del alumno.
* Aplicar los conocimientos de Programación Orientada a Objetos, utilizando interfaces, clases, clases abstractas.
* Resolver problemas aplicando estructuras de datos dinamicas y recursividad.
* Implementar métodos de ordenamiento implicitos (arboles) o explicitos (quicksort) sobre estructuras de datos.
* Utilizar los conocimientos adquiridos de uso de estructuras, listas y árboles dinámicos

## Descripción

La empresa "Tu salud en mis manos" es una distribuidora de fármacos a nivel nacional, actualmente cuenta con un inventario de fármacos los cuales son distribuidos únicamente vía telefónica, para ello le han requerido que construya una aplicación la cual permita administrar el inventario existente y poder crear los pedidos desde esta.

La aplicación debe de permitir la carga del inventario inicial desde un archivo, dado que los inventarios pueden crecer demasiado no podrá cargar todo el archivo a memoria, por lo que deberá de crear un indice utilizando la estructura de árbol binario almacenando el numero de linea y el nombre del fármaco dentro del nodo.

Una vez cargado el archivo el sistema debe de permitir la creación de pedidos, para los cuales se necesita ingresar la siguiente información: nombre del cliente, dirección, nit, el listado de fármacos a despachar y el total a cancelar.

La aplicación deberá estar optimizada para la búsqueda de los fármacos por nombre, y debe permitir la búsqueda de los mismos para poder agregarlos a un pedido.

Dado que se cuenta con una cantidad finita de elementos de un fármaco cuando la cantidad disponible del fármaco sea 0 este elemento se deberá de eliminar del árbol.

Deberá de contar con la interfaz necesaria para poder re abastecer los fármacos que no tengan existencia en un momento dado, el re abastecimiento de los fármacos será a travez de una simulación generando inventario de forma aleatoria entre 1 y 15. Esto hará que el sistema deba de genera nuevamente el indice y poder así incluir a los fármacos con existencia.

En todo momento se podrá evaluar el estado del indice a travez de los recorridos vistos en clase para los arboles binarios, así como poder exportar el mismo a travez de un archivo.

## Fases

### 1. Leer Archivo

* Fecha: Miercoles 15 de Mayo 2019

Leer el archivo csv (Comma separated values) y subirlo a un árbol que contenga un hojas, de tipo nodo con la siguiete estructura:

* ProductTreeNodo 
    * Name (Nombre)
    * Stock (Existencia)
    * Line Number (Numero de Linea)

Luego de llenar el arbol, agregar una opción para desplegarlo.

### 2. Menu y Busqueda

**Fecha: Miercoles 22 de Mayo 2019**

Se debe implemetar la búsqueda de productos en el arbol.  También se debe de hacer un menú con las siguientes opciones:
* Cargar datos de Archvio CSV
* Desplegar Inventario
* Búscar un producto por descripción
* Ingresar Pedido
* Salir

### 3. Pedidos
**Fecha: Miercoles 29 de Mayo 2019**

a) Crear las siguientes estructuras:
* Product
    * Id (Código)
    * Name (Nombre)
    * Quantity (Cantidad)
    * Unit Price (Precio Unitario)
    * Amount (Precio Total)
    * Line Number (Numero de Linea)
* Pedido
    * Tax Id (Nit) 
    * Client Name (Nombre del cliente)
    * Address (Direccion)
    * Product List (Lista de tipo Producto con todos los farmacos que hay en el pedido)
    * Total Amount (Total del pedido)

b) Hacer la forma de ingreso del encabezado  
c) Hacer la forma de ingreso de productos al pedido  
d) Calcular el precio final del pedido y descontar del inventario en el arbol.   
