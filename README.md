# Ejercicio-rpa-excel
Aplicando un bot a una planilla de excel

Software Design Document [SDD] Rocketbot

1- Introducción.

Nombre del proyecto : Ejercicio 2 - EJercici rpa excel.
Autor: Jorge Ferreyra
Fecha de versión: 2025.0
Número de versión: v1
2- Objetivo. Este documento describe la arquitectura y el diseño del proceso RPA desarrollado en Rocketbot, incluyendo flujos, módulos y configuraciones utilizadas.

3- Descripción. Este bot automatiza el filtrado y extraccion de una planilla de excel, crea yguarda los datos filtrdos en una nueva hoja.
hace un backup en un archivo excel, y lo manda por un correo Gmail a un destinatario pre establecido.

4- Sistema Windows 10. Chrome. Rocketbot versión v.2025.01.17

5- Diagrama de flujo
![Facturacion](https://github.com/user-attachments/assets/4524d4cf-7783-417d-9b8f-e12b3542b0d5)

6 Descripción de paso a paso del proceso: Inicio:

Abri un archivo de excel del cual quiero extraer la informacion
Crear una hoja nueva 
Copiar el encabezado y el ancho de las celdas de la hoja Planilla de Facturacion Aa la hoja Responsable Monotributo
Extraer los datos de la columna B
Recorrer los datos con un ciclo While
y filtrar datos segun la condicional IF declarada(detalle en el diagrama)
Copiar y guardar los datos extraidos en la hoja Responsable Monotributo.
Hacer una copia del archivo y enviarlo por correo a un Gmail previamente establecido.

Salida:
Hacer una copia del archivo y enviarlo por correo a un Gmail previamente establecido.

Mensaje final (mensaje_final)

7- Variables

filas																																								
resultado																									
mensaje_alerta
columnas
filas_resp_monot
resp_monot
fecha_final
path_log
path_xlsx
cont_hoja2
error
status
res
correo
pass_correo
destinatario
mensaje
mensaje_final
