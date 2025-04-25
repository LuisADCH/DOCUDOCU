---
sidebar_position: 3
slug: /devtools/estructura-css/styles
---

# 🎨 Styles (Estilos)

:::tip
La pestaña **Styles** te permite visualizar y modificar las reglas CSS aplicadas a cualquier elemento HTML seleccionado. Es esencial para depurar problemas visuales y probar cambios rápidos.
:::

---

## 🎯 ¿Qué puedes hacer en la pestaña Styles?

| Acción                           | Descripción                                                                 |
|---------------------------------|-----------------------------------------------------------------------------|
| Ver reglas CSS aplicadas        | Muestra todas las reglas que afectan al elemento seleccionado.             |
| Editar propiedades directamente | Puedes cambiar valores, añadir nuevas propiedades o eliminarlas.           |
| Activar/desactivar propiedades  | Marca o desmarca para ver efectos sin eliminar código.                     |
| Ver la fuente del estilo        | Indica si el estilo viene de un archivo CSS, del HTML o es inline.         |
| Ver reglas heredadas            | Muestra estilos aplicados desde elementos padre.                           |

---

## 🧩 Panel de estilos

El panel se divide en secciones según la **especificidad** y el **origen** de la regla:

- **Element.style**: Estilos inline escritos directamente en la etiqueta (`style="..."`).
- Reglas de archivos CSS (por orden de cascada).
- Reglas heredadas desde elementos padre.
- Pseudo-clases activas (`:hover`, `:active`, `:focus`).

### 🔍 ¿Cómo reconocer la prioridad?

Las reglas se aplican en orden de:
1. Inline (`style="..."`)
2. ID (`#id`)
3. Clase (`.clase`)
4. Etiqueta (`div`, `p`, etc.)

Las reglas tachadas son las que **no se aplican** por haber sido sobrescritas.

:::danger
Ten en cuenta que usar `!important` puede romper el orden natural de prioridad. Úsalo con precaución.
:::

---

## 🛠 Funciones útiles

### ✍️ Editar estilos al vuelo
Haz clic sobre cualquier propiedad para cambiar su valor. Puedes usar:
- Palabras clave (`block`, `none`, `flex`...)
- Colores (`red`, `#fff`, `rgb(0,0,0)`...)
- Unidades (`px`, `%`, `em`, `vh`...)

### ➕ Añadir nuevas propiedades
Al final del bloque de reglas, haz clic y comienza a escribir una nueva propiedad.

### ✅ Activar/desactivar estilos
Marca o desmarca casillas para ver cómo se comporta el diseño con o sin ciertos estilos.

### 🎯 Estado forzado
Haz clic en `:hov` para aplicar pseudoestados como:
- `:hover` (cuando pasas el mouse)
- `:focus` (cuando haces clic en un input)
- `:active` (cuando haces clic en un botón)

---

## 🧪 Casos prácticos

| Objetivo                          | Cómo hacerlo                                                               |
|----------------------------------|-----------------------------------------------------------------------------|
| Probar un nuevo color de fondo   | Cambiar el valor de `background-color` en el panel                         |
| Ver qué archivo aplica un estilo | Aparece como link al lado derecho de cada regla (`style.css:23`)          |
| Desactivar una clase conflictiva | Desmarca la propiedad correspondiente para ver si cambia el diseño         |

---

## 🔧 Tips avanzados

:::note
Puedes usar **tabulación** y **flechas del teclado** para navegar y ajustar valores numéricos más rápido.
:::

- Usa `Shift + flecha arriba/abajo` para cambiar valores de `10px` en `10px`.
- Escribe `var(--nombre)` si usas variables CSS.
- Puedes usar selectores avanzados como `:nth-child()` en tiempo real.

---

👉 En el siguiente archivo, veremos la pestaña **Console**, donde se gestionan los mensajes de errores y pruebas con JavaScript.

