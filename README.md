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

Markdown trata los asteriscos (*) y los guiones bajos () como indicadores de énfasis. El texto envuelto con uno * o _ se envolverá con una etiqueta HTML <em>; los dobles * ’o ’s se envolverán con una etiqueta HTML <strong>. Por ejemplo, esta entrada:

```bash
*single asterisks*

_single underscores_

**double asterisks**

__double underscores__
```
