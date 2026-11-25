# Validador de Etiquetas Hreflang y SEO Internacional

[![Validador Hreflang](https://img.shields.io/badge/TAVARDT-Hreflang-5b3cf5.svg)](https://tools.tavardt.com/es/validador-etiquetas-hreflang/)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

Auditoria de reciprocidad de enlaces alternativos, etiquetas de idioma y region ISO, y arquitectura de fallback global x-default.

Desarrollado y mantenido por la division de ingenieria de busqueda internacional y estandares web de **TAVARDT**.

***

## Capacidades de Auditoria de Hreflang e SEO Internacional

* **Verificacion de Etiqueta Autorreferencial**: Comprobacion de que la URL auditada se incluye a si misma como enlace alternativo, asegurando validez de rastreo.
* **Inspeccion de Fallback x-default**: Comprobacion de la etiqueta de reserva para visitantes internacionales fuera de regiones especificamente asignadas.
* **Validacion de Estandares ISO 639-1 e ISO 3166-1**: Verificacion estricta de combinaciones de idioma y territorio para evitar sintaxis regional invalida.
* **Deteccion de Conflictos con Canonical**: Identificacion de divergencias criticas donde el enlace canonico contradice las anotaciones hreflang.
* **Extraccion desde Fuente Doble**: Analisis directo de elementos `<link rel="alternate">` en HTML y cabeceras HTTP Link.
* **Puntuacion de Salud Internacional**: Calculo cuantificable de 0 a 100 categorizado en COMPLIANT, WARNING o CRITICAL con recomendaciones precisas.

***

## Instalacion y Ejecucion

Requiere Python 3.8 o superior sin dependencias externas obligatorias.

```bash
git clone https://github.com/TAVARDT-Espana/hreflang-validator-es.git
cd hreflang-validator-es
python hreflang_validator.py https://empresa.es
```

Para generar la salida en formato JSON estructurado en flujos de integracion continua:

```bash
python hreflang_validator.py https://empresa.es -j
```

***

## Diagnostico Completo en la Web

Para auditorias visuales e inspeccion interactiva de etiquetas internacionales:

* [Validador Hreflang](https://tools.tavardt.com/es/validador-etiquetas-hreflang/)
* [Portal Corporativo](https://ag.tavardt.com/es/)

***

## Consultoria en SEO Internacional y Arquitectura Global

Para diseno de portales multirregionales y cumplimiento con estandares W3C, contacte con el equipo tecnico de **TAVARDT**.

***

## Enlaces Utiles

* **Portal Corporativo:** https://ag.tavardt.com/es/
* **Suite de Diagnosticos:** https://tools.tavardt.com/es/
* **Contacto Tecnico:** https://ag.tavardt.com/es/contacto/

***

### Licencia
Distribuido bajo la Licencia MIT. Consulte el archivo LICENSE para mas detalles.

***

© 2026 TAVARDT. Todos los derechos reservados.
