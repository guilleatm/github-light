# Introducción a Markdown

**Markdown** es un lenguaje de marcado ligero que te permite agregar formato a texto plano de manera sencilla. Lo verás mucho en plataformas como **GitHub**, donde se utiliza para crear documentación, README o wikis, entre otros. A continuación, veremos alguna sintaxi básicas de Markdown.


Un documento markdown puede lucir como algo parecido a esto:

```markdown

## Mi documento Markdown

* [Este](https://www.markdownguide.org/basic-syntax/) es un enlace a una web en la que se puede aprender markdown.
* Hay un montón de recursos más como [este otro](https://www.markdowntutorial.com/) por ejemplo. En este caso es un tutorial interactivo!
* Último punto en **negrita** y en *cursiva*

> ¿Sabes que este mismo documento está hecho en **markdown**?

Podemos poner imágenes!  
![Imagen](assets/images/frog100x100.jpg)

Incluso usar código HTML dentro de markdown

<div style="border: 1px solid #309920; padding:10px;">
    Esto es texto dentro de un div verde.
</div>

```

Eso mismo que vemos arriba se renderiza tal que así:

<!-- <div style="border: 4px solid #904060; padding:10px;"> -->

### Mi documento Markdown

* [Este](https://www.markdownguide.org/basic-syntax/) es un enlace a una web en la que se puede aprender markdown.
* Hay un montón de recursos más como [este otro](https://www.markdowntutorial.com/) por ejemplo. En este caso es un tutorial interactivo!
* Último punto en **negrita** y en *cursiva*

> ¿Sabes que este mismo documento está hecho en **markdown**?

Podemos poner incluso imágenes!  
![Imagen](assets/images/frog100x100.jpg)

Incluso podemos usar código HTML dentro de markdown (aunque no todos los motores de render lo aceptan bien)

<div style="border: 1px solid #309920; padding:10px;">
    Esto es texto dentro de un div verde.
</div>

<!-- </div> -->

<br>

> Ir a **[Sinaxis Markdown](markdown-syntax.md)**