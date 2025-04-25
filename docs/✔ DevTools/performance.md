---
sidebar_position: 7
slug: /devtools/performance
---

# ⚡ Performance (Rendimiento)

:::tip
La pestaña **Performance** permite grabar y analizar el rendimiento de tu sitio web, ayudándote a identificar cuellos de botella, tiempos de carga y repintado de elementos.
:::

---

## 🎯 ¿Qué puedes hacer con Performance?

La pestaña **Performance** te permite grabar el rendimiento de la página mientras interactúas con ella. Algunas de las métricas que puedes observar son:

- **Tiempo de ejecución**: ¿Cuánto tiempo tarda cada script en ejecutarse?
- **Repaint**: ¿Cuánto tiempo se tarda en repintar la página?
- **Reflow**: ¿Cuánto tiempo se tarda en cambiar la disposición del contenido?

---

## 🧩 Analizando el rendimiento

1. **Grabar rendimiento**:
   - Haz clic en el botón de grabación (el círculo rojo) para comenzar a grabar el rendimiento de la página.
   - Realiza acciones en la página (desplazarte, hacer clic, navegar).
   - Detén la grabación para ver un desglose de los eventos y tiempos.

2. **Ver la línea de tiempo**:
   - El gráfico de la línea de tiempo muestra las actividades realizadas durante la grabación.
   - Puedes ver cuando ocurre cada repintado, reflujo, o ejecución de script.

3. **Analizar eventos**:
   - En la línea de tiempo, observa los eventos y el tiempo que toma cada uno.
   - Si un evento tarda mucho, es una señal de que podría haber un problema de rendimiento.

---

## 📊 ¿Qué ver en los resultados?

| Métrica                  | Descripción                                                      |
|--------------------------|------------------------------------------------------------------|
| **Frames**               | Representa los fotogramas por segundo.                           |
| **Time**                 | El tiempo total que tarda en completarse la operación.          |
| **Main thread activity** | El tiempo que el hilo principal de ejecución tarda en completar las tareas. |
| **Idle time**            | El tiempo en que el navegador está inactivo entre tareas.       |

---

## 🛠️ Consejos para mejorar el rendimiento

- **Optimiza imágenes**: Las imágenes grandes pueden afectar gravemente el tiempo de carga.
- **Evita repintados y reflujos innecesarios**: Modificar el DOM puede generar repintados que ralentizan la experiencia del usuario.
- **Divide tareas pesadas**: Si tienes operaciones grandes (como animaciones o cálculos), divídelas en fragmentos más pequeños para que no bloqueen el hilo principal.

---

## 🧰 Casos prácticos de uso

| Objetivo                         | Cómo hacerlo                                                |
|----------------------------------|------------------------------------------------------------|
| Mejorar el tiempo de carga      | Graba la página y revisa los tiempos de cada solicitud.    |
| Optimizar el rendimiento JS     | Revisa cuánto tiempo tarda cada función o script en ejecutarse. |
| Detectar problemas de rendimiento| Usa la línea de tiempo para identificar tareas largas.     |

---

## 🚨 Consejos avanzados

- Usa la vista de **Stack** para ver qué funciones específicas están ralentizando el rendimiento.
- Si estás trabajando con **animaciones**, usa la **pestaña Timeline** para ver cuánto tiempo tardan en completarse.

:::warning
Recuerda que el rendimiento puede verse afectado por la conexión a internet y los dispositivos de prueba, así que asegúrate de hacer pruebas en condiciones controladas.
:::

---

👉 En el siguiente archivo, exploraremos **Lighthouse**, una herramienta integrada que audita la calidad de tu sitio.
