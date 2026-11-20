# Framework Consent Mode v2 & Guía AEPD / RGPD | TAVARDT España

[![Validador de Consentimento](https://img.shields.io/badge/TAVARDT-Diagn%C3%B3stico%20T%C3%A9cnico-5b3cf5.svg)](https://tools.tavardt.com/es/validador-consent-mode-v2-rgpd/)
[![Conformidade](https://img.shields.io/badge/Jurisdi%C3%A7%C3%A3o-España-00C853.svg)](https://ag.tavardt.com/es/ciberseguridad/)

Implementación técnica de Google Consent Mode v2, bloqueo previo de cookies de terceros y cumplimiento de la guía de cookies de la AEPD en España.

Desenvolvido e mantido pela divisão de privacidade digital e engenharia de dados da **[TAVARDT España](https://ag.tavardt.com/es/)**.

---

## 1. Arquitectura y Orden de Ejecución

Para cumplir con las directrices de la AEPD, este script debe situarse en la cabecera <head> de la web inmediatamente antes del contenedor de Google Tag Manager:

```html
<script src="consent-mode-v2.js"></script>
<!-- O contentor do Google Tag Manager ou scripts de medição seguem aqui -->
```

---

## 2. Características Técnicas del Módulo

* **Bloqueo Previo Estricto:** Inicializa ad_storage, analytics_storage y ad_user_data en estado 'denied' por defecto.
* **Método de Actualización de Consentimiento:** Implementa window.tavardtUpdateConsent() generando el evento tavardt_consent_updated en el dataLayer.
* **Redacción de Datos Publicitarios:** Elimina identificadores de clic de los enlaces si el usuario no ha otorgado consentimiento de marketing.
* **Pasarela Segura entre Dominios:** Habilita url_passthrough manteniendo la trazabilidad sin vulnerar directivas de privacidad.

---

## 3. Documentación y Requisitos Técnicos

Consulte a lista detalhada de requisitos técnicos para este país:

* [Checklist Técnico de Conformidade](checklist.md)

---

## 4. Herramientas Técnicas Online (España)

Audite a conformidade das suas etiquetas e proteja o seu domínio com ferramentas online verificadas:

* [Validador de Consent Mode v2 y RGPD](https://tools.tavardt.com/es/validador-consent-mode-v2-rgpd/)
* [Comprobador de Cabeceras de Seguridad](https://tools.tavardt.com/es/analisis-cabeceras-seguridad/)
* [Verificador DMARC y Correo Electrónico](https://tools.tavardt.com/es/verificador-dmarc-correo/)
* [Escáner de Archivos Expuestos](https://tools.tavardt.com/es/escaneo-archivos-expuestos/)
* [Portal de Diagnóstico Técnico España](https://tools.tavardt.com/es/)

---

## 5. Consultoría y Adecuación de Etiquetas

Para auditorías de tagueo, adecuación a la guía de cookies de la AEPD y consultoría de privacidad en España, contacte con **[TAVARDT España](https://ag.tavardt.com/es/contacto/)**.
