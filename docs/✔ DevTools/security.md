---
sidebar_position: 10
slug: /devtools/security
---

# 🔒 Security (Seguridad)

:::tip
La pestaña **Security** en DevTools te permite verificar si tu sitio web está protegido adecuadamente, mostrando información sobre el certificado SSL/TLS y la seguridad de las conexiones.
:::

---

## 🎯 ¿Qué puedes hacer con la pestaña Security?

La pestaña **Security** proporciona detalles sobre la seguridad de tu sitio web, incluyendo:

- **Certificado SSL/TLS**: Si tu sitio utiliza HTTPS y si el certificado es válido.
- **Conexión segura**: Información sobre la conexión y la codificación utilizada.
- **Avisos de seguridad**: Te alerta si hay problemas de seguridad, como contenido mixto o problemas de conexión.

---

## 🧩 Información clave en la pestaña Security

| Información                  | Descripción                                                         |
|------------------------------|---------------------------------------------------------------------|
| **Certificado SSL/TLS**      | Verifica si tu sitio está utilizando un certificado de seguridad válido. |
| **Conexión**                 | Muestra si la conexión al sitio es segura y si utiliza un cifrado adecuado. |
| **Contenido mixto**          | Informa si hay contenido no seguro (HTTP) en una página HTTPS.      |

---

## 🚀 Cómo usar la pestaña Security

1. Abre **DevTools** y ve a la pestaña **Security**.
2. Verifica el estado del certificado SSL/TLS de tu página.
3. Si tu sitio tiene problemas de seguridad, como contenido mixto, DevTools te mostrará una advertencia.
4. Si tu sitio no tiene un certificado válido, aparecerá una advertencia de **conexión no segura**.

---

## 🧰 Casos prácticos de uso

| Objetivo                              | Cómo hacerlo                                             |
|---------------------------------------|----------------------------------------------------------|
| Verificar el certificado SSL/TLS      | Revisa la validez y los detalles del certificado en la pestaña Security. |
| Corregir contenido mixto              | Asegúrate de que todos los recursos (imágenes, scripts) estén cargados sobre HTTPS. |
| Diagnosticar problemas de seguridad   | Usa las advertencias para solucionar problemas de seguridad en el sitio. |

---

## 🚨 Consejos avanzados

- Asegúrate de usar **HTTPS en todas las páginas** de tu sitio para proteger la información de tus usuarios.
- Si tu sitio tiene contenido mixto, **actualiza las URLs** para que todas apunten a HTTPS.

:::warning
Si tu sitio utiliza un certificado SSL/TLS incorrecto o expirado, los usuarios recibirán advertencias de seguridad en su navegador.
:::

---

👉 En el siguiente archivo, exploraremos la pestaña **Coverage**, que te permitirá analizar qué recursos se están cargando y cuáles no.
