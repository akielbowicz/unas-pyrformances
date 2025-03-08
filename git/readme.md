# Git

Es una herramienta de control de versiones distribuida. ¿Qué quiere decir esto?

**Control de versiones**

Una herramienta que nos permite manejar las distintas versiones de nuestros archivos

Se va a publicar un libro y hay varias personas trabajando distintos aspectos del libro,
la tapa, contratapa, info legal, formato, contenido ..., distintos capítulos.

Y todos están trabajando sobre un mismo libro. Le cambian páginas y hay que renumerar las páginas.
cambia el tamaño de la tapa, hay que reescribir las páginas en nuevas hojas ...

Hay una sola copia del libro que va cambiando y cada uno tiene que ir pasando y cambiando las cosas

**Distribuida**

Muchas personas pueden trabajar en sus copias de manera asincrónica y en distintos lugares, cuando
quiere agregar sus cambios lo puede hacer hacia la copia maestra.

## Elementos

- Cada archivo es una hoja
- El cuaderno de git tiene los registros de los cambios y los objetos/hojas en cada estado
- Sobres de papel para mandar los cambios
- Marcadores 

## Clone, Add, Commit, Fetch, Pull, Merge, Push

- Cuaderno de Git con el registro de los commits
- Working Copy, Staging Area, Local Copy

**Clone**

Hola, necesito una copia para trabajar
Le entregan el Cuaderno de Git y dos copias del Libro (Working Copy, Local Copy)

**Add**

- Realiza modificaciones en el working copy  
- Elige con que cambios va a quedarse (add), los mueve al stagin area

**Commit**

- Aplica los cambios a la Local Copy y registra los cambios en el Cuaderno de Git

**Fetch**

- Pide una actualización de los cambios de la copia remota, recibe las hojas cambiadas y actualiza el registro de cambios en el cuaderno de git

**Merge**

- Elige un cambio de la Copia Local que quiere aplicar a su Working Copy
- Registra los cambios que agrega

**Push**

- LLeva la Local Copy y el cuaderno de git y copia los registros y entrega los objetos


## Branches, Checkout, Switch

- Crear una nueva branch, nueva hoja en el Cuaderno de Git

## Diff

- Armar las differencias entre dos snapshots