# Whatsapp_analysis
Análisis de chat de Whatsapp de dos personas

Este código funciona para analizar chats entre dos personas a través de la plataforma de mensajería instantánea Whatsapp.

## Preparación del archivo txt
Para poder utilizar este código, el primer paso se realiza directamente desde el celular en Whatsapp.  
Dentro de la conversación que vamos a querer analizar, debemos:  
1- ir a la parte de opciones (los tres puntos en vertical que aparecen arriba a la izquierda)  
2- seleccionar la opción "Más"  
3- Seleccionar "Exportar chat".  
4- Elegir la opción "Sin archivos multimedia", de ese modo el proceso demorará menos y nosotros de todos modos no los estaremos utilizando  
5- Exportarlo por mail suele ser lo mas sencillo  
6- Descargar el txt y guardarlo en la misma carpeta donde descargarán este archivo .ipynb  

## Preparación del código
1- Deberán guardar en la misma carpeta el archivo descargado de texto, y el archivo del proyecto.  
2- El archivo .ipynb lo pueden ejecutar desde Jupyter Notebook, modificando previamente algunos datos:   
2- a) El nombre a ingresar deberá ser su nombre como aparece en Whatsapp. Deberán reemplazar "Isabel" por su nombre.  
```python
mi_nombre = "Isabel"
```

2- b) El nombre del archivo txt que tienen descargado, deberán reemplazar "Chat de Whatsapp.txt" por el nombre de archivo que tengan
```python
#ingresar el nombre del archivo que van a analizar
file = open(r'Chat de Whatsapp.txt',mode='r',encoding="utf8")
data = file.read()
file.close()
```

## Aclaración importante sobre formato
Este archivo funciona para el txt que descargó mi dispositivo, de acuerdo a su sistema operativo y configuración regional.
Este es un ejemplo de las líneas que aparecen en mi archivo. Deberás modificar el RegEx de acuerdo a tu propio formato de fecha y hora:
```python
['4/4/18 5:21 p.\xa0m. - Isabel: Bueno termine',
'4/4/18 5:21 p.\xa0m. - Isabel: Todo ok',
'4/4/18 5:21 p.\xa0m. - xxxx: Genial!!!',
'4/4/18 5:21 p.\xa0m. - xxxx: 👏🏻👏🏻👏']
```          

## Contribuciones
Estoy disponible para conversar cualquier modificación que deseen sugerir al código


