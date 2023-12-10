---
published: false                        # Optional. Set to true to publish the workshop (default: false)
type: workshop                          # Required.
title: Python para principiantes              # Required. Full title of the workshop
short_title: Iniciación a Python     # Optional. Short title displayed in the header
description: Este es un workshop para comenzar en el mundo Python para analistas de datos  # Required.
level: beginner                         # Required. Can be 'beginner', 'intermediate' or 'advanced'
authors:                                # Required. You can add as many authors as needed      
  - Antonio Soto
contacts:                               # Required. Must match the number of authors
  - antoniosotorodriguez@gmail.com, @antoniosql
duration_minutes: 20                    # Required. Estimated duration in minutes
tags: python          # Required. Tags for filtering and searching
#banner_url: assets/banner.jpg           # Optional. Should be a 1280x640px image
#video_url: https://youtube.com/link     # Optional. Link to a video of the workshop
#audience: students                      # Optional. Audience of the workshop (students, pro devs, etc.)
#wt_id: <cxa_tracking_id>                # Optional. Set advocacy tracking code for supported links
#oc_id: <marketing_tracking_id>          # Optional. Set marketing tracking code for supported links
#navigation_levels: 2                    # Optional. Number of levels displayed in the side menu (default: 2)
#sections_title:                         # Optional. Override titles for each section to be displayed in the side bar
#   - Section 1 title
#   - Section 2 title
---
![Verne](assets\logo_VerneGroup_color.png)

# Python para principiantes

Content for first section

---

## Requisitos para aprovechar el curso

### Requisitos técnicos
Para poder reproducir las demostraciones e intentar los ejercicios es necesario que tengáis instalado en vuestro equipo:

- [Python]
- [Visual Studio Code]
- [Extensión de Python para Visual Studio Code]

En caso de que no queráis instalar nada, podéis utilizar el entorno de Google Colaboratory https://colab.research.google.com/notebooks/welcome.ipynb en el que podréis guardar y ejecutar los notebooks jupyter.

### Conocimientos necesarios

El curso parte de la base de que se dispone de experiencia trabajando con datos, ya sea utilizando Excel como herramienta de explotación, consultas SQL, o experiencia en desarrollo de aplicaciones backend. 

Durante el curso se utilizará Python como lenguaje para la ejecución de demostraciones y ejercicios. Aunque lo relevante del curso son los conceptos, y el código generado será muy poco, es de ayuda el tener algo de experiencia con Python, aunque sea básica. Para ayudar con ello, puedes seguir este Tutorial. 

#### Instalación de Python

https://www.codecademy.com/articles/install-python3 
https://recursospython.com/guias-y-manuales/instalacion-y-utilizacion-de-pip-en-windows-linux-y-os-x/
https://recursospython.com/guias-y-manuales/python-no-se-reconoce-como-un-comando-interno-o-externo/

La instalación de Python es sencilla. Puedes descargar la última versión desde este enlace https://www.python.org/downloads/ seleccionado el Sistema Operativo sobre el que quieres trabajar. 
Es importante que a la hora de la instalación, selecciones la opción que permite agregar Python al PATH del sistema operativo, de modo que puedas invocar después a Python estés donde estés. 

![Agregar Python al Path](/recursos/InstalacionPython.jpg)

##### Gestor de Paquetes Anaconda /* REALMENTE ES NECESARIO?? */
 INSTALAR MINICONDA Y UTILIZAR ENTORNOS
Nos será muy útil, disponer de un gestor de paquetes para Python, que nos permita instalar de un modo sencillo y automático, los paquetes que necesitemos a lo largo de nuestro curso o proyecto. En el mundo del Machine Learning, el gestor de paquetes más utilizado es Anaconda, que puedes descargar desde este enlace https://www.anaconda.com/products/individual 

#### Instalar PIP
Una vez disponemos de Python en nuestro equipo, nos ayudará mucho disponer de un gestor de paquetes para poder descargar e instalar los paquetes que iremos utilizando durante el curso de un modo más sencillo. Aunque existe varios gestores de paquetes y algunos de ellos como Anaconda, específicos para Machine Learning, vamos a empezar con el básico, pip. pip es una herramienta escrita en Python para facilitar la descarga e instalación de paquetes del lenguaje que se encuentren en el Python Package Index (PyPI).

Para instalar pip, primero debemos de descargarnos este fichero https://bootstrap.pypa.io/get-pip.py 
Una vez descargado, debemos de ejecutar desde una consola: python get-pip.py 

Puedes comprobar que dispones de la última versión, ejecutando:

python -m pip install --upgrade pip wheel setuptools

### Instalación de Visual Studio Code

Visual Studio Code es en editor de código fuente, multiplataforma (puede instalarse en Windows, macOS y Linux) y que además soporte múltiples lenguajes de programción, además de ser gratuito y de código abierto. 

