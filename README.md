# Validador de Etiquetas Hreflang y SEO Internacional

[![Validador Hreflang](https://img.shields.io/badge/TAVARDT-Hreflang-5b3cf5.svg)](https://tools.tavardt.com/es/validador-etiquetas-hreflang/)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

Auditoria tecnica de enlaces alternativos reciprocos, codigos de idioma y pais y directivas x-default.

***

## Capacidades de Auditoria de Hreflang y SEO Internacional

* **Verificacion de Reciprocidad de Enlaces**: Confirma que cada URL alternativa incluya enlace de retorno correspondiente, requisito indispensable para motores de busqueda.
* **Validacion de Codigos ISO 639-1 e ISO 3166-1**: Deteccion estricta de combinaciones validas de idioma y region geografica (ej: `es-ES`, `en-GB`, `fr-FR`).
* **Presencia de Directiva x-default**: Comprobacion de direccion de reserva para usuarios que acceden desde ubicaciones sin idioma especifico.
* **Consistencia con Etiqueta Canonica**: Alerta de discrepancias entre la etiqueta canonical y la directiva hreflang autorreferencial.
* **Indice de Salud Multilingue**: Puntuacion cuantitativa de 0 a 100 con guia de subsanacion tecnica.

***

## Instalacion y Ejecucion

Requiere Python 3.8 o superior sin dependencias externas.

```bash
git clone https://github.com/TAVARDT-Espana/hreflang-validator-es.git
cd hreflang-validator-es
python hreflang_validator.py https://empresa.es
```

Para generar salida estructurada JSON:

```bash
python hreflang_validator.py https://empresa.es -json
```

***

## Consultoria en SEO Internacional y Expansao Global

Para proyectos de escala transfronteriza y cumplimiento de Estandares W3C y Regulaciones Digitales UE, contacte al equipo de **TAVARDT**.

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
