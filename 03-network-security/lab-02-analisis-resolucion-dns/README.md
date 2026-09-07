# LAB-02 · Análisis del proceso de resolución DNS

## Módulo

**Módulo 3:** Conectar y Proteger: Redes y Seguridad de Redes

## Objetivo

Analizar el proceso de resolución de nombres de dominio (DNS) e identificar los posibles riesgos de seguridad asociados durante la comunicación entre un cliente y un servidor.

## Escenario

Un colaborador de una empresa intenta acceder al portal **www.empresa.com** desde su equipo corporativo. Antes de establecer la conexión, el sistema debe convertir el nombre del dominio en una dirección IP mediante el servicio DNS.

## Flujo de resolución DNS

| Paso | Componente | Función |
|------|------------|---------|
| 1 | Usuario | Solicita el acceso al sitio web. |
| 2 | Resolver DNS | Recibe la consulta del equipo. |
| 3 | Servidor DNS | Busca la dirección IP correspondiente. |
| 4 | Respuesta DNS | Devuelve la dirección IP al cliente. |
| 5 | Navegador | Inicia la conexión con el servidor web. |

## Análisis técnico

### ¿Qué ocurre durante la resolución?

El navegador no conoce la dirección IP del dominio. Por ello envía una consulta DNS, recibe la respuesta y posteriormente establece la comunicación con el servidor utilizando esa dirección IP.

### Riesgos identificados

- Suplantación de servidores DNS.
- Envenenamiento de caché DNS.
- Redirección del usuario hacia sitios maliciosos.
- Interceptación de consultas en redes inseguras.

## Controles de seguridad

- Utilizar proveedores DNS confiables.
- Implementar DNS seguro cuando esté disponible.
- Validar certificados HTTPS después de la resolución.
- Monitorear cambios inusuales en las respuestas DNS.

## Hallazgos

Se identificó que DNS es un servicio crítico para cualquier conexión a Internet. Si la respuesta DNS es alterada, el usuario puede ser dirigido a un sitio fraudulento incluso cuando escribe correctamente la dirección del sitio web.

## Conclusión

Comprender el funcionamiento de DNS permite detectar posibles vectores de ataque relacionados con la resolución de nombres y fortalece el análisis de incidentes en entornos corporativos.
