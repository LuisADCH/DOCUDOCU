---
sidebar_position: 2
slug: /devtools/estructura-css/elements
---

# 🔍 Elements (Elementos)

:::tip
La pestaña **Elements** te permite inspeccionar y modificar la estructura del sitio web en tiempo real. Es ideal para entender cómo está compuesto el HTML y cómo los estilos afectan a cada elemento.
:::

---

## 🧱 ¿Qué puedes hacer en "Elements"?

| Acción                            | Descripción                                                                 |
|----------------------------------|-----------------------------------------------------------------------------|
| Ver el árbol DOM                 | Muestra la estructura HTML del sitio como nodos jerárquicos.               |
| Seleccionar un elemento en la web| Herramienta de selección directa desde la página.                          |
| Editar etiquetas HTML            | Puedes cambiar texto, atributos, clases directamente.                      |
| Ver los estilos CSS aplicados    | En el panel lateral derecho (pestaña Styles).                              |
| Ver qué reglas están anuladas    | Las reglas tachadas indican que no se aplican por alguna prioridad mayor. |

---

## 🛠 Herramientas disponibles dentro de Elements

### 🧲 Selector de elementos (Ctrl + Shift + C)

Te permite seleccionar cualquier componente de la página y ver directamente su código HTML. Ideal para inspecciones rápidas.

### 🧾 Atributos y clases

Haz doble clic sobre el nombre de la etiqueta para modificar atributos, añadir clases o cambiar IDs sin editar el archivo fuente.

### 📋 Menú contextual

Haz clic derecho sobre cualquier nodo del DOM para acceder a funciones como:
- Editar como HTML
- Copiar selector CSS o XPath
- Eliminar el elemento

### 🔄 Cambios visuales

Puedes cambiar temporalmente:
- Contenido textual
- Posición de elementos
- Estructura del sitio para pruebas rápidas de UX/UI

:::warning
Los cambios hechos en DevTools **NO se guardan** en el código original. Se pierden al recargar la página.
:::

---

## 📐 Overlay visual y cajas de modelo (Box Model)

Cada vez que seleccionas un elemento, aparece un recuadro de colores (azul, verde, amarillo, naranja) que representa:

- **Contenido** – El área del texto o imagen (azul)
- **Padding** – Relleno interno (verde)
- **Border** – Borde del elemento (amarillo)
- **Margin** – Margen externo (naranja)

Esto te ayuda a entender cómo se posiciona y distribuye un componente.

---

## 🧪 Casos prácticos

| Objetivo                         | Cómo hacerlo                                                             |
|----------------------------------|---------------------------------------------------------------------------|
| Ver si un botón está oculto      | Revisa su `display`, `visibility` o posición en CSS                      |
| Añadir una clase al header       | Clic en la etiqueta `<header>` > Añadir clase en la barra de atributos   |
| Inspeccionar una imagen rota     | Verifica si el `src` está mal escrito o si la ruta es incorrecta         |

---

## ✅ Consejos útiles

:::note
Puedes mantener abierto el panel y seguir navegando. El panel se actualizará con los nuevos elementos cargados.
:::

- Presiona `H` con un nodo seleccionado para ocultarlo temporalmente (`display: none`).
- Haz clic en el icono de `:hov` para forzar estados como `:hover`, `:active`, `:focus`.
- Puedes buscar por etiquetas, clases o texto presionando `Ctrl + F` dentro de la vista DOM.

---

👉 En el siguiente archivo, exploraremos a fondo la pestaña **Styles**, donde puedes editar estilos CSS directamente.
