# Investigación Ciencia de Datos en Python
## ¿Qué es GIT?
Git es un Sistema de Control de Versiones Distribuido (DVCS) utilizado para guardar diferentes versiones de un archivo (o conjunto de archivos) para que cualquier versión sea recuperable cuando lo desee.
Git también facilita el registro y comparación de diferentes versiones de un archivo. Esto significa que los detalles sobre qué cambió, quién cambió qué, o quién ha iniciado una propuesta, se pueden revisar en cualquier momento.
## ¿Qué es GITHUB?
GitHub es una plataforma basada en la web donde los usuarios pueden alojar repositorios Git. Facilita compartir y colaborar fácilmente en proyectos con cualquier persona en cualquier momento.
GitHub también fomenta una participación más amplia en proyectos Código Abierto al proporcionar una manera segura de editar archivos en repositorios de otros usuarios.

# Markdown y sus comandos
## ¿Para qué se utiliza Markdown?
Al igual que HTML o LaTeX, Markdown es un lenguaje de marcado, pero, a diferencia de estos, pretende ofrecer la máxima facilidad de lectura al usuario. Sus comandos de formateado no son abstractos, sino cercanos al significado real. 

## Comandos

### ENCABEZADOS
Markdown admite dos estilos de encabezados, Setext y atx.

```bash
This is an H1
=============

This is an H2
-------------
```

Los encabezados de estilo Atx usan 1-6 caracteres hash al comienzo de la línea, correspondientes a los niveles de encabezado 1-6.

```bash
# This is an H1

## This is an H2

###### This is an H6
```

### CITAS EN BLOQUE
Markdown utiliza caracteres de estilo de correo electrónico > para comillas en bloque. Si está familiarizado con citar pasajes de texto en un mensaje de correo electrónico, entonces sabe cómo crear una cita en bloque en Markdown. Se ve mejor si ajusta firmemente el texto y pone un > antes de cada línea.

Las citas en bloque se pueden anidar (es decir, una cita en bloque en una cita en bloque) agregando niveles adicionales de >:

```bash
> This is the first level of quoting.
>
> > This is nested blockquote.
>
> Back to the first level.
```

Las citas en bloque pueden contener otros elementos de Markdown, incluidos encabezados, listas y bloques de código:

```bash
> ## This is a header.
> 
> 1.   This is the first list item.
> 2.   This is the second list item.
> 
> Here's some example code:
> 
>     return shell_exec("echo $input | $markdown_script");
```

### LISTAS
Markdown admite listas ordenadas (numeradas) y no ordenadas (con viñetas).

Las listas desordenadas utilizan asteriscos, más y guiones - de manera intercambiable - como marcadores de lista:

```bash
*   Red
*   Green
*   Blue
```
es equivalente a:
```bash
+   Red
+   Green
+   Blue
```
Las listas ordenads usan numeros seguidas de puntos:
```bash
1.  Bird
2.  McHale
3.  Parish
```
### ÉNFASIS

Markdown trata los asteriscos y los guiones bajos como indicadores de énfasis. 

```bash
*single asterisks*

_single underscores_

**double asterisks**

__double underscores__
```
### IMÁGENES

Markdown utiliza una sintaxis de imagen que pretende parecerse a la sintaxis de los enlaces, lo que permite dos estilos: en línea y de referencia.

La sintaxis de la imagen en línea se ve así:

```bash
![Alt text](/path/to/img.jpg)

![Alt text](/path/to/img.jpg "Optional title")
```
### ESCAPE DE BARRA INVERTIDA
Markdown le permite usar escapes de barra invertida para generar caracteres literales que de otro modo tendrían un significado especial en la sintaxis de formato de Markdown. 
```bash
\*literal asterisks\*
```
Markdown proporciona escapes de barra invertida para los siguientes caracteres:
```bash
\   barra invertida
`   retroceso
*   asterisco
_   guion bajo
{}  llaves
[]  corchetes
()  paréntesis
#   símbolo de hash
+   signo más
-   signo menos (guión)
.   punto
!   signo de exclamación
```
# MagicCells
Las celdas de código del Jupyter NoteBook pueden contener comandos especiales que no son código Python válido, pero afectarán el comportamiento del cuaderno.
## %matplotlib inline
Es uno de los mas populares comando :
```bash
%matplotlib inline
```
El uso de este comando al inicio de un Jupyter NoteBook producirá gráficos matplotlib en línea en las celdas del cuaderno. Sin %matplotlib en línea, los gráficos aparecerán como ventanas externas. Un comienzo típico para un cuaderno Jupyter usando matplotlib es:
```bash
import numpy as np
import matplotlib.pyplot as plt
%matplotlib inline
```
###%load
El comando %load llamara un modulo de Python, webpage o archivo dentro de un Jupyter notebook
```bash
# %load hello.py
def main():
    print('This code was run from a seperate Python file')
    print('Hello from the file hello.py')

if name == "main":
    main()
```
### %run
El comando %run seguido de un nombre de un archivo Python, ejecutara el archivo como script. 
```bash
| current_folder
---| notebook.ipynb
---| hello.py
```
```bash
%run hello.py
```
### Otros comandos usados
```bash
%pwd
print the current working directory

%cd
change the current working directory

%ls
list the contents of the current directory

%history
the history of the In [ ]: commands
```
