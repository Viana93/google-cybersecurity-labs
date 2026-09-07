# LAB-04 · Análisis de Puertos y Servicios Críticos

## Módulo

**Módulo 3:** Conectar y Proteger: Redes y Seguridad de Redes

## Objetivo

Identificar los puertos más utilizados en una infraestructura de red y analizar los riesgos asociados a la exposición innecesaria de servicios.

## Escenario

Durante una revisión de seguridad, un analista debe identificar los servicios que se encuentran expuestos en un servidor corporativo y determinar cuáles representan un mayor riesgo para la organización.

## Puertos analizados

| Puerto | Servicio | Riesgo principal |
|---------|----------|------------------|
| 22 | SSH | Acceso remoto no autorizado |
| 53 | DNS | Manipulación de la resolución de nombres |
| 80 | HTTP | Transmisión de información sin cifrar |
| 443 | HTTPS | Servicio web seguro |
| 3389 | RDP | Ataques de fuerza bruta sobre acceso remoto |

## Análisis técnico

### SSH (22)

Permite la administración remota de servidores. Debe protegerse mediante autenticación robusta y restringir el acceso únicamente a usuarios autorizados.

### DNS (53)

Es un servicio esencial para la comunicación en Internet. Una configuración incorrecta puede facilitar ataques de suplantación o envenenamiento de caché.

### HTTP (80)

Al no utilizar cifrado, puede exponer credenciales y datos sensibles durante la transmisión.

### HTTPS (443)

Protege la comunicación mediante cifrado TLS y garantiza la confidencialidad e integridad de la información.

### RDP (3389)

Es uno de los servicios más atacados cuando permanece expuesto a Internet. Requiere controles de acceso y autenticación multifactor.

## Riesgos identificados

- Exposición de servicios administrativos.
- Ataques de fuerza bruta sobre SSH y RDP.
- Captura de información mediante HTTP.
- Configuraciones inseguras en servicios DNS.

## Controles recomendados

- Cerrar los puertos que no sean necesarios.
- Restringir SSH y RDP mediante listas de acceso.
- Utilizar HTTPS en lugar de HTTP.
- Monitorear los intentos de conexión sobre puertos críticos.

## Hallazgos

La exposición innecesaria de puertos incrementa la superficie de ataque de una organización. La correcta gestión de los servicios publicados constituye un control preventivo fundamental.

## Conclusión

Identificar los puertos críticos permite comprender qué servicios están disponibles en una red y priorizar medidas de protección para reducir el riesgo de accesos no autorizados.
