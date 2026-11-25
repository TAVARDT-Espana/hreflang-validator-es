# Validador de Etiquetas Hreflang y SEO Internacional

[![Validador Hreflang](https://img.shields.io/badge/TAVARDT-Hreflang-5b3cf5.svg)](https://tools.tavardt.com/es/validador-etiquetas-hreflang/)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

Auditoria de reciprocidad de enlaces alternativos, etiquetas de idioma y region ISO, y arquitectura de fallback global x-default.

Desarrollado y mantenido por la division de ingenieria de busqueda internacional y estandares web de **TAVARDT**.

***

## Vectores de Riesgo e Impacto Operativo en SEO Internacional

Las directivas hreflang defectuosas generan canibalizacion en motores de busqueda y desindexacion involuntaria de versiones internacionales. Cuando los enlaces de idioma carecen de retorno reciproco o autorreferencia, los rastreadores anulan la segmentacion geografica.

Esta brecha técnica provoca que los usuarios espanoles accedan a versiones de otros mercados, perjudicando la experiencia y la conversion. La inspeccion sistematica previene penalizaciones algoritmicas en arquitecturas multirregionales complejas.

***

## Capacidades Centrales de Auditoria Tecnica

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

## Preguntas Frecuentes (FAQ Tecnico)

### 1. Por que los buscadores ignoran las etiquetas hreflang implementadas?
La falta de reciprocidad en los enlaces de retorno y la ausencia de autorreferencia invalidan la agrupacion de etiquetas ante Google. Esta herramienta audita la simetria completa para evitar la degradacion de la visibilidad internacional.

### 2. Que funcion desempena la etiqueta x-default en portales multirregionales?
La anotacion x-default establece la pagina de destino predeterminada para usuarios ubicados fuera de las zonas linguisticas segmentadas. Su omision obliga a los buscadores a realizar conjeturas que reducen las tasas de conversion.

### 3. Como detecta el auditor las discrepancias entre canonical y hreflang?
El analizador compara los destinos declarados en la etiqueta canonical y en los enlaces alternativos para asegurar coherencia total. Cualquier desalineacion activa una alerta critica y deduce 20 puntos de la calificacion.

### 4. El analizador examina cabeceras HTTP Link ademas de etiquetas HTML?
Si, el motor de analisis inspecciona simultaneamente el encabezado HTML head y las cabeceras HTTP Link devueltas por el servidor. Esto permite auditar recursos no basados en HTML como documentos PDF y respuestas API.

### 5. Que estandares regulan la validacion de codigos de idioma y territorio?
Se exige el cumplimiento de ISO 639-1 para codigos de idioma de dos letras y de ISO 3166-1 alpha-2 para regiones de destino. Las combinaciones incorrectas o invertidas generan deducciones directas en la evaluacion tecnica.

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
