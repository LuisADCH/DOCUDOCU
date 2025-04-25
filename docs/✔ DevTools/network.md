---
sidebar_position: 6
slug: /devtools/network
---

# 📶 Network (Red)

:::tip
La pestaña **Network** muestra todas las solicitudes que realiza el navegador al cargar una página web, como peticiones de archivos, API, recursos externos, etc.
:::

---

## 🧠 ¿Qué es la pestaña Network?

La pestaña **Network** permite monitorizar todas las peticiones de red realizadas por el navegador. Aquí podrás ver:

- Todos los archivos cargados, como HTML, CSS, JS, imágenes, fuentes, etc.
- Las solicitudes de red realizadas a través de AJAX o APIs.
- Tiempos de carga de cada solicitud.
- Estado HTTP de cada recurso (200, 404, 500, etc.).

---

## 🎯 Visualización de solicitudes de red

| Información          | Descripción                                                       |
|----------------------|-------------------------------------------------------------------|
| **Tipo**             | El tipo de archivo o recurso solicitado (XHR, JS, CSS, Img, etc.). |
| **Estado HTTP**      | El código de respuesta de la solicitud (200, 404, etc.).           |
| **Tiempo**           | El tiempo que tardó la solicitud en completarse.                   |
| **Tamaño**           | El tamaño del recurso solicitado.                                 |

---

## 🚀 Filtros disponibles

Puedes filtrar las solicitudes de red por tipo:

- **All**: Ver todas las solicitudes.
- **JS**: Solo los archivos JavaScript.
- **CSS**: Solo hojas de estilo CSS.
- **Img**: Imágenes solicitadas.
- **XHR**: Solicitudes de XMLHttpRequest (AJAX).
- **Font**: Fuentes de la web.

---

## 🧩 Cómo usar Network para depuración

1. **Revisar fallos de recursos**: Si un archivo no se carga correctamente, puedes ver el código de estado HTTP (por ejemplo, 404 si no se encuentra).
2. **Ver tiempos de carga**: Analiza los tiempos de respuesta de las solicitudes y optimiza los recursos lentos.
3. **Examinar APIs**: Si tu sitio hace llamadas a APIs, puedes ver los detalles de cada solicitud y respuesta, incluyendo el cuerpo de la respuesta.

---

## 🧰 Casos prácticos de uso

| Objetivo                      | Acción                                              |
|-------------------------------|-----------------------------------------------------|
| Ver si se carga una imagen     | Filtra por "Img" y busca el recurso específico.     |
| Diagnosticar una API fallida  | Filtra por "XHR" y revisa la respuesta.            |
| Optimizar la carga de archivos | Verifica los tiempos de carga de cada solicitud.    |

---

## 🚨 Consejos avanzados

- Usa la **pestaña Timing** para analizar el tiempo que toma cada fase de la solicitud (DNS, conexión, etc.).
- Si estás depurando una API, puedes inspeccionar tanto la solicitud como la respuesta en formato JSON.

:::warning
Recuerda que las solicitudes de red pueden ser bloqueadas por **políticas CORS** o **firewalls**, por lo que verifica el estado y la configuración del servidor si ves errores.
:::

---

👉 En el siguiente archivo, exploraremos la pestaña **Performance**, que te ayuda a mejorar el rendimiento de tu sitio.
