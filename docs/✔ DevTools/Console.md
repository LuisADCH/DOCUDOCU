---
sidebar_position: 4
slug: /devtools/javascript/console
---

# 📜 Console (Consola)

:::tip
La pestaña **Console** permite interactuar directamente con el navegador mediante comandos de JavaScript, revisar errores del sitio web y mostrar información de depuración.
:::

---

## 🧠 ¿Qué es la consola?

Es un entorno interactivo donde puedes:

- Escribir y ejecutar código JavaScript.
- Ver mensajes, advertencias y errores del sitio.
- Interactuar con elementos HTML seleccionados.
- Probar funciones o fragmentos de código rápidamente.

---

## 📌 Tipos de mensajes

| Tipo         | Descripción                                  | Ejemplo                        |
|--------------|----------------------------------------------|---------------------------------|
| 📘 `log`      | Mensaje informativo                          | `console.log("Hola mundo")`     |
| ⚠️ `warn`     | Advertencia visual, pero no error            | `console.warn("Atención")`      |
| ❌ `error`    | Error crítico del sitio o del código         | `console.error("Algo salió mal")`|
| 🧪 `info`     | Mensaje descriptivo (menos destacado)        | `console.info("Cargando...")`   |

También puedes ver errores de recursos, fallos de red, excepciones no capturadas, etc.

---

## 💬 Comandos útiles

| Comando                     | Uso                                                                 |
|-----------------------------|----------------------------------------------------------------------|
| `$0`, `$1`, etc.            | Referencias a elementos seleccionados en Elements                   |
| `clear()`                   | Limpia la consola                                                    |
| `dir(obj)`                  | Muestra estructura detallada de un objeto                           |
| `table(arr)`                | Muestra arrays/objetos como tabla                                    |
| `console.assert(cond, msg)`| Muestra un error si la condición es falsa                            |

---

## 🧩 Interacción con el DOM

- Puedes acceder directamente al DOM con `document.querySelector()` o `$()`
- Es posible modificar texto, estilos o atributos desde aquí:

```js
let titulo = document.querySelector("h1");
titulo.style.color = "blue";
titulo.innerText = "Nuevo título desde consola";
```

---

## 🐛 Depuración desde Console

Puedes agregar instrucciones de depuración al código:

```js
console.log("Cargando datos", datos);
console.warn("Este método es obsoleto");
console.error("Fallo en conexión");
```

Agrega `debug(miFuncion)` para activar el modo paso a paso en una función.

---

## 🚨 Visualización de errores

Cuando algo falla:
- La consola te mostrará el **mensaje de error**.
- Puedes hacer clic en el enlace para ir directamente al archivo y línea donde ocurrió.
- En errores de red o CORS, también verás detalles técnicos.

:::danger
¡No ignores los errores rojos! Muchos problemas visuales o de comportamiento se detectan desde aquí.
:::

---

## 📊 Consola como herramienta de pruebas

| Tarea                        | ¿Cómo te ayuda la consola?                                |
|-----------------------------|------------------------------------------------------------|
| Probar un nuevo código JS   | Puedes pegarlo directamente y ver el resultado             |
| Ver contenido de variables  | Con `console.log()` o `dir()`                              |
| Diagnosticar fallos en AJAX | Usar `console.log()` antes y después de cada solicitud     |
| Inspeccionar objetos grandes| `console.table()` o `JSON.stringify(obj, null, 2)`         |

---

## 🔍 Consejo extra

:::note
Puedes mantener abierta la consola mientras navegas para ver mensajes en tiempo real. Ideal para detectar errores intermitentes.
:::

También puedes filtrar los mensajes por tipo (error, warning, log...) usando los íconos en la parte superior.

---

👉 En el siguiente archivo hablaremos sobre la pestaña **Sources**, donde se depura el código fuente línea por línea.

