# Sintaxis Markdown

A continuación vamos a ver alguna sintaxi básica de markdown, puedes encontrar mucho más en internet.

> **Tutoriales**: [web recomendada](https://www.markdownguide.org/basic-syntax/) y [tutorial interactivo](https://www.markdowntutorial.com/).


## 1. Títulos

Para agregar títulos, usamos el símbolo `#`. Cuantos más `#` uses, más pequeño será el título (de `#` para un título grande a `######` para uno pequeño).

| Código                                   | Resultado                               |
|------------------------------------------|-----------------------------------------|
| `# Título Grande` <br><br><br><br><br> `## Título Mediano` <br><br> `### Título Pequeño` | <h1>Título Grande</h1> <br> <h2>Título Mediano</h2>  <h3>Título Pequeño</h3> |

> **Tip:** Utiliza los títulos para organizar secciones en tus documentos. 


## 2. Negrita y Cursiva

Para destacar palabras o frases importantes, puedes utilizar **negrita** o *cursiva*.

| Código                                   | Resultado                               |
|------------------------------------------|-----------------------------------------|
| `**Este texto es en negrita**` <br> `*Este texto es en cursiva*` | **Este texto es en negrita** <br> *Este texto es en cursiva* |


## 3. Listas

Puedes crear listas de dos tipos: **desordenadas** y **ordenadas**. Para listas desordenadas, usa `-`, `+` o `*`; y para listas ordenadas, simplemente numera los elementos.

| Código                                   | Resultado                               |
|------------------------------------------|-----------------------------------------|
| `* Elemento A` <br> `* Elemento B` | <ul><li>Elemento A</li> <li>Elemento B</l1></ul> |
| `1. Elemento 1` <br> `2. Elemento 2` | <ol> <li>Elemento 1</li> <li>Elemento 2</l1></ol> |


## 4. Enlaces

Para añadir enlaces a otros sitios web, usa `[texto del enlace](URL)`. Esto crea un enlace clickable.

| Código                                   | Resultado                               |
|------------------------------------------|-----------------------------------------|
| `[Visita GitHub](https://github.com)`    | [Visita GitHub](https://github.com)     |
| `[Visita el Markdown Intro](markdown-intro)`    | [Visita el Markdown Intro](markdown-intro)     |
| `[Visita el siguiente punto](#4-enlaces)`    | [Visita el siguiente punto](#5-imágenes)     |

> Fíjate en que la ruta del enlace puede apuntar a un recurso remoto, local o incluso a una parte de nuestro propio documento si precedimos con el caracter '#'.



## 5. Imágenes

Para insertar una imagen, el formato es similar al de un enlace, pero con un signo de exclamación `!` al principio.

| Código                                   | Resultado                               |
|------------------------------------------|-----------------------------------------|
| `![Imagen de una rana](assets/images/frog100x100.jpg)` | ![Imagen de una rana](assets/images/frog100x100.jpg) |


## 6. Código

Si necesitas mostrar código en tu documento, puedes hacerlo de dos maneras: con ``` ` ``` para código en línea, o con tres acentos graves ```` ``` ```` para bloques de código. Además, podemos especificar qué lenguaje es.

| Código                                   | Resultado                               |
|------------------------------------------|-----------------------------------------|
| `` `sudo apt-get install python` ``          | `sudo apt-get install python`               |

> El formato de bloque no lo podemos mostrar dentro de la tabla. 

<pre>
```python
# Función de python
def suma_uno(int i) -> int:
    return i + 1
```
</pre>

```python
# Función de python
def suma_uno(int i) -> int:
    return i + 1
```


> **Tip:** Usa código en línea para comandos o nombres de clases y bloques para ejemplos de código de múltiples líneas.

---

## 7. Tablas

Markdown también soporta la creación de tablas, como la que estamos utilizando aquí. Usa `|` para separar columnas y `-` para definir los encabezados.

> Tampoco podemo mostrar una tabla dentro de otra, markdown no soporta tablas anidadas. 

```markdown

| Código                                   | Resultado                               |
|------------------------------------------|-----------------------------------------|
| Soy la primera celda de la tabla!        | Y yo la segunda                         |
| Hola hola hola                           | Pues eso, que podemos poner más         |

```


| Código                                   | Resultado                               |
|------------------------------------------|-----------------------------------------|
| Soy la primera celda de la tabla!        | Y yo la segunda                         |
| Hola hola hola                           | Pues eso, que podemos poner más         |

> Ir a **[Github Pages](github-pages.md)**