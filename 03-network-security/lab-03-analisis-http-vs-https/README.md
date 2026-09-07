# LAB-03 · Análisis de HTTP vs HTTPS

## Módulo

**Módulo 3:** Conectar y Proteger: Redes y Seguridad de Redes

## Objetivo

Comparar el comportamiento de HTTP y HTTPS para comprender cómo el cifrado protege la información durante la comunicación entre un cliente y un servidor.

## Escenario

Un usuario inicia sesión en el portal de una empresa utilizando dos versiones del mismo sitio: una mediante HTTP y otra mediante HTTPS. El objetivo es analizar qué información viaja protegida y cuáles son los riesgos de utilizar un protocolo sin cifrado.

## Comparación de protocolos

| Característica | HTTP | HTTPS |
|---------------|------|-------|
| Cifrado de datos | No | Sí |
| Puerto por defecto | 80 | 443 |
| Certificado digital | No | Sí |
| Protección de credenciales | Baja | Alta |
| Integridad de la información | No garantizada | Garantizada mediante TLS |

## Análisis técnico

### Comunicación mediante HTTP

La información viaja en texto plano, lo que permite que un atacante pueda interceptar credenciales, formularios y otros datos sensibles si tiene acceso al tráfico de red.

### Comunicación mediante HTTPS

Antes de intercambiar información, el cliente y el servidor establecen una conexión segura mediante TLS. Esto cifra los datos y protege la confidencialidad e integridad de la comunicación.

## Riesgos identificados

- Intercepción de credenciales.
- Robo de sesiones.
- Manipulación del contenido durante la transmisión.
- Exposición de información personal en redes públicas.

## Controles de seguridad

- Utilizar HTTPS en todos los servicios web.
- Implementar certificados digitales válidos.
- Redireccionar automáticamente HTTP hacia HTTPS.
- Evitar el envío de información sensible mediante protocolos sin cifrado.

## Hallazgos

El análisis demuestra que HTTPS reduce significativamente el riesgo de exposición de información al incorporar cifrado y verificación de identidad mediante certificados digitales.

## Conclusión

La adopción de HTTPS constituye un control esencial para proteger la información durante la comunicación entre usuarios y aplicaciones web, disminuyendo la posibilidad de ataques de interceptación y alteración de datos.
