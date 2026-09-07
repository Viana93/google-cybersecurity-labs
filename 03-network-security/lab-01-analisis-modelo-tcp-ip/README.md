# LAB-01 · Análisis del Modelo TCP/IP

## Módulo

**Módulo 3:** Conectar y Proteger: Redes y Seguridad de Redes

## Objetivo

Analizar cómo viaja la información desde un usuario hasta un servidor utilizando el modelo TCP/IP e identificar los protocolos involucrados en cada capa.

## Escenario

Un usuario en Bogotá ingresa a **www.empresa.com** desde su navegador para iniciar sesión en la plataforma de la compañía. Como analista de ciberseguridad, el objetivo es identificar el recorrido de la comunicación y los protocolos que participan en la conexión.

## Flujo de la comunicación

| Etapa | Protocolo | Función |
|--------|-----------|---------|
| 1 | DNS | Convierte el dominio en una dirección IP. |
| 2 | TCP | Establece una conexión confiable entre cliente y servidor. |
| 3 | TLS | Cifra la comunicación antes del intercambio de datos. |
| 4 | HTTPS | Transfiere la información de forma segura. |
| 5 | IP | Enruta los paquetes hasta el servidor. |

## Análisis técnico

### Capa de aplicación

El usuario interactúa con el navegador utilizando el protocolo HTTPS para enviar sus credenciales de forma cifrada.

### Capa de transporte

TCP garantiza que los paquetes lleguen completos y en el orden correcto mediante el establecimiento de una conexión confiable.

### Capa de internet

El protocolo IP permite direccionar y transportar los paquetes desde el equipo del usuario hasta el servidor de destino.

### Capa de acceso a la red

La tarjeta de red y el router transmiten los paquetes a través del medio físico hasta Internet.

## Riesgos identificados

- Suplantación mediante servidores DNS maliciosos.
- Intercepción del tráfico si la conexión no utiliza TLS.
- Exposición de información sensible en protocolos sin cifrado.

## Controles recomendados

- Utilizar HTTPS con certificados válidos.
- Implementar DNS seguro cuando sea posible.
- Monitorear conexiones inusuales desde la red corporativa.

## Hallazgos

Se identificó que la resolución DNS ocurre antes de establecer la sesión TCP y que el cifrado mediante TLS protege la confidencialidad de las credenciales durante la comunicación.

## Conclusión

Comprender el recorrido de una conexión TCP/IP permite identificar en qué punto pueden aparecer vulnerabilidades y qué controles deben implementarse para proteger la comunicación entre clientes y servidores.