Podéis descargarlo directamente desde este enlace https://code.visualstudio.com/Download y lanzar directamente la instalación ejecutando el archivo descargado. 

Y para comenzar un listado de atajos de teclado predeterminados https://code.visualstudio.com/shortcuts/keyboard-shortcuts-windows.pdf?ocid=AID3019735_TWITTER_oo_spl100001423204315 

#### Instalando el complemento de Python para VS Code

Podemos instalar el complemento de diferentes maneras, pero lo más sencilla es directamente en VS Code, buscar la extensión Python en el Marketplace e instalarla. Con ese paso, VS Code ya reconocerá los ficheros con extensión .py y los interpretará como código Python, permitiéndose escribir nuestras soluciones con ese lenguaje. 

![](/recursos/InstalarComplemento.jpg)

###### Paquetes básicos para empezar a trabajar

Como hemos decidido trabajar con Python básico y no con distribuciones que ya tengan instalados determinados paquetes, necesitaremos instalar los paquetes básicos que necesitemos en nuestros programas Python. Comenzaremos por instalar numpy, pandas, pyodbc, matplotlib, sklearn:

pip install numpy
pip install pandas
pip install pyodbc
pip install matplotlib
pip install sklearn


## Introducción a Markdown
Markdown es un lenguaje de marcado sencillo que sirve para agregar formato, vínculos e imágenes con facilidad al texto simple. Nace como un lenguaje para facilitar la escritura de texto para la Web. No sustituye HTML, sino que podríamos decir que HTML es un formato de publicación mientras que Markdown es un formato de escritura. A día de hoy está soportado por muchos IDE, además de estar soportado de forma nativa por la mayor parte de soluciones SaaS, por lo que es un formato estándar para poder escribir texto en cualquier aplicación. 


https://daringfireball.net/projects/markdown/syntax

### Referencia

Markdown | Visualización
--- | ---
`**texto en negrita**` | **negrita**
`*texto en cursiva*` or `_texto en cursiva_` | *cursiva*
`` `Monospace` `` | `Monospace`
`~~Tachado~~` | ~~tachado~~
`[Un enlace](https://www.google.com)` | [Un enlace](https://www.google.com)
`![Una imagen](https://www.vernegroup.com/wp-content/uploads/2020/07/LOGO-VERNE-TECHNOLOGY-GROUP-3.png)` | ![Una imagen](https://www.vernegroup.com/wp-content/uploads/2020/07/LOGO-VERNE-TECHNOLOGY-GROUP-3.png)


### Títulos

```markdown
# Título 1
# Título 2
## Sub-título bajo Título 2
### Sub-título bajo el sub-título bajo el Título 2
# Título 3
```

# Título 1
# Título 2
## Sub-título bajo Título 2
### Sub-título bajo el sub-título bajo el Título 2
# Título 3

---

```markdown
>Un nivel de tabulación
```

>Un nivel de tabulación


```markdown
>>Dos niveles de tabulación
```

>>Dos niveles de tabulación

---

---

Listas Ordenadas:
```markdown
1. Uno
1. Dos
1. Tres
```
1. Uno
1. Dos
1. Tres

---

Listas No Ordenadas:
```markdown
* Uno
* Dos
* Tres
```
* Uno
* Dos
* Tres

---

---

Tablas:
```markdown
Primer nombre columna  | Segundo nombre de columna 
-------------------|------------------
Fila 1, Col 1       | Fila 1, Col 2 
Fila 2, Col 1       | Fila 2, Col 2 

```

Primer nombre de columna  | Segundo nombre de columna 
-------------------|------------------
Fila 1, Col 1       | Fila 1, Col 2 
Fila 2, Col 1       | Fila 2, Col 2 

---
## Elementos del Lenguaje

```python
# Comentario
variable = 23  # Comentario en línea

""" Varias lineas
y mas lineas """
variable = 32

# Definir una variable
# nombre = valor

altura = 190
peso_kg = 90

# Las constantes son un tipo de variable, que permanece inmutable durante el contexto de la ejecución. Las recomendaciones PEP8, en este caso, pasan por definir las constantes con letras MAYUSCULAS

PESO_MAXIMO = 100

print (PESO_MAXIMO)

#Cadenas de Texto

nombre = "Antonio"
texto = """ Este es un texto
    que puede ocupar
    varias lineas"""
otro_texto = "En este texto \n también tenemos varias líneas"
la_barra = "Si queremos usar \\ debemos hacerla doble"

print (otro_texto)

#Trabajo con Cadenas

cadena_1 = "Esto es "
cadena_2 = "una clase de Python"
print (cadena_1 + cadena_2)

# Cadenas Formateadas
nombre = "Antonio"
f"Mi nombre es {nombre}."

#Métodos de cadenas
nombre.lower()


# Números Enteros
cantidad = 23

# Números en punto flotante
precio = 12.50

# Booleanos

verdadero = True
falso = False

```
