# Framework Consent Mode v2 y Cumplimiento RGPD

[![Diagnóstico Técnico](https://img.shields.io/badge/TAVARDT-Diagn%C3%B3stico%20T%C3%A9cnico-5b3cf5.svg)](https://tools.tavardt.com/es/validador-consent-mode-v2-rgpd/)
[![JavaScript](https://img.shields.io/badge/JavaScript-Node.js-yellow.svg)](https://nodejs.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

Implementación técnica de Google Consent Mode v2, bloqueo preventivo de rastreadores y adecuación estricta a la Guía de Cookies de la AEPD y el RGPD en España.

***

## 1. Arquitectura y Orden de Ejecución

Para cumplir con las directrices de la AEPD y el RGPD, inserte este script en el <head> antes de cargar Google Tag Manager:

```html
<script src="consent-mode-v2.js"></script>
<!- Google Tag Manager / measurement scripts execute here ->
```

***

## 2. Características Técnicas del Módulo

* **Bloqueo por Defecto (Default Denied):** ad_storage y analytics_storage denegados preventivamente antes del banner CMP.
* **Manejo de Estado Unificado:** API modular window.tavardtConsent.update() con registro de eventos en dataLayer.
* **Redacción de Datos Publicitarios:** Supresión de identificadores de clics mediante ads_data_redaction.
* **Passthrough de URL:** Compatibilidad técnica con url_passthrough para análisis agregado sin persistencia.

***

## 3. Documentación y Requisitos Técnicos

Consulte la lista detallada de requisitos técnicos para España:

* Checklist

***

## 4. Herramientas Técnicas Online (España)

Compruebe el estado de seguridad de sus aplicaciones públicas con las herramientas de TAVARDT:

* [Comprobador de Cabeceras de Seguridad](https://tools.tavardt.com/es/analisis-cabeceras-seguridad/)
* [Verificador DMARC y Correo Electrónico](https://tools.tavardt.com/es/verificador-dmarc-correo/)
* [Escáner de Archivos Expuestos](https://tools.tavardt.com/es/escaneo-archivos-expuestos/)
* [Portal de Diagnóstico Técnico España](https://tools.tavardt.com/es/)

***

## 5. Consultoría y Blindaje Técnico

Para auditorías de etiquetas web, verificación de CMP y blindaje de privacidad en España, contacte con el equipo de **TAVARDT**.

***

## Enlaces Útiles

* **Portal Corporativo:** https://ag.tavardt.com/es/
* **Suite de Diagnósticos:** https://tools.tavardt.com/es/
* **Contacto Técnico:** https://ag.tavardt.com/es/contacto/

***

### Licencia
Distribuido bajo la Licencia MIT.

***

© 2026 TAVARDT. Todos los derechos reservados.
